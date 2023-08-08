# Comparing `tmp/vega_sim-1.2.0.tar.gz` & `tmp/vega_sim-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vega_sim-1.2.0.tar", max compression
+gzip compressed data, was "vega_sim-1.2.1.tar", max compression
```

## Comparing `vega_sim-1.2.0.tar` & `vega_sim-1.2.1.tar`

### file list

```diff
@@ -1,236 +1,237 @@
--rw-r--r--   0        0        0     1061 2023-07-13 15:30:06.191975 vega_sim-1.2.0/LICENSE
--rw-r--r--   0        0        0     1736 2023-07-13 15:30:06.255976 vega_sim-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      292 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/__init__.py
--rw-r--r--   0        0        0    53438 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/data.py
--rw-r--r--   0        0        0    23160 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/data_raw.py
--rw-r--r--   0        0        0      548 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/faucet.py
--rw-r--r--   0        0        0    20460 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/governance.py
--rw-r--r--   0        0        0     4995 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/helpers.py
--rw-r--r--   0        0        0    12928 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/market.py
--rw-r--r--   0        0        0    22664 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/trading.py
--rw-r--r--   0        0        0      122 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/constants.py
--rw-r--r--   0        0        0     4575 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/README.md
--rw-r--r--   0        0        0     1377 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/classes.py
--rw-r--r--   0        0        0       41 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/example_tokens.json
--rw-r--r--   0        0        0     7517 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/registry.py
--rw-r--r--   0        0        0     4592 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/run_agent.py
--rw-r--r--   0        0        0     2994 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/run_scenario.py
--rw-r--r--   0        0        0    11453 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/scenario.py
--rw-r--r--   0        0        0     2137 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/wallet.py
--rw-r--r--   0        0        0       48 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/environment/__init__.py
--rw-r--r--   0        0        0     2947 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/environment/agent.py
--rw-r--r--   0        0        0    26761 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/environment/environment.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/grpc/__init__.py
--rw-r--r--   0        0        0     1560 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/grpc/client.py
--rw-r--r--   0        0        0    20381 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/local_data_cache.py
--rw-r--r--   0        0        0    27039 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/network_service.py
--rw-r--r--   0        0        0    27824 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/null_service.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/__init__.py
--rw-r--r--   0        0        0     3042 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/configs.py
--rw-r--r--   0        0        0     6665 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/experiment.py
--rw-r--r--   0        0        0    13541 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/loggers.py
--rw-r--r--   0        0        0      636 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/run.py
--rw-r--r--   0        0        0       63 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/__init__.py
--rw-r--r--   0        0        0     5463 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py
--rw-r--r--   0        0        0     6827 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py
--rw-r--r--   0        0        0       37 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/__init__.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/__init__.py
--rw-r--r--   0        0        0      164 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/__init__.py
--rw-r--r--   0        0        0   136996 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2.py
--rw-r--r--   0        0        0   180423 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py
--rw-r--r--   0        0        0     1075 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/__init__.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/__init__.py
--rw-r--r--   0        0        0      247 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/__init__.py
--rw-r--r--   0        0        0    17777 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2.py
--rw-r--r--   0        0        0    18869 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2_grpc.py
--rw-r--r--   0        0        0     9351 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2.py
--rw-r--r--   0        0        0    22463 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py
--rw-r--r--   0        0        0     3300 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/assets_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/assets_pb2_grpc.py
--rw-r--r--   0        0        0     7856 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/chain_events_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/chain_events_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/__init__.py
--rw-r--r--   0        0        0      152 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/__init__.py
--rw-r--r--   0        0        0    15518 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/__init__.py
--rw-r--r--   0        0        0      700 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/__init__.py
--rw-r--r--   0        0        0    10698 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/commands_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/commands_pb2_grpc.py
--rw-r--r--   0        0        0     1690 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/data_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/data_pb2_grpc.py
--rw-r--r--   0        0        0     1339 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/signature_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/signature_pb2_grpc.py
--rw-r--r--   0        0        0     6323 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/transaction_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/transaction_pb2_grpc.py
--rw-r--r--   0        0        0     6777 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/__init__.py
--rw-r--r--   0        0        0      217 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/__init__.py
--rw-r--r--   0        0        0     2474 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/data_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/data_pb2_grpc.py
--rw-r--r--   0        0        0     2707 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/spec_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/spec_pb2_grpc.py
--rw-r--r--   0        0        0     5045 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data_source_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data_source_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/__init__.py
--rw-r--r--   0        0        0      128 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/v1/__init__.py
--rw-r--r--   0        0        0    36828 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/v1/events_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0    20036 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/governance_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/governance_pb2_grpc.py
--rw-r--r--   0        0        0    10667 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/markets_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/markets_pb2_grpc.py
--rw-r--r--   0        0        0     1626 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/oracle_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/oracle_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/__init__.py
--rw-r--r--   0        0        0      140 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/__init__.py
--rw-r--r--   0        0        0    56652 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0    42924 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/vega_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/vega_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/__init__.py
--rw-r--r--   0        0        0      128 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/__init__.py
--rw-r--r--   0        0        0     5154 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/wallet_pb2.py
--rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/wallet_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/quant/__init__.py
--rw-r--r--   0        0        0     2961 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/quant/quant.py
--rw-r--r--   0        0        0       29 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/.gitignore
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/__init__.py
--rw-r--r--   0        0        0     8048 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent.py
--rw-r--r--   0        0        0    13440 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO.py
--rw-r--r--   0        0        0    18985 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py
--rw-r--r--   0        0        0    13019 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_heuristic.py
--rw-r--r--   0        0        0     4754 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/simple_agent.py
--rw-r--r--   0        0        0      925 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/distributions.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/__init__.py
--rw-r--r--   0        0        0      608 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/environments.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/__init__.py
--rw-r--r--   0        0        0     4458 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/create_csv.py
--rw-r--r--   0        0        0     1932 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py
--rw-r--r--   0        0        0     4782 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/logdata.py
--rw-r--r--   0        0        0     4809 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/strategy.py
--rw-r--r--   0        0        0      662 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/helpers.py
--rw-r--r--   0        0        0     3092 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/la_market_state.py
--rw-r--r--   0        0        0     4243 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/networks.py
--rw-r--r--   0        0        0     4015 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/plot.py
--rw-r--r--   0        0        0     9642 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/run_rl_agent.py
--rw-r--r--   0        0        0     2446 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/run_simple_agent.py
--rw-r--r--   0        0        0      505 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/Bibliography.bib
--rw-r--r--   0        0        0    13970 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/RL.tex
--rw-r--r--   0        0        0    36669 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL.png
--rw-r--r--   0        0        0    29521 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL_inv.png
--rw-r--r--   0        0        0    39266 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo.png
--rw-r--r--   0        0        0    52831 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo_inv.png
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/__init__.py
--rw-r--r--   0        0        0     3661 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent.py
--rw-r--r--   0        0        0    12222 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent_MO.py
--rw-r--r--   0        0        0     4442 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/puppets.py
--rw-r--r--   0        0        0     5571 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/learning_environment.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/__init__.py
--rw-r--r--   0        0        0     8091 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/environment.py
--rw-r--r--   0        0        0     4012 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/run.py
--rw-r--r--   0        0        0     1641 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/rewards.py
--rw-r--r--   0        0        0     4365 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/run.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/__init__.py
--rw-r--r--   0        0        0     5547 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/environment.py
--rw-r--r--   0        0        0      680 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/run.py
--rw-r--r--   0        0        0      867 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/states.py
--rw-r--r--   0        0        0     5070 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/states.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/replay/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/replay/replay.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/scenario/__init__.py
--rw-r--r--   0        0        0     2260 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/scenario/adhoc.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/scenario/common/__init__.py
--rw-r--r--   0        0        0   116585 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/common/agents.py
--rw-r--r--   0        0        0     7797 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/common/utils/ideal_mm_models.py
--rw-r--r--   0        0        0     6107 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/common/utils/price_process.py
--rw-r--r--   0        0        0      779 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/agents.py
--rw-r--r--   0        0        0    12572 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/scenario.py
--rw-r--r--   0        0        0     5609 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/configurable_market/agents.py
--rw-r--r--   0        0        0     9050 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/configurable_market/scenario.py
--rw-r--r--   0        0        0      309 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/constants.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/curve_market_maker/__init__.py
--rw-r--r--   0        0        0    11025 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/curve_market_maker/scenario.py
--rw-r--r--   0        0        0    19699 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/agents.py
--rw-r--r--   0        0        0     3656 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_capsule_test.py
--rw-r--r--   0        0        0     2497 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py
--rw-r--r--   0        0        0    19014 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/scenario.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/__init__.py
--rw-r--r--   0        0        0      827 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/agents.py
--rw-r--r--   0        0        0    18488 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/__init__.py
--rw-r--r--   0        0        0    31515 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/agents.py
--rw-r--r--   0        0        0     3160 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/environments.py
--rw-r--r--   0        0        0     8680 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/__init__.py
--rw-r--r--   0        0        0     4782 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/log_data.py
--rw-r--r--   0        0        0     4818 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/strategy.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/__init__.py
--rw-r--r--   0        0        0    11478 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/agents.py
--rw-r--r--   0        0        0     9525 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/scenario.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/utils/__init__.py
--rw-r--r--   0        0        0     4818 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py
--rw-r--r--   0        0        0     1687 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/market_crash/price_process.py
--rw-r--r--   0        0        0     9288 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/market_crash/scenario.py
--rw-r--r--   0        0        0     1948 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/multi_market/agents.py
--rw-r--r--   0        0        0    20142 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/multi_market/scenario.py
--rw-r--r--   0        0        0    10779 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/parameter_experiment/scenario.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/realtime_market/__init__.py
--rw-r--r--   0        0        0     4646 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/realtime_market/scenario.py
--rw-r--r--   0        0        0     7018 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/registry.py
--rw-r--r--   0        0        0     4105 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/scenario.py
--rw-r--r--   0        0        0    95509 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/service.py
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/__init__.py
--rw-r--r--   0        0        0     2038 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/load_binaries.py
--rw-r--r--   0        0        0    12360 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/scenario_output.py
--rw-r--r--   0        0        0    26331 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/scenario_plots.py
--rw-r--r--   0        0        0     3111 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/config.hcl
--rw-r--r--   0        0        0     3728 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/genesis.tmpl
--rw-r--r--   0        0        0        4 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/passphrase-file
--rw-r--r--   0        0        0     1606 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/smart_contracts_addresses.json
--rw-r--r--   0        0        0     1436 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/data_node_full.tmpl
--rw-r--r--   0        0        0      965 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/tendermint_full.tmpl
--rw-r--r--   0        0        0      965 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/tendermint_validators.tmpl
--rw-r--r--   0        0        0     1920 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/vega_full.tmpl
--rw-r--r--   0        0        0     1971 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/vega_validators.tmpl
--rw-r--r--   0        0        0     2612 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegahome/config/data-node/config.toml
--rw-r--r--   0        0        0      277 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/faucet/config.toml
--rw-r--r--   0        0        0     3968 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/node/config.toml
--rw-r--r--   0        0        0      312 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/node/wallets.encrypted
--rw-r--r--   0        0        0      114 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/wallet-service/config.toml
--rw-r--r--   0        0        0      321 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/wallet-service/networks/local.toml
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276
--rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2021-12-09T12-00-28.751280926Z--b6ea7744971f455bbd754a97e8e05ea13dc1a033
--rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-54-28.446104867Z--d1b7ef68bb457b47837c6e81da24455be7a8be0d
--rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-57-18.522457076Z--dc699ecdab1705ebe83b60345060b6b7620263a3
--rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-58-36.643184436Z--760895ae7f813d685b048336fac88625441d6aa7
--rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-59-08.359696969Z--9e5beec6e56b28ccbd02864840b0f1e0125e42ce
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082
--rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124
--rw-r--r--   0        0        0       46 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/priv_validator_state.json
--rw-r--r--   0        0        0     3243 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem
--rw-r--r--   0        0        0      800 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem
--rw-r--r--   0        0        0     9044 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/genesis.json
--rw-r--r--   0        0        0        3 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/passphrase-file
--rw-r--r--   0        0        0        0 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/__init__.py
--rw-r--r--   0        0        0     1552 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/base.py
--rw-r--r--   0        0        0     6855 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/slim_wallet.py
--rw-r--r--   0        0        0     9442 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/vega_wallet.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 vega_sim-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-08-08 08:29:07.366645 vega_sim-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1757 2023-08-08 08:29:07.426647 vega_sim-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/__init__.py
+-rw-r--r--   0        0        0    53438 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/data.py
+-rw-r--r--   0        0        0    23160 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/data_raw.py
+-rw-r--r--   0        0        0      548 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/faucet.py
+-rw-r--r--   0        0        0    21201 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/governance.py
+-rw-r--r--   0        0        0     5817 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/helpers.py
+-rw-r--r--   0        0        0    13991 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/market.py
+-rw-r--r--   0        0        0    23255 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/api/trading.py
+-rw-r--r--   0        0        0      122 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/constants.py
+-rw-r--r--   0        0        0     4575 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/README.md
+-rw-r--r--   0        0        0     1377 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/classes.py
+-rw-r--r--   0        0        0       41 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/example_tokens.json
+-rw-r--r--   0        0        0     7517 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/registry.py
+-rw-r--r--   0        0        0     4592 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/run_agent.py
+-rw-r--r--   0        0        0     2993 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/run_scenario.py
+-rw-r--r--   0        0        0    11539 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/scenario.py
+-rw-r--r--   0        0        0     2137 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/devops/wallet.py
+-rw-r--r--   0        0        0       48 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/environment/__init__.py
+-rw-r--r--   0        0        0     2947 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/environment/agent.py
+-rw-r--r--   0        0        0    27288 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/environment/environment.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/grpc/__init__.py
+-rw-r--r--   0        0        0     1560 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/grpc/client.py
+-rw-r--r--   0        0        0    20443 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/local_data_cache.py
+-rw-r--r--   0        0        0    27171 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/network_service.py
+-rw-r--r--   0        0        0    32962 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/null_service.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/parameter_test/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/parameter_test/parameter/__init__.py
+-rw-r--r--   0        0        0     3042 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/parameter_test/parameter/configs.py
+-rw-r--r--   0        0        0     6665 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/parameter_test/parameter/experiment.py
+-rw-r--r--   0        0        0    13541 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/parameter_test/parameter/loggers.py
+-rw-r--r--   0        0        0      636 2023-08-08 08:29:07.430647 vega_sim-1.2.1/vega_sim/parameter_test/run.py
+-rw-r--r--   0        0        0       63 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/__init__.py
+-rw-r--r--   0        0        0     5724 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py
+-rw-r--r--   0        0        0     6827 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/data_node/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/data_node/api/__init__.py
+-rw-r--r--   0        0        0      164 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/data_node/api/v2/__init__.py
+-rw-r--r--   0        0        0   140181 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/data_node/api/v2/trading_data_pb2.py
+-rw-r--r--   0        0        0   184384 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py
+-rw-r--r--   0        0        0     1075 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/api/__init__.py
+-rw-r--r--   0        0        0      247 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/api/v1/__init__.py
+-rw-r--r--   0        0        0    17777 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/api/v1/core_pb2.py
+-rw-r--r--   0        0        0    18869 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/api/v1/core_pb2_grpc.py
+-rw-r--r--   0        0        0     9351 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/api/v1/corestate_pb2.py
+-rw-r--r--   0        0        0    22463 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py
+-rw-r--r--   0        0        0     3300 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/assets_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/assets_pb2_grpc.py
+-rw-r--r--   0        0        0     7856 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/chain_events_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/chain_events_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/checkpoint/__init__.py
+-rw-r--r--   0        0        0      152 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/checkpoint/v1/__init__.py
+-rw-r--r--   0        0        0    15518 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/__init__.py
+-rw-r--r--   0        0        0      700 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/__init__.py
+-rw-r--r--   0        0        0    10698 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/commands_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/commands_pb2_grpc.py
+-rw-r--r--   0        0        0     1690 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/data_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/data_pb2_grpc.py
+-rw-r--r--   0        0        0     1339 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/signature_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/signature_pb2_grpc.py
+-rw-r--r--   0        0        0     6323 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/transaction_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/transaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6777 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data/__init__.py
+-rw-r--r--   0        0        0      217 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data/v1/__init__.py
+-rw-r--r--   0        0        0     2474 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data/v1/data_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data/v1/data_pb2_grpc.py
+-rw-r--r--   0        0        0     2707 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data/v1/spec_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data/v1/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     5045 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data_source_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/events/__init__.py
+-rw-r--r--   0        0        0      128 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/events/v1/__init__.py
+-rw-r--r--   0        0        0    36840 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/events/v1/events_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/events/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0    20036 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/governance_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/governance_pb2_grpc.py
+-rw-r--r--   0        0        0    10667 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/markets_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/markets_pb2_grpc.py
+-rw-r--r--   0        0        0     1626 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/oracle_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/oracle_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/snapshot/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/snapshot/v1/__init__.py
+-rw-r--r--   0        0        0    57077 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.434647 vega_sim-1.2.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0    43516 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/proto/vega/vega_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/proto/vega/vega_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/proto/vega/wallet/__init__.py
+-rw-r--r--   0        0        0      128 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/proto/vega/wallet/v1/__init__.py
+-rw-r--r--   0        0        0     5154 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/proto/vega/wallet/v1/wallet_pb2.py
+-rw-r--r--   0        0        0      158 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/proto/vega/wallet/v1/wallet_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/quant/__init__.py
+-rw-r--r--   0        0        0     2961 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/quant/quant.py
+-rw-r--r--   0        0        0       29 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/.gitignore
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/agents/__init__.py
+-rw-r--r--   0        0        0     8048 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent.py
+-rw-r--r--   0        0        0    13440 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent_MO.py
+-rw-r--r--   0        0        0    18985 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py
+-rw-r--r--   0        0        0    13019 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent_heuristic.py
+-rw-r--r--   0        0        0     4754 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/agents/simple_agent.py
+-rw-r--r--   0        0        0      925 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/distributions.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/__init__.py
+-rw-r--r--   0        0        0      608 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/environments.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/__init__.py
+-rw-r--r--   0        0        0     4458 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/create_csv.py
+-rw-r--r--   0        0        0     1932 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py
+-rw-r--r--   0        0        0     4782 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/logdata.py
+-rw-r--r--   0        0        0     4809 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/strategy.py
+-rw-r--r--   0        0        0      662 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/helpers.py
+-rw-r--r--   0        0        0     3092 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/la_market_state.py
+-rw-r--r--   0        0        0     4243 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/networks.py
+-rw-r--r--   0        0        0     4015 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/plot.py
+-rw-r--r--   0        0        0     9642 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/run_rl_agent.py
+-rw-r--r--   0        0        0     2446 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/run_simple_agent.py
+-rw-r--r--   0        0        0      505 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/Bibliography.bib
+-rw-r--r--   0        0        0    13970 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/RL.tex
+-rw-r--r--   0        0        0    36669 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/RL.png
+-rw-r--r--   0        0        0    29521 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/RL_inv.png
+-rw-r--r--   0        0        0    39266 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/logo.png
+-rw-r--r--   0        0        0    52831 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/logo_inv.png
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/__init__.py
+-rw-r--r--   0        0        0     3661 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/learning_agent.py
+-rw-r--r--   0        0        0    12222 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/learning_agent_MO.py
+-rw-r--r--   0        0        0     4442 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/puppets.py
+-rw-r--r--   0        0        0     6285 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/learning_environment.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/pettingzoo/__init__.py
+-rw-r--r--   0        0        0     8335 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/pettingzoo/environment.py
+-rw-r--r--   0        0        0     4117 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/pettingzoo/run.py
+-rw-r--r--   0        0        0     3010 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/rewards.py
+-rw-r--r--   0        0        0     4365 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/run.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/__init__.py
+-rw-r--r--   0        0        0     5547 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/environment.py
+-rw-r--r--   0        0        0      680 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/run.py
+-rw-r--r--   0        0        0      867 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/states.py
+-rw-r--r--   0        0        0     5070 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/reinforcement/v2/states.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/replay/__init__.py
+-rw-r--r--   0        0        0     1386 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/replay/replay.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/scenario/__init__.py
+-rw-r--r--   0        0        0     2260 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/scenario/adhoc.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/scenario/common/__init__.py
+-rw-r--r--   0        0        0   116835 2023-08-08 08:29:07.438648 vega_sim-1.2.1/vega_sim/scenario/common/agents.py
+-rw-r--r--   0        0        0     7797 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/common/utils/ideal_mm_models.py
+-rw-r--r--   0        0        0     6107 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/common/utils/price_process.py
+-rw-r--r--   0        0        0      779 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/comprehensive_market/agents.py
+-rw-r--r--   0        0        0    12572 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/comprehensive_market/scenario.py
+-rw-r--r--   0        0        0     5609 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/configurable_market/agents.py
+-rw-r--r--   0        0        0     9050 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/configurable_market/scenario.py
+-rw-r--r--   0        0        0      309 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/constants.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/curve_market_maker/__init__.py
+-rw-r--r--   0        0        0    11025 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/curve_market_maker/scenario.py
+-rw-r--r--   0        0        0    28642 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/agents.py
+-rw-r--r--   0        0        0     3656 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/run_capsule_test.py
+-rw-r--r--   0        0        0     2497 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py
+-rw-r--r--   0        0        0    19556 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/scenario.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/hedged_market_maker/__init__.py
+-rw-r--r--   0        0        0      827 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/hedged_market_maker/agents.py
+-rw-r--r--   0        0        0    18488 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/hedged_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/__init__.py
+-rw-r--r--   0        0        0    31515 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/agents.py
+-rw-r--r--   0        0        0     3160 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/environments.py
+-rw-r--r--   0        0        0     8680 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/utils/__init__.py
+-rw-r--r--   0        0        0     4782 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/utils/log_data.py
+-rw-r--r--   0        0        0     4818 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/utils/strategy.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/__init__.py
+-rw-r--r--   0        0        0    11478 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/agents.py
+-rw-r--r--   0        0        0     9525 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/scenario.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/utils/__init__.py
+-rw-r--r--   0        0        0     4818 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py
+-rw-r--r--   0        0        0     1687 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/market_crash/price_process.py
+-rw-r--r--   0        0        0     9288 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/market_crash/scenario.py
+-rw-r--r--   0        0        0     1948 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/multi_market/agents.py
+-rw-r--r--   0        0        0    20142 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/multi_market/scenario.py
+-rw-r--r--   0        0        0    10779 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/parameter_experiment/scenario.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/realtime_market/__init__.py
+-rw-r--r--   0        0        0     4646 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/realtime_market/scenario.py
+-rw-r--r--   0        0        0     7018 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/registry.py
+-rw-r--r--   0        0        0     4439 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/scenario/scenario.py
+-rw-r--r--   0        0        0    99709 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/service.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/tools/__init__.py
+-rw-r--r--   0        0        0     2537 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/tools/load_binaries.py
+-rw-r--r--   0        0        0      457 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/tools/retry.py
+-rw-r--r--   0        0        0    13800 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/tools/scenario_output.py
+-rw-r--r--   0        0        0    28662 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/tools/scenario_plots.py
+-rw-r--r--   0        0        0     3111 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/config.hcl
+-rw-r--r--   0        0        0     3728 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/genesis.tmpl
+-rw-r--r--   0        0        0        4 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/passphrase-file
+-rw-r--r--   0        0        0     1606 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/smart_contracts_addresses.json
+-rw-r--r--   0        0        0     1436 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/templates/data_node_full.tmpl
+-rw-r--r--   0        0        0      965 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/templates/tendermint_full.tmpl
+-rw-r--r--   0        0        0      965 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/templates/tendermint_validators.tmpl
+-rw-r--r--   0        0        0     1920 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/templates/vega_full.tmpl
+-rw-r--r--   0        0        0     1971 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegacapsule/templates/vega_validators.tmpl
+-rw-r--r--   0        0        0     2613 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegahome/config/data-node/config.toml
+-rw-r--r--   0        0        0      277 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegahome/config/faucet/config.toml
+-rw-r--r--   0        0        0     3968 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegahome/config/node/config.toml
+-rw-r--r--   0        0        0      312 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegahome/config/node/wallets.encrypted
+-rw-r--r--   0        0        0      114 2023-08-08 08:29:07.442648 vega_sim-1.2.1/vega_sim/vegahome/config/wallet-service/config.toml
+-rw-r--r--   0        0        0      321 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/config/wallet-service/networks/local.toml
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276
+-rw-r--r--   0        0        0      491 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2021-12-09T12-00-28.751280926Z--b6ea7744971f455bbd754a97e8e05ea13dc1a033
+-rw-r--r--   0        0        0      491 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-54-28.446104867Z--d1b7ef68bb457b47837c6e81da24455be7a8be0d
+-rw-r--r--   0        0        0      491 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-57-18.522457076Z--dc699ecdab1705ebe83b60345060b6b7620263a3
+-rw-r--r--   0        0        0      491 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-58-36.643184436Z--760895ae7f813d685b048336fac88625441d6aa7
+-rw-r--r--   0        0        0      491 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-59-08.359696969Z--9e5beec6e56b28ccbd02864840b0f1e0125e42ce
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082
+-rw-r--r--   0        0        0      586 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124
+-rw-r--r--   0        0        0       46 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/priv_validator_state.json
+-rw-r--r--   0        0        0     3243 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem
+-rw-r--r--   0        0        0      800 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem
+-rw-r--r--   0        0        0     9044 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/genesis.json
+-rw-r--r--   0        0        0        3 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/vegahome/passphrase-file
+-rw-r--r--   0        0        0        0 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/wallet/__init__.py
+-rw-r--r--   0        0        0     1552 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/wallet/base.py
+-rw-r--r--   0        0        0     6855 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/wallet/slim_wallet.py
+-rw-r--r--   0        0        0     9442 2023-08-08 08:29:07.446648 vega_sim-1.2.1/vega_sim/wallet/vega_wallet.py
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 vega_sim-1.2.1/PKG-INFO
```

### Comparing `vega_sim-1.2.0/LICENSE` & `vega_sim-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/pyproject.toml` & `vega_sim-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "vega_sim"
 description = "Simulator for running self-contained Vega chain on local PC"
 authors = ["Tom McLean <tom@vegaprotocol.io>"]
 license = "MIT"
-version = "1.2.0"
+version = "1.2.1"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 requests = "*"
@@ -28,16 +28,17 @@
 ipywidgets = {version = "*", optional = true}
 protoc-gen-openapiv2 = "*"
 plotly = "*"
 TA-Lib = {version = "*", optional = true}
 python-dotenv = "*"
 deprecated = "*"
 psutil = "*"
+docker = "*"
 gymnasium = {version = "*", optional = true}
-sb3-contrib = {version = "*", optional = true}
+sb3-contrib = {version = "^2.0.0a1", optional = true}
 stable-baselines3 = {version = "*", optional = true }
 tensorboard = {version = "*", optional = true}
 pettingzoo = {version = "*", optional = true}
 numba = {version = "^0.57.1", optional = true}
 tianshou = {version = "*", optional = true}
 
 
@@ -53,12 +54,13 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 
+
 [tool.poetry.extras]
 learning = ["matplotlib", "tqdm", "torch", "gymnasium", "stable-baselines3", "tensorboard", "tianshou", "numba", "pettingzoo"]
 jupyter = ["jupyterlab", "jupyter", "matplotlib", "ipywidgets"]
 profile = ["snakeviz", "pytest-profiling"]
 agents = ["TA-Lib"]
```

### Comparing `vega_sim-1.2.0/vega_sim/api/data.py` & `vega_sim-1.2.1/vega_sim/api/data.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/api/data_raw.py` & `vega_sim-1.2.1/vega_sim/api/data_raw.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/api/faucet.py` & `vega_sim-1.2.1/vega_sim/api/faucet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/api/governance.py` & `vega_sim-1.2.1/vega_sim/api/governance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import logging
-from typing import Callable, Optional
+from typing import Callable, Optional, Union
 
 import vega_sim.api.data_raw as data_raw
 import vega_sim.grpc.client as vac
 import vega_sim.proto.data_node.api.v2 as data_node_protos_v2
 
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.commands.v1 as commands_protos
@@ -80,16 +80,16 @@
 
 
 def propose_market_from_config(
     data_client: vac.VegaTradingDataClientV2,
     wallet: Wallet,
     proposal_key_name: str,
     market_config: MarketConfig,
-    closing_time: str,
-    enactment_time: str,
+    closing_time: Union[str, int],
+    enactment_time: Union[str, int],
     time_forward_fn: Optional[Callable[[], None]] = None,
     governance_asset: Optional[str] = "VOTE",
     proposal_wallet_name: Optional[str] = None,
 ) -> str:
     # Make sure Vega network has governance asset
     vote_asset_id = find_asset_id(
         governance_asset, raise_on_missing=True, data_client=data_client
@@ -117,16 +117,16 @@
     # Build NewMarketConfiguration proto
     changes = market_config.build()
 
     # Build ProposalTerms proto
     proposal = _build_generic_proposal(
         pub_key=pub_key,
         data_client=data_client,
-        closing_time=closing_time,
-        enactment_time=enactment_time,
+        closing_time=int(closing_time),
+        enactment_time=int(enactment_time),
     )
     proposal.terms.new_market.CopyFrom(changes)
 
     return _make_and_wait_for_proposal(
         wallet=wallet,
         wallet_name=proposal_wallet_name,
         key_name=proposal_key_name,
@@ -152,14 +152,16 @@
     risk_model: Optional[vega_protos.markets.LogNormalRiskModel] = None,
     time_forward_fn: Optional[Callable[[], None]] = None,
     price_monitoring_parameters: Optional[
         vega_protos.markets.PriceMonitoringParameters
     ] = None,
     lp_price_range: float = 1,
     wallet_name: Optional[str] = None,
+    parent_market_id: Optional[str] = None,
+    parent_market_insurance_pool_fraction: float = 1,
 ) -> str:
     """Propose a future market as specified user.
 
     Args:
         market_name:
             str, name of the market
         wallet_name:
@@ -193,14 +195,19 @@
                 will drop into a price auction. If not passed defaults to a very
                 permissive setup
         lp_price_range:
             float, Range allowed for LP price commitments from mid price
             (e.g. 2 allows mid-price +/- 2 * mid-price )
         key_name:
             Optional[str], key name stored in metadata. Defaults to None.
+        parent_market_id:
+            Optional[str], Market to set as the parent market on the proposal
+        parent_market_insurance_pool_fraction:
+            float, Fraction of parent market insurance pool to carry over.
+                defaults to 1. No-op if parent_market_id is not set.
 
     Returns:
         str, the ID of the future market proposal on chain
     """
     # Make sure Vega network has governance asset
     vote_asset_id = find_asset_id(
         governance_asset, raise_on_missing=True, data_client=data_client
@@ -306,14 +313,21 @@
             ),
             price_monitoring_parameters=price_monitoring_parameters,
             log_normal=risk_model,
             linear_slippage_factor="0.001",
             quadratic_slippage_factor="0",
         ),
     )
+    if parent_market_id is not None:
+        market_proposal.changes.successor.CopyFrom(
+            vega_protos.governance.SuccessorConfiguration(
+                parent_market_id=parent_market_id,
+                insurance_pool_fraction=str(parent_market_insurance_pool_fraction),
+            )
+        )
 
     proposal = _build_generic_proposal(
         pub_key=pub_key,
         data_client=data_client,
         closing_time=closing_time,
         enactment_time=enactment_time,
     )
```

### Comparing `vega_sim-1.2.0/vega_sim/api/helpers.py` & `vega_sim-1.2.1/vega_sim/api/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import random
 import string
 import time
-from typing import Any, Optional, TypeVar, Union, Callable
-
+import sys
+from decimal import Decimal
+from typing import Any, Callable, Optional, TypeVar, Union
 import requests
+
 from vega_sim.grpc.client import VegaCoreClient, VegaTradingDataClientV2
 from vega_sim.proto.data_node.api.v2.trading_data_pb2 import GetVegaTimeRequest
 from vega_sim.proto.vega.api.v1.core_pb2 import StatisticsRequest
-
+from vega_sim.tools.retry import retry
 
 T = TypeVar("T")
-
 TIME_FORWARD_URL = "{base_url}/api/v1/forwardtime"
 
 logger = logging.getLogger(__name__)
 
 
 class DataNodeBehindError(Exception):
     pass
@@ -38,97 +39,124 @@
 
 
 def enum_to_str(e: Any, val: int) -> str:
     return e.keys()[e.values().index(val)]
 
 
 def num_to_padded_int(to_convert: float, decimals: int) -> float:
-    return int(to_convert * 10**decimals)
+    return int(Decimal(str(to_convert)) * 10**decimals)
 
 
 def num_from_padded_int(to_convert: Union[str, int], decimals: int) -> float:
     if not to_convert:
         return 0
     to_convert = int(to_convert) if isinstance(to_convert, str) else to_convert
     return float(to_convert) / 10**decimals
 
 
 def wait_for_datanode_sync(
     trading_data_client: VegaTradingDataClientV2,
     core_data_client: VegaCoreClient,
-    max_retries: int = 650,
+    max_retries: int = 100,
 ) -> None:
     """Waits for Datanode to catch up to vega core client.
     Note: Will wait for datanode 'latest' time to catch up to core time
     when function is called. This avoids the case where a datanode
     consistently slightly behind the core client never returns.
 
     As such, this ensures that the data node has data from the core
     *at the time of call* not necessarily the latest data when the function returns.
 
     Wait time is exponential with increasing retries
-    (each attempt waits 0.0005 * 1.01^attempt_num seconds).
+    (each attempt waits 0.05 * 1.03^attempt_num seconds).
     """
     attempts = 1
-    core_time = core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
-    trading_time = trading_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
-
+    core_time = retry(
+        10, 0.5, lambda: core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+    )
+    trading_time = retry(
+        10, 0.5, lambda: trading_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+    )
     while core_time > trading_time:
-        time.sleep(0.0005 * 1.01**attempts)
-        trading_time = trading_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+        logging.debug(f"Sleeping in wait_for_datanode_sync for {0.05 * 1.03**attempts}")
+        time.sleep(0.05 * 1.03**attempts)
+        try:
+            trading_time = retry(
+                10,
+                2.0,
+                lambda: trading_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp,
+            )
+        except Exception as e:
+            logging.warn(e)
+            trading_time = sys.maxsize
+
         attempts += 1
         if attempts >= max_retries:
             raise DataNodeBehindError(
                 f"Data Node is behind and not catching up after {attempts} retries"
             )
 
 
 def wait_for_core_catchup(
     core_data_client: VegaCoreClient,
-    max_retries: int = 1000,
+    max_retries: int = 20,
 ) -> None:
     """Waits for core node to fully execute everything in it's backlog.
     Note that this operates by a rough cut of requesting time twice and checking for it
     being unchanged, so only works on nullchain where we control time. May wait forever
     in a standard tendermint chain
     """
     attempts = 1
-    core_time = core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
-    time.sleep(0.0001)
-    core_time_two = core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+    core_time = retry(
+        10, 0.5, lambda: core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+    )
+    time.sleep(0.1)
+    core_time_two = retry(
+        10, 0.5, lambda: core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+    )
 
     while core_time != core_time_two:
-        core_time = core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
-        time.sleep(0.0001)
-        core_time_two = core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp
+        logging.debug(f"Sleeping in wait_for_core_catchup for {0.05 * 1.03**attempts}")
+
+        core_time = retry(
+            10,
+            0.5,
+            lambda: core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp,
+        )
+        time.sleep(0.05 * 1.03**attempts)
+        core_time_two = retry(
+            10,
+            0.5,
+            lambda: core_data_client.GetVegaTime(GetVegaTimeRequest()).timestamp,
+        )
         attempts += 1
         if attempts >= max_retries:
             raise DataNodeBehindError(
                 f"Core Node is behind and not catching up after {attempts} retries"
             )
 
 
 def wait_for_acceptance(
     submission_ref: str,
     submission_load_func: Callable[[str], T],
 ) -> T:
     logger.debug("Waiting for proposal acceptance")
     submission_accepted = False
-    for _ in range(1000):
+    for i in range(20):
         try:
             proposal = submission_load_func(submission_ref)
         except:
-            time.sleep(0.001)
+            time.sleep(0.05 * 1.1**i)
             continue
 
         if proposal:
             logger.debug("Your proposal has been accepted by the network")
             submission_accepted = True
             break
-        time.sleep(0.001)
+        time.sleep(0.05 * 1.1**i)
 
     if not submission_accepted:
         raise ProposalNotAcceptedError(
             "The market did not accept the proposal within the specified time"
         )
     return proposal
 
@@ -147,8 +175,10 @@
     payload = {"forward": time}
 
     req = requests.post(TIME_FORWARD_URL.format(base_url=vega_node_url), json=payload)
     req.raise_for_status()
 
 
 def statistics(core_data_client: VegaCoreClient):
-    return core_data_client.Statistics(StatisticsRequest()).statistics
+    return retry(
+        10, 0.5, lambda: core_data_client.Statistics(StatisticsRequest()).statistics
+    )
```

### Comparing `vega_sim-1.2.0/vega_sim/api/market.py` & `vega_sim-1.2.1/vega_sim/api/market.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     The NewMarketConfiguration proto can be built with the following:
 
     $ new_market_configuration_proto = market_config.build()
 
 """
 
+import copy
 import functools
 import logging
 from typing import Optional, Union
 
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.data.v1 as oracles_protos
 import vega_sim.proto.vega.data_source_pb2 as data_source_protos
@@ -107,56 +108,87 @@
             "price_monitoring_parameters": "default",
             "liquidity_monitoring_parameters": "default",
             "log_normal": "default",
             "instrument": "default",
             "lp_price_range": 0.5,
             "linear_slippage_factor": 1e-3,
             "quadratic_slippage_factor": 0,
+            "successor": None,
         }
     }
 
     def load(self, opt: Optional[str] = None):
         config = super().load(opt=opt)
 
         self.decimal_places = config["decimal_places"]
         self.position_decimal_places = config["position_decimal_places"]
         self.lp_price_range = str(config["lp_price_range"])
         self.linear_slippage_factor = str(config["linear_slippage_factor"])
         self.quadratic_slippage_factor = str(config["quadratic_slippage_factor"])
         self.metadata = config["metadata"]
 
+        self.successor = (
+            Successor(opt=config["successor"])
+            if config["successor"] is not None
+            else None
+        )
+
         self.instrument = InstrumentConfiguration(opt=config["instrument"])
         self.price_monitoring_parameters = PriceMonitoringParameters(
             opt=config["price_monitoring_parameters"]
         )
         self.liquidity_monitoring_parameters = LiquidityMonitoringParameters(
             opt=config["liquidity_monitoring_parameters"]
         )
         self.log_normal = LogNormalRiskModel(opt=config["log_normal"])
 
     def build(self):
-        return vega_protos.governance.NewMarket(
+        new_market = vega_protos.governance.NewMarket(
             changes=vega_protos.governance.NewMarketConfiguration(
                 decimal_places=self.decimal_places,
                 position_decimal_places=self.position_decimal_places,
                 lp_price_range=self.lp_price_range,
                 metadata=self.metadata,
                 instrument=self.instrument.build(),
                 price_monitoring_parameters=self.price_monitoring_parameters.build(),
                 liquidity_monitoring_parameters=self.liquidity_monitoring_parameters.build(),
                 log_normal=self.log_normal.build(),
                 linear_slippage_factor=self.linear_slippage_factor,
                 quadratic_slippage_factor=self.quadratic_slippage_factor,
             )
         )
+        if self.successor is not None:
+            new_market.changes.successor.CopyFrom(self.successor.build())
+        return new_market
 
     def set(self, parameter, value):
         rsetattr(self, attr=parameter, val=value)
 
 
+class Successor(Config):
+    OPTS = {
+        "default": {
+            "parent_market_id": None,
+            "insurance_pool_fraction": 1,
+        }
+    }
+
+    def load(self, opt: Optional[str] = None):
+        config = super().load(opt=opt)
+        self.parent_market_id = config["parent_market_id"]
+        self.insurance_pool_fraction = config.get("insurance_pool_fraction", 1)
+
+    def build(self) -> Optional[vega_protos.governance.SuccessorConfiguration]:
+        if self.parent_market_id is not None:
+            return vega_protos.governance.SuccessorConfiguration(
+                parent_market_id=self.parent_market_id,
+                insurance_pool_fraction=str(self.insurance_pool_fraction),
+            )
+
+
 class PriceMonitoringParameters(Config):
     OPTS = {
         "default": {
             "triggers": [
                 {
                     "horizon": 900,  # 15 minutes
                     "probability": "0.90001",
```

### Comparing `vega_sim-1.2.0/vega_sim/api/trading.py` & `vega_sim-1.2.1/vega_sim/api/trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     pegged_order: Optional[vega_protos.vega.PeggedOrder] = None,
     wait: bool = True,
     time_forward_fn: Optional[Callable[[], None]] = None,
     order_ref: Optional[str] = None,
     key_name: Optional[str] = None,
     reduce_only: bool = False,
     post_only: bool = False,
+    iceberg_opts: Optional[vega_protos.commands.IcebergOpts] = None,
 ) -> Optional[str]:
     """
     Submit orders as specified to required pre-existing market.
     Optionally wait for acceptance of order (raises on non-acceptance)
 
     Args:
         wallet_name:
@@ -99,14 +100,16 @@
             optional str, reference for later identification of order
         key_name:
             Optional[str], key name stored in metadata. Defaults to None.
         reduce_only:
             bool, whether the order should only reduce a parties position.
         post_only:
             bool, whether an order should be prevented from trading immediately.
+        iceberg_ops:
+            Optional[vega_protos.commands.IcebergOpts], options to make order an iceberg order
 
     Returns:
         Optional[str], Order ID if wait is True, otherwise None
     """
 
     order_data = order_submission(
         data_client=data_client,
@@ -117,14 +120,15 @@
         order_type=order_type,
         expires_at=expires_at,
         reference=order_ref,
         price=price,
         pegged_order=pegged_order,
         reduce_only=reduce_only,
         post_only=post_only,
+        iceberg_opts=iceberg_opts,
     )
 
     # Sign the transaction with an order submission command
     # Note: Setting propagate to true will also submit to a Vega node
     wallet.submit_transaction(
         transaction=order_data,
         wallet_name=wallet_name,
@@ -182,14 +186,15 @@
     price: Optional[str] = None,
     expires_at: Optional[int] = None,
     pegged_offset: Optional[str] = None,
     pegged_reference: Optional[vega_protos.vega.PeggedReference] = None,
     volume_delta: float = 0,
     time_in_force: Optional[Union[vega_protos.vega.Order.TimeInForce, str]] = None,
     key_name: Optional[str] = None,
+    iceberg_opts: Optional[vega_protos.commands.v1.IcebergOpts] = None,
 ):
     """
     Amend a Limit order by orderID in the specified market
 
     Args:
         wallet_name:
             str, the wallet name performing the action
@@ -221,14 +226,15 @@
         market_id=market_id,
         price=price,
         size_delta=volume_delta,
         expires_at=expires_at,
         time_in_force=time_in_force,
         pegged_offset=pegged_offset,
         pegged_reference=pegged_reference,
+        iceberg_opts=iceberg_opts,
     )
 
     wallet.submit_transaction(
         transaction=order_data,
         wallet_name=wallet_name,
         transaction_type="order_amendment",
         key_name=key_name,
@@ -422,14 +428,15 @@
     market_id: str,
     price: str,
     size_delta: int,
     expires_at: Optional[int] = None,
     time_in_force: Optional[vega_protos.vega.Order.TimeInForce] = None,
     pegged_offset: Optional[str] = None,
     pegged_reference: Optional[vega_protos.vega.PeggedReference] = None,
+    iceberg_opts: Optional[vega_protos.commands.v1.IcebergOpts] = None,
 ) -> OrderAmendment:
     """Creates a Vega OrderAmendment object.
 
     Args:
         order_id (str):
             Id of order to amend.
         market_id (str):
@@ -515,14 +522,15 @@
     order_type: Union[vega_protos.vega.Order.Type, str],
     expires_at: Optional[int] = None,
     reference: Optional[str] = None,
     price: Optional[str] = None,
     pegged_order: Optional[Union[vega_protos.PeggedOrder, str]] = None,
     reduce_only: bool = False,
     post_only: bool = False,
+    iceberg_opts: Optional[vega_protos.commands.v1.IcebergOpts] = None,
 ) -> OrderSubmission:
     """Creates a Vega OrderSubmission object.
 
     Args:
         data_client (vac.VegaTradingDataClient):
             Client for trading data api.
         market_id (str):
@@ -575,27 +583,30 @@
         market_id=market_id,
         size=size,
         side=side,
         time_in_force=time_in_force,
         type=order_type,
         reduce_only=reduce_only,
         post_only=post_only,
+        iceberg_opts=iceberg_opts,
     )
 
     # Update OrderSubmission object with optional fields if specified
     for attr, val in [
         ("price", price),
         ("expires_at", expires_at),
         ("reference", reference),
     ]:
         if val is not None:
             setattr(command, attr, val)
 
     if pegged_order is not None:
         command.pegged_order.CopyFrom(pegged_order)
+    if iceberg_opts is not None:
+        command.iceberg_opts.CopyFrom(iceberg_opts)
 
     # Return the created and updated OrderSubmission object
     return command
 
 
 def build_pegged_order(pegged_reference: str, pegged_offset: int):
     pegged_reference = get_enum(pegged_reference, vega_protos.vega.PeggedReference)
```

### Comparing `vega_sim-1.2.0/vega_sim/devops/README.md` & `vega_sim-1.2.1/vega_sim/devops/README.md`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/devops/classes.py` & `vega_sim-1.2.1/vega_sim/devops/classes.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/devops/registry.py` & `vega_sim-1.2.1/vega_sim/devops/registry.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/devops/run_agent.py` & `vega_sim-1.2.1/vega_sim/devops/run_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/devops/run_scenario.py` & `vega_sim-1.2.1/vega_sim/devops/run_scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     scenario.step_length_seconds = args.step_length_seconds
 
     if Network[args.network] == Network.NULLCHAIN:
         with VegaServiceNull(
             seconds_per_block=1,
             transactions_per_block=1000,
             retain_log_files=True,
-            use_full_vega_wallet=False,
+            use_full_vega_wallet=True,
             warn_on_raw_data_access=False,
             run_with_console=args.console,
         ) as vega:
             scenario.run_iteration(
                 vega=vega,
                 network=Network[args.network],
                 pause_at_completion=args.pause,
```

### Comparing `vega_sim-1.2.0/vega_sim/devops/scenario.py` & `vega_sim-1.2.1/vega_sim/devops/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,17 @@
                 tag=None,
             )
 
             # Setup agent for proving a market for traders
             market_maker = ExponentialShapedMarketMaker(
                 wallet_name=MARKET_MAKER_AGENT.wallet_name,
                 key_name=MARKET_MAKER_AGENT.key_name,
-                market_name=self.market_manager_args.market_name,
+                market_name=self.market_name
+                if self.market_name is not None
+                else self.market_manager_args.market_name,
                 asset_name=self.market_manager_args.asset_name,
                 initial_asset_mint=self.market_maker_args.initial_mint,
                 commitment_amount=self.market_maker_args.commitment_amount,
                 market_kappa=self.market_maker_args.market_kappa,
                 kappa=self.market_maker_args.order_kappa,
                 num_levels=self.market_maker_args.order_levels,
                 tick_spacing=self.market_maker_args.order_spacing,
```

### Comparing `vega_sim-1.2.0/vega_sim/devops/wallet.py` & `vega_sim-1.2.1/vega_sim/devops/wallet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/environment/agent.py` & `vega_sim-1.2.1/vega_sim/environment/agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/environment/environment.py` & `vega_sim-1.2.1/vega_sim/environment/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,45 +128,50 @@
         )
 
     def run(
         self,
         run_with_console: bool = False,
         pause_at_completion: bool = False,
         log_every_n_steps: Optional[int] = None,
+        step_end_callback: Optional[Callable[[], None]] = None,
     ) -> Optional[List[Any]]:
         """Run the simulation with specified agents.
 
         Args:
             run_with_console:
                 bool, default False, Whether the environment should attempt
                     to spin up a full Vega console with which to observe
                     the market behaviour
             pause_at_completion:
                 bool, default False, If True will pause with a keypress-prompt
                     once the simulation has completed, allowing the final state
                     to be inspected, either via code or the Console
+            step_end_callback:
+                Optional callable, called after each set of agent steps
         """
         if self._vega is None:
             with VegaServiceNull(
                 run_with_console=run_with_console,
                 warn_on_raw_data_access=False,
                 transactions_per_block=self.transactions_per_block,
                 block_duration=f"{int(self.block_length_seconds)}s",
                 use_full_vega_wallet=False,
             ) as vega:
                 return self._run(
                     vega,
                     pause_at_completion=pause_at_completion,
                     log_every_n_steps=log_every_n_steps,
+                    step_end_callback=step_end_callback,
                 )
         else:
             return self._run(
                 self._vega,
                 pause_at_completion=pause_at_completion,
                 log_every_n_steps=log_every_n_steps,
+                step_end_callback=step_end_callback,
             )
 
     def _start_live_feeds(self, vega: VegaService):
         # Get lists of unique market_ids and party_ids to observe
 
         market_ids = [
             vega.find_market_id(market_name)
@@ -190,24 +195,27 @@
         vega.data_cache.start_live_feeds(market_ids=market_ids, party_ids=party_ids)
 
     def _run(
         self,
         vega: VegaServiceNull,
         pause_at_completion: bool = False,
         log_every_n_steps: Optional[int] = None,
+        step_end_callback: Optional[Callable[[], None]] = None,
     ) -> None:
         """Run the simulation with specified agents.
 
         Args:
             pause_at_completion:
                 bool, default False, If True will pause with a keypress-prompt
                     once the simulation has completed, allowing the final state
                     to be inspected, either via code or the Console
             log_every_n_steps:
                 Optional, int, If passed, will log a progress line every n steps
+            step_end_callback:
+                Optional callable, called after each set of agent steps
         """
         logger.info(f"Running wallet at: {vega.wallet_url}")
         logger.info(f"Running graphql at: http://localhost:{vega.data_node_rest_port}")
 
         start = datetime.datetime.now()
 
         for agent in self.agents:
@@ -261,14 +269,17 @@
                 and i % self._pause_every_n_steps == 0
             ):
                 input(
                     f"Environment run at step {i}. Pausing to allow inspection of"
                     " state. Press Enter to continue"
                 )
 
+            if step_end_callback is not None:
+                step_end_callback()
+
         logger.info(f"Run took {(datetime.datetime.now() - start).seconds}s")
 
         if pause_at_completion:
             input(
                 "Environment run completed. Pausing to allow inspection of state."
                 " Press Enter to continue"
             )
```

### Comparing `vega_sim-1.2.0/vega_sim/grpc/client.py` & `vega_sim-1.2.1/vega_sim/grpc/client.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/local_data_cache.py` & `vega_sim-1.2.1/vega_sim/local_data_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import vega_sim.api.data as data
 import vega_sim.api.data_raw as data_raw
 import vega_sim.api.governance as gov
 import vega_sim.grpc.client as vac
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.events.v1.events_pb2 as events_protos
+from vega_sim.tools.retry import retry
 
 logger = logging.getLogger(__name__)
 
 
 def _queue_forwarder(
     data_client: vac.VegaCoreClient,
     stream_registry: List[
@@ -52,15 +53,15 @@
         for evt in evts:
             handlers[evt] = handler
     try:
         for o in obs:
             for event in o.events:
                 if (kill_thread_sig is not None) and kill_thread_sig.is_set():
                     return
-                output = handlers[event.type](event)
+                output = retry(5, 1.0, lambda: handlers[event.type](event))
                 if isinstance(output, (list, GeneratorType)):
                     for elem in output:
                         sink.put(elem)
                 else:
                     sink.put(output)
     except grpc._channel._MultiThreadedRendezvous as e:
         if e.details() in ["Channel closed!", "Socket closed"]:
```

### Comparing `vega_sim-1.2.0/vega_sim/network_service.py` & `vega_sim-1.2.1/vega_sim/network_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,18 +149,18 @@
         vegaConsoleProcess = _popen_process(
             popen_args=[
                 "yarn",
                 "--cwd",
                 vega_console_path,
                 "nx",
                 "serve",
-                "--port",
-                f"{vega_console_port}",
                 "-o",
                 "trading",
+                "--port",
+                f"{vega_console_port}",
             ],
             dir_root=tmp_vega_dir,
             log_name="console",
             env=env_copy,
         )
         processes.append(vegaConsoleProcess)
 
@@ -222,15 +222,15 @@
         vega_home_path: Optional[str] = None,
         wallet_home_path: Optional[str] = None,
         wallet_token_path: Optional[str] = None,
         wallet_passphrase_path: Optional[str] = None,
         wallet_url: Optional[bool] = None,
         faucet_url: Optional[bool] = None,
         vega_node_grpc_url: Optional[str] = None,
-        load_existing_keys: Optional[bool] = None,
+        load_existing_keys: bool = True,
         governance_symbol: Optional[str] = "VEGA",
         vegacapsule_bin_path: Optional[str] = "./vega_sim/bin/vegacapsule",
         network_on_host: Optional[bool] = False,
     ):
         """Method initialises the class.
 
         Args:
@@ -299,15 +299,20 @@
             vega_home_path if vega_home_path is not None else environ.get("VEGA_HOME")
         )
         self._wallet_home = (
             wallet_home_path
             if wallet_home_path is not None
             else environ.get("WALLET_HOME")
         )
-        self._passphrase_file_path = wallet_passphrase_path
+
+        self._passphrase_file_path = (
+            wallet_passphrase_path
+            if wallet_passphrase_path is not None
+            else environ.get("VEGA_WALLET_TOKENS_PASSPHRASE_FILE")
+        )
 
         self._token_path = (
             wallet_token_path
             if wallet_token_path is not None
             else environ.get("VEGA_WALLET_TOKENS_FILE")
         )
```

### Comparing `vega_sim-1.2.0/vega_sim/null_service.py` & `vega_sim-1.2.1/vega_sim/null_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import atexit
 import functools
 import logging
 import multiprocessing
-import psutil
 import os
 import shutil
 import signal
 import socket
 import subprocess
 import tempfile
 import time
@@ -16,24 +15,27 @@
 from collections import namedtuple
 from contextlib import closing
 from enum import Enum, auto
 from io import BufferedWriter
 from os import path
 from typing import Dict, List, Optional, Set
 
+import docker
 import grpc
+import psutil
 import requests
 import toml
 from urllib3.exceptions import MaxRetryError
 
 import vega_sim.api.governance as gov
 import vega_sim.grpc.client as vac
 from vega_sim import vega_bin_path, vega_home_path
 from vega_sim.service import VegaService
 from vega_sim.tools.load_binaries import download_binaries
+from vega_sim.tools.retry import retry
 from vega_sim.wallet.base import DEFAULT_WALLET_NAME, Wallet
 from vega_sim.wallet.slim_wallet import SlimWallet
 from vega_sim.wallet.vega_wallet import VegaWallet
 
 logger = logging.getLogger(__name__)
 
 PortUpdateConfig = namedtuple(
@@ -274,14 +276,15 @@
 
 
 def _update_node_config(
     vega_home: str,
     port_config: Dict[Ports, int],
     transactions_per_block: int = 1,
     block_duration: str = "1s",
+    use_docker_postgres: bool = False,
 ) -> None:
     config_path = path.join(vega_home, "config", "node", "config.toml")
     config_toml = toml.load(config_path)
     config_toml["Blockchain"]["Null"]["GenesisFile"] = path.join(
         vega_home, "genesis.json"
     )
     config_toml["Blockchain"]["Null"]["BlockDuration"] = block_duration
@@ -303,14 +306,17 @@
             file_path = path.join(vega_home, *config.file_path)
             config_toml = toml.load(file_path)
             elem = config_toml
             for k in config.config_path:
                 elem = elem[k]
             elem[config.key] = config.val_func(port_config[port_key])
 
+            if port_key == Ports.DATA_NODE_POSTGRES:
+                config_toml["SQLStore"]["UseEmbedded"] = not use_docker_postgres
+
             with open(file_path, "w") as f:
                 toml.dump(config_toml, f)
 
 
 def manage_vega_processes(
     child_conn: multiprocessing.Pipe,
     vega_path: str,
@@ -329,14 +335,20 @@
 ) -> None:
     logging.basicConfig(
         level=logging.INFO,
         format="%(asctime)s - %(name)s - %(levelname)s: %(message)s",
     )
     port_config = port_config if port_config is not None else {}
 
+    try:
+        docker_client = docker.from_env()
+        use_docker_postgres = True
+    except:
+        use_docker_postgres = False
+
     # Explicitly not using context here so that crashed logs are retained
     tmp_vega_dir = tempfile.mkdtemp(prefix="vega-sim-") if log_dir is None else log_dir
     logger.info(f"Running NullChain from vegahome of {tmp_vega_dir}")
 
     if port_config.get(Ports.CONSOLE):
         logger.info(f"Launching Console at port {port_config.get(Ports.CONSOLE)}")
     if port_config.get(Ports.DATA_NODE_REST):
@@ -363,16 +375,32 @@
 
     tmp_vega_home = tmp_vega_dir + "/vegahome"
     _update_node_config(
         tmp_vega_home,
         port_config=port_config,
         transactions_per_block=transactions_per_block,
         block_duration=block_duration,
+        use_docker_postgres=use_docker_postgres,
     )
 
+    if use_docker_postgres:
+        data_node_docker_volume = docker_client.volumes.create()
+        data_node_container = docker_client.containers.run(
+            "timescale/timescaledb:2.8.0-pg14",
+            detach=True,
+            ports={5432: port_config[Ports.DATA_NODE_POSTGRES]},
+            volumes=[f"{data_node_docker_volume.name}:/var/lib/postgresql/data"],
+            environment={
+                "POSTGRES_USER": "vega",
+                "POSTGRES_PASSWORD": "vega",
+                "POSTGRES_DB": "vega",
+            },
+            remove=True,
+        )
+
     dataNodeProcess = _popen_process(
         [
             data_node_path,
             "start",
             "--home=" + tmp_vega_home,
             "--chainID=CUSTOM",
         ],
@@ -525,48 +553,135 @@
         console_process = _popen_process(
             [
                 "yarn",
                 "--cwd",
                 vega_console_path,
                 "nx",
                 "serve",
-                "--port",
-                f"{port_config[Ports.CONSOLE]}",
                 "-o",
                 "trading",
+                "--port",
+                f"{port_config[Ports.CONSOLE]}",
             ],
             dir_root=tmp_vega_dir,
             log_name="console",
             env=env_copy,
         )
         processes["console"] = console_process
 
     # Send process pid values for resource monitoring
     child_conn.send({name: process.pid for name, process in processes.items()})
 
-    signal.sigwait([signal.SIGKILL, signal.SIGTERM])
-    for process in processes.values():
-        process.terminate()
-    for name, process in processes.items():
-        attempts = 0
-        while process.poll() is None:
-            time.sleep(1)
-            attempts += 1
-            if attempts > 60:
-                logging.warning(
-                    f"Gracefully terminating process timed-out. Killing process {name}."
+    # According to https://docs.oracle.com/cd/E19455-01/806-5257/gen-75415/index.html
+    # There is no guarantee that signal will be catch by this thread. Usually the
+    # parent process catches the signal and removes it from the list of pending
+    # signals, this leave us with memory leak where we have orphaned vega processes
+    # and the docker containers. Below is hack to maximize chance by catching the
+    # signal.
+    # We call signal.signal method as a workaround to move this thread on top of
+    # the catch stack, then sigwait waits until singal is trapped.
+    # As last resort We catches the `SIGCHLD`  in case the parent process exited
+    # and this is the orphan now.
+    # But to provide 100% guarantee this should be implemented in another way:
+    #   - Signal should be trapped in the main process, and this should be synced
+    #     the shared memory
+    #   - or this entire process manager should be incorporated in the VegaServiceNull
+    #     and containers/processes should be removed as inline call in the __exit__
+    #
+    #
+    # Important assumption is that this signal can be caught multiple times as well
+    def sighandler(signal, frame):
+        if signal is None:
+            logging.debug("VegaServiceNull exited normally")
+        else:
+            logging.debug(f"VegaServiceNull exited after trap the {signal} signal")
+
+        logger.debug("Received signal from parent process")
+        if use_docker_postgres:
+
+            def kill_docker_container() -> None:
+                try:
+                    data_node_container.kill()
+                except requests.exceptions.HTTPError as e:
+                    if e.response.status_code == 404:
+                        logger.debug(
+                            f"Container {data_node_container.name} has been already"
+                            " killed"
+                        )
+                        return
+                    else:
+                        raise e
+
+            logger.debug(f"Stopping container {data_node_container.name}")
+            retry(10, 1.0, kill_docker_container)
+
+            removed = False
+            for _ in range(10):
+                try:
+                    logging.info(f"Removing volume {data_node_docker_volume.name}")
+                    data_node_docker_volume.remove(force=True)
+                    removed = True
+                    break
+                except requests.exceptions.HTTPError as e:
+                    if e.response.status_code == 404:
+                        removed = True
+                        logger.debug(
+                            f"Data node volume {data_node_docker_volume.name} has been"
+                            " already killed"
+                        )
+                        break
+                    else:
+                        time.sleep(1)
+                except docker.errors.APIError:
+                    time.sleep(1)
+            if not removed:
+                logging.exception(
+                    "Docker volume failed to cleanup, will require manual cleaning"
                 )
-                process.kill()
-        if process.poll() == 0:
-            logging.debug(f"Process {name} terminated.")
-        if process.poll() == -9:
-            logging.debug(f"Process {name} killed.")
 
-    if not retain_log_files:
-        shutil.rmtree(tmp_vega_dir)
+        logger.debug("Starting termination for processes")
+        for name, process in processes.items():
+            logger.debug(f"Terminating process {name}(pid: {process.pid})")
+            process.terminate()
+
+        for name, process in processes.items():
+            attempts = 0
+            while process.poll() is None:
+                logger.debug(f"Process {name} still not terminated")
+                time.sleep(1)
+                attempts += 1
+                if attempts > 60:
+                    logger.warning(
+                        "Gracefully terminating process timed-out. Killing process"
+                        f" {name}."
+                    )
+                    process.kill()
+            logger.debug(f"Process {name} stopped with {process.poll()}")
+            if process.poll() == 0:
+                logger.debug(f"Process {name} terminated.")
+            if process.poll() == -9:
+                logger.debug(f"Process {name} killed.")
+
+        if not retain_log_files and os.path.exists(tmp_vega_dir):
+            shutil.rmtree(tmp_vega_dir)
+
+    # The below lines are workaround to put the signal listeners on top of the stack, so this process can handle it.
+    signal.signal(signal.SIGINT, lambda _s, _h: None)
+    signal.signal(signal.SIGTERM, lambda _s, _h: None)
+
+    # The process had previously created one or more child processes with the fork() function.
+    # One or more of these processes has since died.
+    signal.signal(signal.SIGCHLD, sighandler)
+    signal.sigwait(
+        [
+            signal.SIGKILL,  # The process was explicitly killed by somebody wielding the kill program.
+            signal.SIGTERM,  # The process was explicitly killed by somebody wielding the terminate program.
+        ]
+    )
+    sighandler(None, None)
 
 
 class VegaServiceNull(VegaService):
     PORT_TO_FIELD_MAP = {
         Ports.WALLET: "wallet_port",
         Ports.DATA_NODE_GRPC: "data_node_grpc_port",
         Ports.DATA_NODE_REST: "data_node_rest_port",
@@ -631,14 +746,16 @@
 
         self.log_dir = tempfile.mkdtemp(prefix="vega-sim-")
 
         self.launch_graphql = launch_graphql
         self.replay_from_path = replay_from_path
         self.check_for_binaries = check_for_binaries
 
+        self.stopped = False
+
         self._assign_ports(port_config)
 
         if start_immediately:
             self.start()
 
     def __enter__(self):
         self.start()
@@ -789,19 +906,16 @@
                 self.stop()
                 raise VegaStartupTimeoutError(
                     "Timed out waiting for Vega simulator to start up"
                 )
 
             self.process_pids = parent_conn.recv()
 
-            # Create a block before waiting for datanode sync and starting the feeds
-            self.wait_fn(1)
-            self.wait_for_total_catchup()
-            self.wait_for_thread_catchup()
-            self.data_cache
+        # Initialise the data-cache
+        self.data_cache
 
         if self.run_with_console:
             webbrowser.open(f"http://localhost:{port_config[Ports.CONSOLE]}/", new=2)
 
         if self.launch_graphql:
             webbrowser.open(
                 f"http://localhost:{port_config[Ports.DATA_NODE_REST]}/graphql", new=2
@@ -809,21 +923,25 @@
 
     # Class internal as at some point the host may vary as well as the port
     @staticmethod
     def _build_url(port: int, prefix: str = "http://"):
         return f"{prefix}localhost:{port}"
 
     def stop(self) -> None:
+        logging.debug("Calling stop for veganullchain")
+        if self.stopped:
+            return
+        self.stopped = True
         self.core_client.stop()
         self.core_state_client.stop()
         self.trading_data_client_v2.stop()
         if self.proc is None:
             logger.info("Stop called but nothing to stop")
         else:
-            self.proc.terminate()
+            os.kill(self.proc.pid, signal.SIGTERM)
         if isinstance(self.wallet, SlimWallet):
             self.wallet.stop()
         super().stop()
 
     @property
     def wallet_url(self) -> str:
         return self._build_url(self.wallet_port)
```

### Comparing `vega_sim-1.2.0/vega_sim/parameter_test/parameter/configs.py` & `vega_sim-1.2.1/vega_sim/parameter_test/parameter/configs.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/parameter_test/parameter/experiment.py` & `vega_sim-1.2.1/vega_sim/parameter_test/parameter/experiment.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/parameter_test/parameter/loggers.py` & `vega_sim-1.2.1/vega_sim/parameter_test/parameter/loggers.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/parameter_test/run.py` & `vega_sim-1.2.1/vega_sim/parameter_test/run.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,41 +21,43 @@
 )
 from vega.commands.v1 import (
     transaction_pb2 as vega_dot_commands_dot_v1_dot_transaction__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n(blockexplorer/api/v1/blockexplorer.proto\x12\x14\x62lockexplorer.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a vega/commands/v1/signature.proto\x1a"vega/commands/v1/transaction.proto"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"1\n\x15GetTransactionRequest\x12\x18\n\x04hash\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x04hash"]\n\x16GetTransactionResponse\x12\x43\n\x0btransaction\x18\x01 \x01(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0btransaction"\xf1\x02\n\x17ListTransactionsRequest\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x1b\n\x06\x62\x65\x66ore\x18\x02 \x01(\tH\x00R\x06\x62\x65\x66ore\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x03 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12T\n\x07\x66ilters\x18\x04 \x03(\x0b\x32:.blockexplorer.api.v1.ListTransactionsRequest.FiltersEntryR\x07\x66ilters\x12\x1b\n\tcmd_types\x18\x05 \x03(\tR\x08\x63mdTypes\x12*\n\x11\x65xclude_cmd_types\x18\x06 \x03(\tR\x0f\x65xcludeCmdTypes\x12\x18\n\x07parties\x18\x07 \x03(\tR\x07parties\x1a:\n\x0c\x46iltersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\t\n\x07_beforeB\x08\n\x06_after"a\n\x18ListTransactionsResponse\x12\x45\n\x0ctransactions\x18\x03 \x03(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0ctransactions"\xc2\x02\n\x0bTransaction\x12\x14\n\x05\x62lock\x18\x01 \x01(\x04R\x05\x62lock\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x12\n\x04\x63ode\x18\x06 \x01(\rR\x04\x63ode\x12\x16\n\x06\x63ursor\x18\x07 \x01(\tR\x06\x63ursor\x12\x35\n\x07\x63ommand\x18\x08 \x01(\x0b\x32\x1b.vega.commands.v1.InputDataR\x07\x63ommand\x12\x39\n\tsignature\x18\t \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x19\n\x05\x65rror\x18\n \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\xc9\x02\n\x14\x42lockExplorerService\x12m\n\x0eGetTransaction\x12+.blockexplorer.api.v1.GetTransactionRequest\x1a,.blockexplorer.api.v1.GetTransactionResponse"\x00\x12s\n\x10ListTransactions\x12-.blockexplorer.api.v1.ListTransactionsRequest\x1a..blockexplorer.api.v1.ListTransactionsResponse"\x00\x12M\n\x04Info\x12!.blockexplorer.api.v1.InfoRequest\x1a".blockexplorer.api.v1.InfoResponseBxZ5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\x92\x41>\x12#\n\x18Vega block explorer APIs2\x07v0.71.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n(blockexplorer/api/v1/blockexplorer.proto\x12\x14\x62lockexplorer.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a vega/commands/v1/signature.proto\x1a"vega/commands/v1/transaction.proto"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"1\n\x15GetTransactionRequest\x12\x18\n\x04hash\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x04hash"]\n\x16GetTransactionResponse\x12\x43\n\x0btransaction\x18\x01 \x01(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0btransaction"\x9f\x03\n\x17ListTransactionsRequest\x12\x18\n\x05limit\x18\x01 \x01(\rB\x02\x18\x01R\x05limit\x12\x1b\n\x06\x62\x65\x66ore\x18\x02 \x01(\tH\x00R\x06\x62\x65\x66ore\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x03 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12T\n\x07\x66ilters\x18\x04 \x03(\x0b\x32:.blockexplorer.api.v1.ListTransactionsRequest.FiltersEntryR\x07\x66ilters\x12\x1b\n\tcmd_types\x18\x05 \x03(\tR\x08\x63mdTypes\x12*\n\x11\x65xclude_cmd_types\x18\x06 \x03(\tR\x0f\x65xcludeCmdTypes\x12\x18\n\x07parties\x18\x07 \x03(\tR\x07parties\x12\x14\n\x05\x66irst\x18\x08 \x01(\rR\x05\x66irst\x12\x12\n\x04last\x18\t \x01(\rR\x04last\x1a:\n\x0c\x46iltersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\t\n\x07_beforeB\x08\n\x06_after"a\n\x18ListTransactionsResponse\x12\x45\n\x0ctransactions\x18\x03 \x03(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0ctransactions"\xc2\x02\n\x0bTransaction\x12\x14\n\x05\x62lock\x18\x01 \x01(\x04R\x05\x62lock\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x12\n\x04\x63ode\x18\x06 \x01(\rR\x04\x63ode\x12\x16\n\x06\x63ursor\x18\x07 \x01(\tR\x06\x63ursor\x12\x35\n\x07\x63ommand\x18\x08 \x01(\x0b\x32\x1b.vega.commands.v1.InputDataR\x07\x63ommand\x12\x39\n\tsignature\x18\t \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x19\n\x05\x65rror\x18\n \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\xc9\x02\n\x14\x42lockExplorerService\x12m\n\x0eGetTransaction\x12+.blockexplorer.api.v1.GetTransactionRequest\x1a,.blockexplorer.api.v1.GetTransactionResponse"\x00\x12s\n\x10ListTransactions\x12-.blockexplorer.api.v1.ListTransactionsRequest\x1a..blockexplorer.api.v1.ListTransactionsResponse"\x00\x12M\n\x04Info\x12!.blockexplorer.api.v1.InfoRequest\x1a".blockexplorer.api.v1.InfoResponseBxZ5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\x92\x41>\x12#\n\x18Vega block explorer APIs2\x07v0.72.6\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "blockexplorer.api.v1.blockexplorer_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\222A>\022#\n\030Vega block explorer APIs2\007v0.71.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\222A>\022#\n\030Vega block explorer APIs2\007v0.72.6\032\023lb.testnet.vega.xyz*\002\001\002"
     _GETTRANSACTIONREQUEST.fields_by_name["hash"]._options = None
     _GETTRANSACTIONREQUEST.fields_by_name["hash"]._serialized_options = b"\342A\001\002"
     _LISTTRANSACTIONSREQUEST_FILTERSENTRY._options = None
     _LISTTRANSACTIONSREQUEST_FILTERSENTRY._serialized_options = b"8\001"
+    _LISTTRANSACTIONSREQUEST.fields_by_name["limit"]._options = None
+    _LISTTRANSACTIONSREQUEST.fields_by_name["limit"]._serialized_options = b"\030\001"
     _globals["_INFOREQUEST"]._serialized_start = 217
     _globals["_INFOREQUEST"]._serialized_end = 230
     _globals["_INFORESPONSE"]._serialized_start = 232
     _globals["_INFORESPONSE"]._serialized_end = 305
     _globals["_GETTRANSACTIONREQUEST"]._serialized_start = 307
     _globals["_GETTRANSACTIONREQUEST"]._serialized_end = 356
     _globals["_GETTRANSACTIONRESPONSE"]._serialized_start = 358
     _globals["_GETTRANSACTIONRESPONSE"]._serialized_end = 451
     _globals["_LISTTRANSACTIONSREQUEST"]._serialized_start = 454
-    _globals["_LISTTRANSACTIONSREQUEST"]._serialized_end = 823
-    _globals["_LISTTRANSACTIONSREQUEST_FILTERSENTRY"]._serialized_start = 744
-    _globals["_LISTTRANSACTIONSREQUEST_FILTERSENTRY"]._serialized_end = 802
-    _globals["_LISTTRANSACTIONSRESPONSE"]._serialized_start = 825
-    _globals["_LISTTRANSACTIONSRESPONSE"]._serialized_end = 922
-    _globals["_TRANSACTION"]._serialized_start = 925
-    _globals["_TRANSACTION"]._serialized_end = 1247
-    _globals["_BLOCKEXPLORERSERVICE"]._serialized_start = 1250
-    _globals["_BLOCKEXPLORERSERVICE"]._serialized_end = 1579
+    _globals["_LISTTRANSACTIONSREQUEST"]._serialized_end = 869
+    _globals["_LISTTRANSACTIONSREQUEST_FILTERSENTRY"]._serialized_start = 790
+    _globals["_LISTTRANSACTIONSREQUEST_FILTERSENTRY"]._serialized_end = 848
+    _globals["_LISTTRANSACTIONSRESPONSE"]._serialized_start = 871
+    _globals["_LISTTRANSACTIONSRESPONSE"]._serialized_end = 968
+    _globals["_TRANSACTION"]._serialized_start = 971
+    _globals["_TRANSACTION"]._serialized_end = 1293
+    _globals["_BLOCKEXPLORERSERVICE"]._serialized_start = 1296
+    _globals["_BLOCKEXPLORERSERVICE"]._serialized_end = 1625
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py` & `vega_sim-1.2.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/data_node/api/v2/trading_data_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,35 @@
 from ....vega import governance_pb2 as vega_dot_governance__pb2
 from ....vega import markets_pb2 as vega_dot_markets__pb2
 from ....vega import oracle_pb2 as vega_dot_oracle__pb2
 from ....vega import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n#data-node/api/v2/trading_data.proto\x12\x0f\x64\x61tanode.api.v2\x1a\x1fgoogle/api/field_behavior.proto\x1a\x19google/api/httpbody.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\xd9\x01\n\nPagination\x12\x19\n\x05\x66irst\x18\x01 \x01(\x05H\x00R\x05\x66irst\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x02 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12\x17\n\x04last\x18\x03 \x01(\x05H\x02R\x04last\x88\x01\x01\x12\x1b\n\x06\x62\x65\x66ore\x18\x04 \x01(\tH\x03R\x06\x62\x65\x66ore\x88\x01\x01\x12&\n\x0cnewest_first\x18\x05 \x01(\x08H\x04R\x0bnewestFirst\x88\x01\x01\x42\x08\n\x06_firstB\x08\n\x06_afterB\x07\n\x05_lastB\t\n\x07_beforeB\x0f\n\r_newest_first"\x9c\x01\n\x08PageInfo\x12"\n\rhas_next_page\x18\x01 \x01(\x08R\x0bhasNextPage\x12*\n\x11has_previous_page\x18\x02 \x01(\x08R\x0fhasPreviousPage\x12!\n\x0cstart_cursor\x18\x03 \x01(\tR\x0bstartCursor\x12\x1d\n\nend_cursor\x18\x04 \x01(\tR\tendCursor"\x9a\x01\n\x0e\x41\x63\x63ountBalance\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\x9e\x01\n\x13ListAccountsRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"W\n\x14ListAccountsResponse\x12?\n\x08\x61\x63\x63ounts\x18\x01 \x01(\x0b\x32#.datanode.api.v2.AccountsConnectionR\x08\x61\x63\x63ounts"\x80\x01\n\x12\x41\x63\x63ountsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.AccountEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\x0b\x41\x63\x63ountEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x16ObserveAccountsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12%\n\x04type\x18\x04 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\xa6\x01\n\x17ObserveAccountsResponse\x12\x42\n\x08snapshot\x18\x01 \x01(\x0b\x32$.datanode.api.v2.AccountSnapshotPageH\x00R\x08snapshot\x12;\n\x07updates\x18\x02 \x01(\x0b\x32\x1f.datanode.api.v2.AccountUpdatesH\x00R\x07updatesB\n\n\x08response"o\n\x13\x41\x63\x63ountSnapshotPage\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"M\n\x0e\x41\x63\x63ountUpdates\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"]\n\x0fGetOrderRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId\x12\x1d\n\x07version\x18\x02 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version"5\n\x10GetOrderResponse\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xbd\x03\n\x0bOrderFilter\x12.\n\x08statuses\x18\x01 \x03(\x0e\x32\x12.vega.Order.StatusR\x08statuses\x12&\n\x05types\x18\x02 \x03(\x0e\x32\x10.vega.Order.TypeR\x05types\x12=\n\x0etime_in_forces\x18\x03 \x03(\x0e\x32\x17.vega.Order.TimeInForceR\x0ctimeInForces\x12+\n\x11\x65xclude_liquidity\x18\x04 \x01(\x08R\x10\x65xcludeLiquidity\x12\x1b\n\tparty_ids\x18\x05 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x06 \x03(\tR\tmarketIds\x12!\n\treference\x18\x07 \x01(\tH\x00R\treference\x88\x01\x01\x12>\n\ndate_range\x18\x08 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x12 \n\tlive_only\x18\t \x01(\x08H\x02R\x08liveOnly\x88\x01\x01\x42\x0c\n\n_referenceB\r\n\x0b_date_rangeB\x0c\n\n_live_only"\xaa\x01\n\x11ListOrdersRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12\x39\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x1c.datanode.api.v2.OrderFilterH\x01R\x06\x66ilter\x88\x01\x01\x42\r\n\x0b_paginationB\t\n\x07_filter"N\n\x12ListOrdersResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x8c\x01\n\x18ListOrderVersionsRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"U\n\x19ListOrderVersionsResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x9a\x01\n\x14ObserveOrdersRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x30\n\x11\x65xclude_liquidity\x18\x03 \x01(\x08H\x00R\x10\x65xcludeLiquidity\x88\x01\x01\x42\x14\n\x12_exclude_liquidity"\xa0\x01\n\x15ObserveOrdersResponse\x12@\n\x08snapshot\x18\x01 \x01(\x0b\x32".datanode.api.v2.OrderSnapshotPageH\x00R\x08snapshot\x12\x39\n\x07updates\x18\x02 \x01(\x0b\x32\x1d.datanode.api.v2.OrderUpdatesH\x00R\x07updatesB\n\n\x08response"U\n\x11OrderSnapshotPage\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"3\n\x0cOrderUpdates\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"\xa3\x01\n\x14ListPositionsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01:\x02\x18\x01\x42\r\n\x0b_pagination"^\n\x15ListPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions:\x02\x18\x01"M\n\x0fPositionsFilter\x12\x1b\n\tparty_ids\x18\x01 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds"\xa4\x01\n\x17ListAllPositionsRequest\x12\x38\n\x06\x66ilter\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PositionsFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"]\n\x18ListAllPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions"J\n\x0cPositionEdge\x12"\n\x04node\x18\x01 \x01(\x0b\x32\x0e.vega.PositionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12PositionConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.PositionEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"v\n\x17ObservePositionsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_id"\xa9\x01\n\x18ObservePositionsResponse\x12\x43\n\x08snapshot\x18\x01 \x01(\x0b\x32%.datanode.api.v2.PositionSnapshotPageH\x00R\x08snapshot\x12<\n\x07updates\x18\x02 \x01(\x0b\x32 .datanode.api.v2.PositionUpdatesH\x00R\x07updatesB\n\n\x08response"a\n\x14PositionSnapshotPage\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"?\n\x0fPositionUpdates\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions"\xa3\x02\n\x11LedgerEntryFilter\x12\x37\n\x18\x63lose_on_account_filters\x18\x01 \x01(\x08R\x15\x63loseOnAccountFilters\x12N\n\x13\x66rom_account_filter\x18\x02 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x11\x66romAccountFilter\x12J\n\x11to_account_filter\x18\x03 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x0ftoAccountFilter\x12\x39\n\x0etransfer_types\x18\x05 \x03(\x0e\x32\x12.vega.TransferTypeR\rtransferTypes"\xd9\x05\n\x15\x41ggregatedLedgerEntry\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x1a\n\x08quantity\x18\x03 \x01(\tR\x08quantity\x12\x37\n\rtransfer_type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x0ctransferType\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12=\n\x11\x66rom_account_type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x39\n\x0fto_account_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x36\n\x15\x66rom_account_party_id\x18\x08 \x01(\tH\x01R\x12\x66romAccountPartyId\x88\x01\x01\x12\x32\n\x13to_account_party_id\x18\t \x01(\tH\x02R\x10toAccountPartyId\x88\x01\x01\x12\x38\n\x16\x66rom_account_market_id\x18\n \x01(\tH\x03R\x13\x66romAccountMarketId\x88\x01\x01\x12\x34\n\x14to_account_market_id\x18\x0b \x01(\tH\x04R\x11toAccountMarketId\x88\x01\x01\x12\x30\n\x14\x66rom_account_balance\x18\x0c \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\r \x01(\tR\x10toAccountBalanceB\x0b\n\t_asset_idB\x18\n\x16_from_account_party_idB\x16\n\x14_to_account_party_idB\x19\n\x17_from_account_market_idB\x17\n\x15_to_account_market_idJ\x04\x08\x01\x10\x02"\xf6\x01\n\x18ListLedgerEntriesRequest\x12:\n\x06\x66ilter\x18\x01 \x01(\x0b\x32".datanode.api.v2.LedgerEntryFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"\xad\x01\n\x1a\x45xportLedgerEntriesRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12\x1f\n\x08\x61sset_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x00R\tdateRange\x88\x01\x01\x42\r\n\x0b_date_range"v\n\x19ListLedgerEntriesResponse\x12Y\n\x0eledger_entries\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.AggregatedLedgerEntriesConnectionR\rledgerEntries"q\n\x1b\x41ggregatedLedgerEntriesEdge\x12:\n\x04node\x18\x01 \x01(\x0b\x32&.datanode.api.v2.AggregatedLedgerEntryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x9f\x01\n!AggregatedLedgerEntriesConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.AggregatedLedgerEntriesEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xf3\x01\n\x19ListBalanceChangesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"f\n\x1aListBalanceChangesResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"\xac\x02\n\x18GetBalanceHistoryRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12\x38\n\x08group_by\x18\x02 \x03(\x0e\x32\x1d.datanode.api.v2.AccountFieldR\x07groupBy\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"e\n\x19GetBalanceHistoryResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"g\n\x15\x41ggregatedBalanceEdge\x12\x36\n\x04node\x18\x01 \x01(\x0b\x32".datanode.api.v2.AggregatedBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x93\x01\n\x1b\x41ggregatedBalanceConnection\x12<\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32&.datanode.api.v2.AggregatedBalanceEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9e\x01\n\rAccountFilter\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x03 \x03(\tR\tmarketIds\x12\x36\n\raccount_types\x18\x04 \x03(\x0e\x32\x11.vega.AccountTypeR\x0c\x61\x63\x63ountTypes"\xa1\x02\n\x11\x41ggregatedBalance\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x1e\n\x08party_id\x18\x04 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12 \n\tmarket_id\x18\x06 \x01(\tH\x02R\x08marketId\x88\x01\x01\x12\x39\n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeH\x03R\x0b\x61\x63\x63ountType\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\x0c\n\n_market_idB\x0f\n\r_account_type";\n\x1aObserveMarketsDepthRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"S\n\x1bObserveMarketsDepthResponse\x12\x34\n\x0cmarket_depth\x18\x01 \x03(\x0b\x32\x11.vega.MarketDepthR\x0bmarketDepth"B\n!ObserveMarketsDepthUpdatesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"U\n"ObserveMarketsDepthUpdatesResponse\x12/\n\x06update\x18\x01 \x03(\x0b\x32\x17.vega.MarketDepthUpdateR\x06update":\n\x19ObserveMarketsDataRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"O\n\x1aObserveMarketsDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"p\n\x1bGetLatestMarketDepthRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12 \n\tmax_depth\x18\x02 \x01(\x04H\x00R\x08maxDepth\x88\x01\x01\x42\x0c\n\n_max_depth"\xda\x01\n\x1cGetLatestMarketDepthResponse\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12*\n\nlast_trade\x18\x04 \x01(\x0b\x32\x0b.vega.TradeR\tlastTrade\x12\'\n\x0fsequence_number\x18\x05 \x01(\x04R\x0esequenceNumber"\x1d\n\x1bListLatestMarketDataRequest"S\n\x1cListLatestMarketDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"?\n\x1aGetLatestMarketDataRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"P\n\x1bGetLatestMarketDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\nmarketData"\x99\x02\n\x1fGetMarketDataHistoryByIDRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12,\n\x0fstart_timestamp\x18\x02 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x03 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestampB\r\n\x0b_paginationJ\x04\x08\x05\x10\x06"j\n GetMarketDataHistoryByIDResponse\x12\x46\n\x0bmarket_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.MarketDataConnectionR\nmarketData"N\n\x0eMarketDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14MarketDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.MarketDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd1\x01\n\x14ListTransfersRequest\x12\x1b\n\x06pubkey\x18\x01 \x01(\tH\x00R\x06pubkey\x88\x01\x01\x12@\n\tdirection\x18\x02 \x01(\x0e\x32".datanode.api.v2.TransferDirectionR\tdirection\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\t\n\x07_pubkeyB\r\n\x0b_pagination"Z\n\x15ListTransfersResponse\x12\x41\n\ttransfers\x18\x01 \x01(\x0b\x32#.datanode.api.v2.TransferConnectionR\ttransfers"T\n\x0cTransferEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12TransferConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.TransferEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x19\n\x17GetNetworkLimitsRequest"G\n\x18GetNetworkLimitsResponse\x12+\n\x06limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\x06limits"?\n\x1aListCandleIntervalsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"M\n\x12IntervalToCandleId\x12\x1a\n\x08interval\x18\x01 \x01(\tR\x08interval\x12\x1b\n\tcandle_id\x18\x02 \x01(\tR\x08\x63\x61ndleId"u\n\x1bListCandleIntervalsResponse\x12V\n\x15interval_to_candle_id\x18\x01 \x03(\x0b\x32#.datanode.api.v2.IntervalToCandleIdR\x12intervalToCandleId"\xa7\x01\n\x06\x43\x61ndle\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x1f\n\x0blast_update\x18\x02 \x01(\x03R\nlastUpdate\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume"=\n\x18ObserveCandleDataRequest\x12!\n\tcandle_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08\x63\x61ndleId"L\n\x19ObserveCandleDataResponse\x12/\n\x06\x63\x61ndle\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x06\x63\x61ndle"\xdb\x01\n\x15ListCandleDataRequest\x12!\n\tcandle_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08\x63\x61ndleId\x12%\n\x0e\x66rom_timestamp\x18\x02 \x01(\x03R\rfromTimestamp\x12!\n\x0cto_timestamp\x18\x03 \x01(\x03R\x0btoTimestamp\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_paginationJ\x04\x08\x04\x10\x05"Y\n\x16ListCandleDataResponse\x12?\n\x07\x63\x61ndles\x18\x01 \x01(\x0b\x32%.datanode.api.v2.CandleDataConnectionR\x07\x63\x61ndles"Q\n\nCandleEdge\x12+\n\x04node\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x14\x43\x61ndleDataConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.CandleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc6\x01\n\x10ListVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_idB\r\n\x0b_pagination"J\n\x11ListVotesResponse\x12\x35\n\x05votes\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.VoteConnectionR\x05votes"B\n\x08VoteEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"y\n\x0eVoteConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.VoteEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"x\n\x13ObserveVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_id"6\n\x14ObserveVotesResponse\x12\x1e\n\x04vote\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04vote"\xbd\x01\n*ListERC20MultiSigSignerAddedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"|\n+ListERC20MultiSigSignerAddedBundlesResponse\x12M\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedConnectionR\x07\x62undles"t\n\x1c\x45RC20MultiSigSignerAddedEdge\x12<\n\x04node\x18\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n"ERC20MultiSigSignerAddedBundleEdge\x12\x43\n\x04node\x18\x01 \x01(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xa7\x01\n"ERC20MultiSigSignerAddedConnection\x12I\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xce\x01\n\x1e\x45RC20MultiSigSignerAddedBundle\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"\xbf\x01\n,ListERC20MultiSigSignerRemovedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"\x80\x01\n-ListERC20MultiSigSignerRemovedBundlesResponse\x12O\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedConnectionR\x07\x62undles"x\n\x1e\x45RC20MultiSigSignerRemovedEdge\x12>\n\x04node\x18\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n$ERC20MultiSigSignerRemovedBundleEdge\x12\x45\n\x04node\x18\x01 \x01(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xab\x01\n$ERC20MultiSigSignerRemovedConnection\x12K\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd0\x01\n ERC20MultiSigSignerRemovedBundle\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"A\n\x1eGetERC20ListAssetBundleRequest\x12\x1f\n\x08\x61sset_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId"\x9e\x01\n\x1fGetERC20ListAssetBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x04 \x01(\tR\nsignatures"L\n#GetERC20SetAssetLimitsBundleRequest\x12%\n\x0bproposal_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\nproposalId"\xe8\x01\n$GetERC20SetAssetLimitsBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12%\n\x0elifetime_limit\x18\x04 \x01(\tR\rlifetimeLimit\x12\x1c\n\tthreshold\x18\x05 \x01(\tR\tthreshold\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures"N\n!GetERC20WithdrawalApprovalRequest\x12)\n\rwithdrawal_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0cwithdrawalId"\xde\x01\n"GetERC20WithdrawalApprovalResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x05 \x01(\tR\nsignatures\x12%\n\x0etarget_address\x18\x06 \x01(\tR\rtargetAddress\x12\x1a\n\x08\x63reation\x18\x07 \x01(\x03R\x08\x63reationJ\x04\x08\x03\x10\x04"8\n\x13GetLastTradeRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"9\n\x14GetLastTradeResponse\x12!\n\x05trade\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x05trade"\x8c\x02\n\x11ListTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds\x12\x1b\n\tparty_ids\x18\x03 \x03(\tR\x08partyIds\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x05 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"N\n\x12ListTradesResponse\x12\x38\n\x06trades\x18\x01 \x01(\x0b\x32 .datanode.api.v2.TradeConnectionR\x06trades"{\n\x0fTradeConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.TradeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tTradeEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"R\n\x14ObserveTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds"<\n\x15ObserveTradesResponse\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"B\n\x14GetOracleSpecRequest\x12*\n\x0eoracle_spec_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0coracleSpecId"J\n\x15GetOracleSpecResponse\x12\x31\n\x0boracle_spec\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\noracleSpec"i\n\x16ListOracleSpecsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"d\n\x17ListOracleSpecsResponse\x12I\n\x0coracle_specs\x18\x01 \x01(\x0b\x32&.datanode.api.v2.OracleSpecsConnectionR\x0boracleSpecs"\xa6\x01\n\x15ListOracleDataRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tH\x00R\x0coracleSpecId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x11\n\x0f_oracle_spec_idB\r\n\x0b_pagination"`\n\x16ListOracleDataResponse\x12\x46\n\x0boracle_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.OracleDataConnectionR\noracleData"N\n\x0eOracleSpecEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15OracleSpecsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleSpecEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"N\n\x0eOracleDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14OracleDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"5\n\x10GetMarketRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"9\n\x11GetMarketResponse\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market"\xa7\x01\n\x12ListMarketsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12,\n\x0finclude_settled\x18\x03 \x01(\x08H\x01R\x0eincludeSettled\x88\x01\x01\x42\r\n\x0b_paginationB\x12\n\x10_include_settled"R\n\x13ListMarketsResponse\x12;\n\x07markets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarketConnectionR\x07markets"F\n\nMarketEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarketConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xaf\x01\n\x1bListSuccessorMarketsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x30\n\x14include_full_history\x18\x02 \x01(\x08R\x12includeFullHistory\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"k\n\x0fSuccessorMarket\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x32\n\tproposals\x18\x02 \x03(\x0b\x32\x14.vega.GovernanceDataR\tproposals"c\n\x13SuccessorMarketEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .datanode.api.v2.SuccessorMarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8f\x01\n\x19SuccessorMarketConnection\x12:\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32$.datanode.api.v2.SuccessorMarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"d\n\x1cListSuccessorMarketsResponse\x12\x44\n\x07markets\x18\x01 \x01(\x0b\x32*.datanode.api.v2.SuccessorMarketConnectionR\x07markets"2\n\x0fGetPartyRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId"5\n\x10GetPartyResponse\x12!\n\x05party\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x05party"l\n\x12ListPartiesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12;\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"Q\n\x13ListPartiesResponse\x12:\n\x07parties\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PartyConnectionR\x07parties"D\n\tPartyEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"{\n\x0fPartyConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.PartyEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tOrderEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8e\x01\n\x17ListMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"b\n\x18ListMarginLevelsResponse\x12\x46\n\rmargin_levels\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarginConnectionR\x0cmarginLevels"g\n\x1aObserveMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12 \n\tmarket_id\x18\x02 \x01(\tH\x00R\x08marketId\x88\x01\x01\x42\x0c\n\n_market_id"V\n\x1bObserveMarginLevelsResponse\x12\x37\n\rmargin_levels\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"{\n\x0fOrderConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.OrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"L\n\nMarginEdge\x12&\n\x04node\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarginConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarginEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x8d\x02\n\x12ListRewardsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x12"\n\nfrom_epoch\x18\x04 \x01(\x04H\x02R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x05 \x01(\x04H\x03R\x07toEpoch\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_paginationB\r\n\x0b_from_epochB\x0b\n\t_to_epoch"S\n\x13ListRewardsResponse\x12<\n\x07rewards\x18\x01 \x01(\x0b\x32".datanode.api.v2.RewardsConnectionR\x07rewards"F\n\nRewardEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"~\n\x11RewardsConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.RewardEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc7\x01\n\x1aListRewardSummariesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\r\n\x0b_pagination"P\n\x1bListRewardSummariesResponse\x12\x31\n\tsummaries\x18\x01 \x03(\x0b\x32\x13.vega.RewardSummaryR\tsummaries"\xb1\x01\n\x13RewardSummaryFilter\x12\x1b\n\tasset_ids\x18\x01 \x03(\tR\x08\x61ssetIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds\x12"\n\nfrom_epoch\x18\x03 \x01(\x04H\x00R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x04 \x01(\x04H\x01R\x07toEpoch\x88\x01\x01\x42\r\n\x0b_from_epochB\x0b\n\t_to_epoch"\xb0\x01\n\x1fListEpochRewardSummariesRequest\x12<\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.datanode.api.v2.RewardSummaryFilterR\x06\x66ilter\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"o\n ListEpochRewardSummariesResponse\x12K\n\tsummaries\x18\x01 \x01(\x0b\x32-.datanode.api.v2.EpochRewardSummaryConnectionR\tsummaries"\x95\x01\n\x1c\x45pochRewardSummaryConnection\x12=\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\'.datanode.api.v2.EpochRewardSummaryEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"^\n\x16\x45pochRewardSummaryEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.EpochRewardSummaryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"q\n\x15ObserveRewardsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0b\n\t_asset_idB\x0b\n\t_party_id">\n\x16ObserveRewardsResponse\x12$\n\x06reward\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x06reward")\n\x11GetDepositRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"=\n\x12GetDepositResponse\x12\'\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"\xd0\x01\n\x13ListDepositsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"W\n\x14ListDepositsResponse\x12?\n\x08\x64\x65posits\x18\x01 \x01(\x0b\x32#.datanode.api.v2.DepositsConnectionR\x08\x64\x65posits"H\n\x0b\x44\x65positEdge\x12!\n\x04node\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x80\x01\n\x12\x44\x65positsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.DepositEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x14GetWithdrawalRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"I\n\x15GetWithdrawalResponse\x12\x30\n\nwithdrawal\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"\xd3\x01\n\x16ListWithdrawalsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"c\n\x17ListWithdrawalsResponse\x12H\n\x0bwithdrawals\x18\x01 \x01(\x0b\x32&.datanode.api.v2.WithdrawalsConnectionR\x0bwithdrawals"N\n\x0eWithdrawalEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15WithdrawalsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.WithdrawalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"2\n\x0fGetAssetRequest\x12\x1f\n\x08\x61sset_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId"5\n\x10GetAssetResponse\x12!\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x05\x61sset"\x91\x01\n\x11ListAssetsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"O\n\x12ListAssetsResponse\x12\x39\n\x06\x61ssets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.AssetsConnectionR\x06\x61ssets"D\n\tAssetEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"|\n\x10\x41ssetsConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.AssetEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xa1\x02\n\x1eListLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12\x17\n\x04live\x18\x04 \x01(\x08H\x03R\x04live\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x0c\n\n_referenceB\x07\n\x05_liveB\r\n\x0b_pagination"\x84\x01\n\x1fListLiquidityProvisionsResponse\x12\x61\n\x14liquidity_provisions\x18\x01 \x01(\x0b\x32..datanode.api.v2.LiquidityProvisionsConnectionR\x13liquidityProvisions"_\n\x17LiquidityProvisionsEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.LiquidityProvisionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x97\x01\n\x1dLiquidityProvisionsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.LiquidityProvisionsEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x80\x01\n!ObserveLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"q\n"ObserveLiquidityProvisionsResponse\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions"\x81\x01\n\x18GetGovernanceDataRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tH\x00R\nproposalId\x88\x01\x01\x12!\n\treference\x18\x02 \x01(\tH\x01R\treference\x88\x01\x01\x42\x0e\n\x0c_proposal_idB\x0c\n\n_reference"E\n\x19GetGovernanceDataResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xfa\x04\n\x19ListGovernanceDataRequest\x12@\n\x0eproposal_state\x18\x01 \x01(\x0e\x32\x14.vega.Proposal.StateH\x00R\rproposalState\x88\x01\x01\x12Y\n\rproposal_type\x18\x02 \x01(\x0e\x32/.datanode.api.v2.ListGovernanceDataRequest.TypeH\x01R\x0cproposalType\x88\x01\x01\x12/\n\x11proposer_party_id\x18\x03 \x01(\tH\x02R\x0fproposerPartyId\x88\x01\x01\x12\x32\n\x12proposal_reference\x18\x04 \x01(\tH\x03R\x11proposalReference\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01"\xb7\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_ALL\x10\x01\x12\x13\n\x0fTYPE_NEW_MARKET\x10\x02\x12\x16\n\x12TYPE_UPDATE_MARKET\x10\x03\x12\x1b\n\x17TYPE_NETWORK_PARAMETERS\x10\x04\x12\x12\n\x0eTYPE_NEW_ASSET\x10\x05\x12\x16\n\x12TYPE_NEW_FREE_FORM\x10\x06\x12\x15\n\x11TYPE_UPDATE_ASSET\x10\x07\x42\x11\n\x0f_proposal_stateB\x10\n\x0e_proposal_typeB\x14\n\x12_proposer_party_idB\x15\n\x13_proposal_referenceB\r\n\x0b_pagination"g\n\x1aListGovernanceDataResponse\x12I\n\nconnection\x18\x01 \x01(\x0b\x32).datanode.api.v2.GovernanceDataConnectionR\nconnection"V\n\x12GovernanceDataEdge\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x18GovernanceDataConnection\x12\x39\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32#.datanode.api.v2.GovernanceDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"G\n\x18ObserveGovernanceRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x42\x0b\n\t_party_id"E\n\x19ObserveGovernanceResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xed\x01\n\x16ListDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x12\x1e\n\x08\x65poch_id\x18\x03 \x01(\tH\x02R\x07\x65pochId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_idB\x0b\n\t_epoch_idB\r\n\x0b_pagination"c\n\x17ListDelegationsResponse\x12H\n\x0b\x64\x65legations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.DelegationsConnectionR\x0b\x64\x65legations"N\n\x0e\x44\x65legationEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x44\x65legationsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.DelegationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"r\n\x19ObserveDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_id"N\n\x1aObserveDelegationsResponse\x12\x30\n\ndelegation\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\ndelegation"\x91\x02\n\tNodeBasic\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x17\n\x15GetNetworkDataRequest"E\n\x16GetNetworkDataResponse\x12+\n\tnode_data\x18\x01 \x01(\x0b\x32\x0e.vega.NodeDataR\x08nodeData"&\n\x0eGetNodeRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"1\n\x0fGetNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node"\x93\x01\n\x10ListNodesRequest\x12 \n\tepoch_seq\x18\x01 \x01(\x04H\x00R\x08\x65pochSeq\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0c\n\n_epoch_seqB\r\n\x0b_pagination"K\n\x11ListNodesResponse\x12\x36\n\x05nodes\x18\x01 \x01(\x0b\x32 .datanode.api.v2.NodesConnectionR\x05nodes"B\n\x08NodeEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"z\n\x0fNodesConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.NodeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x82\x01\n\x19ListNodeSignaturesRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"g\n\x1aListNodeSignaturesResponse\x12I\n\nsignatures\x18\x01 \x01(\x0b\x32).datanode.api.v2.NodeSignaturesConnectionR\nsignatures"`\n\x11NodeSignatureEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8c\x01\n\x18NodeSignaturesConnection\x12\x38\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32".datanode.api.v2.NodeSignatureEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"R\n\x0fGetEpochRequest\x12\x13\n\x02id\x18\x01 \x01(\x04H\x00R\x02id\x88\x01\x01\x12\x19\n\x05\x62lock\x18\x02 \x01(\x04H\x01R\x05\x62lock\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_block"5\n\x10GetEpochResponse\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch"m\n\x12\x45stimateFeeRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x1a\n\x05price\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x05price\x12\x18\n\x04size\x18\x03 \x01(\x04\x42\x04\xe2\x41\x01\x02R\x04size"2\n\x13\x45stimateFeeResponse\x12\x1b\n\x03\x66\x65\x65\x18\x02 \x01(\x0b\x32\t.vega.FeeR\x03\x66\x65\x65"\xe7\x01\n\x15\x45stimateMarginRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x1f\n\x08party_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12$\n\x04side\x18\x03 \x01(\x0e\x32\n.vega.SideB\x04\xe2\x41\x01\x02R\x04side\x12*\n\x04type\x18\x04 \x01(\x0e\x32\x10.vega.Order.TypeB\x04\xe2\x41\x01\x02R\x04type\x12\x18\n\x04size\x18\x05 \x01(\x04\x42\x04\xe2\x41\x01\x02R\x04size\x12\x1a\n\x05price\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02R\x05price:\x02\x18\x01"U\n\x16\x45stimateMarginResponse\x12\x37\n\rmargin_levels\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels:\x02\x18\x01"o\n\x1cListNetworkParametersRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"{\n\x1dListNetworkParametersResponse\x12Z\n\x12network_parameters\x18\x01 \x01(\x0b\x32+.datanode.api.v2.NetworkParameterConnectionR\x11networkParameters"4\n\x1aGetNetworkParameterRequest\x12\x16\n\x03key\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x03key"b\n\x1bGetNetworkParameterResponse\x12\x43\n\x11network_parameter\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x10networkParameter"Z\n\x14NetworkParameterEdge\x12*\n\x04node\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x91\x01\n\x1aNetworkParameterConnection\x12;\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32%.datanode.api.v2.NetworkParameterEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\nCheckpoint\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12\x19\n\x08\x61t_block\x18\x03 \x01(\x04R\x07\x61tBlock"i\n\x16ListCheckpointsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"c\n\x17ListCheckpointsResponse\x12H\n\x0b\x63heckpoints\x18\x01 \x01(\x0b\x32&.datanode.api.v2.CheckpointsConnectionR\x0b\x63heckpoints"Y\n\x0e\x43heckpointEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.CheckpointR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x43heckpointsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.CheckpointEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x83\x01\n\x0fGetStakeRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"\x94\x01\n\x10GetStakeResponse\x12\x36\n\x17\x63urrent_stake_available\x18\x01 \x01(\tR\x15\x63urrentStakeAvailable\x12H\n\x0estake_linkings\x18\x02 \x01(\x0b\x32!.datanode.api.v2.StakesConnectionR\rstakeLinkings"\\\n\x10StakeLinkingEdge\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x10StakesConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.StakeLinkingEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo":\n\x15GetRiskFactorsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"K\n\x16GetRiskFactorsResponse\x12\x31\n\x0brisk_factor\x18\x01 \x01(\x0b\x32\x10.vega.RiskFactorR\nriskFactor"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x1f\n\x1dObserveLedgerMovementsRequest"_\n\x1eObserveLedgerMovementsResponse\x12=\n\x0fledger_movement\x18\x01 \x01(\x0b\x32\x14.vega.LedgerMovementR\x0eledgerMovement"\x94\x01\n\x17ListKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"`\n\x18ListKeyRotationsResponse\x12\x44\n\trotations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.KeyRotationConnectionR\trotations"Z\n\x0fKeyRotationEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x87\x01\n\x15KeyRotationConnection\x12\x36\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32 .datanode.api.v2.KeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9c\x01\n\x1fListEthereumKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"x\n ListEthereumKeyRotationsResponse\x12T\n\rkey_rotations\x18\x01 \x01(\x0b\x32/.datanode.api.v2.EthereumKeyRotationsConnectionR\x0ckeyRotations"\x98\x01\n\x1e\x45thereumKeyRotationsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.EthereumKeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"j\n\x17\x45thereumKeyRotationEdge\x12\x37\n\x04node\x18\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\x89\x01\n\tDateRange\x12,\n\x0fstart_timestamp\x18\x01 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x02 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestamp"!\n\x1fGetProtocolUpgradeStatusRequest"8\n GetProtocolUpgradeStatusResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready"\x83\x02\n#ListProtocolUpgradeProposalsRequest\x12J\n\x06status\x18\x01 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusH\x00R\x06status\x88\x01\x01\x12$\n\x0b\x61pproved_by\x18\x02 \x01(\tH\x01R\napprovedBy\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\t\n\x07_statusB\x0e\n\x0c_approved_byB\r\n\x0b_pagination"\x98\x01\n$ListProtocolUpgradeProposalsResponse\x12p\n\x1aprotocol_upgrade_proposals\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.ProtocolUpgradeProposalConnectionR\x18protocolUpgradeProposals"\x9f\x01\n!ProtocolUpgradeProposalConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.ProtocolUpgradeProposalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"o\n\x1bProtocolUpgradeProposalEdge\x12\x38\n\x04node\x18\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"k\n\x18ListCoreSnapshotsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"k\n\x19ListCoreSnapshotsResponse\x12N\n\x0e\x63ore_snapshots\x18\x01 \x01(\x0b\x32\'.datanode.api.v2.CoreSnapshotConnectionR\rcoreSnapshots"\x89\x01\n\x16\x43oreSnapshotConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.CoreSnapshotEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"`\n\x10\x43oreSnapshotEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x02\n\x0eHistorySegment\x12\x1f\n\x0b\x66rom_height\x18\x01 \x01(\x03R\nfromHeight\x12\x1b\n\tto_height\x18\x02 \x01(\x03R\x08toHeight\x12,\n\x12history_segment_id\x18\x03 \x01(\tR\x10historySegmentId\x12=\n\x1bprevious_history_segment_id\x18\x04 \x01(\tR\x18previousHistorySegmentId\x12)\n\x10\x64\x61tabase_version\x18\x05 \x01(\x03R\x0f\x64\x61tabaseVersion\x12\x19\n\x08\x63hain_id\x18\x06 \x01(\tR\x07\x63hainId"+\n)GetMostRecentNetworkHistorySegmentRequest"\x8d\x01\n*GetMostRecentNetworkHistorySegmentResponse\x12\x39\n\x07segment\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x07segment\x12$\n\x0eswarm_key_seed\x18\x02 \x01(\tR\x0cswarmKeySeed"&\n$ListAllNetworkHistorySegmentsRequest"d\n%ListAllNetworkHistorySegmentsResponse\x12;\n\x08segments\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x08segments"-\n+GetActiveNetworkHistoryPeerAddressesRequest"Q\n,GetActiveNetworkHistoryPeerAddressesResponse\x12!\n\x0cip_addresses\x18\x01 \x03(\tR\x0bipAddresses" \n\x1eGetNetworkHistoryStatusRequest"\xb0\x01\n\x1fGetNetworkHistoryStatusResponse\x12!\n\x0cipfs_address\x18\x01 \x01(\tR\x0bipfsAddress\x12\x1b\n\tswarm_key\x18\x02 \x01(\tR\x08swarmKey\x12$\n\x0eswarm_key_seed\x18\x03 \x01(\tR\x0cswarmKeySeed\x12\'\n\x0f\x63onnected_peers\x18\x05 \x03(\tR\x0e\x63onnectedPeers"(\n&GetNetworkHistoryBootstrapPeersRequest"R\n\'GetNetworkHistoryBootstrapPeersResponse\x12\'\n\x0f\x62ootstrap_peers\x18\x01 \x03(\tR\x0e\x62ootstrapPeers"\x85\x01\n\x1b\x45xportNetworkHistoryRequest\x12\x1d\n\nfrom_block\x18\x01 \x01(\x03R\tfromBlock\x12\x19\n\x08to_block\x18\x02 \x01(\x03R\x07toBlock\x12,\n\x05table\x18\x03 \x01(\x0e\x32\x16.datanode.api.v2.TableR\x05table"F\n\x13ListEntitiesRequest\x12/\n\x10transaction_hash\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0ftransactionHash"\xad\r\n\x14ListEntitiesResponse\x12)\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x08\x61\x63\x63ounts\x12#\n\x06orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12,\n\tpositions\x18\x03 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x38\n\x0eledger_entries\x18\x04 \x03(\x0b\x32\x11.vega.LedgerEntryR\rledgerEntries\x12H\n\x0f\x62\x61lance_changes\x18\x05 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x0e\x62\x61lanceChanges\x12\x36\n\ttransfers\x18\x06 \x03(\x0b\x32\x18.vega.events.v1.TransferR\ttransfers\x12 \n\x05votes\x18\x07 \x03(\x0b\x32\n.vega.VoteR\x05votes\x12~\n$erc20_multi_sig_signer_added_bundles\x18\x08 \x03(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x1f\x65rc20MultiSigSignerAddedBundles\x12\x84\x01\n&erc20_multi_sig_signer_removed_bundles\x18\t \x03(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR!erc20MultiSigSignerRemovedBundles\x12#\n\x06trades\x18\n \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x33\n\x0coracle_specs\x18\x0b \x03(\x0b\x32\x10.vega.OracleSpecR\x0boracleSpecs\x12\x31\n\x0boracle_data\x18\x0c \x03(\x0b\x32\x10.vega.OracleDataR\noracleData\x12&\n\x07markets\x18\r \x03(\x0b\x32\x0c.vega.MarketR\x07markets\x12%\n\x07parties\x18\x0e \x03(\x0b\x32\x0b.vega.PartyR\x07parties\x12\x37\n\rmargin_levels\x18\x0f \x03(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels\x12&\n\x07rewards\x18\x10 \x03(\x0b\x32\x0c.vega.RewardR\x07rewards\x12)\n\x08\x64\x65posits\x18\x11 \x03(\x0b\x32\r.vega.DepositR\x08\x64\x65posits\x12\x32\n\x0bwithdrawals\x18\x12 \x03(\x0b\x32\x10.vega.WithdrawalR\x0bwithdrawals\x12#\n\x06\x61ssets\x18\x13 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets\x12K\n\x14liquidity_provisions\x18\x14 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions\x12,\n\tproposals\x18\x15 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals\x12\x32\n\x0b\x64\x65legations\x18\x16 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x30\n\x05nodes\x18\x17 \x03(\x0b\x32\x1a.datanode.api.v2.NodeBasicR\x05nodes\x12H\n\x0fnode_signatures\x18\x18 \x03(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x0enodeSignatures\x12\x45\n\x12network_parameters\x18\x19 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters\x12@\n\rkey_rotations\x18\x1a \x03(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x0ckeyRotations\x12Y\n\x16\x65thereum_key_rotations\x18\x1b \x03(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x14\x65thereumKeyRotations\x12\x62\n\x1aprotocol_upgrade_proposals\x18\x1c \x03(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x18protocolUpgradeProposals"\r\n\x0bPingRequest"\x0e\n\x0cPingResponse"\x87\x01\n\tOrderInfo\x12\x1e\n\x04side\x18\x01 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x1c\n\tremaining\x18\x03 \x01(\x04R\tremaining\x12&\n\x0fis_market_order\x18\x04 \x01(\x08R\risMarketOrder"\xe8\x01\n\x17\x45stimatePositionRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12%\n\x0bopen_volume\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02R\nopenVolume\x12\x32\n\x06orders\x18\x03 \x03(\x0b\x32\x1a.datanode.api.v2.OrderInfoR\x06orders\x12\x36\n\x14\x63ollateral_available\x18\x04 \x01(\tH\x00R\x13\x63ollateralAvailable\x88\x01\x01\x42\x17\n\x15_collateral_available"\x9b\x01\n\x18\x45stimatePositionResponse\x12\x37\n\x06margin\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.MarginEstimateR\x06margin\x12\x46\n\x0bliquidation\x18\x02 \x01(\x0b\x32$.datanode.api.v2.LiquidationEstimateR\x0bliquidation"t\n\x0eMarginEstimate\x12\x31\n\nworst_case\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\tworstCase\x12/\n\tbest_case\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x08\x62\x65stCase"\x97\x01\n\x13LiquidationEstimate\x12@\n\nworst_case\x18\x01 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\tworstCase\x12>\n\tbest_case\x18\x02 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\x08\x62\x65stCase"\xa2\x01\n\x10LiquidationPrice\x12(\n\x10open_volume_only\x18\x01 \x01(\tR\x0eopenVolumeOnly\x12\x30\n\x14including_buy_orders\x18\x02 \x01(\tR\x12includingBuyOrders\x12\x32\n\x15including_sell_orders\x18\x03 \x01(\tR\x13includingSellOrders*\xaa\x01\n\x10LedgerEntryField\x12"\n\x1eLEDGER_ENTRY_FIELD_UNSPECIFIED\x10\x00\x12&\n"LEDGER_ENTRY_FIELD_ACCOUNT_FROM_ID\x10\x01\x12$\n LEDGER_ENTRY_FIELD_ACCOUNT_TO_ID\x10\x02\x12$\n LEDGER_ENTRY_FIELD_TRANSFER_TYPE\x10\x03*\xb0\x01\n\x0c\x41\x63\x63ountField\x12\x1d\n\x19\x41\x43\x43OUNT_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_FIELD_ID\x10\x01\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_PARTY_ID\x10\x02\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_ASSET_ID\x10\x03\x12\x1b\n\x17\x41\x43\x43OUNT_FIELD_MARKET_ID\x10\x04\x12\x16\n\x12\x41\x43\x43OUNT_FIELD_TYPE\x10\x05*\xad\x01\n\x11TransferDirection\x12"\n\x1eTRANSFER_DIRECTION_UNSPECIFIED\x10\x00\x12$\n TRANSFER_DIRECTION_TRANSFER_FROM\x10\x01\x12"\n\x1eTRANSFER_DIRECTION_TRANSFER_TO\x10\x02\x12*\n&TRANSFER_DIRECTION_TRANSFER_TO_OR_FROM\x10\x03*\xde\x02\n\x05Table\x12\x15\n\x11TABLE_UNSPECIFIED\x10\x00\x12\x12\n\x0eTABLE_BALANCES\x10\x01\x12\x15\n\x11TABLE_CHECKPOINTS\x10\x02\x12\x15\n\x11TABLE_DELEGATIONS\x10\x03\x12\x10\n\x0cTABLE_LEDGER\x10\x04\x12\x10\n\x0cTABLE_ORDERS\x10\x05\x12\x10\n\x0cTABLE_TRADES\x10\x06\x12\x15\n\x11TABLE_MARKET_DATA\x10\x07\x12\x17\n\x13TABLE_MARGIN_LEVELS\x10\x08\x12\x13\n\x0fTABLE_POSITIONS\x10\t\x12\x1e\n\x1aTABLE_LIQUIDITY_PROVISIONS\x10\n\x12\x11\n\rTABLE_MARKETS\x10\x0b\x12\x12\n\x0eTABLE_DEPOSITS\x10\x0c\x12\x15\n\x11TABLE_WITHDRAWALS\x10\r\x12\x10\n\x0cTABLE_BLOCKS\x10\x0e\x12\x11\n\rTABLE_REWARDS\x10\x0f\x32\x98V\n\x12TradingDataService\x12j\n\x0cListAccounts\x12$.datanode.api.v2.ListAccountsRequest\x1a%.datanode.api.v2.ListAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12u\n\x0fObserveAccounts\x12\'.datanode.api.v2.ObserveAccountsRequest\x1a(.datanode.api.v2.ObserveAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts0\x01\x12Z\n\x04Info\x12\x1c.datanode.api.v2.InfoRequest\x1a\x1d.datanode.api.v2.InfoResponse"\x15\x92\x41\x12\n\x10Node information\x12\\\n\x08GetOrder\x12 .datanode.api.v2.GetOrderRequest\x1a!.datanode.api.v2.GetOrderResponse"\x0b\x92\x41\x08\n\x06Orders\x12\x62\n\nListOrders\x12".datanode.api.v2.ListOrdersRequest\x1a#.datanode.api.v2.ListOrdersResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x11ListOrderVersions\x12).datanode.api.v2.ListOrderVersionsRequest\x1a*.datanode.api.v2.ListOrderVersionsResponse"\x0b\x92\x41\x08\n\x06Orders\x12m\n\rObserveOrders\x12%.datanode.api.v2.ObserveOrdersRequest\x1a&.datanode.api.v2.ObserveOrdersResponse"\x0b\x92\x41\x08\n\x06Orders0\x01\x12q\n\rListPositions\x12%.datanode.api.v2.ListPositionsRequest\x1a&.datanode.api.v2.ListPositionsResponse"\x11\x88\x02\x01\x92\x41\x0b\n\tPositions\x12w\n\x10ListAllPositions\x12(.datanode.api.v2.ListAllPositionsRequest\x1a).datanode.api.v2.ListAllPositionsResponse"\x0e\x92\x41\x0b\n\tPositions\x12y\n\x10ObservePositions\x12(.datanode.api.v2.ObservePositionsRequest\x1a).datanode.api.v2.ObservePositionsResponse"\x0e\x92\x41\x0b\n\tPositions0\x01\x12\x7f\n\x11ListLedgerEntries\x12).datanode.api.v2.ListLedgerEntriesRequest\x1a*.datanode.api.v2.ListLedgerEntriesResponse"\x13\x92\x41\x10\n\x0eLedger entries\x12o\n\x13\x45xportLedgerEntries\x12+.datanode.api.v2.ExportLedgerEntriesRequest\x1a\x14.google.api.HttpBody"\x13\x92\x41\x10\n\x0eLedger entries0\x01\x12|\n\x12ListBalanceChanges\x12*.datanode.api.v2.ListBalanceChangesRequest\x1a+.datanode.api.v2.ListBalanceChangesResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12~\n\x13GetLatestMarketData\x12+.datanode.api.v2.GetLatestMarketDataRequest\x1a,.datanode.api.v2.GetLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListLatestMarketData\x12,.datanode.api.v2.ListLatestMarketDataRequest\x1a-.datanode.api.v2.ListLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14GetLatestMarketDepth\x12,.datanode.api.v2.GetLatestMarketDepthRequest\x1a-.datanode.api.v2.GetLatestMarketDepthResponse"\x0c\x92\x41\t\n\x07Markets\x12\x80\x01\n\x13ObserveMarketsDepth\x12+.datanode.api.v2.ObserveMarketsDepthRequest\x1a,.datanode.api.v2.ObserveMarketsDepthResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x95\x01\n\x1aObserveMarketsDepthUpdates\x12\x32.datanode.api.v2.ObserveMarketsDepthUpdatesRequest\x1a\x33.datanode.api.v2.ObserveMarketsDepthUpdatesResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12}\n\x12ObserveMarketsData\x12*.datanode.api.v2.ObserveMarketsDataRequest\x1a+.datanode.api.v2.ObserveMarketsDataResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x8d\x01\n\x18GetMarketDataHistoryByID\x12\x30.datanode.api.v2.GetMarketDataHistoryByIDRequest\x1a\x31.datanode.api.v2.GetMarketDataHistoryByIDResponse"\x0c\x92\x41\t\n\x07Markets\x12n\n\rListTransfers\x12%.datanode.api.v2.ListTransfersRequest\x1a&.datanode.api.v2.ListTransfersResponse"\x0e\x92\x41\x0b\n\tTransfers\x12u\n\x10GetNetworkLimits\x12(.datanode.api.v2.GetNetworkLimitsRequest\x1a).datanode.api.v2.GetNetworkLimitsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eListCandleData\x12&.datanode.api.v2.ListCandleDataRequest\x1a\'.datanode.api.v2.ListCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12z\n\x11ObserveCandleData\x12).datanode.api.v2.ObserveCandleDataRequest\x1a*.datanode.api.v2.ObserveCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles0\x01\x12~\n\x13ListCandleIntervals\x12+.datanode.api.v2.ListCandleIntervalsRequest\x1a,.datanode.api.v2.ListCandleIntervalsResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12\x63\n\tListVotes\x12!.datanode.api.v2.ListVotesRequest\x1a".datanode.api.v2.ListVotesResponse"\x0f\x92\x41\x0c\n\nGovernance\x12n\n\x0cObserveVotes\x12$.datanode.api.v2.ObserveVotesRequest\x1a%.datanode.api.v2.ObserveVotesResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12\xb3\x01\n#ListERC20MultiSigSignerAddedBundles\x12;.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesRequest\x1a<.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\xb9\x01\n%ListERC20MultiSigSignerRemovedBundles\x12=.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesRequest\x1a>.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x8f\x01\n\x17GetERC20ListAssetBundle\x12/.datanode.api.v2.GetERC20ListAssetBundleRequest\x1a\x30.datanode.api.v2.GetERC20ListAssetBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x9e\x01\n\x1cGetERC20SetAssetLimitsBundle\x12\x34.datanode.api.v2.GetERC20SetAssetLimitsBundleRequest\x1a\x35.datanode.api.v2.GetERC20SetAssetLimitsBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x98\x01\n\x1aGetERC20WithdrawalApproval\x12\x32.datanode.api.v2.GetERC20WithdrawalApprovalRequest\x1a\x33.datanode.api.v2.GetERC20WithdrawalApprovalResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12h\n\x0cGetLastTrade\x12$.datanode.api.v2.GetLastTradeRequest\x1a%.datanode.api.v2.GetLastTradeResponse"\x0b\x92\x41\x08\n\x06Trades\x12\x62\n\nListTrades\x12".datanode.api.v2.ListTradesRequest\x1a#.datanode.api.v2.ListTradesResponse"\x0b\x92\x41\x08\n\x06Trades\x12m\n\rObserveTrades\x12%.datanode.api.v2.ObserveTradesRequest\x1a&.datanode.api.v2.ObserveTradesResponse"\x0b\x92\x41\x08\n\x06Trades0\x01\x12q\n\rGetOracleSpec\x12%.datanode.api.v2.GetOracleSpecRequest\x1a&.datanode.api.v2.GetOracleSpecResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12w\n\x0fListOracleSpecs\x12\'.datanode.api.v2.ListOracleSpecsRequest\x1a(.datanode.api.v2.ListOracleSpecsResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12t\n\x0eListOracleData\x12&.datanode.api.v2.ListOracleDataRequest\x1a\'.datanode.api.v2.ListOracleDataResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12`\n\tGetMarket\x12!.datanode.api.v2.GetMarketRequest\x1a".datanode.api.v2.GetMarketResponse"\x0c\x92\x41\t\n\x07Markets\x12\x66\n\x0bListMarkets\x12#.datanode.api.v2.ListMarketsRequest\x1a$.datanode.api.v2.ListMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListSuccessorMarkets\x12,.datanode.api.v2.ListSuccessorMarketsRequest\x1a-.datanode.api.v2.ListSuccessorMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12]\n\x08GetParty\x12 .datanode.api.v2.GetPartyRequest\x1a!.datanode.api.v2.GetPartyResponse"\x0c\x92\x41\t\n\x07Parties\x12\x66\n\x0bListParties\x12#.datanode.api.v2.ListPartiesRequest\x1a$.datanode.api.v2.ListPartiesResponse"\x0c\x92\x41\t\n\x07Parties\x12{\n\x10ListMarginLevels\x12(.datanode.api.v2.ListMarginLevelsRequest\x1a).datanode.api.v2.ListMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels\x12\x86\x01\n\x13ObserveMarginLevels\x12+.datanode.api.v2.ObserveMarginLevelsRequest\x1a,.datanode.api.v2.ObserveMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels0\x01\x12\x66\n\x0bListRewards\x12#.datanode.api.v2.ListRewardsRequest\x1a$.datanode.api.v2.ListRewardsResponse"\x0c\x92\x41\t\n\x07Rewards\x12~\n\x13ListRewardSummaries\x12+.datanode.api.v2.ListRewardSummariesRequest\x1a,.datanode.api.v2.ListRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x8d\x01\n\x18ListEpochRewardSummaries\x12\x30.datanode.api.v2.ListEpochRewardSummariesRequest\x1a\x31.datanode.api.v2.ListEpochRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x62\n\nGetDeposit\x12".datanode.api.v2.GetDepositRequest\x1a#.datanode.api.v2.GetDepositResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12h\n\x0cListDeposits\x12$.datanode.api.v2.ListDepositsRequest\x1a%.datanode.api.v2.ListDepositsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12k\n\rGetWithdrawal\x12%.datanode.api.v2.GetWithdrawalRequest\x1a&.datanode.api.v2.GetWithdrawalResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12q\n\x0fListWithdrawals\x12\'.datanode.api.v2.ListWithdrawalsRequest\x1a(.datanode.api.v2.ListWithdrawalsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\\\n\x08GetAsset\x12 .datanode.api.v2.GetAssetRequest\x1a!.datanode.api.v2.GetAssetResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x62\n\nListAssets\x12".datanode.api.v2.ListAssetsRequest\x1a#.datanode.api.v2.ListAssetsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x97\x01\n\x17ListLiquidityProvisions\x12/.datanode.api.v2.ListLiquidityProvisionsRequest\x1a\x30.datanode.api.v2.ListLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions\x12\xa2\x01\n\x1aObserveLiquidityProvisions\x12\x32.datanode.api.v2.ObserveLiquidityProvisionsRequest\x1a\x33.datanode.api.v2.ObserveLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions0\x01\x12{\n\x11GetGovernanceData\x12).datanode.api.v2.GetGovernanceDataRequest\x1a*.datanode.api.v2.GetGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12~\n\x12ListGovernanceData\x12*.datanode.api.v2.ListGovernanceDataRequest\x1a+.datanode.api.v2.ListGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12}\n\x11ObserveGovernance\x12).datanode.api.v2.ObserveGovernanceRequest\x1a*.datanode.api.v2.ObserveGovernanceResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12r\n\x0fListDelegations\x12\'.datanode.api.v2.ListDelegationsRequest\x1a(.datanode.api.v2.ListDelegationsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetNetworkData\x12&.datanode.api.v2.GetNetworkDataRequest\x1a\'.datanode.api.v2.GetNetworkDataResponse"\x0c\x92\x41\t\n\x07Network\x12Z\n\x07GetNode\x12\x1f.datanode.api.v2.GetNodeRequest\x1a .datanode.api.v2.GetNodeResponse"\x0c\x92\x41\t\n\x07Network\x12`\n\tListNodes\x12!.datanode.api.v2.ListNodesRequest\x1a".datanode.api.v2.ListNodesResponse"\x0c\x92\x41\t\n\x07Network\x12\x80\x01\n\x12ListNodeSignatures\x12*.datanode.api.v2.ListNodeSignaturesRequest\x1a+.datanode.api.v2.ListNodeSignaturesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12]\n\x08GetEpoch\x12 .datanode.api.v2.GetEpochRequest\x1a!.datanode.api.v2.GetEpochResponse"\x0c\x92\x41\t\n\x07Network\x12\x65\n\x0b\x45stimateFee\x12#.datanode.api.v2.EstimateFeeRequest\x1a$.datanode.api.v2.EstimateFeeResponse"\x0b\x92\x41\x08\n\x06Orders\x12n\n\x0e\x45stimateMargin\x12&.datanode.api.v2.EstimateMarginRequest\x1a\'.datanode.api.v2.EstimateMarginResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x10\x45stimatePosition\x12(.datanode.api.v2.EstimatePositionRequest\x1a).datanode.api.v2.EstimatePositionResponse"\x0e\x92\x41\x0b\n\tPositions\x12\x84\x01\n\x15ListNetworkParameters\x12-.datanode.api.v2.ListNetworkParametersRequest\x1a..datanode.api.v2.ListNetworkParametersResponse"\x0c\x92\x41\t\n\x07Network\x12~\n\x13GetNetworkParameter\x12+.datanode.api.v2.GetNetworkParameterRequest\x1a,.datanode.api.v2.GetNetworkParameterResponse"\x0c\x92\x41\t\n\x07Network\x12r\n\x0fListCheckpoints\x12\'.datanode.api.v2.ListCheckpointsRequest\x1a(.datanode.api.v2.ListCheckpointsResponse"\x0c\x92\x41\t\n\x07Network\x12]\n\x08GetStake\x12 .datanode.api.v2.GetStakeRequest\x1a!.datanode.api.v2.GetStakeResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetRiskFactors\x12&.datanode.api.v2.GetRiskFactorsRequest\x1a\'.datanode.api.v2.GetRiskFactorsResponse"\x0c\x92\x41\t\n\x07Markets\x12u\n\x0fObserveEventBus\x12\'.datanode.api.v2.ObserveEventBusRequest\x1a(.datanode.api.v2.ObserveEventBusResponse"\x0b\x92\x41\x08\n\x06\x45vents(\x01\x30\x01\x12\x92\x01\n\x16ObserveLedgerMovements\x12..datanode.api.v2.ObserveLedgerMovementsRequest\x1a/.datanode.api.v2.ObserveLedgerMovementsResponse"\x15\x92\x41\x12\n\x10Ledger movements0\x01\x12u\n\x10ListKeyRotations\x12(.datanode.api.v2.ListKeyRotationsRequest\x1a).datanode.api.v2.ListKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18ListEthereumKeyRotations\x12\x30.datanode.api.v2.ListEthereumKeyRotationsRequest\x1a\x31.datanode.api.v2.ListEthereumKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x66\n\x0bGetVegaTime\x12#.datanode.api.v2.GetVegaTimeRequest\x1a$.datanode.api.v2.GetVegaTimeResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18GetProtocolUpgradeStatus\x12\x30.datanode.api.v2.GetProtocolUpgradeStatusRequest\x1a\x31.datanode.api.v2.GetProtocolUpgradeStatusResponse"\x0c\x92\x41\t\n\x07Network\x12\x99\x01\n\x1cListProtocolUpgradeProposals\x12\x34.datanode.api.v2.ListProtocolUpgradeProposalsRequest\x1a\x35.datanode.api.v2.ListProtocolUpgradeProposalsResponse"\x0c\x92\x41\t\n\x07Network\x12x\n\x11ListCoreSnapshots\x12).datanode.api.v2.ListCoreSnapshotsRequest\x1a*.datanode.api.v2.ListCoreSnapshotsResponse"\x0c\x92\x41\t\n\x07Network\x12\xb3\x01\n"GetMostRecentNetworkHistorySegment\x12:.datanode.api.v2.GetMostRecentNetworkHistorySegmentRequest\x1a;.datanode.api.v2.GetMostRecentNetworkHistorySegmentResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xa4\x01\n\x1dListAllNetworkHistorySegments\x12\x35.datanode.api.v2.ListAllNetworkHistorySegmentsRequest\x1a\x36.datanode.api.v2.ListAllNetworkHistorySegmentsResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xb9\x01\n$GetActiveNetworkHistoryPeerAddresses\x12<.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesRequest\x1a=.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\x92\x01\n\x17GetNetworkHistoryStatus\x12/.datanode.api.v2.GetNetworkHistoryStatusRequest\x1a\x30.datanode.api.v2.GetNetworkHistoryStatusResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xaa\x01\n\x1fGetNetworkHistoryBootstrapPeers\x12\x37.datanode.api.v2.GetNetworkHistoryBootstrapPeersRequest\x1a\x38.datanode.api.v2.GetNetworkHistoryBootstrapPeersResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12j\n\x0cListEntities\x12$.datanode.api.v2.ListEntitiesRequest\x1a%.datanode.api.v2.ListEntitiesResponse"\r\x92\x41\n\n\x08\x45xplorer\x12r\n\x14\x45xportNetworkHistory\x12,.datanode.api.v2.ExportNetworkHistoryRequest\x1a\x14.google.api.HttpBody"\x14\x92\x41\x11\n\x0fNetwork history0\x01\x12N\n\x04Ping\x12\x1c.datanode.api.v2.PingRequest\x1a\x1d.datanode.api.v2.PingResponse"\t\x92\x41\x06\n\x04MiscB\xc6\x01Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\x92\x41\x8f\x01\x12\x1e\n\x13Vega data node APIs2\x07v0.71.0\x1a\x1chttps://api.testnet.vega.xyz*\x02\x01\x02\x32\x10\x61pplication/jsonR9\n\x03\x35\x30\x30\x12\x32\n\x18\x41n internal server error\x12\x16\n\x14\x1a\x12.google.rpc.Statusb\x06proto3'
+    b'\n#data-node/api/v2/trading_data.proto\x12\x0f\x64\x61tanode.api.v2\x1a\x1fgoogle/api/field_behavior.proto\x1a\x19google/api/httpbody.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\xd9\x01\n\nPagination\x12\x19\n\x05\x66irst\x18\x01 \x01(\x05H\x00R\x05\x66irst\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x02 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12\x17\n\x04last\x18\x03 \x01(\x05H\x02R\x04last\x88\x01\x01\x12\x1b\n\x06\x62\x65\x66ore\x18\x04 \x01(\tH\x03R\x06\x62\x65\x66ore\x88\x01\x01\x12&\n\x0cnewest_first\x18\x05 \x01(\x08H\x04R\x0bnewestFirst\x88\x01\x01\x42\x08\n\x06_firstB\x08\n\x06_afterB\x07\n\x05_lastB\t\n\x07_beforeB\x0f\n\r_newest_first"\x9c\x01\n\x08PageInfo\x12"\n\rhas_next_page\x18\x01 \x01(\x08R\x0bhasNextPage\x12*\n\x11has_previous_page\x18\x02 \x01(\x08R\x0fhasPreviousPage\x12!\n\x0cstart_cursor\x18\x03 \x01(\tR\x0bstartCursor\x12\x1d\n\nend_cursor\x18\x04 \x01(\tR\tendCursor"\x9a\x01\n\x0e\x41\x63\x63ountBalance\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\x9e\x01\n\x13ListAccountsRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"W\n\x14ListAccountsResponse\x12?\n\x08\x61\x63\x63ounts\x18\x01 \x01(\x0b\x32#.datanode.api.v2.AccountsConnectionR\x08\x61\x63\x63ounts"\x80\x01\n\x12\x41\x63\x63ountsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.AccountEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\x0b\x41\x63\x63ountEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x16ObserveAccountsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12%\n\x04type\x18\x04 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\xa6\x01\n\x17ObserveAccountsResponse\x12\x42\n\x08snapshot\x18\x01 \x01(\x0b\x32$.datanode.api.v2.AccountSnapshotPageH\x00R\x08snapshot\x12;\n\x07updates\x18\x02 \x01(\x0b\x32\x1f.datanode.api.v2.AccountUpdatesH\x00R\x07updatesB\n\n\x08response"o\n\x13\x41\x63\x63ountSnapshotPage\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"M\n\x0e\x41\x63\x63ountUpdates\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"]\n\x0fGetOrderRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId\x12\x1d\n\x07version\x18\x02 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version"5\n\x10GetOrderResponse\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xbd\x03\n\x0bOrderFilter\x12.\n\x08statuses\x18\x01 \x03(\x0e\x32\x12.vega.Order.StatusR\x08statuses\x12&\n\x05types\x18\x02 \x03(\x0e\x32\x10.vega.Order.TypeR\x05types\x12=\n\x0etime_in_forces\x18\x03 \x03(\x0e\x32\x17.vega.Order.TimeInForceR\x0ctimeInForces\x12+\n\x11\x65xclude_liquidity\x18\x04 \x01(\x08R\x10\x65xcludeLiquidity\x12\x1b\n\tparty_ids\x18\x05 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x06 \x03(\tR\tmarketIds\x12!\n\treference\x18\x07 \x01(\tH\x00R\treference\x88\x01\x01\x12>\n\ndate_range\x18\x08 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x12 \n\tlive_only\x18\t \x01(\x08H\x02R\x08liveOnly\x88\x01\x01\x42\x0c\n\n_referenceB\r\n\x0b_date_rangeB\x0c\n\n_live_only"\xaa\x01\n\x11ListOrdersRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12\x39\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x1c.datanode.api.v2.OrderFilterH\x01R\x06\x66ilter\x88\x01\x01\x42\r\n\x0b_paginationB\t\n\x07_filter"N\n\x12ListOrdersResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x8c\x01\n\x18ListOrderVersionsRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"U\n\x19ListOrderVersionsResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x9a\x01\n\x14ObserveOrdersRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x30\n\x11\x65xclude_liquidity\x18\x03 \x01(\x08H\x00R\x10\x65xcludeLiquidity\x88\x01\x01\x42\x14\n\x12_exclude_liquidity"\xa0\x01\n\x15ObserveOrdersResponse\x12@\n\x08snapshot\x18\x01 \x01(\x0b\x32".datanode.api.v2.OrderSnapshotPageH\x00R\x08snapshot\x12\x39\n\x07updates\x18\x02 \x01(\x0b\x32\x1d.datanode.api.v2.OrderUpdatesH\x00R\x07updatesB\n\n\x08response"U\n\x11OrderSnapshotPage\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"3\n\x0cOrderUpdates\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"6\n\x13GetStopOrderRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId"L\n\x14GetStopOrderResponse\x12\x34\n\x05order\x18\x01 \x01(\x0b\x32\x1e.vega.events.v1.StopOrderEventR\x05order"\xb2\x01\n\x15ListStopOrdersRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12=\n\x06\x66ilter\x18\x05 \x01(\x0b\x32 .datanode.api.v2.StopOrderFilterH\x01R\x06\x66ilter\x88\x01\x01\x42\r\n\x0b_paginationB\t\n\x07_filter"\x9d\x02\n\x0fStopOrderFilter\x12\x32\n\x08statuses\x18\x01 \x03(\x0e\x32\x16.vega.StopOrder.StatusR\x08statuses\x12K\n\x11\x65xpiry_strategies\x18\x02 \x03(\x0e\x32\x1e.vega.StopOrder.ExpiryStrategyR\x10\x65xpiryStrategies\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x00R\tdateRange\x88\x01\x01\x12\x1b\n\tparty_ids\x18\x04 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x05 \x03(\tR\tmarketIdsB\r\n\x0b_date_range"[\n\rStopOrderEdge\x12\x32\n\x04node\x18\x01 \x01(\x0b\x32\x1e.vega.events.v1.StopOrderEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x13StopOrderConnection\x12\x34\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1e.datanode.api.v2.StopOrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"V\n\x16ListStopOrdersResponse\x12<\n\x06orders\x18\x01 \x01(\x0b\x32$.datanode.api.v2.StopOrderConnectionR\x06orders"\xa3\x01\n\x14ListPositionsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01:\x02\x18\x01\x42\r\n\x0b_pagination"^\n\x15ListPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions:\x02\x18\x01"M\n\x0fPositionsFilter\x12\x1b\n\tparty_ids\x18\x01 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds"\xa4\x01\n\x17ListAllPositionsRequest\x12\x38\n\x06\x66ilter\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PositionsFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"]\n\x18ListAllPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions"J\n\x0cPositionEdge\x12"\n\x04node\x18\x01 \x01(\x0b\x32\x0e.vega.PositionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12PositionConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.PositionEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"v\n\x17ObservePositionsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_id"\xa9\x01\n\x18ObservePositionsResponse\x12\x43\n\x08snapshot\x18\x01 \x01(\x0b\x32%.datanode.api.v2.PositionSnapshotPageH\x00R\x08snapshot\x12<\n\x07updates\x18\x02 \x01(\x0b\x32 .datanode.api.v2.PositionUpdatesH\x00R\x07updatesB\n\n\x08response"a\n\x14PositionSnapshotPage\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"?\n\x0fPositionUpdates\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions"\xa3\x02\n\x11LedgerEntryFilter\x12\x37\n\x18\x63lose_on_account_filters\x18\x01 \x01(\x08R\x15\x63loseOnAccountFilters\x12N\n\x13\x66rom_account_filter\x18\x02 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x11\x66romAccountFilter\x12J\n\x11to_account_filter\x18\x03 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x0ftoAccountFilter\x12\x39\n\x0etransfer_types\x18\x05 \x03(\x0e\x32\x12.vega.TransferTypeR\rtransferTypes"\xd9\x05\n\x15\x41ggregatedLedgerEntry\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x1a\n\x08quantity\x18\x03 \x01(\tR\x08quantity\x12\x37\n\rtransfer_type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x0ctransferType\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12=\n\x11\x66rom_account_type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x39\n\x0fto_account_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x36\n\x15\x66rom_account_party_id\x18\x08 \x01(\tH\x01R\x12\x66romAccountPartyId\x88\x01\x01\x12\x32\n\x13to_account_party_id\x18\t \x01(\tH\x02R\x10toAccountPartyId\x88\x01\x01\x12\x38\n\x16\x66rom_account_market_id\x18\n \x01(\tH\x03R\x13\x66romAccountMarketId\x88\x01\x01\x12\x34\n\x14to_account_market_id\x18\x0b \x01(\tH\x04R\x11toAccountMarketId\x88\x01\x01\x12\x30\n\x14\x66rom_account_balance\x18\x0c \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\r \x01(\tR\x10toAccountBalanceB\x0b\n\t_asset_idB\x18\n\x16_from_account_party_idB\x16\n\x14_to_account_party_idB\x19\n\x17_from_account_market_idB\x17\n\x15_to_account_market_idJ\x04\x08\x01\x10\x02"\xf6\x01\n\x18ListLedgerEntriesRequest\x12:\n\x06\x66ilter\x18\x01 \x01(\x0b\x32".datanode.api.v2.LedgerEntryFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"\xad\x01\n\x1a\x45xportLedgerEntriesRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12\x1f\n\x08\x61sset_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x00R\tdateRange\x88\x01\x01\x42\r\n\x0b_date_range"v\n\x19ListLedgerEntriesResponse\x12Y\n\x0eledger_entries\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.AggregatedLedgerEntriesConnectionR\rledgerEntries"q\n\x1b\x41ggregatedLedgerEntriesEdge\x12:\n\x04node\x18\x01 \x01(\x0b\x32&.datanode.api.v2.AggregatedLedgerEntryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x9f\x01\n!AggregatedLedgerEntriesConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.AggregatedLedgerEntriesEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xf3\x01\n\x19ListBalanceChangesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"f\n\x1aListBalanceChangesResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"\xac\x02\n\x18GetBalanceHistoryRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12\x38\n\x08group_by\x18\x02 \x03(\x0e\x32\x1d.datanode.api.v2.AccountFieldR\x07groupBy\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"e\n\x19GetBalanceHistoryResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"g\n\x15\x41ggregatedBalanceEdge\x12\x36\n\x04node\x18\x01 \x01(\x0b\x32".datanode.api.v2.AggregatedBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x93\x01\n\x1b\x41ggregatedBalanceConnection\x12<\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32&.datanode.api.v2.AggregatedBalanceEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9e\x01\n\rAccountFilter\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x03 \x03(\tR\tmarketIds\x12\x36\n\raccount_types\x18\x04 \x03(\x0e\x32\x11.vega.AccountTypeR\x0c\x61\x63\x63ountTypes"\xa1\x02\n\x11\x41ggregatedBalance\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x1e\n\x08party_id\x18\x04 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12 \n\tmarket_id\x18\x06 \x01(\tH\x02R\x08marketId\x88\x01\x01\x12\x39\n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeH\x03R\x0b\x61\x63\x63ountType\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\x0c\n\n_market_idB\x0f\n\r_account_type";\n\x1aObserveMarketsDepthRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"S\n\x1bObserveMarketsDepthResponse\x12\x34\n\x0cmarket_depth\x18\x01 \x03(\x0b\x32\x11.vega.MarketDepthR\x0bmarketDepth"B\n!ObserveMarketsDepthUpdatesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"U\n"ObserveMarketsDepthUpdatesResponse\x12/\n\x06update\x18\x01 \x03(\x0b\x32\x17.vega.MarketDepthUpdateR\x06update":\n\x19ObserveMarketsDataRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"O\n\x1aObserveMarketsDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"p\n\x1bGetLatestMarketDepthRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12 \n\tmax_depth\x18\x02 \x01(\x04H\x00R\x08maxDepth\x88\x01\x01\x42\x0c\n\n_max_depth"\xda\x01\n\x1cGetLatestMarketDepthResponse\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12*\n\nlast_trade\x18\x04 \x01(\x0b\x32\x0b.vega.TradeR\tlastTrade\x12\'\n\x0fsequence_number\x18\x05 \x01(\x04R\x0esequenceNumber"\x1d\n\x1bListLatestMarketDataRequest"S\n\x1cListLatestMarketDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"?\n\x1aGetLatestMarketDataRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"P\n\x1bGetLatestMarketDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\nmarketData"\x99\x02\n\x1fGetMarketDataHistoryByIDRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12,\n\x0fstart_timestamp\x18\x02 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x03 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestampB\r\n\x0b_paginationJ\x04\x08\x05\x10\x06"j\n GetMarketDataHistoryByIDResponse\x12\x46\n\x0bmarket_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.MarketDataConnectionR\nmarketData"N\n\x0eMarketDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14MarketDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.MarketDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd1\x01\n\x14ListTransfersRequest\x12\x1b\n\x06pubkey\x18\x01 \x01(\tH\x00R\x06pubkey\x88\x01\x01\x12@\n\tdirection\x18\x02 \x01(\x0e\x32".datanode.api.v2.TransferDirectionR\tdirection\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\t\n\x07_pubkeyB\r\n\x0b_pagination"Z\n\x15ListTransfersResponse\x12\x41\n\ttransfers\x18\x01 \x01(\x0b\x32#.datanode.api.v2.TransferConnectionR\ttransfers"T\n\x0cTransferEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12TransferConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.TransferEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x19\n\x17GetNetworkLimitsRequest"G\n\x18GetNetworkLimitsResponse\x12+\n\x06limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\x06limits"?\n\x1aListCandleIntervalsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"M\n\x12IntervalToCandleId\x12\x1a\n\x08interval\x18\x01 \x01(\tR\x08interval\x12\x1b\n\tcandle_id\x18\x02 \x01(\tR\x08\x63\x61ndleId"u\n\x1bListCandleIntervalsResponse\x12V\n\x15interval_to_candle_id\x18\x01 \x03(\x0b\x32#.datanode.api.v2.IntervalToCandleIdR\x12intervalToCandleId"\xc3\x01\n\x06\x43\x61ndle\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x1f\n\x0blast_update\x18\x02 \x01(\x03R\nlastUpdate\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12\x1a\n\x08notional\x18\x08 \x01(\x04R\x08notional"=\n\x18ObserveCandleDataRequest\x12!\n\tcandle_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08\x63\x61ndleId"L\n\x19ObserveCandleDataResponse\x12/\n\x06\x63\x61ndle\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x06\x63\x61ndle"\xdb\x01\n\x15ListCandleDataRequest\x12!\n\tcandle_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08\x63\x61ndleId\x12%\n\x0e\x66rom_timestamp\x18\x02 \x01(\x03R\rfromTimestamp\x12!\n\x0cto_timestamp\x18\x03 \x01(\x03R\x0btoTimestamp\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_paginationJ\x04\x08\x04\x10\x05"Y\n\x16ListCandleDataResponse\x12?\n\x07\x63\x61ndles\x18\x01 \x01(\x0b\x32%.datanode.api.v2.CandleDataConnectionR\x07\x63\x61ndles"Q\n\nCandleEdge\x12+\n\x04node\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x14\x43\x61ndleDataConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.CandleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc6\x01\n\x10ListVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_idB\r\n\x0b_pagination"J\n\x11ListVotesResponse\x12\x35\n\x05votes\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.VoteConnectionR\x05votes"B\n\x08VoteEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"y\n\x0eVoteConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.VoteEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"x\n\x13ObserveVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_id"6\n\x14ObserveVotesResponse\x12\x1e\n\x04vote\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04vote"\xbd\x01\n*ListERC20MultiSigSignerAddedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"|\n+ListERC20MultiSigSignerAddedBundlesResponse\x12M\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedConnectionR\x07\x62undles"t\n\x1c\x45RC20MultiSigSignerAddedEdge\x12<\n\x04node\x18\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n"ERC20MultiSigSignerAddedBundleEdge\x12\x43\n\x04node\x18\x01 \x01(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xa7\x01\n"ERC20MultiSigSignerAddedConnection\x12I\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xce\x01\n\x1e\x45RC20MultiSigSignerAddedBundle\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"\xbf\x01\n,ListERC20MultiSigSignerRemovedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"\x80\x01\n-ListERC20MultiSigSignerRemovedBundlesResponse\x12O\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedConnectionR\x07\x62undles"x\n\x1e\x45RC20MultiSigSignerRemovedEdge\x12>\n\x04node\x18\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n$ERC20MultiSigSignerRemovedBundleEdge\x12\x45\n\x04node\x18\x01 \x01(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xab\x01\n$ERC20MultiSigSignerRemovedConnection\x12K\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd0\x01\n ERC20MultiSigSignerRemovedBundle\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"A\n\x1eGetERC20ListAssetBundleRequest\x12\x1f\n\x08\x61sset_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId"\x9e\x01\n\x1fGetERC20ListAssetBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x04 \x01(\tR\nsignatures"L\n#GetERC20SetAssetLimitsBundleRequest\x12%\n\x0bproposal_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\nproposalId"\xe8\x01\n$GetERC20SetAssetLimitsBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12%\n\x0elifetime_limit\x18\x04 \x01(\tR\rlifetimeLimit\x12\x1c\n\tthreshold\x18\x05 \x01(\tR\tthreshold\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures"N\n!GetERC20WithdrawalApprovalRequest\x12)\n\rwithdrawal_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0cwithdrawalId"\xde\x01\n"GetERC20WithdrawalApprovalResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x05 \x01(\tR\nsignatures\x12%\n\x0etarget_address\x18\x06 \x01(\tR\rtargetAddress\x12\x1a\n\x08\x63reation\x18\x07 \x01(\x03R\x08\x63reationJ\x04\x08\x03\x10\x04"8\n\x13GetLastTradeRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"9\n\x14GetLastTradeResponse\x12!\n\x05trade\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x05trade"\x8c\x02\n\x11ListTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds\x12\x1b\n\tparty_ids\x18\x03 \x03(\tR\x08partyIds\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x05 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"N\n\x12ListTradesResponse\x12\x38\n\x06trades\x18\x01 \x01(\x0b\x32 .datanode.api.v2.TradeConnectionR\x06trades"{\n\x0fTradeConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.TradeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tTradeEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"R\n\x14ObserveTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds"<\n\x15ObserveTradesResponse\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"B\n\x14GetOracleSpecRequest\x12*\n\x0eoracle_spec_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0coracleSpecId"J\n\x15GetOracleSpecResponse\x12\x31\n\x0boracle_spec\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\noracleSpec"i\n\x16ListOracleSpecsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"d\n\x17ListOracleSpecsResponse\x12I\n\x0coracle_specs\x18\x01 \x01(\x0b\x32&.datanode.api.v2.OracleSpecsConnectionR\x0boracleSpecs"\xa6\x01\n\x15ListOracleDataRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tH\x00R\x0coracleSpecId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x11\n\x0f_oracle_spec_idB\r\n\x0b_pagination"`\n\x16ListOracleDataResponse\x12\x46\n\x0boracle_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.OracleDataConnectionR\noracleData"N\n\x0eOracleSpecEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15OracleSpecsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleSpecEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"N\n\x0eOracleDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14OracleDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"5\n\x10GetMarketRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"9\n\x11GetMarketResponse\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market"\xa7\x01\n\x12ListMarketsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12,\n\x0finclude_settled\x18\x03 \x01(\x08H\x01R\x0eincludeSettled\x88\x01\x01\x42\r\n\x0b_paginationB\x12\n\x10_include_settled"R\n\x13ListMarketsResponse\x12;\n\x07markets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarketConnectionR\x07markets"F\n\nMarketEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarketConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xaf\x01\n\x1bListSuccessorMarketsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x30\n\x14include_full_history\x18\x02 \x01(\x08R\x12includeFullHistory\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"k\n\x0fSuccessorMarket\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x32\n\tproposals\x18\x02 \x03(\x0b\x32\x14.vega.GovernanceDataR\tproposals"c\n\x13SuccessorMarketEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .datanode.api.v2.SuccessorMarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8f\x01\n\x19SuccessorMarketConnection\x12:\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32$.datanode.api.v2.SuccessorMarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"w\n\x1cListSuccessorMarketsResponse\x12W\n\x11successor_markets\x18\x01 \x01(\x0b\x32*.datanode.api.v2.SuccessorMarketConnectionR\x10successorMarkets"2\n\x0fGetPartyRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId"5\n\x10GetPartyResponse\x12!\n\x05party\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x05party"l\n\x12ListPartiesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12;\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"Q\n\x13ListPartiesResponse\x12:\n\x07parties\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PartyConnectionR\x07parties"D\n\tPartyEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"{\n\x0fPartyConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.PartyEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tOrderEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8e\x01\n\x17ListMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"b\n\x18ListMarginLevelsResponse\x12\x46\n\rmargin_levels\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarginConnectionR\x0cmarginLevels"g\n\x1aObserveMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12 \n\tmarket_id\x18\x02 \x01(\tH\x00R\x08marketId\x88\x01\x01\x42\x0c\n\n_market_id"V\n\x1bObserveMarginLevelsResponse\x12\x37\n\rmargin_levels\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"{\n\x0fOrderConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.OrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"L\n\nMarginEdge\x12&\n\x04node\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarginConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarginEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x8d\x02\n\x12ListRewardsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x12"\n\nfrom_epoch\x18\x04 \x01(\x04H\x02R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x05 \x01(\x04H\x03R\x07toEpoch\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_paginationB\r\n\x0b_from_epochB\x0b\n\t_to_epoch"S\n\x13ListRewardsResponse\x12<\n\x07rewards\x18\x01 \x01(\x0b\x32".datanode.api.v2.RewardsConnectionR\x07rewards"F\n\nRewardEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"~\n\x11RewardsConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.RewardEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc7\x01\n\x1aListRewardSummariesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\r\n\x0b_pagination"P\n\x1bListRewardSummariesResponse\x12\x31\n\tsummaries\x18\x01 \x03(\x0b\x32\x13.vega.RewardSummaryR\tsummaries"\xb1\x01\n\x13RewardSummaryFilter\x12\x1b\n\tasset_ids\x18\x01 \x03(\tR\x08\x61ssetIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds\x12"\n\nfrom_epoch\x18\x03 \x01(\x04H\x00R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x04 \x01(\x04H\x01R\x07toEpoch\x88\x01\x01\x42\r\n\x0b_from_epochB\x0b\n\t_to_epoch"\xb0\x01\n\x1fListEpochRewardSummariesRequest\x12<\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.datanode.api.v2.RewardSummaryFilterR\x06\x66ilter\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"o\n ListEpochRewardSummariesResponse\x12K\n\tsummaries\x18\x01 \x01(\x0b\x32-.datanode.api.v2.EpochRewardSummaryConnectionR\tsummaries"\x95\x01\n\x1c\x45pochRewardSummaryConnection\x12=\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\'.datanode.api.v2.EpochRewardSummaryEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"^\n\x16\x45pochRewardSummaryEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.EpochRewardSummaryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"q\n\x15ObserveRewardsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0b\n\t_asset_idB\x0b\n\t_party_id">\n\x16ObserveRewardsResponse\x12$\n\x06reward\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x06reward")\n\x11GetDepositRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"=\n\x12GetDepositResponse\x12\'\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"\xd0\x01\n\x13ListDepositsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"W\n\x14ListDepositsResponse\x12?\n\x08\x64\x65posits\x18\x01 \x01(\x0b\x32#.datanode.api.v2.DepositsConnectionR\x08\x64\x65posits"H\n\x0b\x44\x65positEdge\x12!\n\x04node\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x80\x01\n\x12\x44\x65positsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.DepositEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x14GetWithdrawalRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"I\n\x15GetWithdrawalResponse\x12\x30\n\nwithdrawal\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"\xd3\x01\n\x16ListWithdrawalsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"c\n\x17ListWithdrawalsResponse\x12H\n\x0bwithdrawals\x18\x01 \x01(\x0b\x32&.datanode.api.v2.WithdrawalsConnectionR\x0bwithdrawals"N\n\x0eWithdrawalEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15WithdrawalsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.WithdrawalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"2\n\x0fGetAssetRequest\x12\x1f\n\x08\x61sset_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId"5\n\x10GetAssetResponse\x12!\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x05\x61sset"\x91\x01\n\x11ListAssetsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"O\n\x12ListAssetsResponse\x12\x39\n\x06\x61ssets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.AssetsConnectionR\x06\x61ssets"D\n\tAssetEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"|\n\x10\x41ssetsConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.AssetEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xa1\x02\n\x1eListLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12\x17\n\x04live\x18\x04 \x01(\x08H\x03R\x04live\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x0c\n\n_referenceB\x07\n\x05_liveB\r\n\x0b_pagination"\x84\x01\n\x1fListLiquidityProvisionsResponse\x12\x61\n\x14liquidity_provisions\x18\x01 \x01(\x0b\x32..datanode.api.v2.LiquidityProvisionsConnectionR\x13liquidityProvisions"_\n\x17LiquidityProvisionsEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.LiquidityProvisionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x97\x01\n\x1dLiquidityProvisionsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.LiquidityProvisionsEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x80\x01\n!ObserveLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"q\n"ObserveLiquidityProvisionsResponse\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions"\x81\x01\n\x18GetGovernanceDataRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tH\x00R\nproposalId\x88\x01\x01\x12!\n\treference\x18\x02 \x01(\tH\x01R\treference\x88\x01\x01\x42\x0e\n\x0c_proposal_idB\x0c\n\n_reference"E\n\x19GetGovernanceDataResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xfa\x04\n\x19ListGovernanceDataRequest\x12@\n\x0eproposal_state\x18\x01 \x01(\x0e\x32\x14.vega.Proposal.StateH\x00R\rproposalState\x88\x01\x01\x12Y\n\rproposal_type\x18\x02 \x01(\x0e\x32/.datanode.api.v2.ListGovernanceDataRequest.TypeH\x01R\x0cproposalType\x88\x01\x01\x12/\n\x11proposer_party_id\x18\x03 \x01(\tH\x02R\x0fproposerPartyId\x88\x01\x01\x12\x32\n\x12proposal_reference\x18\x04 \x01(\tH\x03R\x11proposalReference\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01"\xb7\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_ALL\x10\x01\x12\x13\n\x0fTYPE_NEW_MARKET\x10\x02\x12\x16\n\x12TYPE_UPDATE_MARKET\x10\x03\x12\x1b\n\x17TYPE_NETWORK_PARAMETERS\x10\x04\x12\x12\n\x0eTYPE_NEW_ASSET\x10\x05\x12\x16\n\x12TYPE_NEW_FREE_FORM\x10\x06\x12\x15\n\x11TYPE_UPDATE_ASSET\x10\x07\x42\x11\n\x0f_proposal_stateB\x10\n\x0e_proposal_typeB\x14\n\x12_proposer_party_idB\x15\n\x13_proposal_referenceB\r\n\x0b_pagination"g\n\x1aListGovernanceDataResponse\x12I\n\nconnection\x18\x01 \x01(\x0b\x32).datanode.api.v2.GovernanceDataConnectionR\nconnection"V\n\x12GovernanceDataEdge\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x18GovernanceDataConnection\x12\x39\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32#.datanode.api.v2.GovernanceDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"G\n\x18ObserveGovernanceRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x42\x0b\n\t_party_id"E\n\x19ObserveGovernanceResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xed\x01\n\x16ListDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x12\x1e\n\x08\x65poch_id\x18\x03 \x01(\tH\x02R\x07\x65pochId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_idB\x0b\n\t_epoch_idB\r\n\x0b_pagination"c\n\x17ListDelegationsResponse\x12H\n\x0b\x64\x65legations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.DelegationsConnectionR\x0b\x64\x65legations"N\n\x0e\x44\x65legationEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x44\x65legationsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.DelegationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"r\n\x19ObserveDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_id"N\n\x1aObserveDelegationsResponse\x12\x30\n\ndelegation\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\ndelegation"\x91\x02\n\tNodeBasic\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x17\n\x15GetNetworkDataRequest"E\n\x16GetNetworkDataResponse\x12+\n\tnode_data\x18\x01 \x01(\x0b\x32\x0e.vega.NodeDataR\x08nodeData"&\n\x0eGetNodeRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"1\n\x0fGetNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node"\x93\x01\n\x10ListNodesRequest\x12 \n\tepoch_seq\x18\x01 \x01(\x04H\x00R\x08\x65pochSeq\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0c\n\n_epoch_seqB\r\n\x0b_pagination"K\n\x11ListNodesResponse\x12\x36\n\x05nodes\x18\x01 \x01(\x0b\x32 .datanode.api.v2.NodesConnectionR\x05nodes"B\n\x08NodeEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"z\n\x0fNodesConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.NodeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x82\x01\n\x19ListNodeSignaturesRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"g\n\x1aListNodeSignaturesResponse\x12I\n\nsignatures\x18\x01 \x01(\x0b\x32).datanode.api.v2.NodeSignaturesConnectionR\nsignatures"`\n\x11NodeSignatureEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8c\x01\n\x18NodeSignaturesConnection\x12\x38\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32".datanode.api.v2.NodeSignatureEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"R\n\x0fGetEpochRequest\x12\x13\n\x02id\x18\x01 \x01(\x04H\x00R\x02id\x88\x01\x01\x12\x19\n\x05\x62lock\x18\x02 \x01(\x04H\x01R\x05\x62lock\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_block"5\n\x10GetEpochResponse\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch"m\n\x12\x45stimateFeeRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x1a\n\x05price\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x05price\x12\x18\n\x04size\x18\x03 \x01(\x04\x42\x04\xe2\x41\x01\x02R\x04size"2\n\x13\x45stimateFeeResponse\x12\x1b\n\x03\x66\x65\x65\x18\x02 \x01(\x0b\x32\t.vega.FeeR\x03\x66\x65\x65"\xe7\x01\n\x15\x45stimateMarginRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x1f\n\x08party_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12$\n\x04side\x18\x03 \x01(\x0e\x32\n.vega.SideB\x04\xe2\x41\x01\x02R\x04side\x12*\n\x04type\x18\x04 \x01(\x0e\x32\x10.vega.Order.TypeB\x04\xe2\x41\x01\x02R\x04type\x12\x18\n\x04size\x18\x05 \x01(\x04\x42\x04\xe2\x41\x01\x02R\x04size\x12\x1a\n\x05price\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02R\x05price:\x02\x18\x01"U\n\x16\x45stimateMarginResponse\x12\x37\n\rmargin_levels\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels:\x02\x18\x01"o\n\x1cListNetworkParametersRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"{\n\x1dListNetworkParametersResponse\x12Z\n\x12network_parameters\x18\x01 \x01(\x0b\x32+.datanode.api.v2.NetworkParameterConnectionR\x11networkParameters"4\n\x1aGetNetworkParameterRequest\x12\x16\n\x03key\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x03key"b\n\x1bGetNetworkParameterResponse\x12\x43\n\x11network_parameter\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x10networkParameter"Z\n\x14NetworkParameterEdge\x12*\n\x04node\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x91\x01\n\x1aNetworkParameterConnection\x12;\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32%.datanode.api.v2.NetworkParameterEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\nCheckpoint\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12\x19\n\x08\x61t_block\x18\x03 \x01(\x04R\x07\x61tBlock"i\n\x16ListCheckpointsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"c\n\x17ListCheckpointsResponse\x12H\n\x0b\x63heckpoints\x18\x01 \x01(\x0b\x32&.datanode.api.v2.CheckpointsConnectionR\x0b\x63heckpoints"Y\n\x0e\x43heckpointEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.CheckpointR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x43heckpointsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.CheckpointEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x83\x01\n\x0fGetStakeRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"\x94\x01\n\x10GetStakeResponse\x12\x36\n\x17\x63urrent_stake_available\x18\x01 \x01(\tR\x15\x63urrentStakeAvailable\x12H\n\x0estake_linkings\x18\x02 \x01(\x0b\x32!.datanode.api.v2.StakesConnectionR\rstakeLinkings"\\\n\x10StakeLinkingEdge\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x10StakesConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.StakeLinkingEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo":\n\x15GetRiskFactorsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"K\n\x16GetRiskFactorsResponse\x12\x31\n\x0brisk_factor\x18\x01 \x01(\x0b\x32\x10.vega.RiskFactorR\nriskFactor"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x1f\n\x1dObserveLedgerMovementsRequest"_\n\x1eObserveLedgerMovementsResponse\x12=\n\x0fledger_movement\x18\x01 \x01(\x0b\x32\x14.vega.LedgerMovementR\x0eledgerMovement"\x94\x01\n\x17ListKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"`\n\x18ListKeyRotationsResponse\x12\x44\n\trotations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.KeyRotationConnectionR\trotations"Z\n\x0fKeyRotationEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x87\x01\n\x15KeyRotationConnection\x12\x36\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32 .datanode.api.v2.KeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9c\x01\n\x1fListEthereumKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"x\n ListEthereumKeyRotationsResponse\x12T\n\rkey_rotations\x18\x01 \x01(\x0b\x32/.datanode.api.v2.EthereumKeyRotationsConnectionR\x0ckeyRotations"\x98\x01\n\x1e\x45thereumKeyRotationsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.EthereumKeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"j\n\x17\x45thereumKeyRotationEdge\x12\x37\n\x04node\x18\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\x89\x01\n\tDateRange\x12,\n\x0fstart_timestamp\x18\x01 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x02 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestamp"!\n\x1fGetProtocolUpgradeStatusRequest"8\n GetProtocolUpgradeStatusResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready"\x83\x02\n#ListProtocolUpgradeProposalsRequest\x12J\n\x06status\x18\x01 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusH\x00R\x06status\x88\x01\x01\x12$\n\x0b\x61pproved_by\x18\x02 \x01(\tH\x01R\napprovedBy\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\t\n\x07_statusB\x0e\n\x0c_approved_byB\r\n\x0b_pagination"\x98\x01\n$ListProtocolUpgradeProposalsResponse\x12p\n\x1aprotocol_upgrade_proposals\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.ProtocolUpgradeProposalConnectionR\x18protocolUpgradeProposals"\x9f\x01\n!ProtocolUpgradeProposalConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.ProtocolUpgradeProposalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"o\n\x1bProtocolUpgradeProposalEdge\x12\x38\n\x04node\x18\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"k\n\x18ListCoreSnapshotsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"k\n\x19ListCoreSnapshotsResponse\x12N\n\x0e\x63ore_snapshots\x18\x01 \x01(\x0b\x32\'.datanode.api.v2.CoreSnapshotConnectionR\rcoreSnapshots"\x89\x01\n\x16\x43oreSnapshotConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.CoreSnapshotEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"`\n\x10\x43oreSnapshotEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x02\n\x0eHistorySegment\x12\x1f\n\x0b\x66rom_height\x18\x01 \x01(\x03R\nfromHeight\x12\x1b\n\tto_height\x18\x02 \x01(\x03R\x08toHeight\x12,\n\x12history_segment_id\x18\x03 \x01(\tR\x10historySegmentId\x12=\n\x1bprevious_history_segment_id\x18\x04 \x01(\tR\x18previousHistorySegmentId\x12)\n\x10\x64\x61tabase_version\x18\x05 \x01(\x03R\x0f\x64\x61tabaseVersion\x12\x19\n\x08\x63hain_id\x18\x06 \x01(\tR\x07\x63hainId"+\n)GetMostRecentNetworkHistorySegmentRequest"\x8d\x01\n*GetMostRecentNetworkHistorySegmentResponse\x12\x39\n\x07segment\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x07segment\x12$\n\x0eswarm_key_seed\x18\x02 \x01(\tR\x0cswarmKeySeed"&\n$ListAllNetworkHistorySegmentsRequest"d\n%ListAllNetworkHistorySegmentsResponse\x12;\n\x08segments\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x08segments"-\n+GetActiveNetworkHistoryPeerAddressesRequest"Q\n,GetActiveNetworkHistoryPeerAddressesResponse\x12!\n\x0cip_addresses\x18\x01 \x03(\tR\x0bipAddresses" \n\x1eGetNetworkHistoryStatusRequest"\xb0\x01\n\x1fGetNetworkHistoryStatusResponse\x12!\n\x0cipfs_address\x18\x01 \x01(\tR\x0bipfsAddress\x12\x1b\n\tswarm_key\x18\x02 \x01(\tR\x08swarmKey\x12$\n\x0eswarm_key_seed\x18\x03 \x01(\tR\x0cswarmKeySeed\x12\'\n\x0f\x63onnected_peers\x18\x05 \x03(\tR\x0e\x63onnectedPeers"(\n&GetNetworkHistoryBootstrapPeersRequest"R\n\'GetNetworkHistoryBootstrapPeersResponse\x12\'\n\x0f\x62ootstrap_peers\x18\x01 \x03(\tR\x0e\x62ootstrapPeers"\x85\x01\n\x1b\x45xportNetworkHistoryRequest\x12\x1d\n\nfrom_block\x18\x01 \x01(\x03R\tfromBlock\x12\x19\n\x08to_block\x18\x02 \x01(\x03R\x07toBlock\x12,\n\x05table\x18\x03 \x01(\x0e\x32\x16.datanode.api.v2.TableR\x05table"F\n\x13ListEntitiesRequest\x12/\n\x10transaction_hash\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0ftransactionHash"\xad\r\n\x14ListEntitiesResponse\x12)\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x08\x61\x63\x63ounts\x12#\n\x06orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12,\n\tpositions\x18\x03 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x38\n\x0eledger_entries\x18\x04 \x03(\x0b\x32\x11.vega.LedgerEntryR\rledgerEntries\x12H\n\x0f\x62\x61lance_changes\x18\x05 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x0e\x62\x61lanceChanges\x12\x36\n\ttransfers\x18\x06 \x03(\x0b\x32\x18.vega.events.v1.TransferR\ttransfers\x12 \n\x05votes\x18\x07 \x03(\x0b\x32\n.vega.VoteR\x05votes\x12~\n$erc20_multi_sig_signer_added_bundles\x18\x08 \x03(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x1f\x65rc20MultiSigSignerAddedBundles\x12\x84\x01\n&erc20_multi_sig_signer_removed_bundles\x18\t \x03(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR!erc20MultiSigSignerRemovedBundles\x12#\n\x06trades\x18\n \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x33\n\x0coracle_specs\x18\x0b \x03(\x0b\x32\x10.vega.OracleSpecR\x0boracleSpecs\x12\x31\n\x0boracle_data\x18\x0c \x03(\x0b\x32\x10.vega.OracleDataR\noracleData\x12&\n\x07markets\x18\r \x03(\x0b\x32\x0c.vega.MarketR\x07markets\x12%\n\x07parties\x18\x0e \x03(\x0b\x32\x0b.vega.PartyR\x07parties\x12\x37\n\rmargin_levels\x18\x0f \x03(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels\x12&\n\x07rewards\x18\x10 \x03(\x0b\x32\x0c.vega.RewardR\x07rewards\x12)\n\x08\x64\x65posits\x18\x11 \x03(\x0b\x32\r.vega.DepositR\x08\x64\x65posits\x12\x32\n\x0bwithdrawals\x18\x12 \x03(\x0b\x32\x10.vega.WithdrawalR\x0bwithdrawals\x12#\n\x06\x61ssets\x18\x13 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets\x12K\n\x14liquidity_provisions\x18\x14 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions\x12,\n\tproposals\x18\x15 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals\x12\x32\n\x0b\x64\x65legations\x18\x16 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x30\n\x05nodes\x18\x17 \x03(\x0b\x32\x1a.datanode.api.v2.NodeBasicR\x05nodes\x12H\n\x0fnode_signatures\x18\x18 \x03(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x0enodeSignatures\x12\x45\n\x12network_parameters\x18\x19 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters\x12@\n\rkey_rotations\x18\x1a \x03(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x0ckeyRotations\x12Y\n\x16\x65thereum_key_rotations\x18\x1b \x03(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x14\x65thereumKeyRotations\x12\x62\n\x1aprotocol_upgrade_proposals\x18\x1c \x03(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x18protocolUpgradeProposals"\r\n\x0bPingRequest"\x0e\n\x0cPingResponse"\x87\x01\n\tOrderInfo\x12\x1e\n\x04side\x18\x01 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x1c\n\tremaining\x18\x03 \x01(\x04R\tremaining\x12&\n\x0fis_market_order\x18\x04 \x01(\x08R\risMarketOrder"\xe8\x01\n\x17\x45stimatePositionRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12%\n\x0bopen_volume\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02R\nopenVolume\x12\x32\n\x06orders\x18\x03 \x03(\x0b\x32\x1a.datanode.api.v2.OrderInfoR\x06orders\x12\x36\n\x14\x63ollateral_available\x18\x04 \x01(\tH\x00R\x13\x63ollateralAvailable\x88\x01\x01\x42\x17\n\x15_collateral_available"\x9b\x01\n\x18\x45stimatePositionResponse\x12\x37\n\x06margin\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.MarginEstimateR\x06margin\x12\x46\n\x0bliquidation\x18\x02 \x01(\x0b\x32$.datanode.api.v2.LiquidationEstimateR\x0bliquidation"t\n\x0eMarginEstimate\x12\x31\n\nworst_case\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\tworstCase\x12/\n\tbest_case\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x08\x62\x65stCase"\x97\x01\n\x13LiquidationEstimate\x12@\n\nworst_case\x18\x01 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\tworstCase\x12>\n\tbest_case\x18\x02 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\x08\x62\x65stCase"\xa2\x01\n\x10LiquidationPrice\x12(\n\x10open_volume_only\x18\x01 \x01(\tR\x0eopenVolumeOnly\x12\x30\n\x14including_buy_orders\x18\x02 \x01(\tR\x12includingBuyOrders\x12\x32\n\x15including_sell_orders\x18\x03 \x01(\tR\x13includingSellOrders*\xaa\x01\n\x10LedgerEntryField\x12"\n\x1eLEDGER_ENTRY_FIELD_UNSPECIFIED\x10\x00\x12&\n"LEDGER_ENTRY_FIELD_ACCOUNT_FROM_ID\x10\x01\x12$\n LEDGER_ENTRY_FIELD_ACCOUNT_TO_ID\x10\x02\x12$\n LEDGER_ENTRY_FIELD_TRANSFER_TYPE\x10\x03*\xb0\x01\n\x0c\x41\x63\x63ountField\x12\x1d\n\x19\x41\x43\x43OUNT_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_FIELD_ID\x10\x01\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_PARTY_ID\x10\x02\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_ASSET_ID\x10\x03\x12\x1b\n\x17\x41\x43\x43OUNT_FIELD_MARKET_ID\x10\x04\x12\x16\n\x12\x41\x43\x43OUNT_FIELD_TYPE\x10\x05*\xad\x01\n\x11TransferDirection\x12"\n\x1eTRANSFER_DIRECTION_UNSPECIFIED\x10\x00\x12$\n TRANSFER_DIRECTION_TRANSFER_FROM\x10\x01\x12"\n\x1eTRANSFER_DIRECTION_TRANSFER_TO\x10\x02\x12*\n&TRANSFER_DIRECTION_TRANSFER_TO_OR_FROM\x10\x03*\xde\x02\n\x05Table\x12\x15\n\x11TABLE_UNSPECIFIED\x10\x00\x12\x12\n\x0eTABLE_BALANCES\x10\x01\x12\x15\n\x11TABLE_CHECKPOINTS\x10\x02\x12\x15\n\x11TABLE_DELEGATIONS\x10\x03\x12\x10\n\x0cTABLE_LEDGER\x10\x04\x12\x10\n\x0cTABLE_ORDERS\x10\x05\x12\x10\n\x0cTABLE_TRADES\x10\x06\x12\x15\n\x11TABLE_MARKET_DATA\x10\x07\x12\x17\n\x13TABLE_MARGIN_LEVELS\x10\x08\x12\x13\n\x0fTABLE_POSITIONS\x10\t\x12\x1e\n\x1aTABLE_LIQUIDITY_PROVISIONS\x10\n\x12\x11\n\rTABLE_MARKETS\x10\x0b\x12\x12\n\x0eTABLE_DEPOSITS\x10\x0c\x12\x15\n\x11TABLE_WITHDRAWALS\x10\r\x12\x10\n\x0cTABLE_BLOCKS\x10\x0e\x12\x11\n\rTABLE_REWARDS\x10\x0f\x32\xf2W\n\x12TradingDataService\x12j\n\x0cListAccounts\x12$.datanode.api.v2.ListAccountsRequest\x1a%.datanode.api.v2.ListAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12u\n\x0fObserveAccounts\x12\'.datanode.api.v2.ObserveAccountsRequest\x1a(.datanode.api.v2.ObserveAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts0\x01\x12Z\n\x04Info\x12\x1c.datanode.api.v2.InfoRequest\x1a\x1d.datanode.api.v2.InfoResponse"\x15\x92\x41\x12\n\x10Node information\x12\\\n\x08GetOrder\x12 .datanode.api.v2.GetOrderRequest\x1a!.datanode.api.v2.GetOrderResponse"\x0b\x92\x41\x08\n\x06Orders\x12\x62\n\nListOrders\x12".datanode.api.v2.ListOrdersRequest\x1a#.datanode.api.v2.ListOrdersResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x11ListOrderVersions\x12).datanode.api.v2.ListOrderVersionsRequest\x1a*.datanode.api.v2.ListOrderVersionsResponse"\x0b\x92\x41\x08\n\x06Orders\x12m\n\rObserveOrders\x12%.datanode.api.v2.ObserveOrdersRequest\x1a&.datanode.api.v2.ObserveOrdersResponse"\x0b\x92\x41\x08\n\x06Orders0\x01\x12h\n\x0cGetStopOrder\x12$.datanode.api.v2.GetStopOrderRequest\x1a%.datanode.api.v2.GetStopOrderResponse"\x0b\x92\x41\x08\n\x06Orders\x12n\n\x0eListStopOrders\x12&.datanode.api.v2.ListStopOrdersRequest\x1a\'.datanode.api.v2.ListStopOrdersResponse"\x0b\x92\x41\x08\n\x06Orders\x12q\n\rListPositions\x12%.datanode.api.v2.ListPositionsRequest\x1a&.datanode.api.v2.ListPositionsResponse"\x11\x88\x02\x01\x92\x41\x0b\n\tPositions\x12w\n\x10ListAllPositions\x12(.datanode.api.v2.ListAllPositionsRequest\x1a).datanode.api.v2.ListAllPositionsResponse"\x0e\x92\x41\x0b\n\tPositions\x12y\n\x10ObservePositions\x12(.datanode.api.v2.ObservePositionsRequest\x1a).datanode.api.v2.ObservePositionsResponse"\x0e\x92\x41\x0b\n\tPositions0\x01\x12\x7f\n\x11ListLedgerEntries\x12).datanode.api.v2.ListLedgerEntriesRequest\x1a*.datanode.api.v2.ListLedgerEntriesResponse"\x13\x92\x41\x10\n\x0eLedger entries\x12o\n\x13\x45xportLedgerEntries\x12+.datanode.api.v2.ExportLedgerEntriesRequest\x1a\x14.google.api.HttpBody"\x13\x92\x41\x10\n\x0eLedger entries0\x01\x12|\n\x12ListBalanceChanges\x12*.datanode.api.v2.ListBalanceChangesRequest\x1a+.datanode.api.v2.ListBalanceChangesResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12~\n\x13GetLatestMarketData\x12+.datanode.api.v2.GetLatestMarketDataRequest\x1a,.datanode.api.v2.GetLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListLatestMarketData\x12,.datanode.api.v2.ListLatestMarketDataRequest\x1a-.datanode.api.v2.ListLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14GetLatestMarketDepth\x12,.datanode.api.v2.GetLatestMarketDepthRequest\x1a-.datanode.api.v2.GetLatestMarketDepthResponse"\x0c\x92\x41\t\n\x07Markets\x12\x80\x01\n\x13ObserveMarketsDepth\x12+.datanode.api.v2.ObserveMarketsDepthRequest\x1a,.datanode.api.v2.ObserveMarketsDepthResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x95\x01\n\x1aObserveMarketsDepthUpdates\x12\x32.datanode.api.v2.ObserveMarketsDepthUpdatesRequest\x1a\x33.datanode.api.v2.ObserveMarketsDepthUpdatesResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12}\n\x12ObserveMarketsData\x12*.datanode.api.v2.ObserveMarketsDataRequest\x1a+.datanode.api.v2.ObserveMarketsDataResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x8d\x01\n\x18GetMarketDataHistoryByID\x12\x30.datanode.api.v2.GetMarketDataHistoryByIDRequest\x1a\x31.datanode.api.v2.GetMarketDataHistoryByIDResponse"\x0c\x92\x41\t\n\x07Markets\x12n\n\rListTransfers\x12%.datanode.api.v2.ListTransfersRequest\x1a&.datanode.api.v2.ListTransfersResponse"\x0e\x92\x41\x0b\n\tTransfers\x12u\n\x10GetNetworkLimits\x12(.datanode.api.v2.GetNetworkLimitsRequest\x1a).datanode.api.v2.GetNetworkLimitsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eListCandleData\x12&.datanode.api.v2.ListCandleDataRequest\x1a\'.datanode.api.v2.ListCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12z\n\x11ObserveCandleData\x12).datanode.api.v2.ObserveCandleDataRequest\x1a*.datanode.api.v2.ObserveCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles0\x01\x12~\n\x13ListCandleIntervals\x12+.datanode.api.v2.ListCandleIntervalsRequest\x1a,.datanode.api.v2.ListCandleIntervalsResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12\x63\n\tListVotes\x12!.datanode.api.v2.ListVotesRequest\x1a".datanode.api.v2.ListVotesResponse"\x0f\x92\x41\x0c\n\nGovernance\x12n\n\x0cObserveVotes\x12$.datanode.api.v2.ObserveVotesRequest\x1a%.datanode.api.v2.ObserveVotesResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12\xb3\x01\n#ListERC20MultiSigSignerAddedBundles\x12;.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesRequest\x1a<.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\xb9\x01\n%ListERC20MultiSigSignerRemovedBundles\x12=.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesRequest\x1a>.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x8f\x01\n\x17GetERC20ListAssetBundle\x12/.datanode.api.v2.GetERC20ListAssetBundleRequest\x1a\x30.datanode.api.v2.GetERC20ListAssetBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x9e\x01\n\x1cGetERC20SetAssetLimitsBundle\x12\x34.datanode.api.v2.GetERC20SetAssetLimitsBundleRequest\x1a\x35.datanode.api.v2.GetERC20SetAssetLimitsBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x98\x01\n\x1aGetERC20WithdrawalApproval\x12\x32.datanode.api.v2.GetERC20WithdrawalApprovalRequest\x1a\x33.datanode.api.v2.GetERC20WithdrawalApprovalResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12h\n\x0cGetLastTrade\x12$.datanode.api.v2.GetLastTradeRequest\x1a%.datanode.api.v2.GetLastTradeResponse"\x0b\x92\x41\x08\n\x06Trades\x12\x62\n\nListTrades\x12".datanode.api.v2.ListTradesRequest\x1a#.datanode.api.v2.ListTradesResponse"\x0b\x92\x41\x08\n\x06Trades\x12m\n\rObserveTrades\x12%.datanode.api.v2.ObserveTradesRequest\x1a&.datanode.api.v2.ObserveTradesResponse"\x0b\x92\x41\x08\n\x06Trades0\x01\x12q\n\rGetOracleSpec\x12%.datanode.api.v2.GetOracleSpecRequest\x1a&.datanode.api.v2.GetOracleSpecResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12w\n\x0fListOracleSpecs\x12\'.datanode.api.v2.ListOracleSpecsRequest\x1a(.datanode.api.v2.ListOracleSpecsResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12t\n\x0eListOracleData\x12&.datanode.api.v2.ListOracleDataRequest\x1a\'.datanode.api.v2.ListOracleDataResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12`\n\tGetMarket\x12!.datanode.api.v2.GetMarketRequest\x1a".datanode.api.v2.GetMarketResponse"\x0c\x92\x41\t\n\x07Markets\x12\x66\n\x0bListMarkets\x12#.datanode.api.v2.ListMarketsRequest\x1a$.datanode.api.v2.ListMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListSuccessorMarkets\x12,.datanode.api.v2.ListSuccessorMarketsRequest\x1a-.datanode.api.v2.ListSuccessorMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12]\n\x08GetParty\x12 .datanode.api.v2.GetPartyRequest\x1a!.datanode.api.v2.GetPartyResponse"\x0c\x92\x41\t\n\x07Parties\x12\x66\n\x0bListParties\x12#.datanode.api.v2.ListPartiesRequest\x1a$.datanode.api.v2.ListPartiesResponse"\x0c\x92\x41\t\n\x07Parties\x12{\n\x10ListMarginLevels\x12(.datanode.api.v2.ListMarginLevelsRequest\x1a).datanode.api.v2.ListMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels\x12\x86\x01\n\x13ObserveMarginLevels\x12+.datanode.api.v2.ObserveMarginLevelsRequest\x1a,.datanode.api.v2.ObserveMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels0\x01\x12\x66\n\x0bListRewards\x12#.datanode.api.v2.ListRewardsRequest\x1a$.datanode.api.v2.ListRewardsResponse"\x0c\x92\x41\t\n\x07Rewards\x12~\n\x13ListRewardSummaries\x12+.datanode.api.v2.ListRewardSummariesRequest\x1a,.datanode.api.v2.ListRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x8d\x01\n\x18ListEpochRewardSummaries\x12\x30.datanode.api.v2.ListEpochRewardSummariesRequest\x1a\x31.datanode.api.v2.ListEpochRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x62\n\nGetDeposit\x12".datanode.api.v2.GetDepositRequest\x1a#.datanode.api.v2.GetDepositResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12h\n\x0cListDeposits\x12$.datanode.api.v2.ListDepositsRequest\x1a%.datanode.api.v2.ListDepositsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12k\n\rGetWithdrawal\x12%.datanode.api.v2.GetWithdrawalRequest\x1a&.datanode.api.v2.GetWithdrawalResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12q\n\x0fListWithdrawals\x12\'.datanode.api.v2.ListWithdrawalsRequest\x1a(.datanode.api.v2.ListWithdrawalsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\\\n\x08GetAsset\x12 .datanode.api.v2.GetAssetRequest\x1a!.datanode.api.v2.GetAssetResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x62\n\nListAssets\x12".datanode.api.v2.ListAssetsRequest\x1a#.datanode.api.v2.ListAssetsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x97\x01\n\x17ListLiquidityProvisions\x12/.datanode.api.v2.ListLiquidityProvisionsRequest\x1a\x30.datanode.api.v2.ListLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions\x12\xa2\x01\n\x1aObserveLiquidityProvisions\x12\x32.datanode.api.v2.ObserveLiquidityProvisionsRequest\x1a\x33.datanode.api.v2.ObserveLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions0\x01\x12{\n\x11GetGovernanceData\x12).datanode.api.v2.GetGovernanceDataRequest\x1a*.datanode.api.v2.GetGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12~\n\x12ListGovernanceData\x12*.datanode.api.v2.ListGovernanceDataRequest\x1a+.datanode.api.v2.ListGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12}\n\x11ObserveGovernance\x12).datanode.api.v2.ObserveGovernanceRequest\x1a*.datanode.api.v2.ObserveGovernanceResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12r\n\x0fListDelegations\x12\'.datanode.api.v2.ListDelegationsRequest\x1a(.datanode.api.v2.ListDelegationsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetNetworkData\x12&.datanode.api.v2.GetNetworkDataRequest\x1a\'.datanode.api.v2.GetNetworkDataResponse"\x0c\x92\x41\t\n\x07Network\x12Z\n\x07GetNode\x12\x1f.datanode.api.v2.GetNodeRequest\x1a .datanode.api.v2.GetNodeResponse"\x0c\x92\x41\t\n\x07Network\x12`\n\tListNodes\x12!.datanode.api.v2.ListNodesRequest\x1a".datanode.api.v2.ListNodesResponse"\x0c\x92\x41\t\n\x07Network\x12\x80\x01\n\x12ListNodeSignatures\x12*.datanode.api.v2.ListNodeSignaturesRequest\x1a+.datanode.api.v2.ListNodeSignaturesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12]\n\x08GetEpoch\x12 .datanode.api.v2.GetEpochRequest\x1a!.datanode.api.v2.GetEpochResponse"\x0c\x92\x41\t\n\x07Network\x12\x65\n\x0b\x45stimateFee\x12#.datanode.api.v2.EstimateFeeRequest\x1a$.datanode.api.v2.EstimateFeeResponse"\x0b\x92\x41\x08\n\x06Orders\x12n\n\x0e\x45stimateMargin\x12&.datanode.api.v2.EstimateMarginRequest\x1a\'.datanode.api.v2.EstimateMarginResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x10\x45stimatePosition\x12(.datanode.api.v2.EstimatePositionRequest\x1a).datanode.api.v2.EstimatePositionResponse"\x0e\x92\x41\x0b\n\tPositions\x12\x84\x01\n\x15ListNetworkParameters\x12-.datanode.api.v2.ListNetworkParametersRequest\x1a..datanode.api.v2.ListNetworkParametersResponse"\x0c\x92\x41\t\n\x07Network\x12~\n\x13GetNetworkParameter\x12+.datanode.api.v2.GetNetworkParameterRequest\x1a,.datanode.api.v2.GetNetworkParameterResponse"\x0c\x92\x41\t\n\x07Network\x12r\n\x0fListCheckpoints\x12\'.datanode.api.v2.ListCheckpointsRequest\x1a(.datanode.api.v2.ListCheckpointsResponse"\x0c\x92\x41\t\n\x07Network\x12]\n\x08GetStake\x12 .datanode.api.v2.GetStakeRequest\x1a!.datanode.api.v2.GetStakeResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetRiskFactors\x12&.datanode.api.v2.GetRiskFactorsRequest\x1a\'.datanode.api.v2.GetRiskFactorsResponse"\x0c\x92\x41\t\n\x07Markets\x12u\n\x0fObserveEventBus\x12\'.datanode.api.v2.ObserveEventBusRequest\x1a(.datanode.api.v2.ObserveEventBusResponse"\x0b\x92\x41\x08\n\x06\x45vents(\x01\x30\x01\x12\x92\x01\n\x16ObserveLedgerMovements\x12..datanode.api.v2.ObserveLedgerMovementsRequest\x1a/.datanode.api.v2.ObserveLedgerMovementsResponse"\x15\x92\x41\x12\n\x10Ledger movements0\x01\x12u\n\x10ListKeyRotations\x12(.datanode.api.v2.ListKeyRotationsRequest\x1a).datanode.api.v2.ListKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18ListEthereumKeyRotations\x12\x30.datanode.api.v2.ListEthereumKeyRotationsRequest\x1a\x31.datanode.api.v2.ListEthereumKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x66\n\x0bGetVegaTime\x12#.datanode.api.v2.GetVegaTimeRequest\x1a$.datanode.api.v2.GetVegaTimeResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18GetProtocolUpgradeStatus\x12\x30.datanode.api.v2.GetProtocolUpgradeStatusRequest\x1a\x31.datanode.api.v2.GetProtocolUpgradeStatusResponse"\x0c\x92\x41\t\n\x07Network\x12\x99\x01\n\x1cListProtocolUpgradeProposals\x12\x34.datanode.api.v2.ListProtocolUpgradeProposalsRequest\x1a\x35.datanode.api.v2.ListProtocolUpgradeProposalsResponse"\x0c\x92\x41\t\n\x07Network\x12x\n\x11ListCoreSnapshots\x12).datanode.api.v2.ListCoreSnapshotsRequest\x1a*.datanode.api.v2.ListCoreSnapshotsResponse"\x0c\x92\x41\t\n\x07Network\x12\xb3\x01\n"GetMostRecentNetworkHistorySegment\x12:.datanode.api.v2.GetMostRecentNetworkHistorySegmentRequest\x1a;.datanode.api.v2.GetMostRecentNetworkHistorySegmentResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xa4\x01\n\x1dListAllNetworkHistorySegments\x12\x35.datanode.api.v2.ListAllNetworkHistorySegmentsRequest\x1a\x36.datanode.api.v2.ListAllNetworkHistorySegmentsResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xb9\x01\n$GetActiveNetworkHistoryPeerAddresses\x12<.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesRequest\x1a=.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\x92\x01\n\x17GetNetworkHistoryStatus\x12/.datanode.api.v2.GetNetworkHistoryStatusRequest\x1a\x30.datanode.api.v2.GetNetworkHistoryStatusResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xaa\x01\n\x1fGetNetworkHistoryBootstrapPeers\x12\x37.datanode.api.v2.GetNetworkHistoryBootstrapPeersRequest\x1a\x38.datanode.api.v2.GetNetworkHistoryBootstrapPeersResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12j\n\x0cListEntities\x12$.datanode.api.v2.ListEntitiesRequest\x1a%.datanode.api.v2.ListEntitiesResponse"\r\x92\x41\n\n\x08\x45xplorer\x12r\n\x14\x45xportNetworkHistory\x12,.datanode.api.v2.ExportNetworkHistoryRequest\x1a\x14.google.api.HttpBody"\x14\x92\x41\x11\n\x0fNetwork history0\x01\x12N\n\x04Ping\x12\x1c.datanode.api.v2.PingRequest\x1a\x1d.datanode.api.v2.PingResponse"\t\x92\x41\x06\n\x04MiscB\xc6\x01Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\x92\x41\x8f\x01\x12\x1e\n\x13Vega data node APIs2\x07v0.72.6\x1a\x1chttps://api.testnet.vega.xyz*\x02\x01\x02\x32\x10\x61pplication/jsonR9\n\x03\x35\x30\x30\x12\x32\n\x18\x41n internal server error\x12\x16\n\x14\x1a\x12.google.rpc.Statusb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "data_node.api.v2.trading_data_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\222A\217\001\022\036\n\023Vega data node APIs2\007v0.71.0\032\034https://api.testnet.vega.xyz*\002\001\0022\020application/jsonR9\n\003500\0222\n\030An internal server error\022\026\n\024\032\022.google.rpc.Status"
+    DESCRIPTOR._serialized_options = b"Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\222A\217\001\022\036\n\023Vega data node APIs2\007v0.72.6\032\034https://api.testnet.vega.xyz*\002\001\0022\020application/jsonR9\n\003500\0222\n\030An internal server error\022\026\n\024\032\022.google.rpc.Status"
     _GETORDERREQUEST.fields_by_name["order_id"]._options = None
     _GETORDERREQUEST.fields_by_name["order_id"]._serialized_options = b"\342A\001\002"
     _LISTORDERVERSIONSREQUEST.fields_by_name["order_id"]._options = None
     _LISTORDERVERSIONSREQUEST.fields_by_name[
         "order_id"
     ]._serialized_options = b"\342A\001\002"
+    _GETSTOPORDERREQUEST.fields_by_name["order_id"]._options = None
+    _GETSTOPORDERREQUEST.fields_by_name[
+        "order_id"
+    ]._serialized_options = b"\342A\001\002"
     _LISTPOSITIONSREQUEST._options = None
     _LISTPOSITIONSREQUEST._serialized_options = b"\030\001"
     _LISTPOSITIONSRESPONSE._options = None
     _LISTPOSITIONSRESPONSE._serialized_options = b"\030\001"
     _EXPORTLEDGERENTRIESREQUEST.fields_by_name["party_id"]._options = None
     _EXPORTLEDGERENTRIESREQUEST.fields_by_name[
         "party_id"
@@ -198,14 +202,22 @@
     _TRADINGDATASERVICE.methods_by_name[
         "ListOrderVersions"
     ]._serialized_options = b"\222A\010\n\006Orders"
     _TRADINGDATASERVICE.methods_by_name["ObserveOrders"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ObserveOrders"
     ]._serialized_options = b"\222A\010\n\006Orders"
+    _TRADINGDATASERVICE.methods_by_name["GetStopOrder"]._options = None
+    _TRADINGDATASERVICE.methods_by_name[
+        "GetStopOrder"
+    ]._serialized_options = b"\222A\010\n\006Orders"
+    _TRADINGDATASERVICE.methods_by_name["ListStopOrders"]._options = None
+    _TRADINGDATASERVICE.methods_by_name[
+        "ListStopOrders"
+    ]._serialized_options = b"\222A\010\n\006Orders"
     _TRADINGDATASERVICE.methods_by_name["ListPositions"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ListPositions"
     ]._serialized_options = b"\210\002\001\222A\013\n\tPositions"
     _TRADINGDATASERVICE.methods_by_name["ListAllPositions"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ListAllPositions"
@@ -536,22 +548,22 @@
     _TRADINGDATASERVICE.methods_by_name[
         "ExportNetworkHistory"
     ]._serialized_options = b"\222A\021\n\017Network history"
     _TRADINGDATASERVICE.methods_by_name["Ping"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "Ping"
     ]._serialized_options = b"\222A\006\n\004Misc"
-    _globals["_LEDGERENTRYFIELD"]._serialized_start = 36394
-    _globals["_LEDGERENTRYFIELD"]._serialized_end = 36564
-    _globals["_ACCOUNTFIELD"]._serialized_start = 36567
-    _globals["_ACCOUNTFIELD"]._serialized_end = 36743
-    _globals["_TRANSFERDIRECTION"]._serialized_start = 36746
-    _globals["_TRANSFERDIRECTION"]._serialized_end = 36919
-    _globals["_TABLE"]._serialized_start = 36922
-    _globals["_TABLE"]._serialized_end = 37272
+    _globals["_LEDGERENTRYFIELD"]._serialized_start = 37359
+    _globals["_LEDGERENTRYFIELD"]._serialized_end = 37529
+    _globals["_ACCOUNTFIELD"]._serialized_start = 37532
+    _globals["_ACCOUNTFIELD"]._serialized_end = 37708
+    _globals["_TRANSFERDIRECTION"]._serialized_start = 37711
+    _globals["_TRANSFERDIRECTION"]._serialized_end = 37884
+    _globals["_TABLE"]._serialized_start = 37887
+    _globals["_TABLE"]._serialized_end = 38237
     _globals["_PAGINATION"]._serialized_start = 335
     _globals["_PAGINATION"]._serialized_end = 552
     _globals["_PAGEINFO"]._serialized_start = 555
     _globals["_PAGEINFO"]._serialized_end = 711
     _globals["_ACCOUNTBALANCE"]._serialized_start = 714
     _globals["_ACCOUNTBALANCE"]._serialized_end = 868
     _globals["_LISTACCOUNTSREQUEST"]._serialized_start = 871
@@ -592,530 +604,544 @@
     _globals["_OBSERVEORDERSREQUEST"]._serialized_end = 3174
     _globals["_OBSERVEORDERSRESPONSE"]._serialized_start = 3177
     _globals["_OBSERVEORDERSRESPONSE"]._serialized_end = 3337
     _globals["_ORDERSNAPSHOTPAGE"]._serialized_start = 3339
     _globals["_ORDERSNAPSHOTPAGE"]._serialized_end = 3424
     _globals["_ORDERUPDATES"]._serialized_start = 3426
     _globals["_ORDERUPDATES"]._serialized_end = 3477
-    _globals["_LISTPOSITIONSREQUEST"]._serialized_start = 3480
-    _globals["_LISTPOSITIONSREQUEST"]._serialized_end = 3643
-    _globals["_LISTPOSITIONSRESPONSE"]._serialized_start = 3645
-    _globals["_LISTPOSITIONSRESPONSE"]._serialized_end = 3739
-    _globals["_POSITIONSFILTER"]._serialized_start = 3741
-    _globals["_POSITIONSFILTER"]._serialized_end = 3818
-    _globals["_LISTALLPOSITIONSREQUEST"]._serialized_start = 3821
-    _globals["_LISTALLPOSITIONSREQUEST"]._serialized_end = 3985
-    _globals["_LISTALLPOSITIONSRESPONSE"]._serialized_start = 3987
-    _globals["_LISTALLPOSITIONSRESPONSE"]._serialized_end = 4080
-    _globals["_POSITIONEDGE"]._serialized_start = 4082
-    _globals["_POSITIONEDGE"]._serialized_end = 4156
-    _globals["_POSITIONCONNECTION"]._serialized_start = 4159
-    _globals["_POSITIONCONNECTION"]._serialized_end = 4288
-    _globals["_OBSERVEPOSITIONSREQUEST"]._serialized_start = 4290
-    _globals["_OBSERVEPOSITIONSREQUEST"]._serialized_end = 4408
-    _globals["_OBSERVEPOSITIONSRESPONSE"]._serialized_start = 4411
-    _globals["_OBSERVEPOSITIONSRESPONSE"]._serialized_end = 4580
-    _globals["_POSITIONSNAPSHOTPAGE"]._serialized_start = 4582
-    _globals["_POSITIONSNAPSHOTPAGE"]._serialized_end = 4679
-    _globals["_POSITIONUPDATES"]._serialized_start = 4681
-    _globals["_POSITIONUPDATES"]._serialized_end = 4744
-    _globals["_LEDGERENTRYFILTER"]._serialized_start = 4747
-    _globals["_LEDGERENTRYFILTER"]._serialized_end = 5038
-    _globals["_AGGREGATEDLEDGERENTRY"]._serialized_start = 5041
-    _globals["_AGGREGATEDLEDGERENTRY"]._serialized_end = 5770
-    _globals["_LISTLEDGERENTRIESREQUEST"]._serialized_start = 5773
-    _globals["_LISTLEDGERENTRIESREQUEST"]._serialized_end = 6019
-    _globals["_EXPORTLEDGERENTRIESREQUEST"]._serialized_start = 6022
-    _globals["_EXPORTLEDGERENTRIESREQUEST"]._serialized_end = 6195
-    _globals["_LISTLEDGERENTRIESRESPONSE"]._serialized_start = 6197
-    _globals["_LISTLEDGERENTRIESRESPONSE"]._serialized_end = 6315
-    _globals["_AGGREGATEDLEDGERENTRIESEDGE"]._serialized_start = 6317
-    _globals["_AGGREGATEDLEDGERENTRIESEDGE"]._serialized_end = 6430
-    _globals["_AGGREGATEDLEDGERENTRIESCONNECTION"]._serialized_start = 6433
-    _globals["_AGGREGATEDLEDGERENTRIESCONNECTION"]._serialized_end = 6592
-    _globals["_LISTBALANCECHANGESREQUEST"]._serialized_start = 6595
-    _globals["_LISTBALANCECHANGESREQUEST"]._serialized_end = 6838
-    _globals["_LISTBALANCECHANGESRESPONSE"]._serialized_start = 6840
-    _globals["_LISTBALANCECHANGESRESPONSE"]._serialized_end = 6942
-    _globals["_GETBALANCEHISTORYREQUEST"]._serialized_start = 6945
-    _globals["_GETBALANCEHISTORYREQUEST"]._serialized_end = 7245
-    _globals["_GETBALANCEHISTORYRESPONSE"]._serialized_start = 7247
-    _globals["_GETBALANCEHISTORYRESPONSE"]._serialized_end = 7348
-    _globals["_AGGREGATEDBALANCEEDGE"]._serialized_start = 7350
-    _globals["_AGGREGATEDBALANCEEDGE"]._serialized_end = 7453
-    _globals["_AGGREGATEDBALANCECONNECTION"]._serialized_start = 7456
-    _globals["_AGGREGATEDBALANCECONNECTION"]._serialized_end = 7603
-    _globals["_ACCOUNTFILTER"]._serialized_start = 7606
-    _globals["_ACCOUNTFILTER"]._serialized_end = 7764
-    _globals["_AGGREGATEDBALANCE"]._serialized_start = 7767
-    _globals["_AGGREGATEDBALANCE"]._serialized_end = 8056
-    _globals["_OBSERVEMARKETSDEPTHREQUEST"]._serialized_start = 8058
-    _globals["_OBSERVEMARKETSDEPTHREQUEST"]._serialized_end = 8117
-    _globals["_OBSERVEMARKETSDEPTHRESPONSE"]._serialized_start = 8119
-    _globals["_OBSERVEMARKETSDEPTHRESPONSE"]._serialized_end = 8202
-    _globals["_OBSERVEMARKETSDEPTHUPDATESREQUEST"]._serialized_start = 8204
-    _globals["_OBSERVEMARKETSDEPTHUPDATESREQUEST"]._serialized_end = 8270
-    _globals["_OBSERVEMARKETSDEPTHUPDATESRESPONSE"]._serialized_start = 8272
-    _globals["_OBSERVEMARKETSDEPTHUPDATESRESPONSE"]._serialized_end = 8357
-    _globals["_OBSERVEMARKETSDATAREQUEST"]._serialized_start = 8359
-    _globals["_OBSERVEMARKETSDATAREQUEST"]._serialized_end = 8417
-    _globals["_OBSERVEMARKETSDATARESPONSE"]._serialized_start = 8419
-    _globals["_OBSERVEMARKETSDATARESPONSE"]._serialized_end = 8498
-    _globals["_GETLATESTMARKETDEPTHREQUEST"]._serialized_start = 8500
-    _globals["_GETLATESTMARKETDEPTHREQUEST"]._serialized_end = 8612
-    _globals["_GETLATESTMARKETDEPTHRESPONSE"]._serialized_start = 8615
-    _globals["_GETLATESTMARKETDEPTHRESPONSE"]._serialized_end = 8833
-    _globals["_LISTLATESTMARKETDATAREQUEST"]._serialized_start = 8835
-    _globals["_LISTLATESTMARKETDATAREQUEST"]._serialized_end = 8864
-    _globals["_LISTLATESTMARKETDATARESPONSE"]._serialized_start = 8866
-    _globals["_LISTLATESTMARKETDATARESPONSE"]._serialized_end = 8949
-    _globals["_GETLATESTMARKETDATAREQUEST"]._serialized_start = 8951
-    _globals["_GETLATESTMARKETDATAREQUEST"]._serialized_end = 9014
-    _globals["_GETLATESTMARKETDATARESPONSE"]._serialized_start = 9016
-    _globals["_GETLATESTMARKETDATARESPONSE"]._serialized_end = 9096
-    _globals["_GETMARKETDATAHISTORYBYIDREQUEST"]._serialized_start = 9099
-    _globals["_GETMARKETDATAHISTORYBYIDREQUEST"]._serialized_end = 9380
-    _globals["_GETMARKETDATAHISTORYBYIDRESPONSE"]._serialized_start = 9382
-    _globals["_GETMARKETDATAHISTORYBYIDRESPONSE"]._serialized_end = 9488
-    _globals["_MARKETDATAEDGE"]._serialized_start = 9490
-    _globals["_MARKETDATAEDGE"]._serialized_end = 9568
-    _globals["_MARKETDATACONNECTION"]._serialized_start = 9571
-    _globals["_MARKETDATACONNECTION"]._serialized_end = 9704
-    _globals["_LISTTRANSFERSREQUEST"]._serialized_start = 9707
-    _globals["_LISTTRANSFERSREQUEST"]._serialized_end = 9916
-    _globals["_LISTTRANSFERSRESPONSE"]._serialized_start = 9918
-    _globals["_LISTTRANSFERSRESPONSE"]._serialized_end = 10008
-    _globals["_TRANSFEREDGE"]._serialized_start = 10010
-    _globals["_TRANSFEREDGE"]._serialized_end = 10094
-    _globals["_TRANSFERCONNECTION"]._serialized_start = 10097
-    _globals["_TRANSFERCONNECTION"]._serialized_end = 10226
-    _globals["_GETNETWORKLIMITSREQUEST"]._serialized_start = 10228
-    _globals["_GETNETWORKLIMITSREQUEST"]._serialized_end = 10253
-    _globals["_GETNETWORKLIMITSRESPONSE"]._serialized_start = 10255
-    _globals["_GETNETWORKLIMITSRESPONSE"]._serialized_end = 10326
-    _globals["_LISTCANDLEINTERVALSREQUEST"]._serialized_start = 10328
-    _globals["_LISTCANDLEINTERVALSREQUEST"]._serialized_end = 10391
-    _globals["_INTERVALTOCANDLEID"]._serialized_start = 10393
-    _globals["_INTERVALTOCANDLEID"]._serialized_end = 10470
-    _globals["_LISTCANDLEINTERVALSRESPONSE"]._serialized_start = 10472
-    _globals["_LISTCANDLEINTERVALSRESPONSE"]._serialized_end = 10589
-    _globals["_CANDLE"]._serialized_start = 10592
-    _globals["_CANDLE"]._serialized_end = 10759
-    _globals["_OBSERVECANDLEDATAREQUEST"]._serialized_start = 10761
-    _globals["_OBSERVECANDLEDATAREQUEST"]._serialized_end = 10822
-    _globals["_OBSERVECANDLEDATARESPONSE"]._serialized_start = 10824
-    _globals["_OBSERVECANDLEDATARESPONSE"]._serialized_end = 10900
-    _globals["_LISTCANDLEDATAREQUEST"]._serialized_start = 10903
-    _globals["_LISTCANDLEDATAREQUEST"]._serialized_end = 11122
-    _globals["_LISTCANDLEDATARESPONSE"]._serialized_start = 11124
-    _globals["_LISTCANDLEDATARESPONSE"]._serialized_end = 11213
-    _globals["_CANDLEEDGE"]._serialized_start = 11215
-    _globals["_CANDLEEDGE"]._serialized_end = 11296
-    _globals["_CANDLEDATACONNECTION"]._serialized_start = 11299
-    _globals["_CANDLEDATACONNECTION"]._serialized_end = 11428
-    _globals["_LISTVOTESREQUEST"]._serialized_start = 11431
-    _globals["_LISTVOTESREQUEST"]._serialized_end = 11629
-    _globals["_LISTVOTESRESPONSE"]._serialized_start = 11631
-    _globals["_LISTVOTESRESPONSE"]._serialized_end = 11705
-    _globals["_VOTEEDGE"]._serialized_start = 11707
-    _globals["_VOTEEDGE"]._serialized_end = 11773
-    _globals["_VOTECONNECTION"]._serialized_start = 11775
-    _globals["_VOTECONNECTION"]._serialized_end = 11896
-    _globals["_OBSERVEVOTESREQUEST"]._serialized_start = 11898
-    _globals["_OBSERVEVOTESREQUEST"]._serialized_end = 12018
-    _globals["_OBSERVEVOTESRESPONSE"]._serialized_start = 12020
-    _globals["_OBSERVEVOTESRESPONSE"]._serialized_end = 12074
-    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST"]._serialized_start = 12077
-    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST"]._serialized_end = 12266
-    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE"]._serialized_start = 12268
-    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE"]._serialized_end = 12392
-    _globals["_ERC20MULTISIGSIGNERADDEDEDGE"]._serialized_start = 12394
-    _globals["_ERC20MULTISIGSIGNERADDEDEDGE"]._serialized_end = 12510
-    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLEEDGE"]._serialized_start = 12513
-    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLEEDGE"]._serialized_end = 12642
-    _globals["_ERC20MULTISIGSIGNERADDEDCONNECTION"]._serialized_start = 12645
-    _globals["_ERC20MULTISIGSIGNERADDEDCONNECTION"]._serialized_end = 12812
-    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLE"]._serialized_start = 12815
-    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLE"]._serialized_end = 13021
-    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST"]._serialized_start = 13024
-    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST"]._serialized_end = 13215
-    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE"]._serialized_start = 13218
-    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE"]._serialized_end = 13346
-    _globals["_ERC20MULTISIGSIGNERREMOVEDEDGE"]._serialized_start = 13348
-    _globals["_ERC20MULTISIGSIGNERREMOVEDEDGE"]._serialized_end = 13468
-    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE"]._serialized_start = 13471
-    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE"]._serialized_end = 13604
-    _globals["_ERC20MULTISIGSIGNERREMOVEDCONNECTION"]._serialized_start = 13607
-    _globals["_ERC20MULTISIGSIGNERREMOVEDCONNECTION"]._serialized_end = 13778
-    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLE"]._serialized_start = 13781
-    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLE"]._serialized_end = 13989
-    _globals["_GETERC20LISTASSETBUNDLEREQUEST"]._serialized_start = 13991
-    _globals["_GETERC20LISTASSETBUNDLEREQUEST"]._serialized_end = 14056
-    _globals["_GETERC20LISTASSETBUNDLERESPONSE"]._serialized_start = 14059
-    _globals["_GETERC20LISTASSETBUNDLERESPONSE"]._serialized_end = 14217
-    _globals["_GETERC20SETASSETLIMITSBUNDLEREQUEST"]._serialized_start = 14219
-    _globals["_GETERC20SETASSETLIMITSBUNDLEREQUEST"]._serialized_end = 14295
-    _globals["_GETERC20SETASSETLIMITSBUNDLERESPONSE"]._serialized_start = 14298
-    _globals["_GETERC20SETASSETLIMITSBUNDLERESPONSE"]._serialized_end = 14530
-    _globals["_GETERC20WITHDRAWALAPPROVALREQUEST"]._serialized_start = 14532
-    _globals["_GETERC20WITHDRAWALAPPROVALREQUEST"]._serialized_end = 14610
-    _globals["_GETERC20WITHDRAWALAPPROVALRESPONSE"]._serialized_start = 14613
-    _globals["_GETERC20WITHDRAWALAPPROVALRESPONSE"]._serialized_end = 14835
-    _globals["_GETLASTTRADEREQUEST"]._serialized_start = 14837
-    _globals["_GETLASTTRADEREQUEST"]._serialized_end = 14893
-    _globals["_GETLASTTRADERESPONSE"]._serialized_start = 14895
-    _globals["_GETLASTTRADERESPONSE"]._serialized_end = 14952
-    _globals["_LISTTRADESREQUEST"]._serialized_start = 14955
-    _globals["_LISTTRADESREQUEST"]._serialized_end = 15223
-    _globals["_LISTTRADESRESPONSE"]._serialized_start = 15225
-    _globals["_LISTTRADESRESPONSE"]._serialized_end = 15303
-    _globals["_TRADECONNECTION"]._serialized_start = 15305
-    _globals["_TRADECONNECTION"]._serialized_end = 15428
-    _globals["_TRADEEDGE"]._serialized_start = 15430
-    _globals["_TRADEEDGE"]._serialized_end = 15498
-    _globals["_OBSERVETRADESREQUEST"]._serialized_start = 15500
-    _globals["_OBSERVETRADESREQUEST"]._serialized_end = 15582
-    _globals["_OBSERVETRADESRESPONSE"]._serialized_start = 15584
-    _globals["_OBSERVETRADESRESPONSE"]._serialized_end = 15644
-    _globals["_GETORACLESPECREQUEST"]._serialized_start = 15646
-    _globals["_GETORACLESPECREQUEST"]._serialized_end = 15712
-    _globals["_GETORACLESPECRESPONSE"]._serialized_start = 15714
-    _globals["_GETORACLESPECRESPONSE"]._serialized_end = 15788
-    _globals["_LISTORACLESPECSREQUEST"]._serialized_start = 15790
-    _globals["_LISTORACLESPECSREQUEST"]._serialized_end = 15895
-    _globals["_LISTORACLESPECSRESPONSE"]._serialized_start = 15897
-    _globals["_LISTORACLESPECSRESPONSE"]._serialized_end = 15997
-    _globals["_LISTORACLEDATAREQUEST"]._serialized_start = 16000
-    _globals["_LISTORACLEDATAREQUEST"]._serialized_end = 16166
-    _globals["_LISTORACLEDATARESPONSE"]._serialized_start = 16168
-    _globals["_LISTORACLEDATARESPONSE"]._serialized_end = 16264
-    _globals["_ORACLESPECEDGE"]._serialized_start = 16266
-    _globals["_ORACLESPECEDGE"]._serialized_end = 16344
-    _globals["_ORACLESPECSCONNECTION"]._serialized_start = 16347
-    _globals["_ORACLESPECSCONNECTION"]._serialized_end = 16481
-    _globals["_ORACLEDATAEDGE"]._serialized_start = 16483
-    _globals["_ORACLEDATAEDGE"]._serialized_end = 16561
-    _globals["_ORACLEDATACONNECTION"]._serialized_start = 16564
-    _globals["_ORACLEDATACONNECTION"]._serialized_end = 16697
-    _globals["_GETMARKETREQUEST"]._serialized_start = 16699
-    _globals["_GETMARKETREQUEST"]._serialized_end = 16752
-    _globals["_GETMARKETRESPONSE"]._serialized_start = 16754
-    _globals["_GETMARKETRESPONSE"]._serialized_end = 16811
-    _globals["_LISTMARKETSREQUEST"]._serialized_start = 16814
-    _globals["_LISTMARKETSREQUEST"]._serialized_end = 16981
-    _globals["_LISTMARKETSRESPONSE"]._serialized_start = 16983
-    _globals["_LISTMARKETSRESPONSE"]._serialized_end = 17065
-    _globals["_MARKETEDGE"]._serialized_start = 17067
-    _globals["_MARKETEDGE"]._serialized_end = 17137
-    _globals["_MARKETCONNECTION"]._serialized_start = 17139
-    _globals["_MARKETCONNECTION"]._serialized_end = 17264
-    _globals["_LISTSUCCESSORMARKETSREQUEST"]._serialized_start = 17267
-    _globals["_LISTSUCCESSORMARKETSREQUEST"]._serialized_end = 17442
-    _globals["_SUCCESSORMARKET"]._serialized_start = 17444
-    _globals["_SUCCESSORMARKET"]._serialized_end = 17551
-    _globals["_SUCCESSORMARKETEDGE"]._serialized_start = 17553
-    _globals["_SUCCESSORMARKETEDGE"]._serialized_end = 17652
-    _globals["_SUCCESSORMARKETCONNECTION"]._serialized_start = 17655
-    _globals["_SUCCESSORMARKETCONNECTION"]._serialized_end = 17798
-    _globals["_LISTSUCCESSORMARKETSRESPONSE"]._serialized_start = 17800
-    _globals["_LISTSUCCESSORMARKETSRESPONSE"]._serialized_end = 17900
-    _globals["_GETPARTYREQUEST"]._serialized_start = 17902
-    _globals["_GETPARTYREQUEST"]._serialized_end = 17952
-    _globals["_GETPARTYRESPONSE"]._serialized_start = 17954
-    _globals["_GETPARTYRESPONSE"]._serialized_end = 18007
-    _globals["_LISTPARTIESREQUEST"]._serialized_start = 18009
-    _globals["_LISTPARTIESREQUEST"]._serialized_end = 18117
-    _globals["_LISTPARTIESRESPONSE"]._serialized_start = 18119
-    _globals["_LISTPARTIESRESPONSE"]._serialized_end = 18200
-    _globals["_PARTYEDGE"]._serialized_start = 18202
-    _globals["_PARTYEDGE"]._serialized_end = 18270
-    _globals["_PARTYCONNECTION"]._serialized_start = 18272
-    _globals["_PARTYCONNECTION"]._serialized_end = 18395
-    _globals["_ORDEREDGE"]._serialized_start = 18397
-    _globals["_ORDEREDGE"]._serialized_end = 18465
-    _globals["_LISTMARGINLEVELSREQUEST"]._serialized_start = 18468
-    _globals["_LISTMARGINLEVELSREQUEST"]._serialized_end = 18610
-    _globals["_LISTMARGINLEVELSRESPONSE"]._serialized_start = 18612
-    _globals["_LISTMARGINLEVELSRESPONSE"]._serialized_end = 18710
-    _globals["_OBSERVEMARGINLEVELSREQUEST"]._serialized_start = 18712
-    _globals["_OBSERVEMARGINLEVELSREQUEST"]._serialized_end = 18815
-    _globals["_OBSERVEMARGINLEVELSRESPONSE"]._serialized_start = 18817
-    _globals["_OBSERVEMARGINLEVELSRESPONSE"]._serialized_end = 18903
-    _globals["_ORDERCONNECTION"]._serialized_start = 18905
-    _globals["_ORDERCONNECTION"]._serialized_end = 19028
-    _globals["_MARGINEDGE"]._serialized_start = 19030
-    _globals["_MARGINEDGE"]._serialized_end = 19106
-    _globals["_MARGINCONNECTION"]._serialized_start = 19108
-    _globals["_MARGINCONNECTION"]._serialized_end = 19233
-    _globals["_LISTREWARDSREQUEST"]._serialized_start = 19236
-    _globals["_LISTREWARDSREQUEST"]._serialized_end = 19505
-    _globals["_LISTREWARDSRESPONSE"]._serialized_start = 19507
-    _globals["_LISTREWARDSRESPONSE"]._serialized_end = 19590
-    _globals["_REWARDEDGE"]._serialized_start = 19592
-    _globals["_REWARDEDGE"]._serialized_end = 19662
-    _globals["_REWARDSCONNECTION"]._serialized_start = 19664
-    _globals["_REWARDSCONNECTION"]._serialized_end = 19790
-    _globals["_LISTREWARDSUMMARIESREQUEST"]._serialized_start = 19793
-    _globals["_LISTREWARDSUMMARIESREQUEST"]._serialized_end = 19992
-    _globals["_LISTREWARDSUMMARIESRESPONSE"]._serialized_start = 19994
-    _globals["_LISTREWARDSUMMARIESRESPONSE"]._serialized_end = 20074
-    _globals["_REWARDSUMMARYFILTER"]._serialized_start = 20077
-    _globals["_REWARDSUMMARYFILTER"]._serialized_end = 20254
-    _globals["_LISTEPOCHREWARDSUMMARIESREQUEST"]._serialized_start = 20257
-    _globals["_LISTEPOCHREWARDSUMMARIESREQUEST"]._serialized_end = 20433
-    _globals["_LISTEPOCHREWARDSUMMARIESRESPONSE"]._serialized_start = 20435
-    _globals["_LISTEPOCHREWARDSUMMARIESRESPONSE"]._serialized_end = 20546
-    _globals["_EPOCHREWARDSUMMARYCONNECTION"]._serialized_start = 20549
-    _globals["_EPOCHREWARDSUMMARYCONNECTION"]._serialized_end = 20698
-    _globals["_EPOCHREWARDSUMMARYEDGE"]._serialized_start = 20700
-    _globals["_EPOCHREWARDSUMMARYEDGE"]._serialized_end = 20794
-    _globals["_OBSERVEREWARDSREQUEST"]._serialized_start = 20796
-    _globals["_OBSERVEREWARDSREQUEST"]._serialized_end = 20909
-    _globals["_OBSERVEREWARDSRESPONSE"]._serialized_start = 20911
-    _globals["_OBSERVEREWARDSRESPONSE"]._serialized_end = 20973
-    _globals["_GETDEPOSITREQUEST"]._serialized_start = 20975
-    _globals["_GETDEPOSITREQUEST"]._serialized_end = 21016
-    _globals["_GETDEPOSITRESPONSE"]._serialized_start = 21018
-    _globals["_GETDEPOSITRESPONSE"]._serialized_end = 21079
-    _globals["_LISTDEPOSITSREQUEST"]._serialized_start = 21082
-    _globals["_LISTDEPOSITSREQUEST"]._serialized_end = 21290
-    _globals["_LISTDEPOSITSRESPONSE"]._serialized_start = 21292
-    _globals["_LISTDEPOSITSRESPONSE"]._serialized_end = 21379
-    _globals["_DEPOSITEDGE"]._serialized_start = 21381
-    _globals["_DEPOSITEDGE"]._serialized_end = 21453
-    _globals["_DEPOSITSCONNECTION"]._serialized_start = 21456
-    _globals["_DEPOSITSCONNECTION"]._serialized_end = 21584
-    _globals["_GETWITHDRAWALREQUEST"]._serialized_start = 21586
-    _globals["_GETWITHDRAWALREQUEST"]._serialized_end = 21630
-    _globals["_GETWITHDRAWALRESPONSE"]._serialized_start = 21632
-    _globals["_GETWITHDRAWALRESPONSE"]._serialized_end = 21705
-    _globals["_LISTWITHDRAWALSREQUEST"]._serialized_start = 21708
-    _globals["_LISTWITHDRAWALSREQUEST"]._serialized_end = 21919
-    _globals["_LISTWITHDRAWALSRESPONSE"]._serialized_start = 21921
-    _globals["_LISTWITHDRAWALSRESPONSE"]._serialized_end = 22020
-    _globals["_WITHDRAWALEDGE"]._serialized_start = 22022
-    _globals["_WITHDRAWALEDGE"]._serialized_end = 22100
-    _globals["_WITHDRAWALSCONNECTION"]._serialized_start = 22103
-    _globals["_WITHDRAWALSCONNECTION"]._serialized_end = 22237
-    _globals["_GETASSETREQUEST"]._serialized_start = 22239
-    _globals["_GETASSETREQUEST"]._serialized_end = 22289
-    _globals["_GETASSETRESPONSE"]._serialized_start = 22291
-    _globals["_GETASSETRESPONSE"]._serialized_end = 22344
-    _globals["_LISTASSETSREQUEST"]._serialized_start = 22347
-    _globals["_LISTASSETSREQUEST"]._serialized_end = 22492
-    _globals["_LISTASSETSRESPONSE"]._serialized_start = 22494
-    _globals["_LISTASSETSRESPONSE"]._serialized_end = 22573
-    _globals["_ASSETEDGE"]._serialized_start = 22575
-    _globals["_ASSETEDGE"]._serialized_end = 22643
-    _globals["_ASSETSCONNECTION"]._serialized_start = 22645
-    _globals["_ASSETSCONNECTION"]._serialized_end = 22769
-    _globals["_LISTLIQUIDITYPROVISIONSREQUEST"]._serialized_start = 22772
-    _globals["_LISTLIQUIDITYPROVISIONSREQUEST"]._serialized_end = 23061
-    _globals["_LISTLIQUIDITYPROVISIONSRESPONSE"]._serialized_start = 23064
-    _globals["_LISTLIQUIDITYPROVISIONSRESPONSE"]._serialized_end = 23196
-    _globals["_LIQUIDITYPROVISIONSEDGE"]._serialized_start = 23198
-    _globals["_LIQUIDITYPROVISIONSEDGE"]._serialized_end = 23293
-    _globals["_LIQUIDITYPROVISIONSCONNECTION"]._serialized_start = 23296
-    _globals["_LIQUIDITYPROVISIONSCONNECTION"]._serialized_end = 23447
-    _globals["_OBSERVELIQUIDITYPROVISIONSREQUEST"]._serialized_start = 23450
-    _globals["_OBSERVELIQUIDITYPROVISIONSREQUEST"]._serialized_end = 23578
-    _globals["_OBSERVELIQUIDITYPROVISIONSRESPONSE"]._serialized_start = 23580
-    _globals["_OBSERVELIQUIDITYPROVISIONSRESPONSE"]._serialized_end = 23693
-    _globals["_GETGOVERNANCEDATAREQUEST"]._serialized_start = 23696
-    _globals["_GETGOVERNANCEDATAREQUEST"]._serialized_end = 23825
-    _globals["_GETGOVERNANCEDATARESPONSE"]._serialized_start = 23827
-    _globals["_GETGOVERNANCEDATARESPONSE"]._serialized_end = 23896
-    _globals["_LISTGOVERNANCEDATAREQUEST"]._serialized_start = 23899
-    _globals["_LISTGOVERNANCEDATAREQUEST"]._serialized_end = 24533
-    _globals["_LISTGOVERNANCEDATAREQUEST_TYPE"]._serialized_start = 24253
-    _globals["_LISTGOVERNANCEDATAREQUEST_TYPE"]._serialized_end = 24436
-    _globals["_LISTGOVERNANCEDATARESPONSE"]._serialized_start = 24535
-    _globals["_LISTGOVERNANCEDATARESPONSE"]._serialized_end = 24638
-    _globals["_GOVERNANCEDATAEDGE"]._serialized_start = 24640
-    _globals["_GOVERNANCEDATAEDGE"]._serialized_end = 24726
-    _globals["_GOVERNANCEDATACONNECTION"]._serialized_start = 24729
-    _globals["_GOVERNANCEDATACONNECTION"]._serialized_end = 24870
-    _globals["_OBSERVEGOVERNANCEREQUEST"]._serialized_start = 24872
-    _globals["_OBSERVEGOVERNANCEREQUEST"]._serialized_end = 24943
-    _globals["_OBSERVEGOVERNANCERESPONSE"]._serialized_start = 24945
-    _globals["_OBSERVEGOVERNANCERESPONSE"]._serialized_end = 25014
-    _globals["_LISTDELEGATIONSREQUEST"]._serialized_start = 25017
-    _globals["_LISTDELEGATIONSREQUEST"]._serialized_end = 25254
-    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_start = 25256
-    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_end = 25355
-    _globals["_DELEGATIONEDGE"]._serialized_start = 25357
-    _globals["_DELEGATIONEDGE"]._serialized_end = 25435
-    _globals["_DELEGATIONSCONNECTION"]._serialized_start = 25438
-    _globals["_DELEGATIONSCONNECTION"]._serialized_end = 25572
-    _globals["_OBSERVEDELEGATIONSREQUEST"]._serialized_start = 25574
-    _globals["_OBSERVEDELEGATIONSREQUEST"]._serialized_end = 25688
-    _globals["_OBSERVEDELEGATIONSRESPONSE"]._serialized_start = 25690
-    _globals["_OBSERVEDELEGATIONSRESPONSE"]._serialized_end = 25768
-    _globals["_NODEBASIC"]._serialized_start = 25771
-    _globals["_NODEBASIC"]._serialized_end = 26044
-    _globals["_GETNETWORKDATAREQUEST"]._serialized_start = 26046
-    _globals["_GETNETWORKDATAREQUEST"]._serialized_end = 26069
-    _globals["_GETNETWORKDATARESPONSE"]._serialized_start = 26071
-    _globals["_GETNETWORKDATARESPONSE"]._serialized_end = 26140
-    _globals["_GETNODEREQUEST"]._serialized_start = 26142
-    _globals["_GETNODEREQUEST"]._serialized_end = 26180
-    _globals["_GETNODERESPONSE"]._serialized_start = 26182
-    _globals["_GETNODERESPONSE"]._serialized_end = 26231
-    _globals["_LISTNODESREQUEST"]._serialized_start = 26234
-    _globals["_LISTNODESREQUEST"]._serialized_end = 26381
-    _globals["_LISTNODESRESPONSE"]._serialized_start = 26383
-    _globals["_LISTNODESRESPONSE"]._serialized_end = 26458
-    _globals["_NODEEDGE"]._serialized_start = 26460
-    _globals["_NODEEDGE"]._serialized_end = 26526
-    _globals["_NODESCONNECTION"]._serialized_start = 26528
-    _globals["_NODESCONNECTION"]._serialized_end = 26650
-    _globals["_LISTNODESIGNATURESREQUEST"]._serialized_start = 26653
-    _globals["_LISTNODESIGNATURESREQUEST"]._serialized_end = 26783
-    _globals["_LISTNODESIGNATURESRESPONSE"]._serialized_start = 26785
-    _globals["_LISTNODESIGNATURESRESPONSE"]._serialized_end = 26888
-    _globals["_NODESIGNATUREEDGE"]._serialized_start = 26890
-    _globals["_NODESIGNATUREEDGE"]._serialized_end = 26986
-    _globals["_NODESIGNATURESCONNECTION"]._serialized_start = 26989
-    _globals["_NODESIGNATURESCONNECTION"]._serialized_end = 27129
-    _globals["_GETEPOCHREQUEST"]._serialized_start = 27131
-    _globals["_GETEPOCHREQUEST"]._serialized_end = 27213
-    _globals["_GETEPOCHRESPONSE"]._serialized_start = 27215
-    _globals["_GETEPOCHRESPONSE"]._serialized_end = 27268
-    _globals["_ESTIMATEFEEREQUEST"]._serialized_start = 27270
-    _globals["_ESTIMATEFEEREQUEST"]._serialized_end = 27379
-    _globals["_ESTIMATEFEERESPONSE"]._serialized_start = 27381
-    _globals["_ESTIMATEFEERESPONSE"]._serialized_end = 27431
-    _globals["_ESTIMATEMARGINREQUEST"]._serialized_start = 27434
-    _globals["_ESTIMATEMARGINREQUEST"]._serialized_end = 27665
-    _globals["_ESTIMATEMARGINRESPONSE"]._serialized_start = 27667
-    _globals["_ESTIMATEMARGINRESPONSE"]._serialized_end = 27752
-    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_start = 27754
-    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_end = 27865
-    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_start = 27867
-    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_end = 27990
-    _globals["_GETNETWORKPARAMETERREQUEST"]._serialized_start = 27992
-    _globals["_GETNETWORKPARAMETERREQUEST"]._serialized_end = 28044
-    _globals["_GETNETWORKPARAMETERRESPONSE"]._serialized_start = 28046
-    _globals["_GETNETWORKPARAMETERRESPONSE"]._serialized_end = 28144
-    _globals["_NETWORKPARAMETEREDGE"]._serialized_start = 28146
-    _globals["_NETWORKPARAMETEREDGE"]._serialized_end = 28236
-    _globals["_NETWORKPARAMETERCONNECTION"]._serialized_start = 28239
-    _globals["_NETWORKPARAMETERCONNECTION"]._serialized_end = 28384
-    _globals["_CHECKPOINT"]._serialized_start = 28386
-    _globals["_CHECKPOINT"]._serialized_end = 28476
-    _globals["_LISTCHECKPOINTSREQUEST"]._serialized_start = 28478
-    _globals["_LISTCHECKPOINTSREQUEST"]._serialized_end = 28583
-    _globals["_LISTCHECKPOINTSRESPONSE"]._serialized_start = 28585
-    _globals["_LISTCHECKPOINTSRESPONSE"]._serialized_end = 28684
-    _globals["_CHECKPOINTEDGE"]._serialized_start = 28686
-    _globals["_CHECKPOINTEDGE"]._serialized_end = 28775
-    _globals["_CHECKPOINTSCONNECTION"]._serialized_start = 28778
-    _globals["_CHECKPOINTSCONNECTION"]._serialized_end = 28912
-    _globals["_GETSTAKEREQUEST"]._serialized_start = 28915
-    _globals["_GETSTAKEREQUEST"]._serialized_end = 29046
-    _globals["_GETSTAKERESPONSE"]._serialized_start = 29049
-    _globals["_GETSTAKERESPONSE"]._serialized_end = 29197
-    _globals["_STAKELINKINGEDGE"]._serialized_start = 29199
-    _globals["_STAKELINKINGEDGE"]._serialized_end = 29291
-    _globals["_STAKESCONNECTION"]._serialized_start = 29294
-    _globals["_STAKESCONNECTION"]._serialized_end = 29425
-    _globals["_GETRISKFACTORSREQUEST"]._serialized_start = 29427
-    _globals["_GETRISKFACTORSREQUEST"]._serialized_end = 29485
-    _globals["_GETRISKFACTORSRESPONSE"]._serialized_start = 29487
-    _globals["_GETRISKFACTORSRESPONSE"]._serialized_end = 29562
-    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_start = 29565
-    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_end = 29726
-    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_start = 29728
-    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_end = 29803
-    _globals["_OBSERVELEDGERMOVEMENTSREQUEST"]._serialized_start = 29805
-    _globals["_OBSERVELEDGERMOVEMENTSREQUEST"]._serialized_end = 29836
-    _globals["_OBSERVELEDGERMOVEMENTSRESPONSE"]._serialized_start = 29838
-    _globals["_OBSERVELEDGERMOVEMENTSRESPONSE"]._serialized_end = 29933
-    _globals["_LISTKEYROTATIONSREQUEST"]._serialized_start = 29936
-    _globals["_LISTKEYROTATIONSREQUEST"]._serialized_end = 30084
-    _globals["_LISTKEYROTATIONSRESPONSE"]._serialized_start = 30086
-    _globals["_LISTKEYROTATIONSRESPONSE"]._serialized_end = 30182
-    _globals["_KEYROTATIONEDGE"]._serialized_start = 30184
-    _globals["_KEYROTATIONEDGE"]._serialized_end = 30274
-    _globals["_KEYROTATIONCONNECTION"]._serialized_start = 30277
-    _globals["_KEYROTATIONCONNECTION"]._serialized_end = 30412
-    _globals["_LISTETHEREUMKEYROTATIONSREQUEST"]._serialized_start = 30415
-    _globals["_LISTETHEREUMKEYROTATIONSREQUEST"]._serialized_end = 30571
-    _globals["_LISTETHEREUMKEYROTATIONSRESPONSE"]._serialized_start = 30573
-    _globals["_LISTETHEREUMKEYROTATIONSRESPONSE"]._serialized_end = 30693
-    _globals["_ETHEREUMKEYROTATIONSCONNECTION"]._serialized_start = 30696
-    _globals["_ETHEREUMKEYROTATIONSCONNECTION"]._serialized_end = 30848
-    _globals["_ETHEREUMKEYROTATIONEDGE"]._serialized_start = 30850
-    _globals["_ETHEREUMKEYROTATIONEDGE"]._serialized_end = 30956
-    _globals["_GETVEGATIMEREQUEST"]._serialized_start = 30958
-    _globals["_GETVEGATIMEREQUEST"]._serialized_end = 30978
-    _globals["_GETVEGATIMERESPONSE"]._serialized_start = 30980
-    _globals["_GETVEGATIMERESPONSE"]._serialized_end = 31031
-    _globals["_DATERANGE"]._serialized_start = 31034
-    _globals["_DATERANGE"]._serialized_end = 31171
-    _globals["_GETPROTOCOLUPGRADESTATUSREQUEST"]._serialized_start = 31173
-    _globals["_GETPROTOCOLUPGRADESTATUSREQUEST"]._serialized_end = 31206
-    _globals["_GETPROTOCOLUPGRADESTATUSRESPONSE"]._serialized_start = 31208
-    _globals["_GETPROTOCOLUPGRADESTATUSRESPONSE"]._serialized_end = 31264
-    _globals["_LISTPROTOCOLUPGRADEPROPOSALSREQUEST"]._serialized_start = 31267
-    _globals["_LISTPROTOCOLUPGRADEPROPOSALSREQUEST"]._serialized_end = 31526
-    _globals["_LISTPROTOCOLUPGRADEPROPOSALSRESPONSE"]._serialized_start = 31529
-    _globals["_LISTPROTOCOLUPGRADEPROPOSALSRESPONSE"]._serialized_end = 31681
-    _globals["_PROTOCOLUPGRADEPROPOSALCONNECTION"]._serialized_start = 31684
-    _globals["_PROTOCOLUPGRADEPROPOSALCONNECTION"]._serialized_end = 31843
-    _globals["_PROTOCOLUPGRADEPROPOSALEDGE"]._serialized_start = 31845
-    _globals["_PROTOCOLUPGRADEPROPOSALEDGE"]._serialized_end = 31956
-    _globals["_LISTCORESNAPSHOTSREQUEST"]._serialized_start = 31958
-    _globals["_LISTCORESNAPSHOTSREQUEST"]._serialized_end = 32065
-    _globals["_LISTCORESNAPSHOTSRESPONSE"]._serialized_start = 32067
-    _globals["_LISTCORESNAPSHOTSRESPONSE"]._serialized_end = 32174
-    _globals["_CORESNAPSHOTCONNECTION"]._serialized_start = 32177
-    _globals["_CORESNAPSHOTCONNECTION"]._serialized_end = 32314
-    _globals["_CORESNAPSHOTEDGE"]._serialized_start = 32316
-    _globals["_CORESNAPSHOTEDGE"]._serialized_end = 32412
-    _globals["_HISTORYSEGMENT"]._serialized_start = 32415
-    _globals["_HISTORYSEGMENT"]._serialized_end = 32672
-    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST"]._serialized_start = 32674
-    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST"]._serialized_end = 32717
-    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE"]._serialized_start = 32720
-    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE"]._serialized_end = 32861
-    _globals["_LISTALLNETWORKHISTORYSEGMENTSREQUEST"]._serialized_start = 32863
-    _globals["_LISTALLNETWORKHISTORYSEGMENTSREQUEST"]._serialized_end = 32901
-    _globals["_LISTALLNETWORKHISTORYSEGMENTSRESPONSE"]._serialized_start = 32903
-    _globals["_LISTALLNETWORKHISTORYSEGMENTSRESPONSE"]._serialized_end = 33003
-    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST"]._serialized_start = 33005
-    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST"]._serialized_end = 33050
-    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE"]._serialized_start = 33052
-    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE"]._serialized_end = 33133
-    _globals["_GETNETWORKHISTORYSTATUSREQUEST"]._serialized_start = 33135
-    _globals["_GETNETWORKHISTORYSTATUSREQUEST"]._serialized_end = 33167
-    _globals["_GETNETWORKHISTORYSTATUSRESPONSE"]._serialized_start = 33170
-    _globals["_GETNETWORKHISTORYSTATUSRESPONSE"]._serialized_end = 33346
-    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST"]._serialized_start = 33348
-    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST"]._serialized_end = 33388
-    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE"]._serialized_start = 33390
-    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE"]._serialized_end = 33472
-    _globals["_EXPORTNETWORKHISTORYREQUEST"]._serialized_start = 33475
-    _globals["_EXPORTNETWORKHISTORYREQUEST"]._serialized_end = 33608
-    _globals["_LISTENTITIESREQUEST"]._serialized_start = 33610
-    _globals["_LISTENTITIESREQUEST"]._serialized_end = 33680
-    _globals["_LISTENTITIESRESPONSE"]._serialized_start = 33683
-    _globals["_LISTENTITIESRESPONSE"]._serialized_end = 35392
-    _globals["_PINGREQUEST"]._serialized_start = 35394
-    _globals["_PINGREQUEST"]._serialized_end = 35407
-    _globals["_PINGRESPONSE"]._serialized_start = 35409
-    _globals["_PINGRESPONSE"]._serialized_end = 35423
-    _globals["_ORDERINFO"]._serialized_start = 35426
-    _globals["_ORDERINFO"]._serialized_end = 35561
-    _globals["_ESTIMATEPOSITIONREQUEST"]._serialized_start = 35564
-    _globals["_ESTIMATEPOSITIONREQUEST"]._serialized_end = 35796
-    _globals["_ESTIMATEPOSITIONRESPONSE"]._serialized_start = 35799
-    _globals["_ESTIMATEPOSITIONRESPONSE"]._serialized_end = 35954
-    _globals["_MARGINESTIMATE"]._serialized_start = 35956
-    _globals["_MARGINESTIMATE"]._serialized_end = 36072
-    _globals["_LIQUIDATIONESTIMATE"]._serialized_start = 36075
-    _globals["_LIQUIDATIONESTIMATE"]._serialized_end = 36226
-    _globals["_LIQUIDATIONPRICE"]._serialized_start = 36229
-    _globals["_LIQUIDATIONPRICE"]._serialized_end = 36391
-    _globals["_TRADINGDATASERVICE"]._serialized_start = 37275
-    _globals["_TRADINGDATASERVICE"]._serialized_end = 48307
+    _globals["_GETSTOPORDERREQUEST"]._serialized_start = 3479
+    _globals["_GETSTOPORDERREQUEST"]._serialized_end = 3533
+    _globals["_GETSTOPORDERRESPONSE"]._serialized_start = 3535
+    _globals["_GETSTOPORDERRESPONSE"]._serialized_end = 3611
+    _globals["_LISTSTOPORDERSREQUEST"]._serialized_start = 3614
+    _globals["_LISTSTOPORDERSREQUEST"]._serialized_end = 3792
+    _globals["_STOPORDERFILTER"]._serialized_start = 3795
+    _globals["_STOPORDERFILTER"]._serialized_end = 4080
+    _globals["_STOPORDEREDGE"]._serialized_start = 4082
+    _globals["_STOPORDEREDGE"]._serialized_end = 4173
+    _globals["_STOPORDERCONNECTION"]._serialized_start = 4176
+    _globals["_STOPORDERCONNECTION"]._serialized_end = 4307
+    _globals["_LISTSTOPORDERSRESPONSE"]._serialized_start = 4309
+    _globals["_LISTSTOPORDERSRESPONSE"]._serialized_end = 4395
+    _globals["_LISTPOSITIONSREQUEST"]._serialized_start = 4398
+    _globals["_LISTPOSITIONSREQUEST"]._serialized_end = 4561
+    _globals["_LISTPOSITIONSRESPONSE"]._serialized_start = 4563
+    _globals["_LISTPOSITIONSRESPONSE"]._serialized_end = 4657
+    _globals["_POSITIONSFILTER"]._serialized_start = 4659
+    _globals["_POSITIONSFILTER"]._serialized_end = 4736
+    _globals["_LISTALLPOSITIONSREQUEST"]._serialized_start = 4739
+    _globals["_LISTALLPOSITIONSREQUEST"]._serialized_end = 4903
+    _globals["_LISTALLPOSITIONSRESPONSE"]._serialized_start = 4905
+    _globals["_LISTALLPOSITIONSRESPONSE"]._serialized_end = 4998
+    _globals["_POSITIONEDGE"]._serialized_start = 5000
+    _globals["_POSITIONEDGE"]._serialized_end = 5074
+    _globals["_POSITIONCONNECTION"]._serialized_start = 5077
+    _globals["_POSITIONCONNECTION"]._serialized_end = 5206
+    _globals["_OBSERVEPOSITIONSREQUEST"]._serialized_start = 5208
+    _globals["_OBSERVEPOSITIONSREQUEST"]._serialized_end = 5326
+    _globals["_OBSERVEPOSITIONSRESPONSE"]._serialized_start = 5329
+    _globals["_OBSERVEPOSITIONSRESPONSE"]._serialized_end = 5498
+    _globals["_POSITIONSNAPSHOTPAGE"]._serialized_start = 5500
+    _globals["_POSITIONSNAPSHOTPAGE"]._serialized_end = 5597
+    _globals["_POSITIONUPDATES"]._serialized_start = 5599
+    _globals["_POSITIONUPDATES"]._serialized_end = 5662
+    _globals["_LEDGERENTRYFILTER"]._serialized_start = 5665
+    _globals["_LEDGERENTRYFILTER"]._serialized_end = 5956
+    _globals["_AGGREGATEDLEDGERENTRY"]._serialized_start = 5959
+    _globals["_AGGREGATEDLEDGERENTRY"]._serialized_end = 6688
+    _globals["_LISTLEDGERENTRIESREQUEST"]._serialized_start = 6691
+    _globals["_LISTLEDGERENTRIESREQUEST"]._serialized_end = 6937
+    _globals["_EXPORTLEDGERENTRIESREQUEST"]._serialized_start = 6940
+    _globals["_EXPORTLEDGERENTRIESREQUEST"]._serialized_end = 7113
+    _globals["_LISTLEDGERENTRIESRESPONSE"]._serialized_start = 7115
+    _globals["_LISTLEDGERENTRIESRESPONSE"]._serialized_end = 7233
+    _globals["_AGGREGATEDLEDGERENTRIESEDGE"]._serialized_start = 7235
+    _globals["_AGGREGATEDLEDGERENTRIESEDGE"]._serialized_end = 7348
+    _globals["_AGGREGATEDLEDGERENTRIESCONNECTION"]._serialized_start = 7351
+    _globals["_AGGREGATEDLEDGERENTRIESCONNECTION"]._serialized_end = 7510
+    _globals["_LISTBALANCECHANGESREQUEST"]._serialized_start = 7513
+    _globals["_LISTBALANCECHANGESREQUEST"]._serialized_end = 7756
+    _globals["_LISTBALANCECHANGESRESPONSE"]._serialized_start = 7758
+    _globals["_LISTBALANCECHANGESRESPONSE"]._serialized_end = 7860
+    _globals["_GETBALANCEHISTORYREQUEST"]._serialized_start = 7863
+    _globals["_GETBALANCEHISTORYREQUEST"]._serialized_end = 8163
+    _globals["_GETBALANCEHISTORYRESPONSE"]._serialized_start = 8165
+    _globals["_GETBALANCEHISTORYRESPONSE"]._serialized_end = 8266
+    _globals["_AGGREGATEDBALANCEEDGE"]._serialized_start = 8268
+    _globals["_AGGREGATEDBALANCEEDGE"]._serialized_end = 8371
+    _globals["_AGGREGATEDBALANCECONNECTION"]._serialized_start = 8374
+    _globals["_AGGREGATEDBALANCECONNECTION"]._serialized_end = 8521
+    _globals["_ACCOUNTFILTER"]._serialized_start = 8524
+    _globals["_ACCOUNTFILTER"]._serialized_end = 8682
+    _globals["_AGGREGATEDBALANCE"]._serialized_start = 8685
+    _globals["_AGGREGATEDBALANCE"]._serialized_end = 8974
+    _globals["_OBSERVEMARKETSDEPTHREQUEST"]._serialized_start = 8976
+    _globals["_OBSERVEMARKETSDEPTHREQUEST"]._serialized_end = 9035
+    _globals["_OBSERVEMARKETSDEPTHRESPONSE"]._serialized_start = 9037
+    _globals["_OBSERVEMARKETSDEPTHRESPONSE"]._serialized_end = 9120
+    _globals["_OBSERVEMARKETSDEPTHUPDATESREQUEST"]._serialized_start = 9122
+    _globals["_OBSERVEMARKETSDEPTHUPDATESREQUEST"]._serialized_end = 9188
+    _globals["_OBSERVEMARKETSDEPTHUPDATESRESPONSE"]._serialized_start = 9190
+    _globals["_OBSERVEMARKETSDEPTHUPDATESRESPONSE"]._serialized_end = 9275
+    _globals["_OBSERVEMARKETSDATAREQUEST"]._serialized_start = 9277
+    _globals["_OBSERVEMARKETSDATAREQUEST"]._serialized_end = 9335
+    _globals["_OBSERVEMARKETSDATARESPONSE"]._serialized_start = 9337
+    _globals["_OBSERVEMARKETSDATARESPONSE"]._serialized_end = 9416
+    _globals["_GETLATESTMARKETDEPTHREQUEST"]._serialized_start = 9418
+    _globals["_GETLATESTMARKETDEPTHREQUEST"]._serialized_end = 9530
+    _globals["_GETLATESTMARKETDEPTHRESPONSE"]._serialized_start = 9533
+    _globals["_GETLATESTMARKETDEPTHRESPONSE"]._serialized_end = 9751
+    _globals["_LISTLATESTMARKETDATAREQUEST"]._serialized_start = 9753
+    _globals["_LISTLATESTMARKETDATAREQUEST"]._serialized_end = 9782
+    _globals["_LISTLATESTMARKETDATARESPONSE"]._serialized_start = 9784
+    _globals["_LISTLATESTMARKETDATARESPONSE"]._serialized_end = 9867
+    _globals["_GETLATESTMARKETDATAREQUEST"]._serialized_start = 9869
+    _globals["_GETLATESTMARKETDATAREQUEST"]._serialized_end = 9932
+    _globals["_GETLATESTMARKETDATARESPONSE"]._serialized_start = 9934
+    _globals["_GETLATESTMARKETDATARESPONSE"]._serialized_end = 10014
+    _globals["_GETMARKETDATAHISTORYBYIDREQUEST"]._serialized_start = 10017
+    _globals["_GETMARKETDATAHISTORYBYIDREQUEST"]._serialized_end = 10298
+    _globals["_GETMARKETDATAHISTORYBYIDRESPONSE"]._serialized_start = 10300
+    _globals["_GETMARKETDATAHISTORYBYIDRESPONSE"]._serialized_end = 10406
+    _globals["_MARKETDATAEDGE"]._serialized_start = 10408
+    _globals["_MARKETDATAEDGE"]._serialized_end = 10486
+    _globals["_MARKETDATACONNECTION"]._serialized_start = 10489
+    _globals["_MARKETDATACONNECTION"]._serialized_end = 10622
+    _globals["_LISTTRANSFERSREQUEST"]._serialized_start = 10625
+    _globals["_LISTTRANSFERSREQUEST"]._serialized_end = 10834
+    _globals["_LISTTRANSFERSRESPONSE"]._serialized_start = 10836
+    _globals["_LISTTRANSFERSRESPONSE"]._serialized_end = 10926
+    _globals["_TRANSFEREDGE"]._serialized_start = 10928
+    _globals["_TRANSFEREDGE"]._serialized_end = 11012
+    _globals["_TRANSFERCONNECTION"]._serialized_start = 11015
+    _globals["_TRANSFERCONNECTION"]._serialized_end = 11144
+    _globals["_GETNETWORKLIMITSREQUEST"]._serialized_start = 11146
+    _globals["_GETNETWORKLIMITSREQUEST"]._serialized_end = 11171
+    _globals["_GETNETWORKLIMITSRESPONSE"]._serialized_start = 11173
+    _globals["_GETNETWORKLIMITSRESPONSE"]._serialized_end = 11244
+    _globals["_LISTCANDLEINTERVALSREQUEST"]._serialized_start = 11246
+    _globals["_LISTCANDLEINTERVALSREQUEST"]._serialized_end = 11309
+    _globals["_INTERVALTOCANDLEID"]._serialized_start = 11311
+    _globals["_INTERVALTOCANDLEID"]._serialized_end = 11388
+    _globals["_LISTCANDLEINTERVALSRESPONSE"]._serialized_start = 11390
+    _globals["_LISTCANDLEINTERVALSRESPONSE"]._serialized_end = 11507
+    _globals["_CANDLE"]._serialized_start = 11510
+    _globals["_CANDLE"]._serialized_end = 11705
+    _globals["_OBSERVECANDLEDATAREQUEST"]._serialized_start = 11707
+    _globals["_OBSERVECANDLEDATAREQUEST"]._serialized_end = 11768
+    _globals["_OBSERVECANDLEDATARESPONSE"]._serialized_start = 11770
+    _globals["_OBSERVECANDLEDATARESPONSE"]._serialized_end = 11846
+    _globals["_LISTCANDLEDATAREQUEST"]._serialized_start = 11849
+    _globals["_LISTCANDLEDATAREQUEST"]._serialized_end = 12068
+    _globals["_LISTCANDLEDATARESPONSE"]._serialized_start = 12070
+    _globals["_LISTCANDLEDATARESPONSE"]._serialized_end = 12159
+    _globals["_CANDLEEDGE"]._serialized_start = 12161
+    _globals["_CANDLEEDGE"]._serialized_end = 12242
+    _globals["_CANDLEDATACONNECTION"]._serialized_start = 12245
+    _globals["_CANDLEDATACONNECTION"]._serialized_end = 12374
+    _globals["_LISTVOTESREQUEST"]._serialized_start = 12377
+    _globals["_LISTVOTESREQUEST"]._serialized_end = 12575
+    _globals["_LISTVOTESRESPONSE"]._serialized_start = 12577
+    _globals["_LISTVOTESRESPONSE"]._serialized_end = 12651
+    _globals["_VOTEEDGE"]._serialized_start = 12653
+    _globals["_VOTEEDGE"]._serialized_end = 12719
+    _globals["_VOTECONNECTION"]._serialized_start = 12721
+    _globals["_VOTECONNECTION"]._serialized_end = 12842
+    _globals["_OBSERVEVOTESREQUEST"]._serialized_start = 12844
+    _globals["_OBSERVEVOTESREQUEST"]._serialized_end = 12964
+    _globals["_OBSERVEVOTESRESPONSE"]._serialized_start = 12966
+    _globals["_OBSERVEVOTESRESPONSE"]._serialized_end = 13020
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST"]._serialized_start = 13023
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST"]._serialized_end = 13212
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE"]._serialized_start = 13214
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE"]._serialized_end = 13338
+    _globals["_ERC20MULTISIGSIGNERADDEDEDGE"]._serialized_start = 13340
+    _globals["_ERC20MULTISIGSIGNERADDEDEDGE"]._serialized_end = 13456
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLEEDGE"]._serialized_start = 13459
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLEEDGE"]._serialized_end = 13588
+    _globals["_ERC20MULTISIGSIGNERADDEDCONNECTION"]._serialized_start = 13591
+    _globals["_ERC20MULTISIGSIGNERADDEDCONNECTION"]._serialized_end = 13758
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLE"]._serialized_start = 13761
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLE"]._serialized_end = 13967
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST"]._serialized_start = 13970
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST"]._serialized_end = 14161
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE"]._serialized_start = 14164
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE"]._serialized_end = 14292
+    _globals["_ERC20MULTISIGSIGNERREMOVEDEDGE"]._serialized_start = 14294
+    _globals["_ERC20MULTISIGSIGNERREMOVEDEDGE"]._serialized_end = 14414
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE"]._serialized_start = 14417
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE"]._serialized_end = 14550
+    _globals["_ERC20MULTISIGSIGNERREMOVEDCONNECTION"]._serialized_start = 14553
+    _globals["_ERC20MULTISIGSIGNERREMOVEDCONNECTION"]._serialized_end = 14724
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLE"]._serialized_start = 14727
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLE"]._serialized_end = 14935
+    _globals["_GETERC20LISTASSETBUNDLEREQUEST"]._serialized_start = 14937
+    _globals["_GETERC20LISTASSETBUNDLEREQUEST"]._serialized_end = 15002
+    _globals["_GETERC20LISTASSETBUNDLERESPONSE"]._serialized_start = 15005
+    _globals["_GETERC20LISTASSETBUNDLERESPONSE"]._serialized_end = 15163
+    _globals["_GETERC20SETASSETLIMITSBUNDLEREQUEST"]._serialized_start = 15165
+    _globals["_GETERC20SETASSETLIMITSBUNDLEREQUEST"]._serialized_end = 15241
+    _globals["_GETERC20SETASSETLIMITSBUNDLERESPONSE"]._serialized_start = 15244
+    _globals["_GETERC20SETASSETLIMITSBUNDLERESPONSE"]._serialized_end = 15476
+    _globals["_GETERC20WITHDRAWALAPPROVALREQUEST"]._serialized_start = 15478
+    _globals["_GETERC20WITHDRAWALAPPROVALREQUEST"]._serialized_end = 15556
+    _globals["_GETERC20WITHDRAWALAPPROVALRESPONSE"]._serialized_start = 15559
+    _globals["_GETERC20WITHDRAWALAPPROVALRESPONSE"]._serialized_end = 15781
+    _globals["_GETLASTTRADEREQUEST"]._serialized_start = 15783
+    _globals["_GETLASTTRADEREQUEST"]._serialized_end = 15839
+    _globals["_GETLASTTRADERESPONSE"]._serialized_start = 15841
+    _globals["_GETLASTTRADERESPONSE"]._serialized_end = 15898
+    _globals["_LISTTRADESREQUEST"]._serialized_start = 15901
+    _globals["_LISTTRADESREQUEST"]._serialized_end = 16169
+    _globals["_LISTTRADESRESPONSE"]._serialized_start = 16171
+    _globals["_LISTTRADESRESPONSE"]._serialized_end = 16249
+    _globals["_TRADECONNECTION"]._serialized_start = 16251
+    _globals["_TRADECONNECTION"]._serialized_end = 16374
+    _globals["_TRADEEDGE"]._serialized_start = 16376
+    _globals["_TRADEEDGE"]._serialized_end = 16444
+    _globals["_OBSERVETRADESREQUEST"]._serialized_start = 16446
+    _globals["_OBSERVETRADESREQUEST"]._serialized_end = 16528
+    _globals["_OBSERVETRADESRESPONSE"]._serialized_start = 16530
+    _globals["_OBSERVETRADESRESPONSE"]._serialized_end = 16590
+    _globals["_GETORACLESPECREQUEST"]._serialized_start = 16592
+    _globals["_GETORACLESPECREQUEST"]._serialized_end = 16658
+    _globals["_GETORACLESPECRESPONSE"]._serialized_start = 16660
+    _globals["_GETORACLESPECRESPONSE"]._serialized_end = 16734
+    _globals["_LISTORACLESPECSREQUEST"]._serialized_start = 16736
+    _globals["_LISTORACLESPECSREQUEST"]._serialized_end = 16841
+    _globals["_LISTORACLESPECSRESPONSE"]._serialized_start = 16843
+    _globals["_LISTORACLESPECSRESPONSE"]._serialized_end = 16943
+    _globals["_LISTORACLEDATAREQUEST"]._serialized_start = 16946
+    _globals["_LISTORACLEDATAREQUEST"]._serialized_end = 17112
+    _globals["_LISTORACLEDATARESPONSE"]._serialized_start = 17114
+    _globals["_LISTORACLEDATARESPONSE"]._serialized_end = 17210
+    _globals["_ORACLESPECEDGE"]._serialized_start = 17212
+    _globals["_ORACLESPECEDGE"]._serialized_end = 17290
+    _globals["_ORACLESPECSCONNECTION"]._serialized_start = 17293
+    _globals["_ORACLESPECSCONNECTION"]._serialized_end = 17427
+    _globals["_ORACLEDATAEDGE"]._serialized_start = 17429
+    _globals["_ORACLEDATAEDGE"]._serialized_end = 17507
+    _globals["_ORACLEDATACONNECTION"]._serialized_start = 17510
+    _globals["_ORACLEDATACONNECTION"]._serialized_end = 17643
+    _globals["_GETMARKETREQUEST"]._serialized_start = 17645
+    _globals["_GETMARKETREQUEST"]._serialized_end = 17698
+    _globals["_GETMARKETRESPONSE"]._serialized_start = 17700
+    _globals["_GETMARKETRESPONSE"]._serialized_end = 17757
+    _globals["_LISTMARKETSREQUEST"]._serialized_start = 17760
+    _globals["_LISTMARKETSREQUEST"]._serialized_end = 17927
+    _globals["_LISTMARKETSRESPONSE"]._serialized_start = 17929
+    _globals["_LISTMARKETSRESPONSE"]._serialized_end = 18011
+    _globals["_MARKETEDGE"]._serialized_start = 18013
+    _globals["_MARKETEDGE"]._serialized_end = 18083
+    _globals["_MARKETCONNECTION"]._serialized_start = 18085
+    _globals["_MARKETCONNECTION"]._serialized_end = 18210
+    _globals["_LISTSUCCESSORMARKETSREQUEST"]._serialized_start = 18213
+    _globals["_LISTSUCCESSORMARKETSREQUEST"]._serialized_end = 18388
+    _globals["_SUCCESSORMARKET"]._serialized_start = 18390
+    _globals["_SUCCESSORMARKET"]._serialized_end = 18497
+    _globals["_SUCCESSORMARKETEDGE"]._serialized_start = 18499
+    _globals["_SUCCESSORMARKETEDGE"]._serialized_end = 18598
+    _globals["_SUCCESSORMARKETCONNECTION"]._serialized_start = 18601
+    _globals["_SUCCESSORMARKETCONNECTION"]._serialized_end = 18744
+    _globals["_LISTSUCCESSORMARKETSRESPONSE"]._serialized_start = 18746
+    _globals["_LISTSUCCESSORMARKETSRESPONSE"]._serialized_end = 18865
+    _globals["_GETPARTYREQUEST"]._serialized_start = 18867
+    _globals["_GETPARTYREQUEST"]._serialized_end = 18917
+    _globals["_GETPARTYRESPONSE"]._serialized_start = 18919
+    _globals["_GETPARTYRESPONSE"]._serialized_end = 18972
+    _globals["_LISTPARTIESREQUEST"]._serialized_start = 18974
+    _globals["_LISTPARTIESREQUEST"]._serialized_end = 19082
+    _globals["_LISTPARTIESRESPONSE"]._serialized_start = 19084
+    _globals["_LISTPARTIESRESPONSE"]._serialized_end = 19165
+    _globals["_PARTYEDGE"]._serialized_start = 19167
+    _globals["_PARTYEDGE"]._serialized_end = 19235
+    _globals["_PARTYCONNECTION"]._serialized_start = 19237
+    _globals["_PARTYCONNECTION"]._serialized_end = 19360
+    _globals["_ORDEREDGE"]._serialized_start = 19362
+    _globals["_ORDEREDGE"]._serialized_end = 19430
+    _globals["_LISTMARGINLEVELSREQUEST"]._serialized_start = 19433
+    _globals["_LISTMARGINLEVELSREQUEST"]._serialized_end = 19575
+    _globals["_LISTMARGINLEVELSRESPONSE"]._serialized_start = 19577
+    _globals["_LISTMARGINLEVELSRESPONSE"]._serialized_end = 19675
+    _globals["_OBSERVEMARGINLEVELSREQUEST"]._serialized_start = 19677
+    _globals["_OBSERVEMARGINLEVELSREQUEST"]._serialized_end = 19780
+    _globals["_OBSERVEMARGINLEVELSRESPONSE"]._serialized_start = 19782
+    _globals["_OBSERVEMARGINLEVELSRESPONSE"]._serialized_end = 19868
+    _globals["_ORDERCONNECTION"]._serialized_start = 19870
+    _globals["_ORDERCONNECTION"]._serialized_end = 19993
+    _globals["_MARGINEDGE"]._serialized_start = 19995
+    _globals["_MARGINEDGE"]._serialized_end = 20071
+    _globals["_MARGINCONNECTION"]._serialized_start = 20073
+    _globals["_MARGINCONNECTION"]._serialized_end = 20198
+    _globals["_LISTREWARDSREQUEST"]._serialized_start = 20201
+    _globals["_LISTREWARDSREQUEST"]._serialized_end = 20470
+    _globals["_LISTREWARDSRESPONSE"]._serialized_start = 20472
+    _globals["_LISTREWARDSRESPONSE"]._serialized_end = 20555
+    _globals["_REWARDEDGE"]._serialized_start = 20557
+    _globals["_REWARDEDGE"]._serialized_end = 20627
+    _globals["_REWARDSCONNECTION"]._serialized_start = 20629
+    _globals["_REWARDSCONNECTION"]._serialized_end = 20755
+    _globals["_LISTREWARDSUMMARIESREQUEST"]._serialized_start = 20758
+    _globals["_LISTREWARDSUMMARIESREQUEST"]._serialized_end = 20957
+    _globals["_LISTREWARDSUMMARIESRESPONSE"]._serialized_start = 20959
+    _globals["_LISTREWARDSUMMARIESRESPONSE"]._serialized_end = 21039
+    _globals["_REWARDSUMMARYFILTER"]._serialized_start = 21042
+    _globals["_REWARDSUMMARYFILTER"]._serialized_end = 21219
+    _globals["_LISTEPOCHREWARDSUMMARIESREQUEST"]._serialized_start = 21222
+    _globals["_LISTEPOCHREWARDSUMMARIESREQUEST"]._serialized_end = 21398
+    _globals["_LISTEPOCHREWARDSUMMARIESRESPONSE"]._serialized_start = 21400
+    _globals["_LISTEPOCHREWARDSUMMARIESRESPONSE"]._serialized_end = 21511
+    _globals["_EPOCHREWARDSUMMARYCONNECTION"]._serialized_start = 21514
+    _globals["_EPOCHREWARDSUMMARYCONNECTION"]._serialized_end = 21663
+    _globals["_EPOCHREWARDSUMMARYEDGE"]._serialized_start = 21665
+    _globals["_EPOCHREWARDSUMMARYEDGE"]._serialized_end = 21759
+    _globals["_OBSERVEREWARDSREQUEST"]._serialized_start = 21761
+    _globals["_OBSERVEREWARDSREQUEST"]._serialized_end = 21874
+    _globals["_OBSERVEREWARDSRESPONSE"]._serialized_start = 21876
+    _globals["_OBSERVEREWARDSRESPONSE"]._serialized_end = 21938
+    _globals["_GETDEPOSITREQUEST"]._serialized_start = 21940
+    _globals["_GETDEPOSITREQUEST"]._serialized_end = 21981
+    _globals["_GETDEPOSITRESPONSE"]._serialized_start = 21983
+    _globals["_GETDEPOSITRESPONSE"]._serialized_end = 22044
+    _globals["_LISTDEPOSITSREQUEST"]._serialized_start = 22047
+    _globals["_LISTDEPOSITSREQUEST"]._serialized_end = 22255
+    _globals["_LISTDEPOSITSRESPONSE"]._serialized_start = 22257
+    _globals["_LISTDEPOSITSRESPONSE"]._serialized_end = 22344
+    _globals["_DEPOSITEDGE"]._serialized_start = 22346
+    _globals["_DEPOSITEDGE"]._serialized_end = 22418
+    _globals["_DEPOSITSCONNECTION"]._serialized_start = 22421
+    _globals["_DEPOSITSCONNECTION"]._serialized_end = 22549
+    _globals["_GETWITHDRAWALREQUEST"]._serialized_start = 22551
+    _globals["_GETWITHDRAWALREQUEST"]._serialized_end = 22595
+    _globals["_GETWITHDRAWALRESPONSE"]._serialized_start = 22597
+    _globals["_GETWITHDRAWALRESPONSE"]._serialized_end = 22670
+    _globals["_LISTWITHDRAWALSREQUEST"]._serialized_start = 22673
+    _globals["_LISTWITHDRAWALSREQUEST"]._serialized_end = 22884
+    _globals["_LISTWITHDRAWALSRESPONSE"]._serialized_start = 22886
+    _globals["_LISTWITHDRAWALSRESPONSE"]._serialized_end = 22985
+    _globals["_WITHDRAWALEDGE"]._serialized_start = 22987
+    _globals["_WITHDRAWALEDGE"]._serialized_end = 23065
+    _globals["_WITHDRAWALSCONNECTION"]._serialized_start = 23068
+    _globals["_WITHDRAWALSCONNECTION"]._serialized_end = 23202
+    _globals["_GETASSETREQUEST"]._serialized_start = 23204
+    _globals["_GETASSETREQUEST"]._serialized_end = 23254
+    _globals["_GETASSETRESPONSE"]._serialized_start = 23256
+    _globals["_GETASSETRESPONSE"]._serialized_end = 23309
+    _globals["_LISTASSETSREQUEST"]._serialized_start = 23312
+    _globals["_LISTASSETSREQUEST"]._serialized_end = 23457
+    _globals["_LISTASSETSRESPONSE"]._serialized_start = 23459
+    _globals["_LISTASSETSRESPONSE"]._serialized_end = 23538
+    _globals["_ASSETEDGE"]._serialized_start = 23540
+    _globals["_ASSETEDGE"]._serialized_end = 23608
+    _globals["_ASSETSCONNECTION"]._serialized_start = 23610
+    _globals["_ASSETSCONNECTION"]._serialized_end = 23734
+    _globals["_LISTLIQUIDITYPROVISIONSREQUEST"]._serialized_start = 23737
+    _globals["_LISTLIQUIDITYPROVISIONSREQUEST"]._serialized_end = 24026
+    _globals["_LISTLIQUIDITYPROVISIONSRESPONSE"]._serialized_start = 24029
+    _globals["_LISTLIQUIDITYPROVISIONSRESPONSE"]._serialized_end = 24161
+    _globals["_LIQUIDITYPROVISIONSEDGE"]._serialized_start = 24163
+    _globals["_LIQUIDITYPROVISIONSEDGE"]._serialized_end = 24258
+    _globals["_LIQUIDITYPROVISIONSCONNECTION"]._serialized_start = 24261
+    _globals["_LIQUIDITYPROVISIONSCONNECTION"]._serialized_end = 24412
+    _globals["_OBSERVELIQUIDITYPROVISIONSREQUEST"]._serialized_start = 24415
+    _globals["_OBSERVELIQUIDITYPROVISIONSREQUEST"]._serialized_end = 24543
+    _globals["_OBSERVELIQUIDITYPROVISIONSRESPONSE"]._serialized_start = 24545
+    _globals["_OBSERVELIQUIDITYPROVISIONSRESPONSE"]._serialized_end = 24658
+    _globals["_GETGOVERNANCEDATAREQUEST"]._serialized_start = 24661
+    _globals["_GETGOVERNANCEDATAREQUEST"]._serialized_end = 24790
+    _globals["_GETGOVERNANCEDATARESPONSE"]._serialized_start = 24792
+    _globals["_GETGOVERNANCEDATARESPONSE"]._serialized_end = 24861
+    _globals["_LISTGOVERNANCEDATAREQUEST"]._serialized_start = 24864
+    _globals["_LISTGOVERNANCEDATAREQUEST"]._serialized_end = 25498
+    _globals["_LISTGOVERNANCEDATAREQUEST_TYPE"]._serialized_start = 25218
+    _globals["_LISTGOVERNANCEDATAREQUEST_TYPE"]._serialized_end = 25401
+    _globals["_LISTGOVERNANCEDATARESPONSE"]._serialized_start = 25500
+    _globals["_LISTGOVERNANCEDATARESPONSE"]._serialized_end = 25603
+    _globals["_GOVERNANCEDATAEDGE"]._serialized_start = 25605
+    _globals["_GOVERNANCEDATAEDGE"]._serialized_end = 25691
+    _globals["_GOVERNANCEDATACONNECTION"]._serialized_start = 25694
+    _globals["_GOVERNANCEDATACONNECTION"]._serialized_end = 25835
+    _globals["_OBSERVEGOVERNANCEREQUEST"]._serialized_start = 25837
+    _globals["_OBSERVEGOVERNANCEREQUEST"]._serialized_end = 25908
+    _globals["_OBSERVEGOVERNANCERESPONSE"]._serialized_start = 25910
+    _globals["_OBSERVEGOVERNANCERESPONSE"]._serialized_end = 25979
+    _globals["_LISTDELEGATIONSREQUEST"]._serialized_start = 25982
+    _globals["_LISTDELEGATIONSREQUEST"]._serialized_end = 26219
+    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_start = 26221
+    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_end = 26320
+    _globals["_DELEGATIONEDGE"]._serialized_start = 26322
+    _globals["_DELEGATIONEDGE"]._serialized_end = 26400
+    _globals["_DELEGATIONSCONNECTION"]._serialized_start = 26403
+    _globals["_DELEGATIONSCONNECTION"]._serialized_end = 26537
+    _globals["_OBSERVEDELEGATIONSREQUEST"]._serialized_start = 26539
+    _globals["_OBSERVEDELEGATIONSREQUEST"]._serialized_end = 26653
+    _globals["_OBSERVEDELEGATIONSRESPONSE"]._serialized_start = 26655
+    _globals["_OBSERVEDELEGATIONSRESPONSE"]._serialized_end = 26733
+    _globals["_NODEBASIC"]._serialized_start = 26736
+    _globals["_NODEBASIC"]._serialized_end = 27009
+    _globals["_GETNETWORKDATAREQUEST"]._serialized_start = 27011
+    _globals["_GETNETWORKDATAREQUEST"]._serialized_end = 27034
+    _globals["_GETNETWORKDATARESPONSE"]._serialized_start = 27036
+    _globals["_GETNETWORKDATARESPONSE"]._serialized_end = 27105
+    _globals["_GETNODEREQUEST"]._serialized_start = 27107
+    _globals["_GETNODEREQUEST"]._serialized_end = 27145
+    _globals["_GETNODERESPONSE"]._serialized_start = 27147
+    _globals["_GETNODERESPONSE"]._serialized_end = 27196
+    _globals["_LISTNODESREQUEST"]._serialized_start = 27199
+    _globals["_LISTNODESREQUEST"]._serialized_end = 27346
+    _globals["_LISTNODESRESPONSE"]._serialized_start = 27348
+    _globals["_LISTNODESRESPONSE"]._serialized_end = 27423
+    _globals["_NODEEDGE"]._serialized_start = 27425
+    _globals["_NODEEDGE"]._serialized_end = 27491
+    _globals["_NODESCONNECTION"]._serialized_start = 27493
+    _globals["_NODESCONNECTION"]._serialized_end = 27615
+    _globals["_LISTNODESIGNATURESREQUEST"]._serialized_start = 27618
+    _globals["_LISTNODESIGNATURESREQUEST"]._serialized_end = 27748
+    _globals["_LISTNODESIGNATURESRESPONSE"]._serialized_start = 27750
+    _globals["_LISTNODESIGNATURESRESPONSE"]._serialized_end = 27853
+    _globals["_NODESIGNATUREEDGE"]._serialized_start = 27855
+    _globals["_NODESIGNATUREEDGE"]._serialized_end = 27951
+    _globals["_NODESIGNATURESCONNECTION"]._serialized_start = 27954
+    _globals["_NODESIGNATURESCONNECTION"]._serialized_end = 28094
+    _globals["_GETEPOCHREQUEST"]._serialized_start = 28096
+    _globals["_GETEPOCHREQUEST"]._serialized_end = 28178
+    _globals["_GETEPOCHRESPONSE"]._serialized_start = 28180
+    _globals["_GETEPOCHRESPONSE"]._serialized_end = 28233
+    _globals["_ESTIMATEFEEREQUEST"]._serialized_start = 28235
+    _globals["_ESTIMATEFEEREQUEST"]._serialized_end = 28344
+    _globals["_ESTIMATEFEERESPONSE"]._serialized_start = 28346
+    _globals["_ESTIMATEFEERESPONSE"]._serialized_end = 28396
+    _globals["_ESTIMATEMARGINREQUEST"]._serialized_start = 28399
+    _globals["_ESTIMATEMARGINREQUEST"]._serialized_end = 28630
+    _globals["_ESTIMATEMARGINRESPONSE"]._serialized_start = 28632
+    _globals["_ESTIMATEMARGINRESPONSE"]._serialized_end = 28717
+    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_start = 28719
+    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_end = 28830
+    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_start = 28832
+    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_end = 28955
+    _globals["_GETNETWORKPARAMETERREQUEST"]._serialized_start = 28957
+    _globals["_GETNETWORKPARAMETERREQUEST"]._serialized_end = 29009
+    _globals["_GETNETWORKPARAMETERRESPONSE"]._serialized_start = 29011
+    _globals["_GETNETWORKPARAMETERRESPONSE"]._serialized_end = 29109
+    _globals["_NETWORKPARAMETEREDGE"]._serialized_start = 29111
+    _globals["_NETWORKPARAMETEREDGE"]._serialized_end = 29201
+    _globals["_NETWORKPARAMETERCONNECTION"]._serialized_start = 29204
+    _globals["_NETWORKPARAMETERCONNECTION"]._serialized_end = 29349
+    _globals["_CHECKPOINT"]._serialized_start = 29351
+    _globals["_CHECKPOINT"]._serialized_end = 29441
+    _globals["_LISTCHECKPOINTSREQUEST"]._serialized_start = 29443
+    _globals["_LISTCHECKPOINTSREQUEST"]._serialized_end = 29548
+    _globals["_LISTCHECKPOINTSRESPONSE"]._serialized_start = 29550
+    _globals["_LISTCHECKPOINTSRESPONSE"]._serialized_end = 29649
+    _globals["_CHECKPOINTEDGE"]._serialized_start = 29651
+    _globals["_CHECKPOINTEDGE"]._serialized_end = 29740
+    _globals["_CHECKPOINTSCONNECTION"]._serialized_start = 29743
+    _globals["_CHECKPOINTSCONNECTION"]._serialized_end = 29877
+    _globals["_GETSTAKEREQUEST"]._serialized_start = 29880
+    _globals["_GETSTAKEREQUEST"]._serialized_end = 30011
+    _globals["_GETSTAKERESPONSE"]._serialized_start = 30014
+    _globals["_GETSTAKERESPONSE"]._serialized_end = 30162
+    _globals["_STAKELINKINGEDGE"]._serialized_start = 30164
+    _globals["_STAKELINKINGEDGE"]._serialized_end = 30256
+    _globals["_STAKESCONNECTION"]._serialized_start = 30259
+    _globals["_STAKESCONNECTION"]._serialized_end = 30390
+    _globals["_GETRISKFACTORSREQUEST"]._serialized_start = 30392
+    _globals["_GETRISKFACTORSREQUEST"]._serialized_end = 30450
+    _globals["_GETRISKFACTORSRESPONSE"]._serialized_start = 30452
+    _globals["_GETRISKFACTORSRESPONSE"]._serialized_end = 30527
+    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_start = 30530
+    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_end = 30691
+    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_start = 30693
+    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_end = 30768
+    _globals["_OBSERVELEDGERMOVEMENTSREQUEST"]._serialized_start = 30770
+    _globals["_OBSERVELEDGERMOVEMENTSREQUEST"]._serialized_end = 30801
+    _globals["_OBSERVELEDGERMOVEMENTSRESPONSE"]._serialized_start = 30803
+    _globals["_OBSERVELEDGERMOVEMENTSRESPONSE"]._serialized_end = 30898
+    _globals["_LISTKEYROTATIONSREQUEST"]._serialized_start = 30901
+    _globals["_LISTKEYROTATIONSREQUEST"]._serialized_end = 31049
+    _globals["_LISTKEYROTATIONSRESPONSE"]._serialized_start = 31051
+    _globals["_LISTKEYROTATIONSRESPONSE"]._serialized_end = 31147
+    _globals["_KEYROTATIONEDGE"]._serialized_start = 31149
+    _globals["_KEYROTATIONEDGE"]._serialized_end = 31239
+    _globals["_KEYROTATIONCONNECTION"]._serialized_start = 31242
+    _globals["_KEYROTATIONCONNECTION"]._serialized_end = 31377
+    _globals["_LISTETHEREUMKEYROTATIONSREQUEST"]._serialized_start = 31380
+    _globals["_LISTETHEREUMKEYROTATIONSREQUEST"]._serialized_end = 31536
+    _globals["_LISTETHEREUMKEYROTATIONSRESPONSE"]._serialized_start = 31538
+    _globals["_LISTETHEREUMKEYROTATIONSRESPONSE"]._serialized_end = 31658
+    _globals["_ETHEREUMKEYROTATIONSCONNECTION"]._serialized_start = 31661
+    _globals["_ETHEREUMKEYROTATIONSCONNECTION"]._serialized_end = 31813
+    _globals["_ETHEREUMKEYROTATIONEDGE"]._serialized_start = 31815
+    _globals["_ETHEREUMKEYROTATIONEDGE"]._serialized_end = 31921
+    _globals["_GETVEGATIMEREQUEST"]._serialized_start = 31923
+    _globals["_GETVEGATIMEREQUEST"]._serialized_end = 31943
+    _globals["_GETVEGATIMERESPONSE"]._serialized_start = 31945
+    _globals["_GETVEGATIMERESPONSE"]._serialized_end = 31996
+    _globals["_DATERANGE"]._serialized_start = 31999
+    _globals["_DATERANGE"]._serialized_end = 32136
+    _globals["_GETPROTOCOLUPGRADESTATUSREQUEST"]._serialized_start = 32138
+    _globals["_GETPROTOCOLUPGRADESTATUSREQUEST"]._serialized_end = 32171
+    _globals["_GETPROTOCOLUPGRADESTATUSRESPONSE"]._serialized_start = 32173
+    _globals["_GETPROTOCOLUPGRADESTATUSRESPONSE"]._serialized_end = 32229
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSREQUEST"]._serialized_start = 32232
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSREQUEST"]._serialized_end = 32491
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSRESPONSE"]._serialized_start = 32494
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSRESPONSE"]._serialized_end = 32646
+    _globals["_PROTOCOLUPGRADEPROPOSALCONNECTION"]._serialized_start = 32649
+    _globals["_PROTOCOLUPGRADEPROPOSALCONNECTION"]._serialized_end = 32808
+    _globals["_PROTOCOLUPGRADEPROPOSALEDGE"]._serialized_start = 32810
+    _globals["_PROTOCOLUPGRADEPROPOSALEDGE"]._serialized_end = 32921
+    _globals["_LISTCORESNAPSHOTSREQUEST"]._serialized_start = 32923
+    _globals["_LISTCORESNAPSHOTSREQUEST"]._serialized_end = 33030
+    _globals["_LISTCORESNAPSHOTSRESPONSE"]._serialized_start = 33032
+    _globals["_LISTCORESNAPSHOTSRESPONSE"]._serialized_end = 33139
+    _globals["_CORESNAPSHOTCONNECTION"]._serialized_start = 33142
+    _globals["_CORESNAPSHOTCONNECTION"]._serialized_end = 33279
+    _globals["_CORESNAPSHOTEDGE"]._serialized_start = 33281
+    _globals["_CORESNAPSHOTEDGE"]._serialized_end = 33377
+    _globals["_HISTORYSEGMENT"]._serialized_start = 33380
+    _globals["_HISTORYSEGMENT"]._serialized_end = 33637
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST"]._serialized_start = 33639
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST"]._serialized_end = 33682
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE"]._serialized_start = 33685
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE"]._serialized_end = 33826
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSREQUEST"]._serialized_start = 33828
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSREQUEST"]._serialized_end = 33866
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSRESPONSE"]._serialized_start = 33868
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSRESPONSE"]._serialized_end = 33968
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST"]._serialized_start = 33970
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST"]._serialized_end = 34015
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE"]._serialized_start = 34017
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE"]._serialized_end = 34098
+    _globals["_GETNETWORKHISTORYSTATUSREQUEST"]._serialized_start = 34100
+    _globals["_GETNETWORKHISTORYSTATUSREQUEST"]._serialized_end = 34132
+    _globals["_GETNETWORKHISTORYSTATUSRESPONSE"]._serialized_start = 34135
+    _globals["_GETNETWORKHISTORYSTATUSRESPONSE"]._serialized_end = 34311
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST"]._serialized_start = 34313
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST"]._serialized_end = 34353
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE"]._serialized_start = 34355
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE"]._serialized_end = 34437
+    _globals["_EXPORTNETWORKHISTORYREQUEST"]._serialized_start = 34440
+    _globals["_EXPORTNETWORKHISTORYREQUEST"]._serialized_end = 34573
+    _globals["_LISTENTITIESREQUEST"]._serialized_start = 34575
+    _globals["_LISTENTITIESREQUEST"]._serialized_end = 34645
+    _globals["_LISTENTITIESRESPONSE"]._serialized_start = 34648
+    _globals["_LISTENTITIESRESPONSE"]._serialized_end = 36357
+    _globals["_PINGREQUEST"]._serialized_start = 36359
+    _globals["_PINGREQUEST"]._serialized_end = 36372
+    _globals["_PINGRESPONSE"]._serialized_start = 36374
+    _globals["_PINGRESPONSE"]._serialized_end = 36388
+    _globals["_ORDERINFO"]._serialized_start = 36391
+    _globals["_ORDERINFO"]._serialized_end = 36526
+    _globals["_ESTIMATEPOSITIONREQUEST"]._serialized_start = 36529
+    _globals["_ESTIMATEPOSITIONREQUEST"]._serialized_end = 36761
+    _globals["_ESTIMATEPOSITIONRESPONSE"]._serialized_start = 36764
+    _globals["_ESTIMATEPOSITIONRESPONSE"]._serialized_end = 36919
+    _globals["_MARGINESTIMATE"]._serialized_start = 36921
+    _globals["_MARGINESTIMATE"]._serialized_end = 37037
+    _globals["_LIQUIDATIONESTIMATE"]._serialized_start = 37040
+    _globals["_LIQUIDATIONESTIMATE"]._serialized_end = 37191
+    _globals["_LIQUIDATIONPRICE"]._serialized_start = 37194
+    _globals["_LIQUIDATIONPRICE"]._serialized_end = 37356
+    _globals["_TRADINGDATASERVICE"]._serialized_start = 38240
+    _globals["_TRADINGDATASERVICE"]._serialized_end = 49490
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py` & `vega_sim-1.2.1/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,24 @@
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListOrderVersionsResponse.FromString,
         )
         self.ObserveOrders = channel.unary_stream(
             "/datanode.api.v2.TradingDataService/ObserveOrders",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObserveOrdersRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObserveOrdersResponse.FromString,
         )
+        self.GetStopOrder = channel.unary_unary(
+            "/datanode.api.v2.TradingDataService/GetStopOrder",
+            request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetStopOrderRequest.SerializeToString,
+            response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetStopOrderResponse.FromString,
+        )
+        self.ListStopOrders = channel.unary_unary(
+            "/datanode.api.v2.TradingDataService/ListStopOrders",
+            request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListStopOrdersRequest.SerializeToString,
+            response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListStopOrdersResponse.FromString,
+        )
         self.ListPositions = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/ListPositions",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsResponse.FromString,
         )
         self.ListAllPositions = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/ListAllPositions",
@@ -528,14 +538,33 @@
 
         Subscribe to a stream of orders
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def GetStopOrder(self, request, context):
+        """Get stop order
+
+        Get a stop order by its ID. A stop order's ID will be the SHA3-256 hash of the signature that the order was submitted with.
+        A stop order's ID is likely to be different from the ID of the order that will be submitted when the stop is triggered.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def ListStopOrders(self, request, context):
+        """List stop orders
+
+        Get a list of stop orders that match the given filters
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
     def ListPositions(self, request, context):
         """Deprecated: List positions
 
         Get a list of positions by party's public key using cursor based pagination
         Deprecated: use ListAllPositions instead
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -1404,14 +1433,24 @@
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListOrderVersionsResponse.SerializeToString,
         ),
         "ObserveOrders": grpc.unary_stream_rpc_method_handler(
             servicer.ObserveOrders,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObserveOrdersRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObserveOrdersResponse.SerializeToString,
         ),
+        "GetStopOrder": grpc.unary_unary_rpc_method_handler(
+            servicer.GetStopOrder,
+            request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetStopOrderRequest.FromString,
+            response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetStopOrderResponse.SerializeToString,
+        ),
+        "ListStopOrders": grpc.unary_unary_rpc_method_handler(
+            servicer.ListStopOrders,
+            request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListStopOrdersRequest.FromString,
+            response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListStopOrdersResponse.SerializeToString,
+        ),
         "ListPositions": grpc.unary_unary_rpc_method_handler(
             servicer.ListPositions,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsResponse.SerializeToString,
         ),
         "ListAllPositions": grpc.unary_unary_rpc_method_handler(
             servicer.ListAllPositions,
@@ -2025,14 +2064,72 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def GetStopOrder(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/datanode.api.v2.TradingDataService/GetStopOrder",
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.GetStopOrderRequest.SerializeToString,
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.GetStopOrderResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def ListStopOrders(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/datanode.api.v2.TradingDataService/ListStopOrders",
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.ListStopOrdersRequest.SerializeToString,
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.ListStopOrdersResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
 
     @staticmethod
     def ListPositions(
         request,
         target,
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/__init__.py` & `vega_sim-1.2.1/vega_sim/proto/vega/__init__.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/api/v1/core_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     transaction_pb2 as vega_dot_commands_dot_v1_dot_transaction__pb2,
 )
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16vega/api/v1/core.proto\x12\x0bvega.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a"vega/commands/v1/transaction.proto\x1a\x1bvega/events/v1/events.proto\x1a\x0fvega/vega.proto"{\n\x1aPropagateChainEventRequest\x12\x1a\n\x05\x65vent\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x05\x65vent\x12\x1d\n\x07pub_key\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x06pubKey\x12"\n\tsignature\x18\x03 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\tsignature"7\n\x1bPropagateChainEventResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success"\xe3\x01\n\x18SubmitTransactionRequest\x12\x33\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x04\xe2\x41\x01\x02R\x02tx\x12\x44\n\x04type\x18\x02 \x01(\x0e\x32*.vega.api.v1.SubmitTransactionRequest.TypeB\x04\xe2\x41\x01\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa0\x01\n\x19SubmitTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"N\n\x17\x43heckTransactionRequest\x12\x33\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x04\xe2\x41\x01\x02R\x02tx"\xbc\x01\n\x18\x43heckTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\xca\x01\n\x1bSubmitRawTransactionRequest\x12\x14\n\x02tx\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x02tx\x12G\n\x04type\x18\x02 \x01(\x0e\x32-.vega.api.v1.SubmitRawTransactionRequest.TypeB\x04\xe2\x41\x01\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa3\x01\n\x1cSubmitRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"2\n\x1a\x43heckRawTransactionRequest\x12\x14\n\x02tx\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x02tx"\xbf\x01\n\x1b\x43heckRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x13\n\x11StatisticsRequest"M\n\x12StatisticsResponse\x12\x37\n\nstatistics\x18\x01 \x01(\x0b\x32\x17.vega.api.v1.StatisticsR\nstatistics"\xc8\x0c\n\nStatistics\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12%\n\x0e\x62\x61\x63klog_length\x18\x02 \x01(\x04R\rbacklogLength\x12\x1f\n\x0btotal_peers\x18\x03 \x01(\x04R\ntotalPeers\x12!\n\x0cgenesis_time\x18\x04 \x01(\tR\x0bgenesisTime\x12!\n\x0c\x63urrent_time\x18\x05 \x01(\tR\x0b\x63urrentTime\x12\x1b\n\tvega_time\x18\x06 \x01(\tR\x08vegaTime\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x11.vega.ChainStatusR\x06status\x12 \n\x0ctx_per_block\x18\x08 \x01(\x04R\ntxPerBlock\x12(\n\x10\x61verage_tx_bytes\x18\t \x01(\x04R\x0e\x61verageTxBytes\x12\x37\n\x18\x61verage_orders_per_block\x18\n \x01(\x04R\x15\x61verageOrdersPerBlock\x12*\n\x11trades_per_second\x18\x0b \x01(\x04R\x0ftradesPerSecond\x12*\n\x11orders_per_second\x18\x0c \x01(\x04R\x0fordersPerSecond\x12#\n\rtotal_markets\x18\r \x01(\x04R\x0ctotalMarkets\x12*\n\x11total_amend_order\x18\x10 \x01(\x04R\x0ftotalAmendOrder\x12,\n\x12total_cancel_order\x18\x11 \x01(\x04R\x10totalCancelOrder\x12,\n\x12total_create_order\x18\x12 \x01(\x04R\x10totalCreateOrder\x12!\n\x0ctotal_orders\x18\x13 \x01(\x04R\x0btotalOrders\x12!\n\x0ctotal_trades\x18\x14 \x01(\x04R\x0btotalTrades\x12/\n\x13order_subscriptions\x18\x15 \x01(\rR\x12orderSubscriptions\x12/\n\x13trade_subscriptions\x18\x16 \x01(\rR\x12tradeSubscriptions\x12\x31\n\x14\x63\x61ndle_subscriptions\x18\x17 \x01(\rR\x13\x63\x61ndleSubscriptions\x12<\n\x1amarket_depth_subscriptions\x18\x18 \x01(\rR\x18marketDepthSubscriptions\x12\x37\n\x17positions_subscriptions\x18\x19 \x01(\rR\x16positionsSubscriptions\x12\x33\n\x15\x61\x63\x63ount_subscriptions\x18\x1a \x01(\rR\x14\x61\x63\x63ountSubscriptions\x12:\n\x19market_data_subscriptions\x18\x1b \x01(\rR\x17marketDataSubscriptions\x12(\n\x10\x61pp_version_hash\x18\x1c \x01(\tR\x0e\x61ppVersionHash\x12\x1f\n\x0b\x61pp_version\x18\x1d \x01(\tR\nappVersion\x12#\n\rchain_version\x18\x1e \x01(\tR\x0c\x63hainVersion\x12%\n\x0e\x62lock_duration\x18\x1f \x01(\x04R\rblockDuration\x12\x16\n\x06uptime\x18  \x01(\tR\x06uptime\x12\x19\n\x08\x63hain_id\x18! \x01(\tR\x07\x63hainId\x12K\n"market_depth_updates_subscriptions\x18" \x01(\rR\x1fmarketDepthUpdatesSubscriptions\x12\x1d\n\nblock_hash\x18# \x01(\tR\tblockHash\x12\x1b\n\tepoch_seq\x18$ \x01(\x04R\x08\x65pochSeq\x12(\n\x10\x65poch_start_time\x18% \x01(\tR\x0e\x65pochStartTime\x12*\n\x11\x65poch_expiry_time\x18& \x01(\tR\x0f\x65pochExpiryTime\x12\x1f\n\x0b\x65vent_count\x18\' \x01(\x04R\neventCount\x12*\n\x11\x65vents_per_second\x18( \x01(\x04R\x0f\x65ventsPerSecond"\x18\n\x16LastBlockHeightRequest"\x91\x03\n\x17LastBlockHeightResponse\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12.\n\x13spam_pow_difficulty\x18\x04 \x01(\rR\x11spamPowDifficulty\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x05 \x01(\rR\x19spamPowNumberOfPastBlocks\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x06 \x01(\rR\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x07 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x19\n\x08\x63hain_id\x18\x08 \x01(\tR\x07\x63hainId";\n\x18GetSpamStatisticsRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId"\xc4\x01\n\rSpamStatistic\x12&\n\x0f\x63ount_for_epoch\x18\x01 \x01(\x04R\rcountForEpoch\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x04 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12.\n\x13min_tokens_required\x18\x05 \x01(\tR\x11minTokensRequiredB\x0f\n\r_banned_until"\xb1\x01\n\x12VoteSpamStatistics\x12>\n\nstatistics\x18\x01 \x03(\x0b\x32\x1e.vega.api.v1.VoteSpamStatisticR\nstatistics\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x03 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\x87\x01\n\x11VoteSpamStatistic\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12&\n\x0f\x63ount_for_epoch\x18\x02 \x01(\x04R\rcountForEpoch\x12.\n\x13min_tokens_required\x18\x03 \x01(\tR\x11minTokensRequired"\xe8\x02\n\rPoWBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12+\n\x11transactions_seen\x18\x03 \x01(\x04R\x10transactionsSeen\x12\x34\n\x13\x65xpected_difficulty\x18\x04 \x01(\x04H\x00R\x12\x65xpectedDifficulty\x88\x01\x01\x12#\n\rhash_function\x18\x05 \x01(\tR\x0chashFunction\x12\x1e\n\ndifficulty\x18\x06 \x01(\x04R\ndifficulty\x12 \n\x0ctx_per_block\x18\x07 \x01(\x04R\ntxPerBlock\x12\x33\n\x15increasing_difficulty\x18\x08 \x01(\x08R\x14increasingDifficultyB\x16\n\x14_expected_difficulty"\xb9\x01\n\x0cPoWStatistic\x12=\n\x0c\x62lock_states\x18\x01 \x03(\x0b\x32\x1a.vega.api.v1.PoWBlockStateR\x0b\x62lockStates\x12&\n\x0c\x62\x61nned_until\x18\x02 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12\x31\n\x15number_of_past_blocks\x18\x03 \x01(\x04R\x12numberOfPastBlocksB\x0f\n\r_banned_until"\xd5\x03\n\x0eSpamStatistics\x12\x38\n\tproposals\x18\x01 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\tproposals\x12<\n\x0b\x64\x65legations\x18\x02 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0b\x64\x65legations\x12\x38\n\ttransfers\x18\x03 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\ttransfers\x12I\n\x12node_announcements\x18\x04 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x11nodeAnnouncements\x12\x35\n\x05votes\x18\x05 \x01(\x0b\x32\x1f.vega.api.v1.VoteSpamStatisticsR\x05votes\x12+\n\x03pow\x18\x06 \x01(\x0b\x32\x19.vega.api.v1.PoWStatisticR\x03pow\x12\x45\n\x10issue_signatures\x18\x07 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0fissueSignatures\x12\x1b\n\tepoch_seq\x18\x08 \x01(\x04R\x08\x65pochSeq"s\n\x19GetSpamStatisticsResponse\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId\x12;\n\nstatistics\x18\x02 \x01(\x0b\x32\x1b.vega.api.v1.SpamStatisticsR\nstatistics2\xd8\x07\n\x0b\x43oreService\x12\x62\n\x11SubmitTransaction\x12%.vega.api.v1.SubmitTransactionRequest\x1a&.vega.api.v1.SubmitTransactionResponse\x12h\n\x13PropagateChainEvent\x12\'.vega.api.v1.PropagateChainEventRequest\x1a(.vega.api.v1.PropagateChainEventResponse\x12M\n\nStatistics\x12\x1e.vega.api.v1.StatisticsRequest\x1a\x1f.vega.api.v1.StatisticsResponse\x12\\\n\x0fLastBlockHeight\x12#.vega.api.v1.LastBlockHeightRequest\x1a$.vega.api.v1.LastBlockHeightResponse\x12P\n\x0bGetVegaTime\x12\x1f.vega.api.v1.GetVegaTimeRequest\x1a .vega.api.v1.GetVegaTimeResponse\x12`\n\x0fObserveEventBus\x12#.vega.api.v1.ObserveEventBusRequest\x1a$.vega.api.v1.ObserveEventBusResponse(\x01\x30\x01\x12k\n\x14SubmitRawTransaction\x12(.vega.api.v1.SubmitRawTransactionRequest\x1a).vega.api.v1.SubmitRawTransactionResponse\x12_\n\x10\x43heckTransaction\x12$.vega.api.v1.CheckTransactionRequest\x1a%.vega.api.v1.CheckTransactionResponse\x12h\n\x13\x43heckRawTransaction\x12\'.vega.api.v1.CheckRawTransactionRequest\x1a(.vega.api.v1.CheckRawTransactionResponse\x12\x62\n\x11GetSpamStatistics\x12%.vega.api.v1.GetSpamStatisticsRequest\x1a&.vega.api.v1.GetSpamStatisticsResponseBeZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41\x34\x12\x19\n\x0eVega core APIs2\x07v0.71.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n\x16vega/api/v1/core.proto\x12\x0bvega.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a"vega/commands/v1/transaction.proto\x1a\x1bvega/events/v1/events.proto\x1a\x0fvega/vega.proto"{\n\x1aPropagateChainEventRequest\x12\x1a\n\x05\x65vent\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x05\x65vent\x12\x1d\n\x07pub_key\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x06pubKey\x12"\n\tsignature\x18\x03 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\tsignature"7\n\x1bPropagateChainEventResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success"\xe3\x01\n\x18SubmitTransactionRequest\x12\x33\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x04\xe2\x41\x01\x02R\x02tx\x12\x44\n\x04type\x18\x02 \x01(\x0e\x32*.vega.api.v1.SubmitTransactionRequest.TypeB\x04\xe2\x41\x01\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa0\x01\n\x19SubmitTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"N\n\x17\x43heckTransactionRequest\x12\x33\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x04\xe2\x41\x01\x02R\x02tx"\xbc\x01\n\x18\x43heckTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\xca\x01\n\x1bSubmitRawTransactionRequest\x12\x14\n\x02tx\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x02tx\x12G\n\x04type\x18\x02 \x01(\x0e\x32-.vega.api.v1.SubmitRawTransactionRequest.TypeB\x04\xe2\x41\x01\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa3\x01\n\x1cSubmitRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"2\n\x1a\x43heckRawTransactionRequest\x12\x14\n\x02tx\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x02tx"\xbf\x01\n\x1b\x43heckRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x13\n\x11StatisticsRequest"M\n\x12StatisticsResponse\x12\x37\n\nstatistics\x18\x01 \x01(\x0b\x32\x17.vega.api.v1.StatisticsR\nstatistics"\xc8\x0c\n\nStatistics\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12%\n\x0e\x62\x61\x63klog_length\x18\x02 \x01(\x04R\rbacklogLength\x12\x1f\n\x0btotal_peers\x18\x03 \x01(\x04R\ntotalPeers\x12!\n\x0cgenesis_time\x18\x04 \x01(\tR\x0bgenesisTime\x12!\n\x0c\x63urrent_time\x18\x05 \x01(\tR\x0b\x63urrentTime\x12\x1b\n\tvega_time\x18\x06 \x01(\tR\x08vegaTime\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x11.vega.ChainStatusR\x06status\x12 \n\x0ctx_per_block\x18\x08 \x01(\x04R\ntxPerBlock\x12(\n\x10\x61verage_tx_bytes\x18\t \x01(\x04R\x0e\x61verageTxBytes\x12\x37\n\x18\x61verage_orders_per_block\x18\n \x01(\x04R\x15\x61verageOrdersPerBlock\x12*\n\x11trades_per_second\x18\x0b \x01(\x04R\x0ftradesPerSecond\x12*\n\x11orders_per_second\x18\x0c \x01(\x04R\x0fordersPerSecond\x12#\n\rtotal_markets\x18\r \x01(\x04R\x0ctotalMarkets\x12*\n\x11total_amend_order\x18\x10 \x01(\x04R\x0ftotalAmendOrder\x12,\n\x12total_cancel_order\x18\x11 \x01(\x04R\x10totalCancelOrder\x12,\n\x12total_create_order\x18\x12 \x01(\x04R\x10totalCreateOrder\x12!\n\x0ctotal_orders\x18\x13 \x01(\x04R\x0btotalOrders\x12!\n\x0ctotal_trades\x18\x14 \x01(\x04R\x0btotalTrades\x12/\n\x13order_subscriptions\x18\x15 \x01(\rR\x12orderSubscriptions\x12/\n\x13trade_subscriptions\x18\x16 \x01(\rR\x12tradeSubscriptions\x12\x31\n\x14\x63\x61ndle_subscriptions\x18\x17 \x01(\rR\x13\x63\x61ndleSubscriptions\x12<\n\x1amarket_depth_subscriptions\x18\x18 \x01(\rR\x18marketDepthSubscriptions\x12\x37\n\x17positions_subscriptions\x18\x19 \x01(\rR\x16positionsSubscriptions\x12\x33\n\x15\x61\x63\x63ount_subscriptions\x18\x1a \x01(\rR\x14\x61\x63\x63ountSubscriptions\x12:\n\x19market_data_subscriptions\x18\x1b \x01(\rR\x17marketDataSubscriptions\x12(\n\x10\x61pp_version_hash\x18\x1c \x01(\tR\x0e\x61ppVersionHash\x12\x1f\n\x0b\x61pp_version\x18\x1d \x01(\tR\nappVersion\x12#\n\rchain_version\x18\x1e \x01(\tR\x0c\x63hainVersion\x12%\n\x0e\x62lock_duration\x18\x1f \x01(\x04R\rblockDuration\x12\x16\n\x06uptime\x18  \x01(\tR\x06uptime\x12\x19\n\x08\x63hain_id\x18! \x01(\tR\x07\x63hainId\x12K\n"market_depth_updates_subscriptions\x18" \x01(\rR\x1fmarketDepthUpdatesSubscriptions\x12\x1d\n\nblock_hash\x18# \x01(\tR\tblockHash\x12\x1b\n\tepoch_seq\x18$ \x01(\x04R\x08\x65pochSeq\x12(\n\x10\x65poch_start_time\x18% \x01(\tR\x0e\x65pochStartTime\x12*\n\x11\x65poch_expiry_time\x18& \x01(\tR\x0f\x65pochExpiryTime\x12\x1f\n\x0b\x65vent_count\x18\' \x01(\x04R\neventCount\x12*\n\x11\x65vents_per_second\x18( \x01(\x04R\x0f\x65ventsPerSecond"\x18\n\x16LastBlockHeightRequest"\x91\x03\n\x17LastBlockHeightResponse\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12.\n\x13spam_pow_difficulty\x18\x04 \x01(\rR\x11spamPowDifficulty\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x05 \x01(\rR\x19spamPowNumberOfPastBlocks\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x06 \x01(\rR\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x07 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x19\n\x08\x63hain_id\x18\x08 \x01(\tR\x07\x63hainId";\n\x18GetSpamStatisticsRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId"\xc4\x01\n\rSpamStatistic\x12&\n\x0f\x63ount_for_epoch\x18\x01 \x01(\x04R\rcountForEpoch\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x04 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12.\n\x13min_tokens_required\x18\x05 \x01(\tR\x11minTokensRequiredB\x0f\n\r_banned_until"\xb1\x01\n\x12VoteSpamStatistics\x12>\n\nstatistics\x18\x01 \x03(\x0b\x32\x1e.vega.api.v1.VoteSpamStatisticR\nstatistics\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x03 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\x87\x01\n\x11VoteSpamStatistic\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12&\n\x0f\x63ount_for_epoch\x18\x02 \x01(\x04R\rcountForEpoch\x12.\n\x13min_tokens_required\x18\x03 \x01(\tR\x11minTokensRequired"\xe8\x02\n\rPoWBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12+\n\x11transactions_seen\x18\x03 \x01(\x04R\x10transactionsSeen\x12\x34\n\x13\x65xpected_difficulty\x18\x04 \x01(\x04H\x00R\x12\x65xpectedDifficulty\x88\x01\x01\x12#\n\rhash_function\x18\x05 \x01(\tR\x0chashFunction\x12\x1e\n\ndifficulty\x18\x06 \x01(\x04R\ndifficulty\x12 \n\x0ctx_per_block\x18\x07 \x01(\x04R\ntxPerBlock\x12\x33\n\x15increasing_difficulty\x18\x08 \x01(\x08R\x14increasingDifficultyB\x16\n\x14_expected_difficulty"\xb9\x01\n\x0cPoWStatistic\x12=\n\x0c\x62lock_states\x18\x01 \x03(\x0b\x32\x1a.vega.api.v1.PoWBlockStateR\x0b\x62lockStates\x12&\n\x0c\x62\x61nned_until\x18\x02 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12\x31\n\x15number_of_past_blocks\x18\x03 \x01(\x04R\x12numberOfPastBlocksB\x0f\n\r_banned_until"\xd5\x03\n\x0eSpamStatistics\x12\x38\n\tproposals\x18\x01 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\tproposals\x12<\n\x0b\x64\x65legations\x18\x02 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0b\x64\x65legations\x12\x38\n\ttransfers\x18\x03 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\ttransfers\x12I\n\x12node_announcements\x18\x04 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x11nodeAnnouncements\x12\x35\n\x05votes\x18\x05 \x01(\x0b\x32\x1f.vega.api.v1.VoteSpamStatisticsR\x05votes\x12+\n\x03pow\x18\x06 \x01(\x0b\x32\x19.vega.api.v1.PoWStatisticR\x03pow\x12\x45\n\x10issue_signatures\x18\x07 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0fissueSignatures\x12\x1b\n\tepoch_seq\x18\x08 \x01(\x04R\x08\x65pochSeq"s\n\x19GetSpamStatisticsResponse\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId\x12;\n\nstatistics\x18\x02 \x01(\x0b\x32\x1b.vega.api.v1.SpamStatisticsR\nstatistics2\xd8\x07\n\x0b\x43oreService\x12\x62\n\x11SubmitTransaction\x12%.vega.api.v1.SubmitTransactionRequest\x1a&.vega.api.v1.SubmitTransactionResponse\x12h\n\x13PropagateChainEvent\x12\'.vega.api.v1.PropagateChainEventRequest\x1a(.vega.api.v1.PropagateChainEventResponse\x12M\n\nStatistics\x12\x1e.vega.api.v1.StatisticsRequest\x1a\x1f.vega.api.v1.StatisticsResponse\x12\\\n\x0fLastBlockHeight\x12#.vega.api.v1.LastBlockHeightRequest\x1a$.vega.api.v1.LastBlockHeightResponse\x12P\n\x0bGetVegaTime\x12\x1f.vega.api.v1.GetVegaTimeRequest\x1a .vega.api.v1.GetVegaTimeResponse\x12`\n\x0fObserveEventBus\x12#.vega.api.v1.ObserveEventBusRequest\x1a$.vega.api.v1.ObserveEventBusResponse(\x01\x30\x01\x12k\n\x14SubmitRawTransaction\x12(.vega.api.v1.SubmitRawTransactionRequest\x1a).vega.api.v1.SubmitRawTransactionResponse\x12_\n\x10\x43heckTransaction\x12$.vega.api.v1.CheckTransactionRequest\x1a%.vega.api.v1.CheckTransactionResponse\x12h\n\x13\x43heckRawTransaction\x12\'.vega.api.v1.CheckRawTransactionRequest\x1a(.vega.api.v1.CheckRawTransactionResponse\x12\x62\n\x11GetSpamStatistics\x12%.vega.api.v1.GetSpamStatisticsRequest\x1a&.vega.api.v1.GetSpamStatisticsResponseBeZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41\x34\x12\x19\n\x0eVega core APIs2\x07v0.72.6\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.api.v1.core_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A4\022\031\n\016Vega core APIs2\007v0.71.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A4\022\031\n\016Vega core APIs2\007v0.72.6\032\023lb.testnet.vega.xyz*\002\001\002"
     _PROPAGATECHAINEVENTREQUEST.fields_by_name["event"]._options = None
     _PROPAGATECHAINEVENTREQUEST.fields_by_name[
         "event"
     ]._serialized_options = b"\342A\001\002"
     _PROPAGATECHAINEVENTREQUEST.fields_by_name["pub_key"]._options = None
     _PROPAGATECHAINEVENTREQUEST.fields_by_name[
         "pub_key"
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2_grpc.py` & `vega_sim-1.2.1/vega_sim/proto/vega/api/v1/core_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/api/v1/corestate_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import markets_pb2 as vega_dot_markets__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/api/v1/corestate.proto\x12\x0bvega.api.v1\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"{\n\x07\x41\x63\x63ount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type"C\n\x13ListAccountsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market"H\n\x14ListAccountsResponse\x12\x30\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x14.vega.api.v1.AccountR\x08\x61\x63\x63ounts")\n\x11ListAssetsRequest\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset"9\n\x12ListAssetsResponse\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"R\n\x1cListNetworkParametersRequest\x12\x32\n\x15network_parameter_key\x18\x01 \x01(\tR\x13networkParameterKey"f\n\x1dListNetworkParametersResponse\x12\x45\n\x12network_parameters\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters"\x1a\n\x18ListNetworkLimitsRequest"W\n\x19ListNetworkLimitsResponse\x12:\n\x0enetwork_limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\rnetworkLimits"\x14\n\x12ListPartiesRequest"<\n\x13ListPartiesResponse\x12%\n\x07parties\x18\x01 \x03(\x0b\x32\x0b.vega.PartyR\x07parties"\x17\n\x15ListValidatorsRequest"Y\n\x16ListValidatorsResponse\x12?\n\nvalidators\x18\x01 \x03(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\nvalidators",\n\x12ListMarketsRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"=\n\x13ListMarketsResponse\x12&\n\x07markets\x18\x01 \x03(\x0b\x32\x0c.vega.MarketR\x07markets"N\n\x14ListProposalsRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x1a\n\x08proposer\x18\x02 \x01(\tR\x08proposer"E\n\x15ListProposalsResponse\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"0\n\x16ListMarketsDataRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"N\n\x17ListMarketsDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"D\n\x10ListVotesRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x14\n\x05party\x18\x02 \x01(\tR\x05party"5\n\x11ListVotesResponse\x12 \n\x05votes\x18\x01 \x03(\x0b\x32\n.vega.VoteR\x05votes"\x9f\x01\n\nPartyStake\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x36\n\x17\x63urrent_stake_available\x18\x02 \x01(\tR\x15\x63urrentStakeAvailable\x12\x43\n\x0estake_linkings\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\rstakeLinkings"/\n\x17ListPartiesStakeRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party"X\n\x18ListPartiesStakeResponse\x12<\n\rparties_stake\x18\x01 \x03(\x0b\x32\x17.vega.api.v1.PartyStakeR\x0cpartiesStake"_\n\x16ListDelegationsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"M\n\x17ListDelegationsResponse\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations2\xca\x08\n\x10\x43oreStateService\x12S\n\x0cListAccounts\x12 .vega.api.v1.ListAccountsRequest\x1a!.vega.api.v1.ListAccountsResponse\x12M\n\nListAssets\x12\x1e.vega.api.v1.ListAssetsRequest\x1a\x1f.vega.api.v1.ListAssetsResponse\x12n\n\x15ListNetworkParameters\x12).vega.api.v1.ListNetworkParametersRequest\x1a*.vega.api.v1.ListNetworkParametersResponse\x12\x62\n\x11ListNetworkLimits\x12%.vega.api.v1.ListNetworkLimitsRequest\x1a&.vega.api.v1.ListNetworkLimitsResponse\x12P\n\x0bListParties\x12\x1f.vega.api.v1.ListPartiesRequest\x1a .vega.api.v1.ListPartiesResponse\x12Y\n\x0eListValidators\x12".vega.api.v1.ListValidatorsRequest\x1a#.vega.api.v1.ListValidatorsResponse\x12P\n\x0bListMarkets\x12\x1f.vega.api.v1.ListMarketsRequest\x1a .vega.api.v1.ListMarketsResponse\x12V\n\rListProposals\x12!.vega.api.v1.ListProposalsRequest\x1a".vega.api.v1.ListProposalsResponse\x12\\\n\x0fListMarketsData\x12#.vega.api.v1.ListMarketsDataRequest\x1a$.vega.api.v1.ListMarketsDataResponse\x12J\n\tListVotes\x12\x1d.vega.api.v1.ListVotesRequest\x1a\x1e.vega.api.v1.ListVotesResponse\x12_\n\x10ListPartiesStake\x12$.vega.api.v1.ListPartiesStakeRequest\x1a%.vega.api.v1.ListPartiesStakeResponse\x12\\\n\x0fListDelegations\x12#.vega.api.v1.ListDelegationsRequest\x1a$.vega.api.v1.ListDelegationsResponseBkZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41:\x12\x1f\n\x14Vega core state APIs2\x07v0.71.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n\x1bvega/api/v1/corestate.proto\x12\x0bvega.api.v1\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"{\n\x07\x41\x63\x63ount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type"C\n\x13ListAccountsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market"H\n\x14ListAccountsResponse\x12\x30\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x14.vega.api.v1.AccountR\x08\x61\x63\x63ounts")\n\x11ListAssetsRequest\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset"9\n\x12ListAssetsResponse\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"R\n\x1cListNetworkParametersRequest\x12\x32\n\x15network_parameter_key\x18\x01 \x01(\tR\x13networkParameterKey"f\n\x1dListNetworkParametersResponse\x12\x45\n\x12network_parameters\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters"\x1a\n\x18ListNetworkLimitsRequest"W\n\x19ListNetworkLimitsResponse\x12:\n\x0enetwork_limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\rnetworkLimits"\x14\n\x12ListPartiesRequest"<\n\x13ListPartiesResponse\x12%\n\x07parties\x18\x01 \x03(\x0b\x32\x0b.vega.PartyR\x07parties"\x17\n\x15ListValidatorsRequest"Y\n\x16ListValidatorsResponse\x12?\n\nvalidators\x18\x01 \x03(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\nvalidators",\n\x12ListMarketsRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"=\n\x13ListMarketsResponse\x12&\n\x07markets\x18\x01 \x03(\x0b\x32\x0c.vega.MarketR\x07markets"N\n\x14ListProposalsRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x1a\n\x08proposer\x18\x02 \x01(\tR\x08proposer"E\n\x15ListProposalsResponse\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"0\n\x16ListMarketsDataRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"N\n\x17ListMarketsDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"D\n\x10ListVotesRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x14\n\x05party\x18\x02 \x01(\tR\x05party"5\n\x11ListVotesResponse\x12 \n\x05votes\x18\x01 \x03(\x0b\x32\n.vega.VoteR\x05votes"\x9f\x01\n\nPartyStake\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x36\n\x17\x63urrent_stake_available\x18\x02 \x01(\tR\x15\x63urrentStakeAvailable\x12\x43\n\x0estake_linkings\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\rstakeLinkings"/\n\x17ListPartiesStakeRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party"X\n\x18ListPartiesStakeResponse\x12<\n\rparties_stake\x18\x01 \x03(\x0b\x32\x17.vega.api.v1.PartyStakeR\x0cpartiesStake"_\n\x16ListDelegationsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"M\n\x17ListDelegationsResponse\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations2\xca\x08\n\x10\x43oreStateService\x12S\n\x0cListAccounts\x12 .vega.api.v1.ListAccountsRequest\x1a!.vega.api.v1.ListAccountsResponse\x12M\n\nListAssets\x12\x1e.vega.api.v1.ListAssetsRequest\x1a\x1f.vega.api.v1.ListAssetsResponse\x12n\n\x15ListNetworkParameters\x12).vega.api.v1.ListNetworkParametersRequest\x1a*.vega.api.v1.ListNetworkParametersResponse\x12\x62\n\x11ListNetworkLimits\x12%.vega.api.v1.ListNetworkLimitsRequest\x1a&.vega.api.v1.ListNetworkLimitsResponse\x12P\n\x0bListParties\x12\x1f.vega.api.v1.ListPartiesRequest\x1a .vega.api.v1.ListPartiesResponse\x12Y\n\x0eListValidators\x12".vega.api.v1.ListValidatorsRequest\x1a#.vega.api.v1.ListValidatorsResponse\x12P\n\x0bListMarkets\x12\x1f.vega.api.v1.ListMarketsRequest\x1a .vega.api.v1.ListMarketsResponse\x12V\n\rListProposals\x12!.vega.api.v1.ListProposalsRequest\x1a".vega.api.v1.ListProposalsResponse\x12\\\n\x0fListMarketsData\x12#.vega.api.v1.ListMarketsDataRequest\x1a$.vega.api.v1.ListMarketsDataResponse\x12J\n\tListVotes\x12\x1d.vega.api.v1.ListVotesRequest\x1a\x1e.vega.api.v1.ListVotesResponse\x12_\n\x10ListPartiesStake\x12$.vega.api.v1.ListPartiesStakeRequest\x1a%.vega.api.v1.ListPartiesStakeResponse\x12\\\n\x0fListDelegations\x12#.vega.api.v1.ListDelegationsRequest\x1a$.vega.api.v1.ListDelegationsResponseBkZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41:\x12\x1f\n\x14Vega core state APIs2\x07v0.72.6\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.api.v1.corestate_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A:\022\037\n\024Vega core state APIs2\007v0.71.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A:\022\037\n\024Vega core state APIs2\007v0.72.6\032\023lb.testnet.vega.xyz*\002\001\002"
     _globals["_ACCOUNT"]._serialized_start = 200
     _globals["_ACCOUNT"]._serialized_end = 323
     _globals["_LISTACCOUNTSREQUEST"]._serialized_start = 325
     _globals["_LISTACCOUNTSREQUEST"]._serialized_end = 392
     _globals["_LISTACCOUNTSRESPONSE"]._serialized_start = 394
     _globals["_LISTACCOUNTSRESPONSE"]._serialized_end = 466
     _globals["_LISTASSETSREQUEST"]._serialized_start = 468
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py` & `vega_sim-1.2.1/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/assets_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/assets_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/chain_events_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/chain_events_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/__init__.py` & `vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/commands_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/commands_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/data_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/signature_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/signature_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/transaction_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/data/v1/data_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/data/v1/spec_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/data/v1/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/data_source_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/events/v1/events_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/events/v1/events_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import markets_pb2 as vega_dot_markets__pb2
 from ... import oracle_pb2 as vega_dot_oracle__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/events/v1/events.proto\x12\x0evega.events.v1\x1a\x11vega/assets.proto\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\x83\x01\n\x0eStopOrderEvent\x12\x41\n\nsubmission\x18\x01 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionR\nsubmission\x12.\n\nstop_order\x18\x02 \x01(\x0b\x32\x0f.vega.StopOrderR\tstopOrder"\xee\x01\n\x18\x45RC20MultiSigSignerAdded\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nnew_signer\x18\x04 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x05 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x06 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"f\n#ERC20MultiSigSignerRemovedSubmitter\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter"\x97\x02\n\x1a\x45RC20MultiSigSignerRemoved\x12\x66\n\x14signature_submitters\x18\x01 \x03(\x0b\x32\x33.vega.events.v1.ERC20MultiSigSignerRemovedSubmitterR\x13signatureSubmitters\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nold_signer\x18\x04 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x05 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x06 \x01(\tR\x08\x65pochSeq"\xcc\x06\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x66rom\x18\x02 \x01(\tR\x04\x66rom\x12=\n\x11\x66rom_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x04 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x05 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x06 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x07 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x37\n\x06status\x18\t \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12\x1b\n\x06reason\x18\x0b \x01(\tH\x01R\x06reason\x88\x01\x01\x12\x39\n\x07one_off\x18\x65 \x01(\x0b\x32\x1e.vega.events.v1.OneOffTransferH\x00R\x06oneOff\x12\x41\n\trecurring\x18\x66 \x01(\x0b\x32!.vega.events.v1.RecurringTransferH\x00R\trecurring\x12X\n\x12one_off_governance\x18g \x01(\x0b\x32(.vega.events.v1.OneOffGovernanceTransferH\x00R\x10oneOffGovernance\x12`\n\x14recurring_governance\x18h \x01(\x0b\x32+.vega.events.v1.RecurringGovernanceTransferH\x00R\x13recurringGovernance"\x84\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x0f\n\x0bSTATUS_DONE\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x14\n\x10STATUS_CANCELLED\x10\x05\x42\x06\n\x04kindB\t\n\x07_reason"9\n\x18OneOffGovernanceTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"n\n\x1bRecurringGovernanceTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x42\x0c\n\n_end_epoch"\xb4\x04\n\x0cStakeLinking\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x35\n\x04type\x18\x02 \x01(\x0e\x32!.vega.events.v1.StakeLinking.TypeR\x04type\x12\x0e\n\x02ts\x18\x03 \x01(\x03R\x02ts\x12\x14\n\x05party\x18\x04 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12;\n\x06status\x18\x06 \x01(\x0e\x32#.vega.events.v1.StakeLinking.StatusR\x06status\x12!\n\x0c\x66inalized_at\x18\x07 \x01(\x03R\x0b\x66inalizedAt\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12!\n\x0c\x62lock_height\x18\t \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\n \x01(\x03R\tblockTime\x12\x1b\n\tlog_index\x18\x0b \x01(\x04R\x08logIndex\x12)\n\x10\x65thereum_address\x18\x0c \x01(\tR\x0f\x65thereumAddress"<\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\r\n\tTYPE_LINK\x10\x01\x12\x0f\n\x0bTYPE_UNLINK\x10\x02"^\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x13\n\x0fSTATUS_ACCEPTED\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03"\xd3\x02\n\x18\x45RC20MultiSigSignerEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.events.v1.ERC20MultiSigSignerEvent.TypeR\x04type\x12\x16\n\x06signer\x18\x03 \x01(\tR\x06signer\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x05 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x07 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x08 \x01(\x04R\x0b\x62lockNumber">\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ADDED\x10\x01\x12\x10\n\x0cTYPE_REMOVED\x10\x02"\xe3\x01\n\x1e\x45RC20MultiSigThresholdSetEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rnew_threshold\x18\x02 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x05 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x07 \x01(\x04R\x0b\x62lockNumber"g\n\x0f\x43heckpointEvent\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x62lock_height\x18\x03 \x01(\x04R\x0b\x62lockHeight"-\n\x10StreamStartEvent\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId"\x82\x02\n\x11RewardPayoutEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x35\n\x17percent_of_total_reward\x18\x05 \x01(\tR\x14percentOfTotalReward\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp\x12\x1f\n\x0breward_type\x18\x07 \x01(\tR\nrewardType\x12\x16\n\x06market\x18\x08 \x01(\tR\x06market"\xd6\x02\n\x13ValidatorScoreEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\'\n\x0fvalidator_score\x18\x03 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x04 \x01(\tR\x0fnormalisedScore\x12\x33\n\x15validator_performance\x18\x05 \x01(\tR\x14validatorPerformance\x12.\n\x13raw_validator_score\x18\x06 \x01(\tR\x11rawValidatorScore\x12)\n\x10validator_status\x18\x07 \x01(\tR\x0fvalidatorStatus\x12%\n\x0emultisig_score\x18\x08 \x01(\tR\rmultisigScore"|\n\x16\x44\x65legationBalanceEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"D\n\x0bMarketEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07payload\x18\x02 \x01(\tR\x07payload"\xaf\x12\n\x11TransactionResult\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x16\n\x06status\x18\x02 \x01(\x08R\x06status\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12[\n\x15key_rotate_submission\x18x \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12t\n\x1e\x65thereum_key_rotate_submission\x18y \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12\\\n\x15stop_order_submission\x18z \x01(\x0b\x32&.vega.commands.v1.StopOrdersSubmissionH\x00R\x13stopOrderSubmission\x12\x62\n\x17stop_order_cancellation\x18{ \x01(\x0b\x32(.vega.commands.v1.StopOrdersCancellationH\x00R\x15stopOrderCancellation\x12M\n\x07success\x18\xe9\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.SuccessDetailsH\x01R\x07success\x12M\n\x07\x66\x61ilure\x18\xea\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.FailureDetailsH\x01R\x07\x66\x61ilure\x1a\x10\n\x0eSuccessDetails\x1a&\n\x0e\x46\x61ilureDetails\x12\x14\n\x05\x65rror\x18\x01 \x01(\tR\x05\x65rrorB\r\n\x0btransactionB\x07\n\x05\x65xtra"\xa7\r\n\x0cTxErrorEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x17\n\x07\x65rr_msg\x18\x02 \x01(\tR\x06\x65rrMsg\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructionsB\r\n\x0btransactionJ\x04\x08n\x10o"*\n\nTimeUpdate\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa4\x01\n\nEpochEvent\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12)\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x11.vega.EpochActionR\x06\x61\x63tion\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x19\n\x08\x65nd_time\x18\x05 \x01(\x03R\x07\x65ndTime"R\n\x0fLedgerMovements\x12?\n\x10ledger_movements\x18\x01 \x03(\x0b\x32\x14.vega.LedgerMovementR\x0fledgerMovements"\x88\x01\n\x12PositionResolution\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1e\n\ndistressed\x18\x02 \x01(\x03R\ndistressed\x12\x16\n\x06\x63losed\x18\x03 \x01(\x03R\x06\x63losed\x12\x1d\n\nmark_price\x18\x04 \x01(\tR\tmarkPrice"c\n\x11LossSocialization\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"^\n\x0fTradeSettlement\x12\x12\n\x04size\x18\x01 \x01(\x03R\x04size\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice"\xd5\x01\n\x0eSettlePosition\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12L\n\x11trade_settlements\x18\x04 \x03(\x0b\x32\x1f.vega.events.v1.TradeSettlementR\x10tradeSettlements\x12\'\n\x0fposition_factor\x18\x05 \x01(\tR\x0epositionFactor"j\n\x0cSettleMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\'\n\x0fposition_factor\x18\x03 \x01(\tR\x0epositionFactor"\xf6\x01\n\x12PositionStateEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x12\n\x04size\x18\x03 \x01(\x03R\x04size\x12%\n\x0epotential_buys\x18\x04 \x01(\x03R\rpotentialBuys\x12\'\n\x0fpotential_sells\x18\x05 \x01(\x03R\x0epotentialSells\x12 \n\x0cvw_buy_price\x18\x06 \x01(\tR\nvwBuyPrice\x12"\n\rvw_sell_price\x18\x07 \x01(\tR\x0bvwSellPrice"x\n\x10SettleDistressed\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06margin\x18\x03 \x01(\tR\x06margin\x12\x14\n\x05price\x18\x04 \x01(\tR\x05price"I\n\x10\x44istressedOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07parties\x18\x02 \x03(\tR\x07parties"\x84\x01\n\x13\x44istressedPositions\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12-\n\x12\x64istressed_parties\x18\x02 \x03(\tR\x11\x64istressedParties\x12!\n\x0csafe_parties\x18\x03 \x03(\tR\x0bsafeParties"0\n\nMarketTick\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\x85\x02\n\x0c\x41uctionEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\'\n\x0fopening_auction\x18\x02 \x01(\x08R\x0eopeningAuction\x12\x14\n\x05leave\x18\x03 \x01(\x08R\x05leave\x12\x14\n\x05start\x18\x04 \x01(\x03R\x05start\x12\x10\n\x03\x65nd\x18\x05 \x01(\x03R\x03\x65nd\x12.\n\x07trigger\x18\x06 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x07 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger"\xa9\x03\n\x0fValidatorUpdate\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12 \n\x0cvega_pub_key\x18\x02 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x03 \x01(\tR\x0f\x65thereumAddress\x12\x1c\n\ntm_pub_key\x18\x04 \x01(\tR\x08tmPubKey\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x06 \x01(\tR\x07\x63ountry\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\n \x01(\x08R\x05\x61\x64\x64\x65\x64\x12\x1d\n\nfrom_epoch\x18\x0b \x01(\x04R\tfromEpoch\x12+\n\x11submitter_address\x18\x0c \x01(\tR\x10submitterAddress\x12\x1b\n\tepoch_seq\x18\r \x01(\x04R\x08\x65pochSeq"\xb2\x02\n\x15ValidatorRankingEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bstake_score\x18\x02 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x03 \x01(\tR\x10performanceScore\x12#\n\rranking_score\x18\x04 \x01(\tR\x0crankingScore\x12\'\n\x0fprevious_status\x18\x05 \x01(\tR\x0epreviousStatus\x12\x1f\n\x0bnext_status\x18\x06 \x01(\tR\nnextStatus\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq\x12&\n\x0ftm_voting_power\x18\x08 \x01(\rR\rtmVotingPower"\x89\x01\n\x0bKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1e\n\x0bold_pub_key\x18\x02 \x01(\tR\toldPubKey\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\x93\x01\n\x13\x45thereumKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bold_address\x18\x02 \x01(\tR\noldAddress\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\xd7\x01\n\x14ProtocolUpgradeEvent\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag\x12\x1c\n\tapprovers\x18\x03 \x03(\tR\tapprovers\x12\x45\n\x06status\x18\x04 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusR\x06status"K\n\x08StateVar\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12\x14\n\x05state\x18\x03 \x01(\tR\x05state"V\n\nBeginBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash""\n\x08\x45ndBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height"D\n\x16ProtocolUpgradeStarted\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"J\n\x1cProtocolUpgradeDataNodeReady\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"\xad\x01\n\x10\x43oreSnapshotData\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x63ore_version\x18\x03 \x01(\tR\x0b\x63oreVersion\x12\x34\n\x16protocol_upgrade_block\x18\x04 \x01(\x08R\x14protocolUpgradeBlock"\xeb!\n\x08\x42usEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12=\n\x0btime_update\x18\x65 \x01(\x0b\x32\x1a.vega.events.v1.TimeUpdateH\x00R\ntimeUpdate\x12L\n\x10ledger_movements\x18\x66 \x01(\x0b\x32\x1f.vega.events.v1.LedgerMovementsH\x00R\x0fledgerMovements\x12U\n\x13position_resolution\x18g \x01(\x0b\x32".vega.events.v1.PositionResolutionH\x00R\x12positionResolution\x12#\n\x05order\x18h \x01(\x0b\x32\x0b.vega.OrderH\x00R\x05order\x12)\n\x07\x61\x63\x63ount\x18i \x01(\x0b\x32\r.vega.AccountH\x00R\x07\x61\x63\x63ount\x12#\n\x05party\x18j \x01(\x0b\x32\x0b.vega.PartyH\x00R\x05party\x12#\n\x05trade\x18k \x01(\x0b\x32\x0b.vega.TradeH\x00R\x05trade\x12\x39\n\rmargin_levels\x18l \x01(\x0b\x32\x12.vega.MarginLevelsH\x00R\x0cmarginLevels\x12,\n\x08proposal\x18m \x01(\x0b\x32\x0e.vega.ProposalH\x00R\x08proposal\x12 \n\x04vote\x18n \x01(\x0b\x32\n.vega.VoteH\x00R\x04vote\x12\x33\n\x0bmarket_data\x18o \x01(\x0b\x32\x10.vega.MarketDataH\x00R\nmarketData\x12H\n\x0enode_signature\x18p \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12R\n\x12loss_socialization\x18q \x01(\x0b\x32!.vega.events.v1.LossSocializationH\x00R\x11lossSocialization\x12I\n\x0fsettle_position\x18r \x01(\x0b\x32\x1e.vega.events.v1.SettlePositionH\x00R\x0esettlePosition\x12O\n\x11settle_distressed\x18s \x01(\x0b\x32 .vega.events.v1.SettleDistressedH\x00R\x10settleDistressed\x12\x35\n\x0emarket_created\x18t \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketCreated\x12#\n\x05\x61sset\x18u \x01(\x0b\x32\x0b.vega.AssetH\x00R\x05\x61sset\x12=\n\x0bmarket_tick\x18v \x01(\x0b\x32\x1a.vega.events.v1.MarketTickH\x00R\nmarketTick\x12\x32\n\nwithdrawal\x18w \x01(\x0b\x32\x10.vega.WithdrawalH\x00R\nwithdrawal\x12)\n\x07\x64\x65posit\x18x \x01(\x0b\x32\r.vega.DepositH\x00R\x07\x64\x65posit\x12\x38\n\x07\x61uction\x18y \x01(\x0b\x32\x1c.vega.events.v1.AuctionEventH\x00R\x07\x61uction\x12\x33\n\x0brisk_factor\x18z \x01(\x0b\x32\x10.vega.RiskFactorH\x00R\nriskFactor\x12\x45\n\x11network_parameter\x18{ \x01(\x0b\x32\x16.vega.NetworkParameterH\x00R\x10networkParameter\x12K\n\x13liquidity_provision\x18| \x01(\x0b\x32\x18.vega.LiquidityProvisionH\x00R\x12liquidityProvision\x12\x35\n\x0emarket_updated\x18} \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketUpdated\x12\x33\n\x0boracle_spec\x18~ \x01(\x0b\x32\x10.vega.OracleSpecH\x00R\noracleSpec\x12\x33\n\x0boracle_data\x18\x7f \x01(\x0b\x32\x10.vega.OracleDataH\x00R\noracleData\x12X\n\x12\x64\x65legation_balance\x18\x81\x01 \x01(\x0b\x32&.vega.events.v1.DelegationBalanceEventH\x00R\x11\x64\x65legationBalance\x12O\n\x0fvalidator_score\x18\x82\x01 \x01(\x0b\x32#.vega.events.v1.ValidatorScoreEventH\x00R\x0evalidatorScore\x12>\n\x0b\x65poch_event\x18\x83\x01 \x01(\x0b\x32\x1a.vega.events.v1.EpochEventH\x00R\nepochEvent\x12M\n\x10validator_update\x18\x84\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateH\x00R\x0fvalidatorUpdate\x12\x44\n\rstake_linking\x18\x85\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingH\x00R\x0cstakeLinking\x12I\n\rreward_payout\x18\x86\x01 \x01(\x0b\x32!.vega.events.v1.RewardPayoutEventH\x00R\x0crewardPayout\x12\x42\n\ncheckpoint\x18\x87\x01 \x01(\x0b\x32\x1f.vega.events.v1.CheckpointEventH\x00R\ncheckpoint\x12\x41\n\x0ckey_rotation\x18\x88\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationH\x00R\x0bkeyRotation\x12\x38\n\tstate_var\x18\x89\x01 \x01(\x0b\x32\x18.vega.events.v1.StateVarH\x00R\x08stateVar\x12=\n\x0enetwork_limits\x18\x8a\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsH\x00R\rnetworkLimits\x12\x37\n\x08transfer\x18\x8b\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferH\x00R\x08transfer\x12M\n\rranking_event\x18\x8c\x01 \x01(\x0b\x32%.vega.events.v1.ValidatorRankingEventH\x00R\x0crankingEvent\x12j\n\x1b\x65rc20_multisig_signer_event\x18\x8d\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventH\x00R\x18\x65rc20MultisigSignerEvent\x12}\n"erc20_multisig_set_threshold_event\x18\x8e\x01 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventH\x00R\x1e\x65rc20MultisigSetThresholdEvent\x12j\n\x1b\x65rc20_multisig_signer_added\x18\x8f\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedH\x00R\x18\x65rc20MultisigSignerAdded\x12p\n\x1d\x65rc20_multisig_signer_removed\x18\x90\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedH\x00R\x1a\x65rc20MultisigSignerRemoved\x12W\n\x14position_state_event\x18\x91\x01 \x01(\x0b\x32".vega.events.v1.PositionStateEventH\x00R\x12positionStateEvent\x12Z\n\x15\x65thereum_key_rotation\x18\x92\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationH\x00R\x13\x65thereumKeyRotation\x12]\n\x16protocol_upgrade_event\x18\x93\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventH\x00R\x14protocolUpgradeEvent\x12>\n\x0b\x62\x65gin_block\x18\x94\x01 \x01(\x0b\x32\x1a.vega.events.v1.BeginBlockH\x00R\nbeginBlock\x12\x38\n\tend_block\x18\x95\x01 \x01(\x0b\x32\x18.vega.events.v1.EndBlockH\x00R\x08\x65ndBlock\x12\x63\n\x18protocol_upgrade_started\x18\x96\x01 \x01(\x0b\x32&.vega.events.v1.ProtocolUpgradeStartedH\x00R\x16protocolUpgradeStarted\x12\x44\n\rsettle_market\x18\x97\x01 \x01(\x0b\x32\x1c.vega.events.v1.SettleMarketH\x00R\x0csettleMarket\x12S\n\x12transaction_result\x18\x98\x01 \x01(\x0b\x32!.vega.events.v1.TransactionResultH\x00R\x11transactionResult\x12S\n\x13\x63ore_snapshot_event\x18\x99\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataH\x00R\x11\x63oreSnapshotEvent\x12w\n protocol_upgrade_data_node_ready\x18\x9a\x01 \x01(\x0b\x32,.vega.events.v1.ProtocolUpgradeDataNodeReadyH\x00R\x1cprotocolUpgradeDataNodeReady\x12P\n\x11\x64istressed_orders\x18\x9b\x01 \x01(\x0b\x32 .vega.events.v1.DistressedOrdersH\x00R\x10\x64istressedOrders\x12G\n\x0e\x65xpired_orders\x18\x9c\x01 \x01(\x0b\x32\x1d.vega.events.v1.ExpiredOrdersH\x00R\rexpiredOrders\x12Y\n\x14\x64istressed_positions\x18\x9d\x01 \x01(\x0b\x32#.vega.events.v1.DistressedPositionsH\x00R\x13\x64istressedPositions\x12\x31\n\nstop_order\x18\x9e\x01 \x01(\x0b\x32\x0f.vega.StopOrderH\x00R\tstopOrder\x12\x36\n\x06market\x18\xe9\x07 \x01(\x0b\x32\x1b.vega.events.v1.MarketEventH\x00R\x06market\x12\x41\n\x0ctx_err_event\x18\xd1\x0f \x01(\x0b\x32\x1c.vega.events.v1.TxErrorEventH\x00R\ntxErrEvent\x12\x18\n\x07version\x18\x04 \x01(\rR\x07version\x12\x19\n\x08\x63hain_id\x18\x05 \x01(\tR\x07\x63hainId\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHashB\x07\n\x05\x65vent"I\n\rExpiredOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds*\xdd\x01\n\x1dProtocolUpgradeProposalStatus\x12\x30\n,PROTOCOL_UPGRADE_PROPOSAL_STATUS_UNSPECIFIED\x10\x00\x12,\n(PROTOCOL_UPGRADE_PROPOSAL_STATUS_PENDING\x10\x01\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_APPROVED\x10\x02\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_REJECTED\x10\x03*\xba\x11\n\x0c\x42usEventType\x12\x1e\n\x1a\x42US_EVENT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42US_EVENT_TYPE_ALL\x10\x01\x12\x1e\n\x1a\x42US_EVENT_TYPE_TIME_UPDATE\x10\x02\x12#\n\x1f\x42US_EVENT_TYPE_LEDGER_MOVEMENTS\x10\x03\x12&\n"BUS_EVENT_TYPE_POSITION_RESOLUTION\x10\x04\x12\x18\n\x14\x42US_EVENT_TYPE_ORDER\x10\x05\x12\x1a\n\x16\x42US_EVENT_TYPE_ACCOUNT\x10\x06\x12\x18\n\x14\x42US_EVENT_TYPE_PARTY\x10\x07\x12\x18\n\x14\x42US_EVENT_TYPE_TRADE\x10\x08\x12 \n\x1c\x42US_EVENT_TYPE_MARGIN_LEVELS\x10\t\x12\x1b\n\x17\x42US_EVENT_TYPE_PROPOSAL\x10\n\x12\x17\n\x13\x42US_EVENT_TYPE_VOTE\x10\x0b\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_DATA\x10\x0c\x12!\n\x1d\x42US_EVENT_TYPE_NODE_SIGNATURE\x10\r\x12%\n!BUS_EVENT_TYPE_LOSS_SOCIALIZATION\x10\x0e\x12"\n\x1e\x42US_EVENT_TYPE_SETTLE_POSITION\x10\x0f\x12$\n BUS_EVENT_TYPE_SETTLE_DISTRESSED\x10\x10\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_CREATED\x10\x11\x12\x18\n\x14\x42US_EVENT_TYPE_ASSET\x10\x12\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_TICK\x10\x13\x12\x1d\n\x19\x42US_EVENT_TYPE_WITHDRAWAL\x10\x14\x12\x1a\n\x16\x42US_EVENT_TYPE_DEPOSIT\x10\x15\x12\x1a\n\x16\x42US_EVENT_TYPE_AUCTION\x10\x16\x12\x1e\n\x1a\x42US_EVENT_TYPE_RISK_FACTOR\x10\x17\x12$\n BUS_EVENT_TYPE_NETWORK_PARAMETER\x10\x18\x12&\n"BUS_EVENT_TYPE_LIQUIDITY_PROVISION\x10\x19\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_UPDATED\x10\x1a\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_SPEC\x10\x1b\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_DATA\x10\x1c\x12%\n!BUS_EVENT_TYPE_DELEGATION_BALANCE\x10\x1d\x12"\n\x1e\x42US_EVENT_TYPE_VALIDATOR_SCORE\x10\x1e\x12\x1f\n\x1b\x42US_EVENT_TYPE_EPOCH_UPDATE\x10\x1f\x12#\n\x1f\x42US_EVENT_TYPE_VALIDATOR_UPDATE\x10 \x12 \n\x1c\x42US_EVENT_TYPE_STAKE_LINKING\x10!\x12&\n"BUS_EVENT_TYPE_REWARD_PAYOUT_EVENT\x10"\x12\x1d\n\x19\x42US_EVENT_TYPE_CHECKPOINT\x10#\x12\x1f\n\x1b\x42US_EVENT_TYPE_STREAM_START\x10$\x12\x1f\n\x1b\x42US_EVENT_TYPE_KEY_ROTATION\x10%\x12\x1c\n\x18\x42US_EVENT_TYPE_STATE_VAR\x10&\x12!\n\x1d\x42US_EVENT_TYPE_NETWORK_LIMITS\x10\'\x12\x1b\n\x17\x42US_EVENT_TYPE_TRANSFER\x10(\x12$\n BUS_EVENT_TYPE_VALIDATOR_RANKING\x10)\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_EVENT\x10*\x12\x30\n,BUS_EVENT_TYPE_ERC20_MULTI_SIG_SET_THRESHOLD\x10+\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_ADDED\x10,\x12\x31\n-BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_REMOVED\x10-\x12!\n\x1d\x42US_EVENT_TYPE_POSITION_STATE\x10.\x12(\n$BUS_EVENT_TYPE_ETHEREUM_KEY_ROTATION\x10/\x12,\n(BUS_EVENT_TYPE_PROTOCOL_UPGRADE_PROPOSAL\x10\x30\x12\x1e\n\x1a\x42US_EVENT_TYPE_BEGIN_BLOCK\x10\x31\x12\x1c\n\x18\x42US_EVENT_TYPE_END_BLOCK\x10\x32\x12+\n\'BUS_EVENT_TYPE_PROTOCOL_UPGRADE_STARTED\x10\x33\x12 \n\x1c\x42US_EVENT_TYPE_SETTLE_MARKET\x10\x34\x12%\n!BUS_EVENT_TYPE_TRANSACTION_RESULT\x10\x35\x12!\n\x1d\x42US_EVENT_TYPE_SNAPSHOT_TAKEN\x10\x36\x12\x33\n/BUS_EVENT_TYPE_PROTOCOL_UPGRADE_DATA_NODE_READY\x10\x37\x12+\n\'BUS_EVENT_TYPE_DISTRESSED_ORDERS_CLOSED\x10\x38\x12!\n\x1d\x42US_EVENT_TYPE_EXPIRED_ORDERS\x10\x39\x12\'\n#BUS_EVENT_TYPE_DISTRESSED_POSITIONS\x10:\x12+\n\'BUS_EVENT_TYPE_SPOT_LIQUIDITY_PROVISION\x10;\x12\x1d\n\x19\x42US_EVENT_TYPE_STOP_ORDER\x10<\x12\x19\n\x15\x42US_EVENT_TYPE_MARKET\x10\x65\x12\x1c\n\x17\x42US_EVENT_TYPE_TX_ERROR\x10\xc9\x01\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/events/v1b\x06proto3'
+    b'\n\x1bvega/events/v1/events.proto\x12\x0evega.events.v1\x1a\x11vega/assets.proto\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\x83\x01\n\x0eStopOrderEvent\x12\x41\n\nsubmission\x18\x01 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionR\nsubmission\x12.\n\nstop_order\x18\x02 \x01(\x0b\x32\x0f.vega.StopOrderR\tstopOrder"\xee\x01\n\x18\x45RC20MultiSigSignerAdded\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nnew_signer\x18\x04 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x05 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x06 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"f\n#ERC20MultiSigSignerRemovedSubmitter\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter"\x97\x02\n\x1a\x45RC20MultiSigSignerRemoved\x12\x66\n\x14signature_submitters\x18\x01 \x03(\x0b\x32\x33.vega.events.v1.ERC20MultiSigSignerRemovedSubmitterR\x13signatureSubmitters\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nold_signer\x18\x04 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x05 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x06 \x01(\tR\x08\x65pochSeq"\xcc\x06\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x66rom\x18\x02 \x01(\tR\x04\x66rom\x12=\n\x11\x66rom_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x04 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x05 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x06 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x07 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x37\n\x06status\x18\t \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12\x1b\n\x06reason\x18\x0b \x01(\tH\x01R\x06reason\x88\x01\x01\x12\x39\n\x07one_off\x18\x65 \x01(\x0b\x32\x1e.vega.events.v1.OneOffTransferH\x00R\x06oneOff\x12\x41\n\trecurring\x18\x66 \x01(\x0b\x32!.vega.events.v1.RecurringTransferH\x00R\trecurring\x12X\n\x12one_off_governance\x18g \x01(\x0b\x32(.vega.events.v1.OneOffGovernanceTransferH\x00R\x10oneOffGovernance\x12`\n\x14recurring_governance\x18h \x01(\x0b\x32+.vega.events.v1.RecurringGovernanceTransferH\x00R\x13recurringGovernance"\x84\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x0f\n\x0bSTATUS_DONE\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x14\n\x10STATUS_CANCELLED\x10\x05\x42\x06\n\x04kindB\t\n\x07_reason"9\n\x18OneOffGovernanceTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"n\n\x1bRecurringGovernanceTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x42\x0c\n\n_end_epoch"\xb4\x04\n\x0cStakeLinking\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x35\n\x04type\x18\x02 \x01(\x0e\x32!.vega.events.v1.StakeLinking.TypeR\x04type\x12\x0e\n\x02ts\x18\x03 \x01(\x03R\x02ts\x12\x14\n\x05party\x18\x04 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12;\n\x06status\x18\x06 \x01(\x0e\x32#.vega.events.v1.StakeLinking.StatusR\x06status\x12!\n\x0c\x66inalized_at\x18\x07 \x01(\x03R\x0b\x66inalizedAt\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12!\n\x0c\x62lock_height\x18\t \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\n \x01(\x03R\tblockTime\x12\x1b\n\tlog_index\x18\x0b \x01(\x04R\x08logIndex\x12)\n\x10\x65thereum_address\x18\x0c \x01(\tR\x0f\x65thereumAddress"<\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\r\n\tTYPE_LINK\x10\x01\x12\x0f\n\x0bTYPE_UNLINK\x10\x02"^\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x13\n\x0fSTATUS_ACCEPTED\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03"\xd3\x02\n\x18\x45RC20MultiSigSignerEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.events.v1.ERC20MultiSigSignerEvent.TypeR\x04type\x12\x16\n\x06signer\x18\x03 \x01(\tR\x06signer\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x05 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x07 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x08 \x01(\x04R\x0b\x62lockNumber">\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ADDED\x10\x01\x12\x10\n\x0cTYPE_REMOVED\x10\x02"\xe3\x01\n\x1e\x45RC20MultiSigThresholdSetEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rnew_threshold\x18\x02 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x05 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x07 \x01(\x04R\x0b\x62lockNumber"g\n\x0f\x43heckpointEvent\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x62lock_height\x18\x03 \x01(\x04R\x0b\x62lockHeight"-\n\x10StreamStartEvent\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId"\x82\x02\n\x11RewardPayoutEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x35\n\x17percent_of_total_reward\x18\x05 \x01(\tR\x14percentOfTotalReward\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp\x12\x1f\n\x0breward_type\x18\x07 \x01(\tR\nrewardType\x12\x16\n\x06market\x18\x08 \x01(\tR\x06market"\xd6\x02\n\x13ValidatorScoreEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\'\n\x0fvalidator_score\x18\x03 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x04 \x01(\tR\x0fnormalisedScore\x12\x33\n\x15validator_performance\x18\x05 \x01(\tR\x14validatorPerformance\x12.\n\x13raw_validator_score\x18\x06 \x01(\tR\x11rawValidatorScore\x12)\n\x10validator_status\x18\x07 \x01(\tR\x0fvalidatorStatus\x12%\n\x0emultisig_score\x18\x08 \x01(\tR\rmultisigScore"|\n\x16\x44\x65legationBalanceEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"D\n\x0bMarketEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07payload\x18\x02 \x01(\tR\x07payload"\xaf\x12\n\x11TransactionResult\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x16\n\x06status\x18\x02 \x01(\x08R\x06status\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12[\n\x15key_rotate_submission\x18x \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12t\n\x1e\x65thereum_key_rotate_submission\x18y \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12\\\n\x15stop_order_submission\x18z \x01(\x0b\x32&.vega.commands.v1.StopOrdersSubmissionH\x00R\x13stopOrderSubmission\x12\x62\n\x17stop_order_cancellation\x18{ \x01(\x0b\x32(.vega.commands.v1.StopOrdersCancellationH\x00R\x15stopOrderCancellation\x12M\n\x07success\x18\xe9\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.SuccessDetailsH\x01R\x07success\x12M\n\x07\x66\x61ilure\x18\xea\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.FailureDetailsH\x01R\x07\x66\x61ilure\x1a\x10\n\x0eSuccessDetails\x1a&\n\x0e\x46\x61ilureDetails\x12\x14\n\x05\x65rror\x18\x01 \x01(\tR\x05\x65rrorB\r\n\x0btransactionB\x07\n\x05\x65xtra"\xa7\r\n\x0cTxErrorEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x17\n\x07\x65rr_msg\x18\x02 \x01(\tR\x06\x65rrMsg\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructionsB\r\n\x0btransactionJ\x04\x08n\x10o"*\n\nTimeUpdate\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa4\x01\n\nEpochEvent\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12)\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x11.vega.EpochActionR\x06\x61\x63tion\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x19\n\x08\x65nd_time\x18\x05 \x01(\x03R\x07\x65ndTime"R\n\x0fLedgerMovements\x12?\n\x10ledger_movements\x18\x01 \x03(\x0b\x32\x14.vega.LedgerMovementR\x0fledgerMovements"\x88\x01\n\x12PositionResolution\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1e\n\ndistressed\x18\x02 \x01(\x03R\ndistressed\x12\x16\n\x06\x63losed\x18\x03 \x01(\x03R\x06\x63losed\x12\x1d\n\nmark_price\x18\x04 \x01(\tR\tmarkPrice"c\n\x11LossSocialization\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"^\n\x0fTradeSettlement\x12\x12\n\x04size\x18\x01 \x01(\x03R\x04size\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice"\xd5\x01\n\x0eSettlePosition\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12L\n\x11trade_settlements\x18\x04 \x03(\x0b\x32\x1f.vega.events.v1.TradeSettlementR\x10tradeSettlements\x12\'\n\x0fposition_factor\x18\x05 \x01(\tR\x0epositionFactor"j\n\x0cSettleMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\'\n\x0fposition_factor\x18\x03 \x01(\tR\x0epositionFactor"\xf6\x01\n\x12PositionStateEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x12\n\x04size\x18\x03 \x01(\x03R\x04size\x12%\n\x0epotential_buys\x18\x04 \x01(\x03R\rpotentialBuys\x12\'\n\x0fpotential_sells\x18\x05 \x01(\x03R\x0epotentialSells\x12 \n\x0cvw_buy_price\x18\x06 \x01(\tR\nvwBuyPrice\x12"\n\rvw_sell_price\x18\x07 \x01(\tR\x0bvwSellPrice"x\n\x10SettleDistressed\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06margin\x18\x03 \x01(\tR\x06margin\x12\x14\n\x05price\x18\x04 \x01(\tR\x05price"I\n\x10\x44istressedOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07parties\x18\x02 \x03(\tR\x07parties"\x84\x01\n\x13\x44istressedPositions\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12-\n\x12\x64istressed_parties\x18\x02 \x03(\tR\x11\x64istressedParties\x12!\n\x0csafe_parties\x18\x03 \x03(\tR\x0bsafeParties"0\n\nMarketTick\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\x85\x02\n\x0c\x41uctionEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\'\n\x0fopening_auction\x18\x02 \x01(\x08R\x0eopeningAuction\x12\x14\n\x05leave\x18\x03 \x01(\x08R\x05leave\x12\x14\n\x05start\x18\x04 \x01(\x03R\x05start\x12\x10\n\x03\x65nd\x18\x05 \x01(\x03R\x03\x65nd\x12.\n\x07trigger\x18\x06 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x07 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger"\xa9\x03\n\x0fValidatorUpdate\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12 \n\x0cvega_pub_key\x18\x02 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x03 \x01(\tR\x0f\x65thereumAddress\x12\x1c\n\ntm_pub_key\x18\x04 \x01(\tR\x08tmPubKey\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x06 \x01(\tR\x07\x63ountry\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\n \x01(\x08R\x05\x61\x64\x64\x65\x64\x12\x1d\n\nfrom_epoch\x18\x0b \x01(\x04R\tfromEpoch\x12+\n\x11submitter_address\x18\x0c \x01(\tR\x10submitterAddress\x12\x1b\n\tepoch_seq\x18\r \x01(\x04R\x08\x65pochSeq"\xb2\x02\n\x15ValidatorRankingEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bstake_score\x18\x02 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x03 \x01(\tR\x10performanceScore\x12#\n\rranking_score\x18\x04 \x01(\tR\x0crankingScore\x12\'\n\x0fprevious_status\x18\x05 \x01(\tR\x0epreviousStatus\x12\x1f\n\x0bnext_status\x18\x06 \x01(\tR\nnextStatus\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq\x12&\n\x0ftm_voting_power\x18\x08 \x01(\rR\rtmVotingPower"\x89\x01\n\x0bKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1e\n\x0bold_pub_key\x18\x02 \x01(\tR\toldPubKey\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\x93\x01\n\x13\x45thereumKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bold_address\x18\x02 \x01(\tR\noldAddress\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\xd7\x01\n\x14ProtocolUpgradeEvent\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag\x12\x1c\n\tapprovers\x18\x03 \x03(\tR\tapprovers\x12\x45\n\x06status\x18\x04 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusR\x06status"K\n\x08StateVar\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12\x14\n\x05state\x18\x03 \x01(\tR\x05state"V\n\nBeginBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash""\n\x08\x45ndBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height"D\n\x16ProtocolUpgradeStarted\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"J\n\x1cProtocolUpgradeDataNodeReady\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"\xad\x01\n\x10\x43oreSnapshotData\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x63ore_version\x18\x03 \x01(\tR\x0b\x63oreVersion\x12\x34\n\x16protocol_upgrade_block\x18\x04 \x01(\x08R\x14protocolUpgradeBlock"\xfa!\n\x08\x42usEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12=\n\x0btime_update\x18\x65 \x01(\x0b\x32\x1a.vega.events.v1.TimeUpdateH\x00R\ntimeUpdate\x12L\n\x10ledger_movements\x18\x66 \x01(\x0b\x32\x1f.vega.events.v1.LedgerMovementsH\x00R\x0fledgerMovements\x12U\n\x13position_resolution\x18g \x01(\x0b\x32".vega.events.v1.PositionResolutionH\x00R\x12positionResolution\x12#\n\x05order\x18h \x01(\x0b\x32\x0b.vega.OrderH\x00R\x05order\x12)\n\x07\x61\x63\x63ount\x18i \x01(\x0b\x32\r.vega.AccountH\x00R\x07\x61\x63\x63ount\x12#\n\x05party\x18j \x01(\x0b\x32\x0b.vega.PartyH\x00R\x05party\x12#\n\x05trade\x18k \x01(\x0b\x32\x0b.vega.TradeH\x00R\x05trade\x12\x39\n\rmargin_levels\x18l \x01(\x0b\x32\x12.vega.MarginLevelsH\x00R\x0cmarginLevels\x12,\n\x08proposal\x18m \x01(\x0b\x32\x0e.vega.ProposalH\x00R\x08proposal\x12 \n\x04vote\x18n \x01(\x0b\x32\n.vega.VoteH\x00R\x04vote\x12\x33\n\x0bmarket_data\x18o \x01(\x0b\x32\x10.vega.MarketDataH\x00R\nmarketData\x12H\n\x0enode_signature\x18p \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12R\n\x12loss_socialization\x18q \x01(\x0b\x32!.vega.events.v1.LossSocializationH\x00R\x11lossSocialization\x12I\n\x0fsettle_position\x18r \x01(\x0b\x32\x1e.vega.events.v1.SettlePositionH\x00R\x0esettlePosition\x12O\n\x11settle_distressed\x18s \x01(\x0b\x32 .vega.events.v1.SettleDistressedH\x00R\x10settleDistressed\x12\x35\n\x0emarket_created\x18t \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketCreated\x12#\n\x05\x61sset\x18u \x01(\x0b\x32\x0b.vega.AssetH\x00R\x05\x61sset\x12=\n\x0bmarket_tick\x18v \x01(\x0b\x32\x1a.vega.events.v1.MarketTickH\x00R\nmarketTick\x12\x32\n\nwithdrawal\x18w \x01(\x0b\x32\x10.vega.WithdrawalH\x00R\nwithdrawal\x12)\n\x07\x64\x65posit\x18x \x01(\x0b\x32\r.vega.DepositH\x00R\x07\x64\x65posit\x12\x38\n\x07\x61uction\x18y \x01(\x0b\x32\x1c.vega.events.v1.AuctionEventH\x00R\x07\x61uction\x12\x33\n\x0brisk_factor\x18z \x01(\x0b\x32\x10.vega.RiskFactorH\x00R\nriskFactor\x12\x45\n\x11network_parameter\x18{ \x01(\x0b\x32\x16.vega.NetworkParameterH\x00R\x10networkParameter\x12K\n\x13liquidity_provision\x18| \x01(\x0b\x32\x18.vega.LiquidityProvisionH\x00R\x12liquidityProvision\x12\x35\n\x0emarket_updated\x18} \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketUpdated\x12\x33\n\x0boracle_spec\x18~ \x01(\x0b\x32\x10.vega.OracleSpecH\x00R\noracleSpec\x12\x33\n\x0boracle_data\x18\x7f \x01(\x0b\x32\x10.vega.OracleDataH\x00R\noracleData\x12X\n\x12\x64\x65legation_balance\x18\x81\x01 \x01(\x0b\x32&.vega.events.v1.DelegationBalanceEventH\x00R\x11\x64\x65legationBalance\x12O\n\x0fvalidator_score\x18\x82\x01 \x01(\x0b\x32#.vega.events.v1.ValidatorScoreEventH\x00R\x0evalidatorScore\x12>\n\x0b\x65poch_event\x18\x83\x01 \x01(\x0b\x32\x1a.vega.events.v1.EpochEventH\x00R\nepochEvent\x12M\n\x10validator_update\x18\x84\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateH\x00R\x0fvalidatorUpdate\x12\x44\n\rstake_linking\x18\x85\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingH\x00R\x0cstakeLinking\x12I\n\rreward_payout\x18\x86\x01 \x01(\x0b\x32!.vega.events.v1.RewardPayoutEventH\x00R\x0crewardPayout\x12\x42\n\ncheckpoint\x18\x87\x01 \x01(\x0b\x32\x1f.vega.events.v1.CheckpointEventH\x00R\ncheckpoint\x12\x41\n\x0ckey_rotation\x18\x88\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationH\x00R\x0bkeyRotation\x12\x38\n\tstate_var\x18\x89\x01 \x01(\x0b\x32\x18.vega.events.v1.StateVarH\x00R\x08stateVar\x12=\n\x0enetwork_limits\x18\x8a\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsH\x00R\rnetworkLimits\x12\x37\n\x08transfer\x18\x8b\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferH\x00R\x08transfer\x12M\n\rranking_event\x18\x8c\x01 \x01(\x0b\x32%.vega.events.v1.ValidatorRankingEventH\x00R\x0crankingEvent\x12j\n\x1b\x65rc20_multisig_signer_event\x18\x8d\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventH\x00R\x18\x65rc20MultisigSignerEvent\x12}\n"erc20_multisig_set_threshold_event\x18\x8e\x01 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventH\x00R\x1e\x65rc20MultisigSetThresholdEvent\x12j\n\x1b\x65rc20_multisig_signer_added\x18\x8f\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedH\x00R\x18\x65rc20MultisigSignerAdded\x12p\n\x1d\x65rc20_multisig_signer_removed\x18\x90\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedH\x00R\x1a\x65rc20MultisigSignerRemoved\x12W\n\x14position_state_event\x18\x91\x01 \x01(\x0b\x32".vega.events.v1.PositionStateEventH\x00R\x12positionStateEvent\x12Z\n\x15\x65thereum_key_rotation\x18\x92\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationH\x00R\x13\x65thereumKeyRotation\x12]\n\x16protocol_upgrade_event\x18\x93\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventH\x00R\x14protocolUpgradeEvent\x12>\n\x0b\x62\x65gin_block\x18\x94\x01 \x01(\x0b\x32\x1a.vega.events.v1.BeginBlockH\x00R\nbeginBlock\x12\x38\n\tend_block\x18\x95\x01 \x01(\x0b\x32\x18.vega.events.v1.EndBlockH\x00R\x08\x65ndBlock\x12\x63\n\x18protocol_upgrade_started\x18\x96\x01 \x01(\x0b\x32&.vega.events.v1.ProtocolUpgradeStartedH\x00R\x16protocolUpgradeStarted\x12\x44\n\rsettle_market\x18\x97\x01 \x01(\x0b\x32\x1c.vega.events.v1.SettleMarketH\x00R\x0csettleMarket\x12S\n\x12transaction_result\x18\x98\x01 \x01(\x0b\x32!.vega.events.v1.TransactionResultH\x00R\x11transactionResult\x12S\n\x13\x63ore_snapshot_event\x18\x99\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataH\x00R\x11\x63oreSnapshotEvent\x12w\n protocol_upgrade_data_node_ready\x18\x9a\x01 \x01(\x0b\x32,.vega.events.v1.ProtocolUpgradeDataNodeReadyH\x00R\x1cprotocolUpgradeDataNodeReady\x12P\n\x11\x64istressed_orders\x18\x9b\x01 \x01(\x0b\x32 .vega.events.v1.DistressedOrdersH\x00R\x10\x64istressedOrders\x12G\n\x0e\x65xpired_orders\x18\x9c\x01 \x01(\x0b\x32\x1d.vega.events.v1.ExpiredOrdersH\x00R\rexpiredOrders\x12Y\n\x14\x64istressed_positions\x18\x9d\x01 \x01(\x0b\x32#.vega.events.v1.DistressedPositionsH\x00R\x13\x64istressedPositions\x12@\n\nstop_order\x18\x9e\x01 \x01(\x0b\x32\x1e.vega.events.v1.StopOrderEventH\x00R\tstopOrder\x12\x36\n\x06market\x18\xe9\x07 \x01(\x0b\x32\x1b.vega.events.v1.MarketEventH\x00R\x06market\x12\x41\n\x0ctx_err_event\x18\xd1\x0f \x01(\x0b\x32\x1c.vega.events.v1.TxErrorEventH\x00R\ntxErrEvent\x12\x18\n\x07version\x18\x04 \x01(\rR\x07version\x12\x19\n\x08\x63hain_id\x18\x05 \x01(\tR\x07\x63hainId\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHashB\x07\n\x05\x65vent"I\n\rExpiredOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds*\xdd\x01\n\x1dProtocolUpgradeProposalStatus\x12\x30\n,PROTOCOL_UPGRADE_PROPOSAL_STATUS_UNSPECIFIED\x10\x00\x12,\n(PROTOCOL_UPGRADE_PROPOSAL_STATUS_PENDING\x10\x01\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_APPROVED\x10\x02\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_REJECTED\x10\x03*\xba\x11\n\x0c\x42usEventType\x12\x1e\n\x1a\x42US_EVENT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42US_EVENT_TYPE_ALL\x10\x01\x12\x1e\n\x1a\x42US_EVENT_TYPE_TIME_UPDATE\x10\x02\x12#\n\x1f\x42US_EVENT_TYPE_LEDGER_MOVEMENTS\x10\x03\x12&\n"BUS_EVENT_TYPE_POSITION_RESOLUTION\x10\x04\x12\x18\n\x14\x42US_EVENT_TYPE_ORDER\x10\x05\x12\x1a\n\x16\x42US_EVENT_TYPE_ACCOUNT\x10\x06\x12\x18\n\x14\x42US_EVENT_TYPE_PARTY\x10\x07\x12\x18\n\x14\x42US_EVENT_TYPE_TRADE\x10\x08\x12 \n\x1c\x42US_EVENT_TYPE_MARGIN_LEVELS\x10\t\x12\x1b\n\x17\x42US_EVENT_TYPE_PROPOSAL\x10\n\x12\x17\n\x13\x42US_EVENT_TYPE_VOTE\x10\x0b\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_DATA\x10\x0c\x12!\n\x1d\x42US_EVENT_TYPE_NODE_SIGNATURE\x10\r\x12%\n!BUS_EVENT_TYPE_LOSS_SOCIALIZATION\x10\x0e\x12"\n\x1e\x42US_EVENT_TYPE_SETTLE_POSITION\x10\x0f\x12$\n BUS_EVENT_TYPE_SETTLE_DISTRESSED\x10\x10\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_CREATED\x10\x11\x12\x18\n\x14\x42US_EVENT_TYPE_ASSET\x10\x12\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_TICK\x10\x13\x12\x1d\n\x19\x42US_EVENT_TYPE_WITHDRAWAL\x10\x14\x12\x1a\n\x16\x42US_EVENT_TYPE_DEPOSIT\x10\x15\x12\x1a\n\x16\x42US_EVENT_TYPE_AUCTION\x10\x16\x12\x1e\n\x1a\x42US_EVENT_TYPE_RISK_FACTOR\x10\x17\x12$\n BUS_EVENT_TYPE_NETWORK_PARAMETER\x10\x18\x12&\n"BUS_EVENT_TYPE_LIQUIDITY_PROVISION\x10\x19\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_UPDATED\x10\x1a\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_SPEC\x10\x1b\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_DATA\x10\x1c\x12%\n!BUS_EVENT_TYPE_DELEGATION_BALANCE\x10\x1d\x12"\n\x1e\x42US_EVENT_TYPE_VALIDATOR_SCORE\x10\x1e\x12\x1f\n\x1b\x42US_EVENT_TYPE_EPOCH_UPDATE\x10\x1f\x12#\n\x1f\x42US_EVENT_TYPE_VALIDATOR_UPDATE\x10 \x12 \n\x1c\x42US_EVENT_TYPE_STAKE_LINKING\x10!\x12&\n"BUS_EVENT_TYPE_REWARD_PAYOUT_EVENT\x10"\x12\x1d\n\x19\x42US_EVENT_TYPE_CHECKPOINT\x10#\x12\x1f\n\x1b\x42US_EVENT_TYPE_STREAM_START\x10$\x12\x1f\n\x1b\x42US_EVENT_TYPE_KEY_ROTATION\x10%\x12\x1c\n\x18\x42US_EVENT_TYPE_STATE_VAR\x10&\x12!\n\x1d\x42US_EVENT_TYPE_NETWORK_LIMITS\x10\'\x12\x1b\n\x17\x42US_EVENT_TYPE_TRANSFER\x10(\x12$\n BUS_EVENT_TYPE_VALIDATOR_RANKING\x10)\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_EVENT\x10*\x12\x30\n,BUS_EVENT_TYPE_ERC20_MULTI_SIG_SET_THRESHOLD\x10+\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_ADDED\x10,\x12\x31\n-BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_REMOVED\x10-\x12!\n\x1d\x42US_EVENT_TYPE_POSITION_STATE\x10.\x12(\n$BUS_EVENT_TYPE_ETHEREUM_KEY_ROTATION\x10/\x12,\n(BUS_EVENT_TYPE_PROTOCOL_UPGRADE_PROPOSAL\x10\x30\x12\x1e\n\x1a\x42US_EVENT_TYPE_BEGIN_BLOCK\x10\x31\x12\x1c\n\x18\x42US_EVENT_TYPE_END_BLOCK\x10\x32\x12+\n\'BUS_EVENT_TYPE_PROTOCOL_UPGRADE_STARTED\x10\x33\x12 \n\x1c\x42US_EVENT_TYPE_SETTLE_MARKET\x10\x34\x12%\n!BUS_EVENT_TYPE_TRANSACTION_RESULT\x10\x35\x12!\n\x1d\x42US_EVENT_TYPE_SNAPSHOT_TAKEN\x10\x36\x12\x33\n/BUS_EVENT_TYPE_PROTOCOL_UPGRADE_DATA_NODE_READY\x10\x37\x12+\n\'BUS_EVENT_TYPE_DISTRESSED_ORDERS_CLOSED\x10\x38\x12!\n\x1d\x42US_EVENT_TYPE_EXPIRED_ORDERS\x10\x39\x12\'\n#BUS_EVENT_TYPE_DISTRESSED_POSITIONS\x10:\x12+\n\'BUS_EVENT_TYPE_SPOT_LIQUIDITY_PROVISION\x10;\x12\x1d\n\x19\x42US_EVENT_TYPE_STOP_ORDER\x10<\x12\x19\n\x15\x42US_EVENT_TYPE_MARKET\x10\x65\x12\x1c\n\x17\x42US_EVENT_TYPE_TX_ERROR\x10\xc9\x01\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/events/v1b\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.events.v1.events_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z/code.vegaprotocol.io/vega/protos/vega/events/v1"
     )
-    _globals["_PROTOCOLUPGRADEPROPOSALSTATUS"]._serialized_start = 16455
-    _globals["_PROTOCOLUPGRADEPROPOSALSTATUS"]._serialized_end = 16676
-    _globals["_BUSEVENTTYPE"]._serialized_start = 16679
-    _globals["_BUSEVENTTYPE"]._serialized_end = 18913
+    _globals["_PROTOCOLUPGRADEPROPOSALSTATUS"]._serialized_start = 16470
+    _globals["_PROTOCOLUPGRADEPROPOSALSTATUS"]._serialized_end = 16691
+    _globals["_BUSEVENTTYPE"]._serialized_start = 16694
+    _globals["_BUSEVENTTYPE"]._serialized_end = 18928
     _globals["_STOPORDEREVENT"]._serialized_start = 251
     _globals["_STOPORDEREVENT"]._serialized_end = 382
     _globals["_ERC20MULTISIGSIGNERADDED"]._serialized_start = 385
     _globals["_ERC20MULTISIGSIGNERADDED"]._serialized_end = 623
     _globals["_ERC20MULTISIGSIGNERREMOVEDSUBMITTER"]._serialized_start = 625
     _globals["_ERC20MULTISIGSIGNERREMOVEDSUBMITTER"]._serialized_end = 727
     _globals["_ERC20MULTISIGSIGNERREMOVED"]._serialized_start = 730
@@ -141,11 +141,11 @@
     _globals["_PROTOCOLUPGRADESTARTED"]._serialized_start = 11723
     _globals["_PROTOCOLUPGRADESTARTED"]._serialized_end = 11791
     _globals["_PROTOCOLUPGRADEDATANODEREADY"]._serialized_start = 11793
     _globals["_PROTOCOLUPGRADEDATANODEREADY"]._serialized_end = 11867
     _globals["_CORESNAPSHOTDATA"]._serialized_start = 11870
     _globals["_CORESNAPSHOTDATA"]._serialized_end = 12043
     _globals["_BUSEVENT"]._serialized_start = 12046
-    _globals["_BUSEVENT"]._serialized_end = 16377
-    _globals["_EXPIREDORDERS"]._serialized_start = 16379
-    _globals["_EXPIREDORDERS"]._serialized_end = 16452
+    _globals["_BUSEVENT"]._serialized_end = 16392
+    _globals["_EXPIREDORDERS"]._serialized_start = 16394
+    _globals["_EXPIREDORDERS"]._serialized_end = 16467
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/governance_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/governance_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/markets_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/markets_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/oracle_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/oracle_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import markets_pb2 as vega_dot_markets__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1fvega/snapshot/v1/snapshot.proto\x12\x10vega.snapshot.v1\x1a\x11vega/assets.proto\x1a\x17vega/chain_events.proto\x1a#vega/checkpoint/v1/checkpoint.proto\x1a\x17vega/data/v1/data.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"\x9c\x01\n\x08Snapshot\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x30\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.vega.snapshot.v1.FormatR\x06\x66ormat\x12\x16\n\x06\x63hunks\x18\x03 \x01(\rR\x06\x63hunks\x12\x12\n\x04hash\x18\x04 \x01(\x0cR\x04hash\x12\x1a\n\x08metadata\x18\x05 \x01(\x0cR\x08metadata"{\n\x08NodeHash\x12\x10\n\x03key\x18\x03 \x01(\tR\x03key\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hash\x12\x16\n\x06height\x18\x05 \x01(\x05R\x06height\x12\x18\n\x07version\x18\x06 \x01(\x03R\x07version\x12\x17\n\x07is_leaf\x18\x07 \x01(\x08R\x06isLeaf"\x84\x01\n\x08Metadata\x12\x18\n\x07version\x18\x01 \x01(\x03R\x07version\x12!\n\x0c\x63hunk_hashes\x18\x02 \x03(\tR\x0b\x63hunkHashes\x12;\n\x0bnode_hashes\x18\x03 \x03(\x0b\x32\x1a.vega.snapshot.v1.NodeHashR\nnodeHashes"V\n\x05\x43hunk\x12-\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x19.vega.snapshot.v1.PayloadR\x04\x64\x61ta\x12\x0e\n\x02nr\x18\x02 \x01(\x03R\x02nr\x12\x0e\n\x02of\x18\x03 \x01(\x03R\x02of"\xc6&\n\x07Payload\x12\x45\n\ractive_assets\x18\x01 \x01(\x0b\x32\x1e.vega.snapshot.v1.ActiveAssetsH\x00R\x0c\x61\x63tiveAssets\x12H\n\x0epending_assets\x18\x02 \x01(\x0b\x32\x1f.vega.snapshot.v1.PendingAssetsH\x00R\rpendingAssets\x12W\n\x13\x62\x61nking_withdrawals\x18\x03 \x01(\x0b\x32$.vega.snapshot.v1.BankingWithdrawalsH\x00R\x12\x62\x61nkingWithdrawals\x12N\n\x10\x62\x61nking_deposits\x18\x04 \x01(\x0b\x32!.vega.snapshot.v1.BankingDepositsH\x00R\x0f\x62\x61nkingDeposits\x12\x42\n\x0c\x62\x61nking_seen\x18\x05 \x01(\x0b\x32\x1d.vega.snapshot.v1.BankingSeenH\x00R\x0b\x62\x61nkingSeen\x12[\n\x15\x62\x61nking_asset_actions\x18\x06 \x01(\x0b\x32%.vega.snapshot.v1.BankingAssetActionsH\x00R\x13\x62\x61nkingAssetActions\x12>\n\ncheckpoint\x18\x07 \x01(\x0b\x32\x1c.vega.snapshot.v1.CheckpointH\x00R\ncheckpoint\x12W\n\x13\x63ollateral_accounts\x18\x08 \x01(\x0b\x32$.vega.snapshot.v1.CollateralAccountsH\x00R\x12\x63ollateralAccounts\x12Q\n\x11\x63ollateral_assets\x18\t \x01(\x0b\x32".vega.snapshot.v1.CollateralAssetsH\x00R\x10\x63ollateralAssets\x12Q\n\x11\x64\x65legation_active\x18\n \x01(\x0b\x32".vega.snapshot.v1.DelegationActiveH\x00R\x10\x64\x65legationActive\x12T\n\x12\x64\x65legation_pending\x18\x0b \x01(\x0b\x32#.vega.snapshot.v1.DelegationPendingH\x00R\x11\x64\x65legationPending\x12K\n\x0f\x64\x65legation_auto\x18\x0c \x01(\x0b\x32 .vega.snapshot.v1.DelegationAutoH\x00R\x0e\x64\x65legationAuto\x12Q\n\x11governance_active\x18\r \x01(\x0b\x32".vega.snapshot.v1.GovernanceActiveH\x00R\x10governanceActive\x12T\n\x12governance_enacted\x18\x0e \x01(\x0b\x32#.vega.snapshot.v1.GovernanceEnactedH\x00R\x11governanceEnacted\x12N\n\x10staking_accounts\x18\x0f \x01(\x0b\x32!.vega.snapshot.v1.StakingAccountsH\x00R\x0fstakingAccounts\x12\x45\n\rmatching_book\x18\x10 \x01(\x0b\x32\x1e.vega.snapshot.v1.MatchingBookH\x00R\x0cmatchingBook\x12L\n\x12network_parameters\x18\x11 \x01(\x0b\x32\x1b.vega.snapshot.v1.NetParamsH\x00R\x11networkParameters\x12Q\n\x11\x65xecution_markets\x18\x12 \x01(\x0b\x32".vega.snapshot.v1.ExecutionMarketsH\x00R\x10\x65xecutionMarkets\x12N\n\x10market_positions\x18\x13 \x01(\x0b\x32!.vega.snapshot.v1.MarketPositionsH\x00R\x0fmarketPositions\x12\x39\n\tapp_state\x18\x14 \x01(\x0b\x32\x1a.vega.snapshot.v1.AppStateH\x00R\x08\x61ppState\x12\x34\n\x05\x65poch\x18\x15 \x01(\x0b\x32\x1c.vega.snapshot.v1.EpochStateH\x00R\x05\x65poch\x12\x61\n\x17rewards_pending_payouts\x18\x17 \x01(\x0b\x32\'.vega.snapshot.v1.RewardsPendingPayoutsH\x00R\x15rewardsPendingPayouts\x12K\n\x0fgovernance_node\x18\x18 \x01(\x0b\x32 .vega.snapshot.v1.GovernanceNodeH\x00R\x0egovernanceNode\x12?\n\x0blimit_state\x18\x19 \x01(\x0b\x32\x1c.vega.snapshot.v1.LimitStateH\x00R\nlimitState\x12L\n\x10vote_spam_policy\x18\x1a \x01(\x0b\x32 .vega.snapshot.v1.VoteSpamPolicyH\x00R\x0evoteSpamPolicy\x12R\n\x12simple_spam_policy\x18\x1b \x01(\x0b\x32".vega.snapshot.v1.SimpleSpamPolicyH\x00R\x10simpleSpamPolicy\x12\x32\n\x06notary\x18\x1c \x01(\x0b\x32\x18.vega.snapshot.v1.NotaryH\x00R\x06notary\x12K\n\x0f\x65vent_forwarder\x18\x1f \x01(\x0b\x32 .vega.snapshot.v1.EventForwarderH\x00R\x0e\x65ventForwarder\x12\x64\n\x18stake_verifier_deposited\x18  \x01(\x0b\x32(.vega.snapshot.v1.StakeVerifierDepositedH\x00R\x16stakeVerifierDeposited\x12^\n\x16stake_verifier_removed\x18! \x01(\x0b\x32&.vega.snapshot.v1.StakeVerifierRemovedH\x00R\x14stakeVerifierRemoved\x12\x35\n\x07witness\x18" \x01(\x0b\x32\x19.vega.snapshot.v1.WitnessH\x00R\x07witness\x12\x83\x01\n#delegation_last_reconciliation_time\x18# \x01(\x0b\x32\x32.vega.snapshot.v1.DelegationLastReconciliationTimeH\x00R delegationLastReconciliationTime\x12\x38\n\x08topology\x18$ \x01(\x0b\x32\x1a.vega.snapshot.v1.TopologyH\x00R\x08topology\x12\x44\n\x0boracle_data\x18% \x01(\x0b\x32!.vega.snapshot.v1.OracleDataBatchH\x00R\noracleData\x12Z\n\x14liquidity_parameters\x18& \x01(\x0b\x32%.vega.snapshot.v1.LiquidityParametersH\x00R\x13liquidityParameters\x12p\n\x1cliquidity_pending_provisions\x18\' \x01(\x0b\x32,.vega.snapshot.v1.LiquidityPendingProvisionsH\x00R\x1aliquidityPendingProvisions\x12\x80\x01\n"liquidity_parties_liquidity_orders\x18( \x01(\x0b\x32\x31.vega.snapshot.v1.LiquidityPartiesLiquidityOrdersH\x00R\x1fliquidityPartiesLiquidityOrders\x12\x64\n\x18liquidity_parties_orders\x18) \x01(\x0b\x32(.vega.snapshot.v1.LiquidityPartiesOrdersH\x00R\x16liquidityPartiesOrders\x12Z\n\x14liquidity_provisions\x18* \x01(\x0b\x32%.vega.snapshot.v1.LiquidityProvisionsH\x00R\x13liquidityProvisions\x12T\n\x12liquidity_supplied\x18+ \x01(\x0b\x32#.vega.snapshot.v1.LiquiditySuppliedH\x00R\x11liquiditySupplied\x12N\n\x10liquidity_target\x18, \x01(\x0b\x32!.vega.snapshot.v1.LiquidityTargetH\x00R\x0fliquidityTarget\x12\x64\n\x18\x66loating_point_consensus\x18. \x01(\x0b\x32(.vega.snapshot.v1.FloatingPointConsensusH\x00R\x16\x66loatingPointConsensus\x12H\n\x0emarket_tracker\x18/ \x01(\x0b\x32\x1f.vega.snapshot.v1.MarketTrackerH\x00R\rmarketTracker\x12m\n\x1b\x62\x61nking_recurring_transfers\x18\x31 \x01(\x0b\x32+.vega.snapshot.v1.BankingRecurringTransfersH\x00R\x19\x62\x61nkingRecurringTransfers\x12m\n\x1b\x62\x61nking_scheduled_transfers\x18\x32 \x01(\x0b\x32+.vega.snapshot.v1.BankingScheduledTransfersH\x00R\x19\x62\x61nkingScheduledTransfers\x12z\n erc20_multisig_topology_verified\x18\x33 \x01(\x0b\x32/.vega.snapshot.v1.ERC20MultiSigTopologyVerifiedH\x00R\x1d\x65rc20MultisigTopologyVerified\x12w\n\x1f\x65rc20_multisig_topology_pending\x18\x34 \x01(\x0b\x32..vega.snapshot.v1.ERC20MultiSigTopologyPendingH\x00R\x1c\x65rc20MultisigTopologyPending\x12\x43\n\rproof_of_work\x18\x35 \x01(\x0b\x32\x1d.vega.snapshot.v1.ProofOfWorkH\x00R\x0bproofOfWork\x12[\n\x15pending_asset_updates\x18\x36 \x01(\x0b\x32%.vega.snapshot.v1.PendingAssetUpdatesH\x00R\x13pendingAssetUpdates\x12j\n\x1aprotocol_upgrade_proposals\x18\x37 \x01(\x0b\x32*.vega.snapshot.v1.ProtocolUpgradeProposalsH\x00R\x18protocolUpgradeProposals\x12X\n\x14\x62\x61nking_bridge_state\x18\x38 \x01(\x0b\x32$.vega.snapshot.v1.BankingBridgeStateH\x00R\x12\x62\x61nkingBridgeState\x12N\n\x10settlement_state\x18\x39 \x01(\x0b\x32!.vega.snapshot.v1.SettlementStateH\x00R\x0fsettlementState\x12N\n\x10liquidity_scores\x18: \x01(\x0b\x32!.vega.snapshot.v1.LiquidityScoresH\x00R\x0fliquidityScores\x12[\n\x15spot_liquidity_target\x18; \x01(\x0b\x32%.vega.snapshot.v1.SpotLiquidityTargetH\x00R\x13spotLiquidityTarget\x12\x8c\x01\n&banking_recurring_governance_transfers\x18< \x01(\x0b\x32\x35.vega.snapshot.v1.BankingRecurringGovernanceTransfersH\x00R#bankingRecurringGovernanceTransfers\x12\x8c\x01\n&banking_scheduled_governance_transfers\x18= \x01(\x0b\x32\x35.vega.snapshot.v1.BankingScheduledGovernanceTransfersH\x00R#bankingScheduledGovernanceTransfersB\x06\n\x04\x64\x61ta"L\n\x15TimestampedTotalStake\x12\x1f\n\x0btotal_stake\x18\x01 \x01(\x04R\ntotalStake\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"R\n\x17TimestampedOpenInterest\x12#\n\ropen_interest\x18\x01 \x01(\x04R\x0copenInterest\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\xf2\x02\n\x0fLiquidityTarget\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12!\n\x0c\x63urrent_time\x18\x02 \x01(\x03R\x0b\x63urrentTime\x12-\n\x12scheduled_truncate\x18\x03 \x01(\x03R\x11scheduledTruncate\x12\x34\n\x16\x63urrent_open_interests\x18\x04 \x03(\x04R\x14\x63urrentOpenInterests\x12\x61\n\x17previous_open_interests\x18\x05 \x03(\x0b\x32).vega.snapshot.v1.TimestampedOpenInterestR\x15previousOpenInterests\x12W\n\x12max_open_interests\x18\x06 \x01(\x0b\x32).vega.snapshot.v1.TimestampedOpenInterestR\x10maxOpenInterests"\xe0\x02\n\x13SpotLiquidityTarget\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12!\n\x0c\x63urrent_time\x18\x02 \x01(\x03R\x0b\x63urrentTime\x12-\n\x12scheduled_truncate\x18\x03 \x01(\x03R\x11scheduledTruncate\x12.\n\x13\x63urrent_total_stake\x18\x04 \x03(\x04R\x11\x63urrentTotalStake\x12Y\n\x14previous_total_stake\x18\x05 \x03(\x0b\x32\'.vega.snapshot.v1.TimestampedTotalStakeR\x12previousTotalStake\x12O\n\x0fmax_total_stake\x18\x06 \x01(\x0b\x32\'.vega.snapshot.v1.TimestampedTotalStakeR\rmaxTotalStake"Z\n\x1eLiquidityOffsetProbabilityPair\x12\x16\n\x06offset\x18\x01 \x01(\rR\x06offset\x12 \n\x0bprobability\x18\x02 \x01(\tR\x0bprobability"\xfb\x01\n\x11LiquiditySupplied\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63onsensus_reached\x18\x02 \x01(\x08R\x10\x63onsensusReached\x12M\n\tbid_cache\x18\x03 \x03(\x0b\x32\x30.vega.snapshot.v1.LiquidityOffsetProbabilityPairR\x08\x62idCache\x12M\n\task_cache\x18\x04 \x03(\x0b\x32\x30.vega.snapshot.v1.LiquidityOffsetProbabilityPairR\x08\x61skCache"P\n\x0fOracleDataBatch\x12=\n\x0boracle_data\x18\x01 \x03(\x0b\x32\x1c.vega.snapshot.v1.OracleDataR\noracleData"r\n\nOracleData\x12.\n\x07signers\x18\x01 \x03(\x0b\x32\x14.vega.data.v1.SignerR\x07signers\x12\x34\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.OracleDataPairR\x04\x64\x61ta"8\n\x0eOracleDataPair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"C\n\x07Witness\x12\x38\n\tresources\x18\x01 \x03(\x0b\x32\x1a.vega.snapshot.v1.ResourceR\tresources"g\n\x08Resource\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x63heck_until\x18\x02 \x01(\x03R\ncheckUntil\x12\x14\n\x05votes\x18\x03 \x03(\tR\x05votes\x12\x14\n\x05state\x18\x04 \x01(\rR\x05state"3\n\x0e\x45ventForwarder\x12!\n\x0c\x61\x63ked_events\x18\x01 \x03(\tR\x0b\x61\x63kedEvents"?\n\x12\x43ollateralAccounts\x12)\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x08\x61\x63\x63ounts"7\n\x10\x43ollateralAssets\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"3\n\x0c\x41\x63tiveAssets\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"4\n\rPendingAssets\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets":\n\x13PendingAssetUpdates\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"P\n\nWithdrawal\x12\x10\n\x03ref\x18\x01 \x01(\tR\x03ref\x12\x30\n\nwithdrawal\x18\x02 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"B\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\'\n\x07\x64\x65posit\x18\x02 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"i\n\x05TxRef\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset\x12\x19\n\x08\x62lock_nr\x18\x02 \x01(\x04R\x07\x62lockNr\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1b\n\tlog_index\x18\x04 \x01(\x04R\x08logIndex"T\n\x12\x42\x61nkingWithdrawals\x12>\n\x0bwithdrawals\x18\x01 \x03(\x0b\x32\x1c.vega.snapshot.v1.WithdrawalR\x0bwithdrawals"F\n\x0f\x42\x61nkingDeposits\x12\x33\n\x07\x64\x65posit\x18\x01 \x03(\x0b\x32\x19.vega.snapshot.v1.DepositR\x07\x64\x65posit"P\n\x0b\x42\x61nkingSeen\x12\x12\n\x04refs\x18\x01 \x03(\tR\x04refs\x12-\n\x13last_seen_eth_block\x18\x02 \x01(\x04R\x10lastSeenEthBlock"Y\n\x13\x42\x61nkingAssetActions\x12\x42\n\x0c\x61sset_action\x18\x01 \x03(\x0b\x32\x1f.vega.checkpoint.v1.AssetActionR\x0b\x61ssetAction"t\n\x19\x42\x61nkingRecurringTransfers\x12W\n\x13recurring_transfers\x18\x01 \x01(\x0b\x32&.vega.checkpoint.v1.RecurringTransfersR\x12recurringTransfers"t\n\x19\x42\x61nkingScheduledTransfers\x12W\n\x11transfers_at_time\x18\x01 \x03(\x0b\x32+.vega.checkpoint.v1.ScheduledTransferAtTimeR\x0ftransfersAtTime"~\n#BankingRecurringGovernanceTransfers\x12W\n\x13recurring_transfers\x18\x01 \x03(\x0b\x32&.vega.checkpoint.v1.GovernanceTransferR\x12recurringTransfers"\x88\x01\n#BankingScheduledGovernanceTransfers\x12\x61\n\x11transfers_at_time\x18\x01 \x03(\x0b\x32\x35.vega.checkpoint.v1.ScheduledGovernanceTransferAtTimeR\x0ftransfersAtTime"X\n\x12\x42\x61nkingBridgeState\x12\x42\n\x0c\x62ridge_state\x18\x01 \x01(\x0b\x32\x1f.vega.checkpoint.v1.BridgeStateR\x0b\x62ridgeState"%\n\nCheckpoint\x12\x17\n\x07next_cp\x18\x01 \x01(\x03R\x06nextCp"\\\n DelegationLastReconciliationTime\x12\x38\n\x18last_reconciliation_time\x18\x01 \x01(\x03R\x16lastReconciliationTime"F\n\x10\x44\x65legationActive\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"}\n\x11\x44\x65legationPending\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0cundelegation\x18\x02 \x03(\x0b\x32\x10.vega.DelegationR\x0cundelegation"*\n\x0e\x44\x65legationAuto\x12\x18\n\x07parties\x18\x01 \x03(\tR\x07parties"\x9a\x01\n\x0cProposalData\x12*\n\x08proposal\x18\x01 \x01(\x0b\x32\x0e.vega.ProposalR\x08proposal\x12\x1c\n\x03yes\x18\x02 \x03(\x0b\x32\n.vega.VoteR\x03yes\x12\x1a\n\x02no\x18\x03 \x03(\x0b\x32\n.vega.VoteR\x02no\x12$\n\x07invalid\x18\x04 \x03(\x0b\x32\n.vega.VoteR\x07invalid"Q\n\x11GovernanceEnacted\x12<\n\tproposals\x18\x01 \x03(\x0b\x32\x1e.vega.snapshot.v1.ProposalDataR\tproposals"P\n\x10GovernanceActive\x12<\n\tproposals\x18\x01 \x03(\x0b\x32\x1e.vega.snapshot.v1.ProposalDataR\tproposals">\n\x0eGovernanceNode\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"v\n\x0eStakingAccount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x34\n\x06\x65vents\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x06\x65vents"\xe1\x01\n\x0fStakingAccounts\x12<\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32 .vega.snapshot.v1.StakingAccountR\x08\x61\x63\x63ounts\x12;\n\x1astaking_asset_total_supply\x18\x02 \x01(\tR\x17stakingAssetTotalSupply\x12S\n\x1apending_stake_total_supply\x18\x03 \x01(\x0b\x32\x16.vega.StakeTotalSupplyR\x17pendingStakeTotalSupply"\xcc\x01\n\x0cMatchingBook\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1d\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x03\x62uy\x12\x1f\n\x04sell\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x04sell\x12*\n\x11last_traded_price\x18\x04 \x01(\tR\x0flastTradedPrice\x12\x18\n\x07\x61uction\x18\x05 \x01(\x08R\x07\x61uction\x12\x19\n\x08\x62\x61tch_id\x18\x06 \x01(\x04R\x07\x62\x61tchId";\n\tNetParams\x12.\n\x06params\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x06params"0\n\nDecimalMap\x12\x10\n\x03key\x18\x01 \x01(\x03R\x03key\x12\x10\n\x03val\x18\x02 \x01(\tR\x03val"5\n\tTimePrice\x12\x12\n\x04time\x18\x01 \x01(\x03R\x04time\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price";\n\x0bPriceVolume\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"B\n\nPriceRange\x12\x10\n\x03min\x18\x01 \x01(\tR\x03min\x12\x10\n\x03max\x18\x02 \x01(\tR\x03max\x12\x10\n\x03ref\x18\x03 \x01(\tR\x03ref"\x9a\x01\n\nPriceBound\x12\x16\n\x06\x61\x63tive\x18\x01 \x01(\x08R\x06\x61\x63tive\x12\x1b\n\tup_factor\x18\x02 \x01(\tR\x08upFactor\x12\x1f\n\x0b\x64own_factor\x18\x03 \x01(\tR\ndownFactor\x12\x36\n\x07trigger\x18\x04 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger"y\n\x0fPriceRangeCache\x12\x32\n\x05\x62ound\x18\x01 \x01(\x0b\x32\x1c.vega.snapshot.v1.PriceBoundR\x05\x62ound\x12\x32\n\x05range\x18\x02 \x01(\x0b\x32\x1c.vega.snapshot.v1.PriceRangeR\x05range"<\n\x0c\x43urrentPrice\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"S\n\tPastPrice\x12\x12\n\x04time\x18\x01 \x01(\x03R\x04time\x12\x32\n\x15volume_weighted_price\x18\x02 \x01(\tR\x13volumeWeightedPrice"\xf4\x04\n\x0cPriceMonitor\x12 \n\x0binitialised\x18\x03 \x01(\x08R\x0binitialised\x12=\n\x0b\x66p_horizons\x18\x04 \x03(\x0b\x32\x1c.vega.snapshot.v1.DecimalMapR\nfpHorizons\x12\x10\n\x03now\x18\x05 \x01(\x03R\x03now\x12\x16\n\x06update\x18\x06 \x01(\x03R\x06update\x12\x34\n\x06\x62ounds\x18\x07 \x03(\x0b\x32\x1c.vega.snapshot.v1.PriceBoundR\x06\x62ounds\x12\x33\n\x16price_range_cache_time\x18\x08 \x01(\x03R\x13priceRangeCacheTime\x12M\n\x11price_range_cache\x18\t \x03(\x0b\x32!.vega.snapshot.v1.PriceRangeCacheR\x0fpriceRangeCache\x12/\n\x14ref_price_cache_time\x18\n \x01(\x03R\x11refPriceCacheTime\x12\x44\n\x0fref_price_cache\x18\x0b \x03(\x0b\x32\x1c.vega.snapshot.v1.DecimalMapR\rrefPriceCache\x12=\n\nprices_now\x18\x0c \x03(\x0b\x32\x1e.vega.snapshot.v1.CurrentPriceR\tpricesNow\x12<\n\x0bprices_past\x18\r \x03(\x0b\x32\x1b.vega.snapshot.v1.PastPriceR\npricesPast\x12+\n\x11\x63onsensus_reached\x18\x0e \x01(\x08R\x10\x63onsensusReached"\xf8\x02\n\x0c\x41uctionState\x12,\n\x04mode\x18\x01 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x04mode\x12;\n\x0c\x64\x65\x66\x61ult_mode\x18\x02 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x0b\x64\x65\x66\x61ultMode\x12.\n\x07trigger\x18\x03 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x14\n\x05\x62\x65gin\x18\x04 \x01(\x03R\x05\x62\x65gin\x12\'\n\x03\x65nd\x18\x05 \x01(\x0b\x32\x15.vega.AuctionDurationR\x03\x65nd\x12\x14\n\x05start\x18\x06 \x01(\x08R\x05start\x12\x12\n\x04stop\x18\x07 \x01(\x08R\x04stop\x12\x32\n\textension\x18\x08 \x01(\x0e\x32\x14.vega.AuctionTriggerR\textension\x12\x30\n\x14\x65xtension_event_sent\x18\t \x01(\x08R\x12\x65xtensionEventSent"u\n\rEquityShareLP\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05stake\x18\x02 \x01(\tR\x05stake\x12\x14\n\x05share\x18\x03 \x01(\tR\x05share\x12\x10\n\x03\x61vg\x18\x04 \x01(\tR\x03\x61vg\x12\x16\n\x06vshare\x18\x05 \x01(\tR\x06vshare"\xa9\x01\n\x0b\x45quityShare\x12\x10\n\x03mvp\x18\x01 \x01(\tR\x03mvp\x12\x32\n\x15opening_auction_ended\x18\x02 \x01(\x08R\x13openingAuctionEnded\x12\x31\n\x03lps\x18\x03 \x03(\x0b\x32\x1f.vega.snapshot.v1.EquityShareLPR\x03lps\x12\x0c\n\x01r\x18\x04 \x01(\tR\x01r\x12\x13\n\x05p_mvp\x18\x05 \x01(\tR\x04pMvp"\x84\x01\n\x0b\x46\x65\x65Splitter\x12*\n\x11time_window_start\x18\x01 \x01(\x03R\x0ftimeWindowStart\x12\x1f\n\x0btrade_value\x18\x02 \x01(\tR\ntradeValue\x12\x10\n\x03\x61vg\x18\x03 \x01(\tR\x03\x61vg\x12\x16\n\x06window\x18\x04 \x01(\x04R\x06window"\xfc\x06\n\nSpotMarket\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x43\n\rprice_monitor\x18\x02 \x01(\x0b\x32\x1e.vega.snapshot.v1.PriceMonitorR\x0cpriceMonitor\x12\x43\n\rauction_state\x18\x03 \x01(\x0b\x32\x1e.vega.snapshot.v1.AuctionStateR\x0c\x61uctionState\x12\x43\n\rpegged_orders\x18\x04 \x01(\x0b\x32\x1e.vega.snapshot.v1.PeggedOrdersR\x0cpeggedOrders\x12\x34\n\x0f\x65xpiring_orders\x18\x05 \x03(\x0b\x32\x0b.vega.OrderR\x0e\x65xpiringOrders\x12"\n\rlast_best_bid\x18\x06 \x01(\tR\x0blastBestBid\x12"\n\rlast_best_ask\x18\x07 \x01(\tR\x0blastBestAsk\x12 \n\x0clast_mid_bid\x18\x08 \x01(\tR\nlastMidBid\x12 \n\x0clast_mid_ask\x18\t \x01(\tR\nlastMidAsk\x12\x35\n\x17last_market_value_proxy\x18\n \x01(\tR\x14lastMarketValueProxy\x12\x41\n\x1dlast_equity_share_distributed\x18\x0b \x01(\x03R\x1alastEquityShareDistributed\x12@\n\x0c\x65quity_share\x18\x0c \x01(\x0b\x32\x1d.vega.snapshot.v1.EquityShareR\x0b\x65quityShare\x12,\n\x12\x63urrent_mark_price\x18\r \x01(\tR\x10\x63urrentMarkPrice\x12@\n\x0c\x66\x65\x65_splitter\x18\x0e \x01(\x0b\x32\x1d.vega.snapshot.v1.FeeSplitterR\x0b\x66\x65\x65Splitter\x12-\n\x13next_mark_to_market\x18\x0f \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x10 \x01(\tR\x0flastTradedPrice\x12\x18\n\x07parties\x18\x11 \x03(\tR\x07parties\x12\x16\n\x06\x63losed\x18\x12 \x01(\x08R\x06\x63losed"\x97\t\n\x06Market\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x43\n\rprice_monitor\x18\x02 \x01(\x0b\x32\x1e.vega.snapshot.v1.PriceMonitorR\x0cpriceMonitor\x12\x43\n\rauction_state\x18\x03 \x01(\x0b\x32\x1e.vega.snapshot.v1.AuctionStateR\x0c\x61uctionState\x12\x43\n\rpegged_orders\x18\x04 \x01(\x0b\x32\x1e.vega.snapshot.v1.PeggedOrdersR\x0cpeggedOrders\x12\x34\n\x0f\x65xpiring_orders\x18\x05 \x03(\x0b\x32\x0b.vega.OrderR\x0e\x65xpiringOrders\x12"\n\rlast_best_bid\x18\x06 \x01(\tR\x0blastBestBid\x12"\n\rlast_best_ask\x18\x07 \x01(\tR\x0blastBestAsk\x12 \n\x0clast_mid_bid\x18\x08 \x01(\tR\nlastMidBid\x12 \n\x0clast_mid_ask\x18\t \x01(\tR\nlastMidAsk\x12\x35\n\x17last_market_value_proxy\x18\n \x01(\tR\x14lastMarketValueProxy\x12\x41\n\x1dlast_equity_share_distributed\x18\x0b \x01(\x03R\x1alastEquityShareDistributed\x12@\n\x0c\x65quity_share\x18\x0c \x01(\x0b\x32\x1d.vega.snapshot.v1.EquityShareR\x0b\x65quityShare\x12,\n\x12\x63urrent_mark_price\x18\r \x01(\tR\x10\x63urrentMarkPrice\x12*\n\x11risk_factor_short\x18\x0e \x01(\tR\x0friskFactorShort\x12(\n\x10risk_factor_long\x18\x0f \x01(\tR\x0eriskFactorLong\x12\x41\n\x1drisk_factor_consensus_reached\x18\x10 \x01(\x08R\x1ariskFactorConsensusReached\x12@\n\x0c\x66\x65\x65_splitter\x18\x11 \x01(\x0b\x32\x1d.vega.snapshot.v1.FeeSplitterR\x0b\x66\x65\x65Splitter\x12\'\n\x0fsettlement_data\x18\x12 \x01(\tR\x0esettlementData\x12-\n\x13next_mark_to_market\x18\x13 \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x14 \x01(\tR\x0flastTradedPrice\x12\x18\n\x07parties\x18\x15 \x03(\tR\x07parties\x12\x16\n\x06\x63losed\x18\x16 \x01(\x08R\x06\x63losed\x12\x1c\n\tsucceeded\x18\x17 \x01(\x08R\tsucceeded\x12=\n\x0bstop_orders\x18\x18 \x01(\x0b\x32\x1c.vega.snapshot.v1.StopOrdersR\nstopOrders"=\n\rOrdersAtPrice\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12\x16\n\x06orders\x18\x02 \x03(\tR\x06orders"\x98\x01\n\x10PricedStopOrders\x12\x42\n\x0c\x66\x61lls_bellow\x18\x01 \x03(\x0b\x32\x1f.vega.snapshot.v1.OrdersAtPriceR\x0b\x66\x61llsBellow\x12@\n\x0brises_above\x18\x02 \x03(\x0b\x32\x1f.vega.snapshot.v1.OrdersAtPriceR\nrisesAbove"\xc4\x01\n\x12TrailingStopOrders\x12&\n\x0flast_seen_price\x18\x01 \x01(\tR\rlastSeenPrice\x12\x43\n\x0c\x66\x61lls_bellow\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.OffsetsAtPriceR\x0b\x66\x61llsBellow\x12\x41\n\x0brises_above\x18\x03 \x03(\x0b\x32 .vega.snapshot.v1.OffsetsAtPriceR\nrisesAbove"@\n\x0eOrdersAtOffset\x12\x16\n\x06offset\x18\x01 \x01(\tR\x06offset\x12\x16\n\x06orders\x18\x02 \x03(\tR\x06orders"b\n\x0eOffsetsAtPrice\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12:\n\x07offsets\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.OrdersAtOffsetR\x07offsets"\xf7\x01\n\nStopOrders\x12?\n\x0bstop_orders\x18\x01 \x03(\x0b\x32\x1e.vega.events.v1.StopOrderEventR\nstopOrders\x12P\n\x12priced_stop_orders\x18\x02 \x01(\x0b\x32".vega.snapshot.v1.PricedStopOrdersR\x10pricedStopOrders\x12V\n\x14trailing_stop_orders\x18\x03 \x01(\x0b\x32$.vega.snapshot.v1.TrailingStopOrdersR\x12trailingStopOrders"@\n\x0cPeggedOrders\x12\x30\n\rparked_orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x0cparkedOrders"\xd1\x01\n\x10\x45xecutionMarkets\x12\x32\n\x07markets\x18\x01 \x03(\x0b\x32\x18.vega.snapshot.v1.MarketR\x07markets\x12?\n\x0cspot_markets\x18\x02 \x03(\x0b\x32\x1c.vega.snapshot.v1.SpotMarketR\x0bspotMarkets\x12H\n\x0fsettled_markets\x18\x03 \x03(\x0b\x32\x1f.vega.checkpoint.v1.MarketStateR\x0esettledMarkets"\xe7\x01\n\x08Position\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x12\n\x04size\x18\x02 \x01(\x03R\x04size\x12\x10\n\x03\x62uy\x18\x03 \x01(\x03R\x03\x62uy\x12\x12\n\x04sell\x18\x04 \x01(\x03R\x04sell\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12&\n\x0f\x62uy_sum_product\x18\x06 \x01(\tR\rbuySumProduct\x12(\n\x10sell_sum_product\x18\x07 \x01(\tR\x0esellSumProduct\x12\x1e\n\ndistressed\x18\x08 \x01(\x08R\ndistressed"h\n\x0fMarketPositions\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x38\n\tpositions\x18\x02 \x03(\x0b\x32\x1a.vega.snapshot.v1.PositionR\tpositions"\xee\x01\n\x0fSettlementState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12&\n\x0flast_mark_price\x18\x02 \x01(\tR\rlastMarkPrice\x12[\n\x16last_settled_positions\x18\x03 \x03(\x0b\x32%.vega.snapshot.v1.LastSettledPositionR\x14lastSettledPositions\x12\x39\n\x06trades\x18\x04 \x03(\x0b\x32!.vega.snapshot.v1.SettlementTradeR\x06trades"V\n\x13LastSettledPosition\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12)\n\x10settled_position\x18\x02 \x01(\x03R\x0fsettledPosition"\x94\x01\n\x0fSettlementTrade\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice\x12\x12\n\x04size\x18\x04 \x01(\x03R\x04size\x12\x19\n\x08new_size\x18\x05 \x01(\x03R\x07newSize"g\n\x08\x41ppState\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x12\n\x04time\x18\x03 \x01(\x03R\x04time\x12\x19\n\x08\x63hain_id\x18\x04 \x01(\tR\x07\x63hainId"\xc3\x01\n\nEpochState\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x36\n\x18ready_to_start_new_epoch\x18\x06 \x01(\x08R\x14readyToStartNewEpoch\x12+\n\x12ready_to_end_epoch\x18\x07 \x01(\x08R\x0freadyToEndEpoch"{\n\x15RewardsPendingPayouts\x12\x62\n\x18scheduled_rewards_payout\x18\x01 \x03(\x0b\x32(.vega.snapshot.v1.ScheduledRewardsPayoutR\x16scheduledRewardsPayout"\x81\x01\n\x16ScheduledRewardsPayout\x12\x1f\n\x0bpayout_time\x18\x01 \x01(\x03R\npayoutTime\x12\x46\n\x0erewards_payout\x18\x02 \x03(\x0b\x32\x1f.vega.snapshot.v1.RewardsPayoutR\rrewardsPayout"\xfc\x01\n\rRewardsPayout\x12!\n\x0c\x66rom_account\x18\x01 \x01(\tR\x0b\x66romAccount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12T\n\x13reward_party_amount\x18\x03 \x03(\x0b\x32$.vega.snapshot.v1.RewardsPartyAmountR\x11rewardPartyAmount\x12!\n\x0ctotal_reward\x18\x04 \x01(\tR\x0btotalReward\x12\x1b\n\tepoch_seq\x18\x05 \x01(\tR\x08\x65pochSeq\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp"B\n\x12RewardsPartyAmount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\x94\x03\n\nLimitState\x12\x1f\n\x0b\x62lock_count\x18\x01 \x01(\rR\nblockCount\x12,\n\x12\x63\x61n_propose_market\x18\x02 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x03 \x01(\x08R\x0f\x63\x61nProposeAsset\x12%\n\x0egenesis_loaded\x18\x04 \x01(\x08R\rgenesisLoaded\x12\x34\n\x16propose_market_enabled\x18\x05 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x06 \x01(\x08R\x13proposeAssetEnabled\x12=\n\x1bpropose_market_enabled_from\x18\x07 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\x08 \x01(\x03R\x17proposeAssetEnabledFrom"\x94\x04\n\x0eVoteSpamPolicy\x12L\n\rparty_to_vote\x18\x01 \x03(\x0b\x32(.vega.snapshot.v1.PartyProposalVoteCountR\x0bpartyToVote\x12\x44\n\x0e\x62\x61nned_parties\x18\x02 \x03(\x0b\x32\x1d.vega.snapshot.v1.BannedPartyR\rbannedParties\x12H\n\rtoken_balance\x18\x03 \x03(\x0b\x32#.vega.snapshot.v1.PartyTokenBalanceR\x0ctokenBalance\x12_\n\x1arecent_blocks_reject_stats\x18\x04 \x03(\x0b\x32".vega.snapshot.v1.BlockRejectStatsR\x17recentBlocksRejectStats\x12.\n\x13\x63urrent_block_index\x18\x05 \x01(\x04R\x11\x63urrentBlockIndex\x12.\n\x13last_increase_block\x18\x06 \x01(\x04R\x11lastIncreaseBlock\x12*\n\x11\x63urrent_epoch_seq\x18\x07 \x01(\x04R\x0f\x63urrentEpochSeq\x12\x37\n\x18min_voting_tokens_factor\x18\x08 \x01(\tR\x15minVotingTokensFactor"`\n\x16PartyProposalVoteCount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1a\n\x08proposal\x18\x02 \x01(\tR\x08proposal\x12\x14\n\x05\x63ount\x18\x03 \x01(\x04R\x05\x63ount"C\n\x11PartyTokenBalance\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"D\n\x10\x42lockRejectStats\x12\x1a\n\x08rejected\x18\x01 \x01(\x04R\x08rejected\x12\x14\n\x05total\x18\x02 \x01(\x04R\x05total"G\n\x19SpamPartyTransactionCount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x14\n\x05\x63ount\x18\x02 \x01(\x04R\x05\x63ount"\xc2\x02\n\x10SimpleSpamPolicy\x12\x1f\n\x0bpolicy_name\x18\x01 \x01(\tR\npolicyName\x12Q\n\x0eparty_to_count\x18\x02 \x03(\x0b\x32+.vega.snapshot.v1.SpamPartyTransactionCountR\x0cpartyToCount\x12\x44\n\x0e\x62\x61nned_parties\x18\x03 \x03(\x0b\x32\x1d.vega.snapshot.v1.BannedPartyR\rbannedParties\x12H\n\rtoken_balance\x18\x04 \x03(\x0b\x32#.vega.snapshot.v1.PartyTokenBalanceR\x0ctokenBalance\x12*\n\x11\x63urrent_epoch_seq\x18\x05 \x01(\x04R\x0f\x63urrentEpochSeq"p\n\nNotarySigs\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04kind\x18\x02 \x01(\x05R\x04kind\x12\x12\n\x04node\x18\x03 \x01(\tR\x04node\x12\x10\n\x03sig\x18\x04 \x01(\tR\x03sig\x12\x18\n\x07pending\x18\x05 \x01(\x08R\x07pending"G\n\x06Notary\x12=\n\x0bnotary_sigs\x18\x01 \x03(\x0b\x32\x1c.vega.snapshot.v1.NotarySigsR\nnotarySigs"m\n\x16StakeVerifierDeposited\x12S\n\x11pending_deposited\x18\x01 \x03(\x0b\x32&.vega.snapshot.v1.StakeVerifierPendingR\x10pendingDeposited"g\n\x14StakeVerifierRemoved\x12O\n\x0fpending_removed\x18\x01 \x03(\x0b\x32&.vega.snapshot.v1.StakeVerifierPendingR\x0ependingRemoved"\x85\x02\n\x14StakeVerifierPending\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12!\n\x0c\x62lock_number\x18\x05 \x01(\x04R\x0b\x62lockNumber\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12\x13\n\x05tx_id\x18\x07 \x01(\tR\x04txId\x12\x0e\n\x02id\x18\x08 \x01(\tR\x02id"\x9b\x01\n\x12PendingKeyRotation\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12)\n\x11new_pub_key_index\x18\x04 \x01(\rR\x0enewPubKeyIndex"\xb8\x01\n\x1aPendingEthereumKeyRotation\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x1f\n\x0bold_address\x18\x05 \x01(\tR\noldAddress"\xdd\x04\n\x08Topology\x12G\n\x0evalidator_data\x18\x01 \x03(\x0b\x32 .vega.snapshot.v1.ValidatorStateR\rvalidatorData\x12\x1d\n\nchain_keys\x18\x02 \x03(\tR\tchainKeys\x12_\n\x19pending_pub_key_rotations\x18\x03 \x03(\x0b\x32$.vega.snapshot.v1.PendingKeyRotationR\x16pendingPubKeyRotations\x12[\n\x15validator_performance\x18\x04 \x01(\x0b\x32&.vega.snapshot.v1.ValidatorPerformanceR\x14validatorPerformance\x12q\n\x1epending_ethereum_key_rotations\x18\x05 \x03(\x0b\x32,.vega.snapshot.v1.PendingEthereumKeyRotationR\x1bpendingEthereumKeyRotations\x12\x43\n\nsignatures\x18\x06 \x01(\x0b\x32#.vega.snapshot.v1.ToplogySignaturesR\nsignatures\x12s\n\x1funsolved_ethereum_key_rotations\x18\x07 \x03(\x0b\x32,.vega.snapshot.v1.PendingEthereumKeyRotationR\x1cunsolvedEthereumKeyRotations"\xde\x01\n\x11ToplogySignatures\x12\x65\n\x12pending_signatures\x18\x01 \x03(\x0b\x32\x36.vega.snapshot.v1.PendingERC20MultisigControlSignatureR\x11pendingSignatures\x12\x62\n\x11issued_signatures\x18\x02 \x03(\x0b\x32\x35.vega.snapshot.v1.IssuedERC20MultisigControlSignatureR\x10issuedSignatures"\xb3\x01\n$PendingERC20MultisigControlSignature\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x04 \x01(\x04R\x08\x65pochSeq\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\x05 \x01(\x08R\x05\x61\x64\x64\x65\x64"\x9e\x01\n#IssuedERC20MultisigControlSignature\x12\x1f\n\x0bresource_id\x18\x01 \x01(\tR\nresourceId\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12+\n\x11submitter_address\x18\x03 \x01(\tR\x10submitterAddress"\xf2\x03\n\x0eValidatorState\x12J\n\x10validator_update\x18\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\x0fvalidatorUpdate\x12\x1f\n\x0b\x62lock_added\x18\x02 \x01(\x04R\nblockAdded\x12\x16\n\x06status\x18\x03 \x01(\x05R\x06status\x12.\n\x13status_change_block\x18\x04 \x01(\x04R\x11statusChangeBlock\x12\x46\n last_block_with_positive_ranking\x18\x05 \x01(\x04R\x1clastBlockWithPositiveRanking\x12\x30\n\x14\x65th_events_forwarded\x18\x06 \x01(\x04R\x12\x65thEventsForwarded\x12O\n\x11heartbeat_tracker\x18\x07 \x01(\x0b\x32".vega.snapshot.v1.HeartbeatTrackerR\x10heartbeatTracker\x12\'\n\x0fvalidator_power\x18\x08 \x01(\x03R\x0evalidatorPower\x12\x37\n\rranking_score\x18\t \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore"\xb9\x01\n\x10HeartbeatTracker\x12,\n\x12\x65xpected_next_hash\x18\x01 \x01(\tR\x10\x65xpectedNextHash\x12\x37\n\x18\x65xpected_next_hash_since\x18\x02 \x01(\x03R\x15\x65xpectedNextHashSince\x12\x1f\n\x0b\x62lock_index\x18\x03 \x01(\x05R\nblockIndex\x12\x1d\n\nblock_sigs\x18\x04 \x03(\x08R\tblockSigs"\x99\x02\n\x10PerformanceStats\x12+\n\x11validator_address\x18\x01 \x01(\tR\x10validatorAddress\x12\x1a\n\x08proposed\x18\x02 \x01(\x04R\x08proposed\x12\x18\n\x07\x65lected\x18\x03 \x01(\x04R\x07\x65lected\x12\x14\n\x05voted\x18\x04 \x01(\x04R\x05voted\x12*\n\x11last_height_voted\x18\x05 \x01(\x03R\x0flastHeightVoted\x12\x30\n\x14last_height_proposed\x18\x06 \x01(\x03R\x12lastHeightProposed\x12.\n\x13last_height_elected\x18\x07 \x01(\x03R\x11lastHeightElected"l\n\x14ValidatorPerformance\x12T\n\x14validator_perf_stats\x18\x01 \x03(\x0b\x32".vega.snapshot.v1.PerformanceStatsR\x12validatorPerfStats"\xae\x01\n\x13LiquidityParameters\x12\x17\n\x07max_fee\x18\x01 \x01(\tR\x06maxFee\x12$\n\x0emax_shape_size\x18\x02 \x01(\tR\x0cmaxShapeSize\x12;\n\x1astake_to_obligation_factor\x18\x03 \x01(\tR\x17stakeToObligationFactor\x12\x1b\n\tmarket_id\x18\x04 \x01(\tR\x08marketId"h\n\x1aLiquidityPendingProvisions\x12-\n\x12pending_provisions\x18\x01 \x03(\tR\x11pendingProvisions\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\x80\x01\n\x1fLiquidityPartiesLiquidityOrders\x12@\n\x0cparty_orders\x18\x01 \x03(\x0b\x32\x1d.vega.snapshot.v1.PartyOrdersR\x0bpartyOrders\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"H\n\x0bPartyOrders\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12#\n\x06orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"w\n\x16LiquidityPartiesOrders\x12@\n\x0cparty_orders\x18\x01 \x03(\x0b\x32\x1d.vega.snapshot.v1.PartyOrdersR\x0bpartyOrders\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\x7f\n\x13LiquidityProvisions\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\xa0\x01\n\x0fLiquidityScores\x12\x36\n\x17running_average_counter\x18\x01 \x01(\x05R\x15runningAverageCounter\x12\x38\n\x06scores\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.LiquidityScoreR\x06scores\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId"A\n\x0eLiquidityScore\x12\x14\n\x05score\x18\x01 \x01(\tR\x05score\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId"\xb9\x01\n\x16\x46loatingPointConsensus\x12M\n\x11next_time_trigger\x18\x01 \x03(\x0b\x32!.vega.snapshot.v1.NextTimeTriggerR\x0fnextTimeTrigger\x12P\n\x0fstate_variables\x18\x02 \x03(\x0b\x32\'.vega.snapshot.v1.StateVarInternalStateR\x0estateVariables"\xfc\x01\n\x15StateVarInternalState\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05state\x18\x02 \x01(\x05R\x05state\x12\x19\n\x08\x65vent_id\x18\x03 \x01(\tR\x07\x65ventId\x12]\n\x12validators_results\x18\x04 \x03(\x0b\x32..vega.snapshot.v1.FloatingPointValidatorResultR\x11validatorsResults\x12\x43\n\x1erounds_since_meaningful_update\x18\x05 \x01(\x05R\x1broundsSinceMeaningfulUpdate"\\\n\x1c\x46loatingPointValidatorResult\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06\x62undle\x18\x02 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x06\x62undle"r\n\x0fNextTimeTrigger\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x0e\n\x02id\x18\x03 \x01(\tR\x02id\x12!\n\x0cnext_trigger\x18\x04 \x01(\x03R\x0bnextTrigger"c\n\rMarketTracker\x12R\n\x0fmarket_activity\x18\x01 \x03(\x0b\x32).vega.checkpoint.v1.MarketActivityTrackerR\x0emarketActivity"t\n\x16SignerEventsPerAddress\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12@\n\x06\x65vents\x18\x02 \x03(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventR\x06\x65vents"\x80\x02\n\x1d\x45RC20MultiSigTopologyVerified\x12\x18\n\x07signers\x18\x01 \x03(\tR\x07signers\x12V\n\x12\x65vents_per_address\x18\x02 \x03(\x0b\x32(.vega.snapshot.v1.SignerEventsPerAddressR\x10\x65ventsPerAddress\x12L\n\tthreshold\x18\x03 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventR\tthreshold\x12\x1f\n\x0bseen_events\x18\x04 \x03(\tR\nseenEvents"\xbc\x02\n\x1c\x45RC20MultiSigTopologyPending\x12Q\n\x0fpending_signers\x18\x01 \x03(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventR\x0ependingSigners\x12\x62\n\x15pending_threshold_set\x18\x02 \x03(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventR\x13pendingThresholdSet\x12+\n\x11witnessed_signers\x18\x03 \x03(\tR\x10witnessedSigners\x12\x38\n\x18witnessed_threshold_sets\x18\x04 \x03(\tR\x16witnessedThresholdSets"\xa1\x03\n\x0bProofOfWork\x12!\n\x0c\x62lock_height\x18\x01 \x03(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x03(\tR\tblockHash\x12H\n\x0ctx_at_height\x18\x04 \x03(\x0b\x32&.vega.snapshot.v1.TransactionsAtHeightR\ntxAtHeight\x12J\n\rtid_at_height\x18\x06 \x03(\x0b\x32&.vega.snapshot.v1.TransactionsAtHeightR\x0btidAtHeight\x12\x35\n\x06\x62\x61nned\x18\x07 \x03(\x0b\x32\x1d.vega.snapshot.v1.BannedPartyR\x06\x62\x61nned\x12\x42\n\npow_params\x18\x08 \x03(\x0b\x32#.vega.snapshot.v1.ProofOfWorkParamsR\tpowParams\x12?\n\tpow_state\x18\t \x03(\x0b\x32".vega.snapshot.v1.ProofOfWorkStateR\x08powState"9\n\x0b\x42\x61nnedParty\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x14\n\x05until\x18\x02 \x01(\x03R\x05until"\x84\x03\n\x11ProofOfWorkParams\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x01 \x01(\x04R\x19spamPowNumberOfPastBlocks\x12.\n\x13spam_pow_difficulty\x18\x02 \x01(\rR\x11spamPowDifficulty\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x04 \x01(\x04R\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x05 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x1d\n\nfrom_block\x18\x06 \x01(\x04R\tfromBlock\x12\x1f\n\x0buntil_block\x18\x07 \x01(\x03R\nuntilBlock"X\n\x10ProofOfWorkState\x12\x44\n\tpow_state\x18\x01 \x03(\x0b\x32\'.vega.snapshot.v1.ProofOfWorkBlockStateR\x08powState"\x8c\x01\n\x15ProofOfWorkBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12P\n\x0bparty_state\x18\x02 \x03(\x0b\x32/.vega.snapshot.v1.ProofOfWorkPartyStateForBlockR\npartyState"\x85\x01\n\x1dProofOfWorkPartyStateForBlock\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1d\n\nseen_count\x18\x02 \x01(\x04R\tseenCount\x12/\n\x13observed_difficulty\x18\x03 \x01(\x04R\x12observedDifficulty"R\n\x14TransactionsAtHeight\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12"\n\x0ctransactions\x18\x02 \x03(\tR\x0ctransactions"\xcb\x01\n\x18ProtocolUpgradeProposals\x12O\n\x10\x61\x63tive_proposals\x18\x01 \x03(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x0f\x61\x63tiveProposals\x12^\n\x11\x61\x63\x63\x65pted_proposal\x18\x02 \x01(\x0b\x32\x31.vega.snapshot.v1.AcceptedProtocolUpgradeProposalR\x10\x61\x63\x63\x65ptedProposal"}\n\x1f\x41\x63\x63\x65ptedProtocolUpgradeProposal\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag*`\n\x06\x46ormat\x12\x16\n\x12\x46ORMAT_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x46ORMAT_PROTO\x10\x01\x12\x1b\n\x17\x46ORMAT_PROTO_COMPRESSED\x10\x02\x12\x0f\n\x0b\x46ORMAT_JSON\x10\x03\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/snapshot/v1b\x06proto3'
+    b'\n\x1fvega/snapshot/v1/snapshot.proto\x12\x10vega.snapshot.v1\x1a\x11vega/assets.proto\x1a\x17vega/chain_events.proto\x1a#vega/checkpoint/v1/checkpoint.proto\x1a\x17vega/data/v1/data.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"\x9c\x01\n\x08Snapshot\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x30\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.vega.snapshot.v1.FormatR\x06\x66ormat\x12\x16\n\x06\x63hunks\x18\x03 \x01(\rR\x06\x63hunks\x12\x12\n\x04hash\x18\x04 \x01(\x0cR\x04hash\x12\x1a\n\x08metadata\x18\x05 \x01(\x0cR\x08metadata"{\n\x08NodeHash\x12\x10\n\x03key\x18\x03 \x01(\tR\x03key\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hash\x12\x16\n\x06height\x18\x05 \x01(\x05R\x06height\x12\x18\n\x07version\x18\x06 \x01(\x03R\x07version\x12\x17\n\x07is_leaf\x18\x07 \x01(\x08R\x06isLeaf"\x84\x01\n\x08Metadata\x12\x18\n\x07version\x18\x01 \x01(\x03R\x07version\x12!\n\x0c\x63hunk_hashes\x18\x02 \x03(\tR\x0b\x63hunkHashes\x12;\n\x0bnode_hashes\x18\x03 \x03(\x0b\x32\x1a.vega.snapshot.v1.NodeHashR\nnodeHashes"V\n\x05\x43hunk\x12-\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x19.vega.snapshot.v1.PayloadR\x04\x64\x61ta\x12\x0e\n\x02nr\x18\x02 \x01(\x03R\x02nr\x12\x0e\n\x02of\x18\x03 \x01(\x03R\x02of"\xc6&\n\x07Payload\x12\x45\n\ractive_assets\x18\x01 \x01(\x0b\x32\x1e.vega.snapshot.v1.ActiveAssetsH\x00R\x0c\x61\x63tiveAssets\x12H\n\x0epending_assets\x18\x02 \x01(\x0b\x32\x1f.vega.snapshot.v1.PendingAssetsH\x00R\rpendingAssets\x12W\n\x13\x62\x61nking_withdrawals\x18\x03 \x01(\x0b\x32$.vega.snapshot.v1.BankingWithdrawalsH\x00R\x12\x62\x61nkingWithdrawals\x12N\n\x10\x62\x61nking_deposits\x18\x04 \x01(\x0b\x32!.vega.snapshot.v1.BankingDepositsH\x00R\x0f\x62\x61nkingDeposits\x12\x42\n\x0c\x62\x61nking_seen\x18\x05 \x01(\x0b\x32\x1d.vega.snapshot.v1.BankingSeenH\x00R\x0b\x62\x61nkingSeen\x12[\n\x15\x62\x61nking_asset_actions\x18\x06 \x01(\x0b\x32%.vega.snapshot.v1.BankingAssetActionsH\x00R\x13\x62\x61nkingAssetActions\x12>\n\ncheckpoint\x18\x07 \x01(\x0b\x32\x1c.vega.snapshot.v1.CheckpointH\x00R\ncheckpoint\x12W\n\x13\x63ollateral_accounts\x18\x08 \x01(\x0b\x32$.vega.snapshot.v1.CollateralAccountsH\x00R\x12\x63ollateralAccounts\x12Q\n\x11\x63ollateral_assets\x18\t \x01(\x0b\x32".vega.snapshot.v1.CollateralAssetsH\x00R\x10\x63ollateralAssets\x12Q\n\x11\x64\x65legation_active\x18\n \x01(\x0b\x32".vega.snapshot.v1.DelegationActiveH\x00R\x10\x64\x65legationActive\x12T\n\x12\x64\x65legation_pending\x18\x0b \x01(\x0b\x32#.vega.snapshot.v1.DelegationPendingH\x00R\x11\x64\x65legationPending\x12K\n\x0f\x64\x65legation_auto\x18\x0c \x01(\x0b\x32 .vega.snapshot.v1.DelegationAutoH\x00R\x0e\x64\x65legationAuto\x12Q\n\x11governance_active\x18\r \x01(\x0b\x32".vega.snapshot.v1.GovernanceActiveH\x00R\x10governanceActive\x12T\n\x12governance_enacted\x18\x0e \x01(\x0b\x32#.vega.snapshot.v1.GovernanceEnactedH\x00R\x11governanceEnacted\x12N\n\x10staking_accounts\x18\x0f \x01(\x0b\x32!.vega.snapshot.v1.StakingAccountsH\x00R\x0fstakingAccounts\x12\x45\n\rmatching_book\x18\x10 \x01(\x0b\x32\x1e.vega.snapshot.v1.MatchingBookH\x00R\x0cmatchingBook\x12L\n\x12network_parameters\x18\x11 \x01(\x0b\x32\x1b.vega.snapshot.v1.NetParamsH\x00R\x11networkParameters\x12Q\n\x11\x65xecution_markets\x18\x12 \x01(\x0b\x32".vega.snapshot.v1.ExecutionMarketsH\x00R\x10\x65xecutionMarkets\x12N\n\x10market_positions\x18\x13 \x01(\x0b\x32!.vega.snapshot.v1.MarketPositionsH\x00R\x0fmarketPositions\x12\x39\n\tapp_state\x18\x14 \x01(\x0b\x32\x1a.vega.snapshot.v1.AppStateH\x00R\x08\x61ppState\x12\x34\n\x05\x65poch\x18\x15 \x01(\x0b\x32\x1c.vega.snapshot.v1.EpochStateH\x00R\x05\x65poch\x12\x61\n\x17rewards_pending_payouts\x18\x17 \x01(\x0b\x32\'.vega.snapshot.v1.RewardsPendingPayoutsH\x00R\x15rewardsPendingPayouts\x12K\n\x0fgovernance_node\x18\x18 \x01(\x0b\x32 .vega.snapshot.v1.GovernanceNodeH\x00R\x0egovernanceNode\x12?\n\x0blimit_state\x18\x19 \x01(\x0b\x32\x1c.vega.snapshot.v1.LimitStateH\x00R\nlimitState\x12L\n\x10vote_spam_policy\x18\x1a \x01(\x0b\x32 .vega.snapshot.v1.VoteSpamPolicyH\x00R\x0evoteSpamPolicy\x12R\n\x12simple_spam_policy\x18\x1b \x01(\x0b\x32".vega.snapshot.v1.SimpleSpamPolicyH\x00R\x10simpleSpamPolicy\x12\x32\n\x06notary\x18\x1c \x01(\x0b\x32\x18.vega.snapshot.v1.NotaryH\x00R\x06notary\x12K\n\x0f\x65vent_forwarder\x18\x1f \x01(\x0b\x32 .vega.snapshot.v1.EventForwarderH\x00R\x0e\x65ventForwarder\x12\x64\n\x18stake_verifier_deposited\x18  \x01(\x0b\x32(.vega.snapshot.v1.StakeVerifierDepositedH\x00R\x16stakeVerifierDeposited\x12^\n\x16stake_verifier_removed\x18! \x01(\x0b\x32&.vega.snapshot.v1.StakeVerifierRemovedH\x00R\x14stakeVerifierRemoved\x12\x35\n\x07witness\x18" \x01(\x0b\x32\x19.vega.snapshot.v1.WitnessH\x00R\x07witness\x12\x83\x01\n#delegation_last_reconciliation_time\x18# \x01(\x0b\x32\x32.vega.snapshot.v1.DelegationLastReconciliationTimeH\x00R delegationLastReconciliationTime\x12\x38\n\x08topology\x18$ \x01(\x0b\x32\x1a.vega.snapshot.v1.TopologyH\x00R\x08topology\x12\x44\n\x0boracle_data\x18% \x01(\x0b\x32!.vega.snapshot.v1.OracleDataBatchH\x00R\noracleData\x12Z\n\x14liquidity_parameters\x18& \x01(\x0b\x32%.vega.snapshot.v1.LiquidityParametersH\x00R\x13liquidityParameters\x12p\n\x1cliquidity_pending_provisions\x18\' \x01(\x0b\x32,.vega.snapshot.v1.LiquidityPendingProvisionsH\x00R\x1aliquidityPendingProvisions\x12\x80\x01\n"liquidity_parties_liquidity_orders\x18( \x01(\x0b\x32\x31.vega.snapshot.v1.LiquidityPartiesLiquidityOrdersH\x00R\x1fliquidityPartiesLiquidityOrders\x12\x64\n\x18liquidity_parties_orders\x18) \x01(\x0b\x32(.vega.snapshot.v1.LiquidityPartiesOrdersH\x00R\x16liquidityPartiesOrders\x12Z\n\x14liquidity_provisions\x18* \x01(\x0b\x32%.vega.snapshot.v1.LiquidityProvisionsH\x00R\x13liquidityProvisions\x12T\n\x12liquidity_supplied\x18+ \x01(\x0b\x32#.vega.snapshot.v1.LiquiditySuppliedH\x00R\x11liquiditySupplied\x12N\n\x10liquidity_target\x18, \x01(\x0b\x32!.vega.snapshot.v1.LiquidityTargetH\x00R\x0fliquidityTarget\x12\x64\n\x18\x66loating_point_consensus\x18. \x01(\x0b\x32(.vega.snapshot.v1.FloatingPointConsensusH\x00R\x16\x66loatingPointConsensus\x12H\n\x0emarket_tracker\x18/ \x01(\x0b\x32\x1f.vega.snapshot.v1.MarketTrackerH\x00R\rmarketTracker\x12m\n\x1b\x62\x61nking_recurring_transfers\x18\x31 \x01(\x0b\x32+.vega.snapshot.v1.BankingRecurringTransfersH\x00R\x19\x62\x61nkingRecurringTransfers\x12m\n\x1b\x62\x61nking_scheduled_transfers\x18\x32 \x01(\x0b\x32+.vega.snapshot.v1.BankingScheduledTransfersH\x00R\x19\x62\x61nkingScheduledTransfers\x12z\n erc20_multisig_topology_verified\x18\x33 \x01(\x0b\x32/.vega.snapshot.v1.ERC20MultiSigTopologyVerifiedH\x00R\x1d\x65rc20MultisigTopologyVerified\x12w\n\x1f\x65rc20_multisig_topology_pending\x18\x34 \x01(\x0b\x32..vega.snapshot.v1.ERC20MultiSigTopologyPendingH\x00R\x1c\x65rc20MultisigTopologyPending\x12\x43\n\rproof_of_work\x18\x35 \x01(\x0b\x32\x1d.vega.snapshot.v1.ProofOfWorkH\x00R\x0bproofOfWork\x12[\n\x15pending_asset_updates\x18\x36 \x01(\x0b\x32%.vega.snapshot.v1.PendingAssetUpdatesH\x00R\x13pendingAssetUpdates\x12j\n\x1aprotocol_upgrade_proposals\x18\x37 \x01(\x0b\x32*.vega.snapshot.v1.ProtocolUpgradeProposalsH\x00R\x18protocolUpgradeProposals\x12X\n\x14\x62\x61nking_bridge_state\x18\x38 \x01(\x0b\x32$.vega.snapshot.v1.BankingBridgeStateH\x00R\x12\x62\x61nkingBridgeState\x12N\n\x10settlement_state\x18\x39 \x01(\x0b\x32!.vega.snapshot.v1.SettlementStateH\x00R\x0fsettlementState\x12N\n\x10liquidity_scores\x18: \x01(\x0b\x32!.vega.snapshot.v1.LiquidityScoresH\x00R\x0fliquidityScores\x12[\n\x15spot_liquidity_target\x18; \x01(\x0b\x32%.vega.snapshot.v1.SpotLiquidityTargetH\x00R\x13spotLiquidityTarget\x12\x8c\x01\n&banking_recurring_governance_transfers\x18< \x01(\x0b\x32\x35.vega.snapshot.v1.BankingRecurringGovernanceTransfersH\x00R#bankingRecurringGovernanceTransfers\x12\x8c\x01\n&banking_scheduled_governance_transfers\x18= \x01(\x0b\x32\x35.vega.snapshot.v1.BankingScheduledGovernanceTransfersH\x00R#bankingScheduledGovernanceTransfersB\x06\n\x04\x64\x61ta"L\n\x15TimestampedTotalStake\x12\x1f\n\x0btotal_stake\x18\x01 \x01(\x04R\ntotalStake\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"R\n\x17TimestampedOpenInterest\x12#\n\ropen_interest\x18\x01 \x01(\x04R\x0copenInterest\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\xf2\x02\n\x0fLiquidityTarget\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12!\n\x0c\x63urrent_time\x18\x02 \x01(\x03R\x0b\x63urrentTime\x12-\n\x12scheduled_truncate\x18\x03 \x01(\x03R\x11scheduledTruncate\x12\x34\n\x16\x63urrent_open_interests\x18\x04 \x03(\x04R\x14\x63urrentOpenInterests\x12\x61\n\x17previous_open_interests\x18\x05 \x03(\x0b\x32).vega.snapshot.v1.TimestampedOpenInterestR\x15previousOpenInterests\x12W\n\x12max_open_interests\x18\x06 \x01(\x0b\x32).vega.snapshot.v1.TimestampedOpenInterestR\x10maxOpenInterests"\xe0\x02\n\x13SpotLiquidityTarget\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12!\n\x0c\x63urrent_time\x18\x02 \x01(\x03R\x0b\x63urrentTime\x12-\n\x12scheduled_truncate\x18\x03 \x01(\x03R\x11scheduledTruncate\x12.\n\x13\x63urrent_total_stake\x18\x04 \x03(\x04R\x11\x63urrentTotalStake\x12Y\n\x14previous_total_stake\x18\x05 \x03(\x0b\x32\'.vega.snapshot.v1.TimestampedTotalStakeR\x12previousTotalStake\x12O\n\x0fmax_total_stake\x18\x06 \x01(\x0b\x32\'.vega.snapshot.v1.TimestampedTotalStakeR\rmaxTotalStake"Z\n\x1eLiquidityOffsetProbabilityPair\x12\x16\n\x06offset\x18\x01 \x01(\rR\x06offset\x12 \n\x0bprobability\x18\x02 \x01(\tR\x0bprobability"\xfb\x01\n\x11LiquiditySupplied\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63onsensus_reached\x18\x02 \x01(\x08R\x10\x63onsensusReached\x12M\n\tbid_cache\x18\x03 \x03(\x0b\x32\x30.vega.snapshot.v1.LiquidityOffsetProbabilityPairR\x08\x62idCache\x12M\n\task_cache\x18\x04 \x03(\x0b\x32\x30.vega.snapshot.v1.LiquidityOffsetProbabilityPairR\x08\x61skCache"P\n\x0fOracleDataBatch\x12=\n\x0boracle_data\x18\x01 \x03(\x0b\x32\x1c.vega.snapshot.v1.OracleDataR\noracleData"r\n\nOracleData\x12.\n\x07signers\x18\x01 \x03(\x0b\x32\x14.vega.data.v1.SignerR\x07signers\x12\x34\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.OracleDataPairR\x04\x64\x61ta"8\n\x0eOracleDataPair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"C\n\x07Witness\x12\x38\n\tresources\x18\x01 \x03(\x0b\x32\x1a.vega.snapshot.v1.ResourceR\tresources"g\n\x08Resource\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x63heck_until\x18\x02 \x01(\x03R\ncheckUntil\x12\x14\n\x05votes\x18\x03 \x03(\tR\x05votes\x12\x14\n\x05state\x18\x04 \x01(\rR\x05state"3\n\x0e\x45ventForwarder\x12!\n\x0c\x61\x63ked_events\x18\x01 \x03(\tR\x0b\x61\x63kedEvents"?\n\x12\x43ollateralAccounts\x12)\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x08\x61\x63\x63ounts"7\n\x10\x43ollateralAssets\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"3\n\x0c\x41\x63tiveAssets\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"4\n\rPendingAssets\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets":\n\x13PendingAssetUpdates\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"P\n\nWithdrawal\x12\x10\n\x03ref\x18\x01 \x01(\tR\x03ref\x12\x30\n\nwithdrawal\x18\x02 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"B\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\'\n\x07\x64\x65posit\x18\x02 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"i\n\x05TxRef\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset\x12\x19\n\x08\x62lock_nr\x18\x02 \x01(\x04R\x07\x62lockNr\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1b\n\tlog_index\x18\x04 \x01(\x04R\x08logIndex"T\n\x12\x42\x61nkingWithdrawals\x12>\n\x0bwithdrawals\x18\x01 \x03(\x0b\x32\x1c.vega.snapshot.v1.WithdrawalR\x0bwithdrawals"F\n\x0f\x42\x61nkingDeposits\x12\x33\n\x07\x64\x65posit\x18\x01 \x03(\x0b\x32\x19.vega.snapshot.v1.DepositR\x07\x64\x65posit"P\n\x0b\x42\x61nkingSeen\x12\x12\n\x04refs\x18\x01 \x03(\tR\x04refs\x12-\n\x13last_seen_eth_block\x18\x02 \x01(\x04R\x10lastSeenEthBlock"Y\n\x13\x42\x61nkingAssetActions\x12\x42\n\x0c\x61sset_action\x18\x01 \x03(\x0b\x32\x1f.vega.checkpoint.v1.AssetActionR\x0b\x61ssetAction"t\n\x19\x42\x61nkingRecurringTransfers\x12W\n\x13recurring_transfers\x18\x01 \x01(\x0b\x32&.vega.checkpoint.v1.RecurringTransfersR\x12recurringTransfers"t\n\x19\x42\x61nkingScheduledTransfers\x12W\n\x11transfers_at_time\x18\x01 \x03(\x0b\x32+.vega.checkpoint.v1.ScheduledTransferAtTimeR\x0ftransfersAtTime"~\n#BankingRecurringGovernanceTransfers\x12W\n\x13recurring_transfers\x18\x01 \x03(\x0b\x32&.vega.checkpoint.v1.GovernanceTransferR\x12recurringTransfers"\x88\x01\n#BankingScheduledGovernanceTransfers\x12\x61\n\x11transfers_at_time\x18\x01 \x03(\x0b\x32\x35.vega.checkpoint.v1.ScheduledGovernanceTransferAtTimeR\x0ftransfersAtTime"X\n\x12\x42\x61nkingBridgeState\x12\x42\n\x0c\x62ridge_state\x18\x01 \x01(\x0b\x32\x1f.vega.checkpoint.v1.BridgeStateR\x0b\x62ridgeState"%\n\nCheckpoint\x12\x17\n\x07next_cp\x18\x01 \x01(\x03R\x06nextCp"\\\n DelegationLastReconciliationTime\x12\x38\n\x18last_reconciliation_time\x18\x01 \x01(\x03R\x16lastReconciliationTime"F\n\x10\x44\x65legationActive\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"}\n\x11\x44\x65legationPending\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0cundelegation\x18\x02 \x03(\x0b\x32\x10.vega.DelegationR\x0cundelegation"*\n\x0e\x44\x65legationAuto\x12\x18\n\x07parties\x18\x01 \x03(\tR\x07parties"\x9a\x01\n\x0cProposalData\x12*\n\x08proposal\x18\x01 \x01(\x0b\x32\x0e.vega.ProposalR\x08proposal\x12\x1c\n\x03yes\x18\x02 \x03(\x0b\x32\n.vega.VoteR\x03yes\x12\x1a\n\x02no\x18\x03 \x03(\x0b\x32\n.vega.VoteR\x02no\x12$\n\x07invalid\x18\x04 \x03(\x0b\x32\n.vega.VoteR\x07invalid"Q\n\x11GovernanceEnacted\x12<\n\tproposals\x18\x01 \x03(\x0b\x32\x1e.vega.snapshot.v1.ProposalDataR\tproposals"P\n\x10GovernanceActive\x12<\n\tproposals\x18\x01 \x03(\x0b\x32\x1e.vega.snapshot.v1.ProposalDataR\tproposals">\n\x0eGovernanceNode\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"v\n\x0eStakingAccount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x34\n\x06\x65vents\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x06\x65vents"\xe1\x01\n\x0fStakingAccounts\x12<\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32 .vega.snapshot.v1.StakingAccountR\x08\x61\x63\x63ounts\x12;\n\x1astaking_asset_total_supply\x18\x02 \x01(\tR\x17stakingAssetTotalSupply\x12S\n\x1apending_stake_total_supply\x18\x03 \x01(\x0b\x32\x16.vega.StakeTotalSupplyR\x17pendingStakeTotalSupply"\xcc\x01\n\x0cMatchingBook\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1d\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x03\x62uy\x12\x1f\n\x04sell\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x04sell\x12*\n\x11last_traded_price\x18\x04 \x01(\tR\x0flastTradedPrice\x12\x18\n\x07\x61uction\x18\x05 \x01(\x08R\x07\x61uction\x12\x19\n\x08\x62\x61tch_id\x18\x06 \x01(\x04R\x07\x62\x61tchId";\n\tNetParams\x12.\n\x06params\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x06params"0\n\nDecimalMap\x12\x10\n\x03key\x18\x01 \x01(\x03R\x03key\x12\x10\n\x03val\x18\x02 \x01(\tR\x03val"5\n\tTimePrice\x12\x12\n\x04time\x18\x01 \x01(\x03R\x04time\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price";\n\x0bPriceVolume\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"B\n\nPriceRange\x12\x10\n\x03min\x18\x01 \x01(\tR\x03min\x12\x10\n\x03max\x18\x02 \x01(\tR\x03max\x12\x10\n\x03ref\x18\x03 \x01(\tR\x03ref"\x9a\x01\n\nPriceBound\x12\x16\n\x06\x61\x63tive\x18\x01 \x01(\x08R\x06\x61\x63tive\x12\x1b\n\tup_factor\x18\x02 \x01(\tR\x08upFactor\x12\x1f\n\x0b\x64own_factor\x18\x03 \x01(\tR\ndownFactor\x12\x36\n\x07trigger\x18\x04 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger"y\n\x0fPriceRangeCache\x12\x32\n\x05\x62ound\x18\x01 \x01(\x0b\x32\x1c.vega.snapshot.v1.PriceBoundR\x05\x62ound\x12\x32\n\x05range\x18\x02 \x01(\x0b\x32\x1c.vega.snapshot.v1.PriceRangeR\x05range"<\n\x0c\x43urrentPrice\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"S\n\tPastPrice\x12\x12\n\x04time\x18\x01 \x01(\x03R\x04time\x12\x32\n\x15volume_weighted_price\x18\x02 \x01(\tR\x13volumeWeightedPrice"\xf4\x04\n\x0cPriceMonitor\x12 \n\x0binitialised\x18\x03 \x01(\x08R\x0binitialised\x12=\n\x0b\x66p_horizons\x18\x04 \x03(\x0b\x32\x1c.vega.snapshot.v1.DecimalMapR\nfpHorizons\x12\x10\n\x03now\x18\x05 \x01(\x03R\x03now\x12\x16\n\x06update\x18\x06 \x01(\x03R\x06update\x12\x34\n\x06\x62ounds\x18\x07 \x03(\x0b\x32\x1c.vega.snapshot.v1.PriceBoundR\x06\x62ounds\x12\x33\n\x16price_range_cache_time\x18\x08 \x01(\x03R\x13priceRangeCacheTime\x12M\n\x11price_range_cache\x18\t \x03(\x0b\x32!.vega.snapshot.v1.PriceRangeCacheR\x0fpriceRangeCache\x12/\n\x14ref_price_cache_time\x18\n \x01(\x03R\x11refPriceCacheTime\x12\x44\n\x0fref_price_cache\x18\x0b \x03(\x0b\x32\x1c.vega.snapshot.v1.DecimalMapR\rrefPriceCache\x12=\n\nprices_now\x18\x0c \x03(\x0b\x32\x1e.vega.snapshot.v1.CurrentPriceR\tpricesNow\x12<\n\x0bprices_past\x18\r \x03(\x0b\x32\x1b.vega.snapshot.v1.PastPriceR\npricesPast\x12+\n\x11\x63onsensus_reached\x18\x0e \x01(\x08R\x10\x63onsensusReached"\xf8\x02\n\x0c\x41uctionState\x12,\n\x04mode\x18\x01 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x04mode\x12;\n\x0c\x64\x65\x66\x61ult_mode\x18\x02 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x0b\x64\x65\x66\x61ultMode\x12.\n\x07trigger\x18\x03 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x14\n\x05\x62\x65gin\x18\x04 \x01(\x03R\x05\x62\x65gin\x12\'\n\x03\x65nd\x18\x05 \x01(\x0b\x32\x15.vega.AuctionDurationR\x03\x65nd\x12\x14\n\x05start\x18\x06 \x01(\x08R\x05start\x12\x12\n\x04stop\x18\x07 \x01(\x08R\x04stop\x12\x32\n\textension\x18\x08 \x01(\x0e\x32\x14.vega.AuctionTriggerR\textension\x12\x30\n\x14\x65xtension_event_sent\x18\t \x01(\x08R\x12\x65xtensionEventSent"u\n\rEquityShareLP\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05stake\x18\x02 \x01(\tR\x05stake\x12\x14\n\x05share\x18\x03 \x01(\tR\x05share\x12\x10\n\x03\x61vg\x18\x04 \x01(\tR\x03\x61vg\x12\x16\n\x06vshare\x18\x05 \x01(\tR\x06vshare"\xa9\x01\n\x0b\x45quityShare\x12\x10\n\x03mvp\x18\x01 \x01(\tR\x03mvp\x12\x32\n\x15opening_auction_ended\x18\x02 \x01(\x08R\x13openingAuctionEnded\x12\x31\n\x03lps\x18\x03 \x03(\x0b\x32\x1f.vega.snapshot.v1.EquityShareLPR\x03lps\x12\x0c\n\x01r\x18\x04 \x01(\tR\x01r\x12\x13\n\x05p_mvp\x18\x05 \x01(\tR\x04pMvp"\x84\x01\n\x0b\x46\x65\x65Splitter\x12*\n\x11time_window_start\x18\x01 \x01(\x03R\x0ftimeWindowStart\x12\x1f\n\x0btrade_value\x18\x02 \x01(\tR\ntradeValue\x12\x10\n\x03\x61vg\x18\x03 \x01(\tR\x03\x61vg\x12\x16\n\x06window\x18\x04 \x01(\x04R\x06window"\xfc\x06\n\nSpotMarket\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x43\n\rprice_monitor\x18\x02 \x01(\x0b\x32\x1e.vega.snapshot.v1.PriceMonitorR\x0cpriceMonitor\x12\x43\n\rauction_state\x18\x03 \x01(\x0b\x32\x1e.vega.snapshot.v1.AuctionStateR\x0c\x61uctionState\x12\x43\n\rpegged_orders\x18\x04 \x01(\x0b\x32\x1e.vega.snapshot.v1.PeggedOrdersR\x0cpeggedOrders\x12\x34\n\x0f\x65xpiring_orders\x18\x05 \x03(\x0b\x32\x0b.vega.OrderR\x0e\x65xpiringOrders\x12"\n\rlast_best_bid\x18\x06 \x01(\tR\x0blastBestBid\x12"\n\rlast_best_ask\x18\x07 \x01(\tR\x0blastBestAsk\x12 \n\x0clast_mid_bid\x18\x08 \x01(\tR\nlastMidBid\x12 \n\x0clast_mid_ask\x18\t \x01(\tR\nlastMidAsk\x12\x35\n\x17last_market_value_proxy\x18\n \x01(\tR\x14lastMarketValueProxy\x12\x41\n\x1dlast_equity_share_distributed\x18\x0b \x01(\x03R\x1alastEquityShareDistributed\x12@\n\x0c\x65quity_share\x18\x0c \x01(\x0b\x32\x1d.vega.snapshot.v1.EquityShareR\x0b\x65quityShare\x12,\n\x12\x63urrent_mark_price\x18\r \x01(\tR\x10\x63urrentMarkPrice\x12@\n\x0c\x66\x65\x65_splitter\x18\x0e \x01(\x0b\x32\x1d.vega.snapshot.v1.FeeSplitterR\x0b\x66\x65\x65Splitter\x12-\n\x13next_mark_to_market\x18\x0f \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x10 \x01(\tR\x0flastTradedPrice\x12\x18\n\x07parties\x18\x11 \x03(\tR\x07parties\x12\x16\n\x06\x63losed\x18\x12 \x01(\x08R\x06\x63losed"\xd6\t\n\x06Market\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x43\n\rprice_monitor\x18\x02 \x01(\x0b\x32\x1e.vega.snapshot.v1.PriceMonitorR\x0cpriceMonitor\x12\x43\n\rauction_state\x18\x03 \x01(\x0b\x32\x1e.vega.snapshot.v1.AuctionStateR\x0c\x61uctionState\x12\x43\n\rpegged_orders\x18\x04 \x01(\x0b\x32\x1e.vega.snapshot.v1.PeggedOrdersR\x0cpeggedOrders\x12\x34\n\x0f\x65xpiring_orders\x18\x05 \x03(\x0b\x32\x0b.vega.OrderR\x0e\x65xpiringOrders\x12"\n\rlast_best_bid\x18\x06 \x01(\tR\x0blastBestBid\x12"\n\rlast_best_ask\x18\x07 \x01(\tR\x0blastBestAsk\x12 \n\x0clast_mid_bid\x18\x08 \x01(\tR\nlastMidBid\x12 \n\x0clast_mid_ask\x18\t \x01(\tR\nlastMidAsk\x12\x35\n\x17last_market_value_proxy\x18\n \x01(\tR\x14lastMarketValueProxy\x12\x41\n\x1dlast_equity_share_distributed\x18\x0b \x01(\x03R\x1alastEquityShareDistributed\x12@\n\x0c\x65quity_share\x18\x0c \x01(\x0b\x32\x1d.vega.snapshot.v1.EquityShareR\x0b\x65quityShare\x12,\n\x12\x63urrent_mark_price\x18\r \x01(\tR\x10\x63urrentMarkPrice\x12*\n\x11risk_factor_short\x18\x0e \x01(\tR\x0friskFactorShort\x12(\n\x10risk_factor_long\x18\x0f \x01(\tR\x0eriskFactorLong\x12\x41\n\x1drisk_factor_consensus_reached\x18\x10 \x01(\x08R\x1ariskFactorConsensusReached\x12@\n\x0c\x66\x65\x65_splitter\x18\x11 \x01(\x0b\x32\x1d.vega.snapshot.v1.FeeSplitterR\x0b\x66\x65\x65Splitter\x12\'\n\x0fsettlement_data\x18\x12 \x01(\tR\x0esettlementData\x12-\n\x13next_mark_to_market\x18\x13 \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x14 \x01(\tR\x0flastTradedPrice\x12\x18\n\x07parties\x18\x15 \x03(\tR\x07parties\x12\x16\n\x06\x63losed\x18\x16 \x01(\x08R\x06\x63losed\x12\x1c\n\tsucceeded\x18\x17 \x01(\x08R\tsucceeded\x12=\n\x0bstop_orders\x18\x18 \x01(\x0b\x32\x1c.vega.snapshot.v1.StopOrdersR\nstopOrders\x12=\n\x14\x65xpiring_stop_orders\x18\x19 \x03(\x0b\x32\x0b.vega.OrderR\x12\x65xpiringStopOrders"=\n\rOrdersAtPrice\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12\x16\n\x06orders\x18\x02 \x03(\tR\x06orders"\x98\x01\n\x10PricedStopOrders\x12\x42\n\x0c\x66\x61lls_bellow\x18\x01 \x03(\x0b\x32\x1f.vega.snapshot.v1.OrdersAtPriceR\x0b\x66\x61llsBellow\x12@\n\x0brises_above\x18\x02 \x03(\x0b\x32\x1f.vega.snapshot.v1.OrdersAtPriceR\nrisesAbove"\xc4\x01\n\x12TrailingStopOrders\x12&\n\x0flast_seen_price\x18\x01 \x01(\tR\rlastSeenPrice\x12\x43\n\x0c\x66\x61lls_bellow\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.OffsetsAtPriceR\x0b\x66\x61llsBellow\x12\x41\n\x0brises_above\x18\x03 \x03(\x0b\x32 .vega.snapshot.v1.OffsetsAtPriceR\nrisesAbove"@\n\x0eOrdersAtOffset\x12\x16\n\x06offset\x18\x01 \x01(\tR\x06offset\x12\x16\n\x06orders\x18\x02 \x03(\tR\x06orders"b\n\x0eOffsetsAtPrice\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12:\n\x07offsets\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.OrdersAtOffsetR\x07offsets"\xf7\x01\n\nStopOrders\x12?\n\x0bstop_orders\x18\x01 \x03(\x0b\x32\x1e.vega.events.v1.StopOrderEventR\nstopOrders\x12P\n\x12priced_stop_orders\x18\x02 \x01(\x0b\x32".vega.snapshot.v1.PricedStopOrdersR\x10pricedStopOrders\x12V\n\x14trailing_stop_orders\x18\x03 \x01(\x0b\x32$.vega.snapshot.v1.TrailingStopOrdersR\x12trailingStopOrders"@\n\x0cPeggedOrders\x12\x30\n\rparked_orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x0cparkedOrders"\x8f\x02\n\x10\x45xecutionMarkets\x12\x32\n\x07markets\x18\x01 \x03(\x0b\x32\x18.vega.snapshot.v1.MarketR\x07markets\x12?\n\x0cspot_markets\x18\x02 \x03(\x0b\x32\x1c.vega.snapshot.v1.SpotMarketR\x0bspotMarkets\x12H\n\x0fsettled_markets\x18\x03 \x03(\x0b\x32\x1f.vega.checkpoint.v1.MarketStateR\x0esettledMarkets\x12<\n\nsuccessors\x18\x04 \x03(\x0b\x32\x1c.vega.snapshot.v1.SuccessorsR\nsuccessors"^\n\nSuccessors\x12#\n\rparent_market\x18\x01 \x01(\tR\x0cparentMarket\x12+\n\x11successor_markets\x18\x02 \x03(\tR\x10successorMarkets"\xe7\x01\n\x08Position\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x12\n\x04size\x18\x02 \x01(\x03R\x04size\x12\x10\n\x03\x62uy\x18\x03 \x01(\x03R\x03\x62uy\x12\x12\n\x04sell\x18\x04 \x01(\x03R\x04sell\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12&\n\x0f\x62uy_sum_product\x18\x06 \x01(\tR\rbuySumProduct\x12(\n\x10sell_sum_product\x18\x07 \x01(\tR\x0esellSumProduct\x12\x1e\n\ndistressed\x18\x08 \x01(\x08R\ndistressed"h\n\x0fMarketPositions\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x38\n\tpositions\x18\x02 \x03(\x0b\x32\x1a.vega.snapshot.v1.PositionR\tpositions"\xee\x01\n\x0fSettlementState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12&\n\x0flast_mark_price\x18\x02 \x01(\tR\rlastMarkPrice\x12[\n\x16last_settled_positions\x18\x03 \x03(\x0b\x32%.vega.snapshot.v1.LastSettledPositionR\x14lastSettledPositions\x12\x39\n\x06trades\x18\x04 \x03(\x0b\x32!.vega.snapshot.v1.SettlementTradeR\x06trades"V\n\x13LastSettledPosition\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12)\n\x10settled_position\x18\x02 \x01(\x03R\x0fsettledPosition"\x94\x01\n\x0fSettlementTrade\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice\x12\x12\n\x04size\x18\x04 \x01(\x03R\x04size\x12\x19\n\x08new_size\x18\x05 \x01(\x03R\x07newSize"g\n\x08\x41ppState\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x12\n\x04time\x18\x03 \x01(\x03R\x04time\x12\x19\n\x08\x63hain_id\x18\x04 \x01(\tR\x07\x63hainId"\xc3\x01\n\nEpochState\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x36\n\x18ready_to_start_new_epoch\x18\x06 \x01(\x08R\x14readyToStartNewEpoch\x12+\n\x12ready_to_end_epoch\x18\x07 \x01(\x08R\x0freadyToEndEpoch"{\n\x15RewardsPendingPayouts\x12\x62\n\x18scheduled_rewards_payout\x18\x01 \x03(\x0b\x32(.vega.snapshot.v1.ScheduledRewardsPayoutR\x16scheduledRewardsPayout"\x81\x01\n\x16ScheduledRewardsPayout\x12\x1f\n\x0bpayout_time\x18\x01 \x01(\x03R\npayoutTime\x12\x46\n\x0erewards_payout\x18\x02 \x03(\x0b\x32\x1f.vega.snapshot.v1.RewardsPayoutR\rrewardsPayout"\xfc\x01\n\rRewardsPayout\x12!\n\x0c\x66rom_account\x18\x01 \x01(\tR\x0b\x66romAccount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12T\n\x13reward_party_amount\x18\x03 \x03(\x0b\x32$.vega.snapshot.v1.RewardsPartyAmountR\x11rewardPartyAmount\x12!\n\x0ctotal_reward\x18\x04 \x01(\tR\x0btotalReward\x12\x1b\n\tepoch_seq\x18\x05 \x01(\tR\x08\x65pochSeq\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp"B\n\x12RewardsPartyAmount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\x94\x03\n\nLimitState\x12\x1f\n\x0b\x62lock_count\x18\x01 \x01(\rR\nblockCount\x12,\n\x12\x63\x61n_propose_market\x18\x02 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x03 \x01(\x08R\x0f\x63\x61nProposeAsset\x12%\n\x0egenesis_loaded\x18\x04 \x01(\x08R\rgenesisLoaded\x12\x34\n\x16propose_market_enabled\x18\x05 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x06 \x01(\x08R\x13proposeAssetEnabled\x12=\n\x1bpropose_market_enabled_from\x18\x07 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\x08 \x01(\x03R\x17proposeAssetEnabledFrom"\x94\x04\n\x0eVoteSpamPolicy\x12L\n\rparty_to_vote\x18\x01 \x03(\x0b\x32(.vega.snapshot.v1.PartyProposalVoteCountR\x0bpartyToVote\x12\x44\n\x0e\x62\x61nned_parties\x18\x02 \x03(\x0b\x32\x1d.vega.snapshot.v1.BannedPartyR\rbannedParties\x12H\n\rtoken_balance\x18\x03 \x03(\x0b\x32#.vega.snapshot.v1.PartyTokenBalanceR\x0ctokenBalance\x12_\n\x1arecent_blocks_reject_stats\x18\x04 \x03(\x0b\x32".vega.snapshot.v1.BlockRejectStatsR\x17recentBlocksRejectStats\x12.\n\x13\x63urrent_block_index\x18\x05 \x01(\x04R\x11\x63urrentBlockIndex\x12.\n\x13last_increase_block\x18\x06 \x01(\x04R\x11lastIncreaseBlock\x12*\n\x11\x63urrent_epoch_seq\x18\x07 \x01(\x04R\x0f\x63urrentEpochSeq\x12\x37\n\x18min_voting_tokens_factor\x18\x08 \x01(\tR\x15minVotingTokensFactor"`\n\x16PartyProposalVoteCount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1a\n\x08proposal\x18\x02 \x01(\tR\x08proposal\x12\x14\n\x05\x63ount\x18\x03 \x01(\x04R\x05\x63ount"C\n\x11PartyTokenBalance\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"D\n\x10\x42lockRejectStats\x12\x1a\n\x08rejected\x18\x01 \x01(\x04R\x08rejected\x12\x14\n\x05total\x18\x02 \x01(\x04R\x05total"G\n\x19SpamPartyTransactionCount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x14\n\x05\x63ount\x18\x02 \x01(\x04R\x05\x63ount"\xc2\x02\n\x10SimpleSpamPolicy\x12\x1f\n\x0bpolicy_name\x18\x01 \x01(\tR\npolicyName\x12Q\n\x0eparty_to_count\x18\x02 \x03(\x0b\x32+.vega.snapshot.v1.SpamPartyTransactionCountR\x0cpartyToCount\x12\x44\n\x0e\x62\x61nned_parties\x18\x03 \x03(\x0b\x32\x1d.vega.snapshot.v1.BannedPartyR\rbannedParties\x12H\n\rtoken_balance\x18\x04 \x03(\x0b\x32#.vega.snapshot.v1.PartyTokenBalanceR\x0ctokenBalance\x12*\n\x11\x63urrent_epoch_seq\x18\x05 \x01(\x04R\x0f\x63urrentEpochSeq"p\n\nNotarySigs\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04kind\x18\x02 \x01(\x05R\x04kind\x12\x12\n\x04node\x18\x03 \x01(\tR\x04node\x12\x10\n\x03sig\x18\x04 \x01(\tR\x03sig\x12\x18\n\x07pending\x18\x05 \x01(\x08R\x07pending"G\n\x06Notary\x12=\n\x0bnotary_sigs\x18\x01 \x03(\x0b\x32\x1c.vega.snapshot.v1.NotarySigsR\nnotarySigs"m\n\x16StakeVerifierDeposited\x12S\n\x11pending_deposited\x18\x01 \x03(\x0b\x32&.vega.snapshot.v1.StakeVerifierPendingR\x10pendingDeposited"g\n\x14StakeVerifierRemoved\x12O\n\x0fpending_removed\x18\x01 \x03(\x0b\x32&.vega.snapshot.v1.StakeVerifierPendingR\x0ependingRemoved"\x85\x02\n\x14StakeVerifierPending\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12!\n\x0c\x62lock_number\x18\x05 \x01(\x04R\x0b\x62lockNumber\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12\x13\n\x05tx_id\x18\x07 \x01(\tR\x04txId\x12\x0e\n\x02id\x18\x08 \x01(\tR\x02id"\x9b\x01\n\x12PendingKeyRotation\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12)\n\x11new_pub_key_index\x18\x04 \x01(\rR\x0enewPubKeyIndex"\xb8\x01\n\x1aPendingEthereumKeyRotation\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x1f\n\x0bold_address\x18\x05 \x01(\tR\noldAddress"\xdd\x04\n\x08Topology\x12G\n\x0evalidator_data\x18\x01 \x03(\x0b\x32 .vega.snapshot.v1.ValidatorStateR\rvalidatorData\x12\x1d\n\nchain_keys\x18\x02 \x03(\tR\tchainKeys\x12_\n\x19pending_pub_key_rotations\x18\x03 \x03(\x0b\x32$.vega.snapshot.v1.PendingKeyRotationR\x16pendingPubKeyRotations\x12[\n\x15validator_performance\x18\x04 \x01(\x0b\x32&.vega.snapshot.v1.ValidatorPerformanceR\x14validatorPerformance\x12q\n\x1epending_ethereum_key_rotations\x18\x05 \x03(\x0b\x32,.vega.snapshot.v1.PendingEthereumKeyRotationR\x1bpendingEthereumKeyRotations\x12\x43\n\nsignatures\x18\x06 \x01(\x0b\x32#.vega.snapshot.v1.ToplogySignaturesR\nsignatures\x12s\n\x1funsolved_ethereum_key_rotations\x18\x07 \x03(\x0b\x32,.vega.snapshot.v1.PendingEthereumKeyRotationR\x1cunsolvedEthereumKeyRotations"\xde\x01\n\x11ToplogySignatures\x12\x65\n\x12pending_signatures\x18\x01 \x03(\x0b\x32\x36.vega.snapshot.v1.PendingERC20MultisigControlSignatureR\x11pendingSignatures\x12\x62\n\x11issued_signatures\x18\x02 \x03(\x0b\x32\x35.vega.snapshot.v1.IssuedERC20MultisigControlSignatureR\x10issuedSignatures"\xb3\x01\n$PendingERC20MultisigControlSignature\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x04 \x01(\x04R\x08\x65pochSeq\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\x05 \x01(\x08R\x05\x61\x64\x64\x65\x64"\x9e\x01\n#IssuedERC20MultisigControlSignature\x12\x1f\n\x0bresource_id\x18\x01 \x01(\tR\nresourceId\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12+\n\x11submitter_address\x18\x03 \x01(\tR\x10submitterAddress"\xf2\x03\n\x0eValidatorState\x12J\n\x10validator_update\x18\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\x0fvalidatorUpdate\x12\x1f\n\x0b\x62lock_added\x18\x02 \x01(\x04R\nblockAdded\x12\x16\n\x06status\x18\x03 \x01(\x05R\x06status\x12.\n\x13status_change_block\x18\x04 \x01(\x04R\x11statusChangeBlock\x12\x46\n last_block_with_positive_ranking\x18\x05 \x01(\x04R\x1clastBlockWithPositiveRanking\x12\x30\n\x14\x65th_events_forwarded\x18\x06 \x01(\x04R\x12\x65thEventsForwarded\x12O\n\x11heartbeat_tracker\x18\x07 \x01(\x0b\x32".vega.snapshot.v1.HeartbeatTrackerR\x10heartbeatTracker\x12\'\n\x0fvalidator_power\x18\x08 \x01(\x03R\x0evalidatorPower\x12\x37\n\rranking_score\x18\t \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore"\xb9\x01\n\x10HeartbeatTracker\x12,\n\x12\x65xpected_next_hash\x18\x01 \x01(\tR\x10\x65xpectedNextHash\x12\x37\n\x18\x65xpected_next_hash_since\x18\x02 \x01(\x03R\x15\x65xpectedNextHashSince\x12\x1f\n\x0b\x62lock_index\x18\x03 \x01(\x05R\nblockIndex\x12\x1d\n\nblock_sigs\x18\x04 \x03(\x08R\tblockSigs"\x99\x02\n\x10PerformanceStats\x12+\n\x11validator_address\x18\x01 \x01(\tR\x10validatorAddress\x12\x1a\n\x08proposed\x18\x02 \x01(\x04R\x08proposed\x12\x18\n\x07\x65lected\x18\x03 \x01(\x04R\x07\x65lected\x12\x14\n\x05voted\x18\x04 \x01(\x04R\x05voted\x12*\n\x11last_height_voted\x18\x05 \x01(\x03R\x0flastHeightVoted\x12\x30\n\x14last_height_proposed\x18\x06 \x01(\x03R\x12lastHeightProposed\x12.\n\x13last_height_elected\x18\x07 \x01(\x03R\x11lastHeightElected"l\n\x14ValidatorPerformance\x12T\n\x14validator_perf_stats\x18\x01 \x03(\x0b\x32".vega.snapshot.v1.PerformanceStatsR\x12validatorPerfStats"\xae\x01\n\x13LiquidityParameters\x12\x17\n\x07max_fee\x18\x01 \x01(\tR\x06maxFee\x12$\n\x0emax_shape_size\x18\x02 \x01(\tR\x0cmaxShapeSize\x12;\n\x1astake_to_obligation_factor\x18\x03 \x01(\tR\x17stakeToObligationFactor\x12\x1b\n\tmarket_id\x18\x04 \x01(\tR\x08marketId"h\n\x1aLiquidityPendingProvisions\x12-\n\x12pending_provisions\x18\x01 \x03(\tR\x11pendingProvisions\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\x80\x01\n\x1fLiquidityPartiesLiquidityOrders\x12@\n\x0cparty_orders\x18\x01 \x03(\x0b\x32\x1d.vega.snapshot.v1.PartyOrdersR\x0bpartyOrders\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"H\n\x0bPartyOrders\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12#\n\x06orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"w\n\x16LiquidityPartiesOrders\x12@\n\x0cparty_orders\x18\x01 \x03(\x0b\x32\x1d.vega.snapshot.v1.PartyOrdersR\x0bpartyOrders\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\x7f\n\x13LiquidityProvisions\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\xa0\x01\n\x0fLiquidityScores\x12\x36\n\x17running_average_counter\x18\x01 \x01(\x05R\x15runningAverageCounter\x12\x38\n\x06scores\x18\x02 \x03(\x0b\x32 .vega.snapshot.v1.LiquidityScoreR\x06scores\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId"A\n\x0eLiquidityScore\x12\x14\n\x05score\x18\x01 \x01(\tR\x05score\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId"\xb9\x01\n\x16\x46loatingPointConsensus\x12M\n\x11next_time_trigger\x18\x01 \x03(\x0b\x32!.vega.snapshot.v1.NextTimeTriggerR\x0fnextTimeTrigger\x12P\n\x0fstate_variables\x18\x02 \x03(\x0b\x32\'.vega.snapshot.v1.StateVarInternalStateR\x0estateVariables"\xfc\x01\n\x15StateVarInternalState\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05state\x18\x02 \x01(\x05R\x05state\x12\x19\n\x08\x65vent_id\x18\x03 \x01(\tR\x07\x65ventId\x12]\n\x12validators_results\x18\x04 \x03(\x0b\x32..vega.snapshot.v1.FloatingPointValidatorResultR\x11validatorsResults\x12\x43\n\x1erounds_since_meaningful_update\x18\x05 \x01(\x05R\x1broundsSinceMeaningfulUpdate"\\\n\x1c\x46loatingPointValidatorResult\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06\x62undle\x18\x02 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x06\x62undle"r\n\x0fNextTimeTrigger\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x0e\n\x02id\x18\x03 \x01(\tR\x02id\x12!\n\x0cnext_trigger\x18\x04 \x01(\x03R\x0bnextTrigger"c\n\rMarketTracker\x12R\n\x0fmarket_activity\x18\x01 \x03(\x0b\x32).vega.checkpoint.v1.MarketActivityTrackerR\x0emarketActivity"t\n\x16SignerEventsPerAddress\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12@\n\x06\x65vents\x18\x02 \x03(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventR\x06\x65vents"\x80\x02\n\x1d\x45RC20MultiSigTopologyVerified\x12\x18\n\x07signers\x18\x01 \x03(\tR\x07signers\x12V\n\x12\x65vents_per_address\x18\x02 \x03(\x0b\x32(.vega.snapshot.v1.SignerEventsPerAddressR\x10\x65ventsPerAddress\x12L\n\tthreshold\x18\x03 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventR\tthreshold\x12\x1f\n\x0bseen_events\x18\x04 \x03(\tR\nseenEvents"\xbc\x02\n\x1c\x45RC20MultiSigTopologyPending\x12Q\n\x0fpending_signers\x18\x01 \x03(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventR\x0ependingSigners\x12\x62\n\x15pending_threshold_set\x18\x02 \x03(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventR\x13pendingThresholdSet\x12+\n\x11witnessed_signers\x18\x03 \x03(\tR\x10witnessedSigners\x12\x38\n\x18witnessed_threshold_sets\x18\x04 \x03(\tR\x16witnessedThresholdSets"\xa1\x03\n\x0bProofOfWork\x12!\n\x0c\x62lock_height\x18\x01 \x03(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x03(\tR\tblockHash\x12H\n\x0ctx_at_height\x18\x04 \x03(\x0b\x32&.vega.snapshot.v1.TransactionsAtHeightR\ntxAtHeight\x12J\n\rtid_at_height\x18\x06 \x03(\x0b\x32&.vega.snapshot.v1.TransactionsAtHeightR\x0btidAtHeight\x12\x35\n\x06\x62\x61nned\x18\x07 \x03(\x0b\x32\x1d.vega.snapshot.v1.BannedPartyR\x06\x62\x61nned\x12\x42\n\npow_params\x18\x08 \x03(\x0b\x32#.vega.snapshot.v1.ProofOfWorkParamsR\tpowParams\x12?\n\tpow_state\x18\t \x03(\x0b\x32".vega.snapshot.v1.ProofOfWorkStateR\x08powState"9\n\x0b\x42\x61nnedParty\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x14\n\x05until\x18\x02 \x01(\x03R\x05until"\x84\x03\n\x11ProofOfWorkParams\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x01 \x01(\x04R\x19spamPowNumberOfPastBlocks\x12.\n\x13spam_pow_difficulty\x18\x02 \x01(\rR\x11spamPowDifficulty\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x04 \x01(\x04R\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x05 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x1d\n\nfrom_block\x18\x06 \x01(\x04R\tfromBlock\x12\x1f\n\x0buntil_block\x18\x07 \x01(\x03R\nuntilBlock"X\n\x10ProofOfWorkState\x12\x44\n\tpow_state\x18\x01 \x03(\x0b\x32\'.vega.snapshot.v1.ProofOfWorkBlockStateR\x08powState"\x8c\x01\n\x15ProofOfWorkBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12P\n\x0bparty_state\x18\x02 \x03(\x0b\x32/.vega.snapshot.v1.ProofOfWorkPartyStateForBlockR\npartyState"\x85\x01\n\x1dProofOfWorkPartyStateForBlock\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1d\n\nseen_count\x18\x02 \x01(\x04R\tseenCount\x12/\n\x13observed_difficulty\x18\x03 \x01(\x04R\x12observedDifficulty"R\n\x14TransactionsAtHeight\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12"\n\x0ctransactions\x18\x02 \x03(\tR\x0ctransactions"\xcb\x01\n\x18ProtocolUpgradeProposals\x12O\n\x10\x61\x63tive_proposals\x18\x01 \x03(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x0f\x61\x63tiveProposals\x12^\n\x11\x61\x63\x63\x65pted_proposal\x18\x02 \x01(\x0b\x32\x31.vega.snapshot.v1.AcceptedProtocolUpgradeProposalR\x10\x61\x63\x63\x65ptedProposal"}\n\x1f\x41\x63\x63\x65ptedProtocolUpgradeProposal\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag*`\n\x06\x46ormat\x12\x16\n\x12\x46ORMAT_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x46ORMAT_PROTO\x10\x01\x12\x1b\n\x17\x46ORMAT_PROTO_COMPRESSED\x10\x02\x12\x0f\n\x0b\x46ORMAT_JSON\x10\x03\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/snapshot/v1b\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.snapshot.v1.snapshot_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/snapshot/v1"
     )
-    _globals["_FORMAT"]._serialized_start = 26165
-    _globals["_FORMAT"]._serialized_end = 26261
+    _globals["_FORMAT"]._serialized_start = 26386
+    _globals["_FORMAT"]._serialized_end = 26482
     _globals["_SNAPSHOT"]._serialized_start = 249
     _globals["_SNAPSHOT"]._serialized_end = 405
     _globals["_NODEHASH"]._serialized_start = 407
     _globals["_NODEHASH"]._serialized_end = 530
     _globals["_METADATA"]._serialized_start = 533
     _globals["_METADATA"]._serialized_end = 665
     _globals["_CHUNK"]._serialized_start = 667
@@ -159,141 +159,143 @@
     _globals["_EQUITYSHARE"]._serialized_start = 12050
     _globals["_EQUITYSHARE"]._serialized_end = 12219
     _globals["_FEESPLITTER"]._serialized_start = 12222
     _globals["_FEESPLITTER"]._serialized_end = 12354
     _globals["_SPOTMARKET"]._serialized_start = 12357
     _globals["_SPOTMARKET"]._serialized_end = 13249
     _globals["_MARKET"]._serialized_start = 13252
-    _globals["_MARKET"]._serialized_end = 14427
-    _globals["_ORDERSATPRICE"]._serialized_start = 14429
-    _globals["_ORDERSATPRICE"]._serialized_end = 14490
-    _globals["_PRICEDSTOPORDERS"]._serialized_start = 14493
-    _globals["_PRICEDSTOPORDERS"]._serialized_end = 14645
-    _globals["_TRAILINGSTOPORDERS"]._serialized_start = 14648
-    _globals["_TRAILINGSTOPORDERS"]._serialized_end = 14844
-    _globals["_ORDERSATOFFSET"]._serialized_start = 14846
-    _globals["_ORDERSATOFFSET"]._serialized_end = 14910
-    _globals["_OFFSETSATPRICE"]._serialized_start = 14912
-    _globals["_OFFSETSATPRICE"]._serialized_end = 15010
-    _globals["_STOPORDERS"]._serialized_start = 15013
-    _globals["_STOPORDERS"]._serialized_end = 15260
-    _globals["_PEGGEDORDERS"]._serialized_start = 15262
-    _globals["_PEGGEDORDERS"]._serialized_end = 15326
-    _globals["_EXECUTIONMARKETS"]._serialized_start = 15329
-    _globals["_EXECUTIONMARKETS"]._serialized_end = 15538
-    _globals["_POSITION"]._serialized_start = 15541
-    _globals["_POSITION"]._serialized_end = 15772
-    _globals["_MARKETPOSITIONS"]._serialized_start = 15774
-    _globals["_MARKETPOSITIONS"]._serialized_end = 15878
-    _globals["_SETTLEMENTSTATE"]._serialized_start = 15881
-    _globals["_SETTLEMENTSTATE"]._serialized_end = 16119
-    _globals["_LASTSETTLEDPOSITION"]._serialized_start = 16121
-    _globals["_LASTSETTLEDPOSITION"]._serialized_end = 16207
-    _globals["_SETTLEMENTTRADE"]._serialized_start = 16210
-    _globals["_SETTLEMENTTRADE"]._serialized_end = 16358
-    _globals["_APPSTATE"]._serialized_start = 16360
-    _globals["_APPSTATE"]._serialized_end = 16463
-    _globals["_EPOCHSTATE"]._serialized_start = 16466
-    _globals["_EPOCHSTATE"]._serialized_end = 16661
-    _globals["_REWARDSPENDINGPAYOUTS"]._serialized_start = 16663
-    _globals["_REWARDSPENDINGPAYOUTS"]._serialized_end = 16786
-    _globals["_SCHEDULEDREWARDSPAYOUT"]._serialized_start = 16789
-    _globals["_SCHEDULEDREWARDSPAYOUT"]._serialized_end = 16918
-    _globals["_REWARDSPAYOUT"]._serialized_start = 16921
-    _globals["_REWARDSPAYOUT"]._serialized_end = 17173
-    _globals["_REWARDSPARTYAMOUNT"]._serialized_start = 17175
-    _globals["_REWARDSPARTYAMOUNT"]._serialized_end = 17241
-    _globals["_LIMITSTATE"]._serialized_start = 17244
-    _globals["_LIMITSTATE"]._serialized_end = 17648
-    _globals["_VOTESPAMPOLICY"]._serialized_start = 17651
-    _globals["_VOTESPAMPOLICY"]._serialized_end = 18183
-    _globals["_PARTYPROPOSALVOTECOUNT"]._serialized_start = 18185
-    _globals["_PARTYPROPOSALVOTECOUNT"]._serialized_end = 18281
-    _globals["_PARTYTOKENBALANCE"]._serialized_start = 18283
-    _globals["_PARTYTOKENBALANCE"]._serialized_end = 18350
-    _globals["_BLOCKREJECTSTATS"]._serialized_start = 18352
-    _globals["_BLOCKREJECTSTATS"]._serialized_end = 18420
-    _globals["_SPAMPARTYTRANSACTIONCOUNT"]._serialized_start = 18422
-    _globals["_SPAMPARTYTRANSACTIONCOUNT"]._serialized_end = 18493
-    _globals["_SIMPLESPAMPOLICY"]._serialized_start = 18496
-    _globals["_SIMPLESPAMPOLICY"]._serialized_end = 18818
-    _globals["_NOTARYSIGS"]._serialized_start = 18820
-    _globals["_NOTARYSIGS"]._serialized_end = 18932
-    _globals["_NOTARY"]._serialized_start = 18934
-    _globals["_NOTARY"]._serialized_end = 19005
-    _globals["_STAKEVERIFIERDEPOSITED"]._serialized_start = 19007
-    _globals["_STAKEVERIFIERDEPOSITED"]._serialized_end = 19116
-    _globals["_STAKEVERIFIERREMOVED"]._serialized_start = 19118
-    _globals["_STAKEVERIFIERREMOVED"]._serialized_end = 19221
-    _globals["_STAKEVERIFIERPENDING"]._serialized_start = 19224
-    _globals["_STAKEVERIFIERPENDING"]._serialized_end = 19485
-    _globals["_PENDINGKEYROTATION"]._serialized_start = 19488
-    _globals["_PENDINGKEYROTATION"]._serialized_end = 19643
-    _globals["_PENDINGETHEREUMKEYROTATION"]._serialized_start = 19646
-    _globals["_PENDINGETHEREUMKEYROTATION"]._serialized_end = 19830
-    _globals["_TOPOLOGY"]._serialized_start = 19833
-    _globals["_TOPOLOGY"]._serialized_end = 20438
-    _globals["_TOPLOGYSIGNATURES"]._serialized_start = 20441
-    _globals["_TOPLOGYSIGNATURES"]._serialized_end = 20663
-    _globals["_PENDINGERC20MULTISIGCONTROLSIGNATURE"]._serialized_start = 20666
-    _globals["_PENDINGERC20MULTISIGCONTROLSIGNATURE"]._serialized_end = 20845
-    _globals["_ISSUEDERC20MULTISIGCONTROLSIGNATURE"]._serialized_start = 20848
-    _globals["_ISSUEDERC20MULTISIGCONTROLSIGNATURE"]._serialized_end = 21006
-    _globals["_VALIDATORSTATE"]._serialized_start = 21009
-    _globals["_VALIDATORSTATE"]._serialized_end = 21507
-    _globals["_HEARTBEATTRACKER"]._serialized_start = 21510
-    _globals["_HEARTBEATTRACKER"]._serialized_end = 21695
-    _globals["_PERFORMANCESTATS"]._serialized_start = 21698
-    _globals["_PERFORMANCESTATS"]._serialized_end = 21979
-    _globals["_VALIDATORPERFORMANCE"]._serialized_start = 21981
-    _globals["_VALIDATORPERFORMANCE"]._serialized_end = 22089
-    _globals["_LIQUIDITYPARAMETERS"]._serialized_start = 22092
-    _globals["_LIQUIDITYPARAMETERS"]._serialized_end = 22266
-    _globals["_LIQUIDITYPENDINGPROVISIONS"]._serialized_start = 22268
-    _globals["_LIQUIDITYPENDINGPROVISIONS"]._serialized_end = 22372
-    _globals["_LIQUIDITYPARTIESLIQUIDITYORDERS"]._serialized_start = 22375
-    _globals["_LIQUIDITYPARTIESLIQUIDITYORDERS"]._serialized_end = 22503
-    _globals["_PARTYORDERS"]._serialized_start = 22505
-    _globals["_PARTYORDERS"]._serialized_end = 22577
-    _globals["_LIQUIDITYPARTIESORDERS"]._serialized_start = 22579
-    _globals["_LIQUIDITYPARTIESORDERS"]._serialized_end = 22698
-    _globals["_LIQUIDITYPROVISIONS"]._serialized_start = 22700
-    _globals["_LIQUIDITYPROVISIONS"]._serialized_end = 22827
-    _globals["_LIQUIDITYSCORES"]._serialized_start = 22830
-    _globals["_LIQUIDITYSCORES"]._serialized_end = 22990
-    _globals["_LIQUIDITYSCORE"]._serialized_start = 22992
-    _globals["_LIQUIDITYSCORE"]._serialized_end = 23057
-    _globals["_FLOATINGPOINTCONSENSUS"]._serialized_start = 23060
-    _globals["_FLOATINGPOINTCONSENSUS"]._serialized_end = 23245
-    _globals["_STATEVARINTERNALSTATE"]._serialized_start = 23248
-    _globals["_STATEVARINTERNALSTATE"]._serialized_end = 23500
-    _globals["_FLOATINGPOINTVALIDATORRESULT"]._serialized_start = 23502
-    _globals["_FLOATINGPOINTVALIDATORRESULT"]._serialized_end = 23594
-    _globals["_NEXTTIMETRIGGER"]._serialized_start = 23596
-    _globals["_NEXTTIMETRIGGER"]._serialized_end = 23710
-    _globals["_MARKETTRACKER"]._serialized_start = 23712
-    _globals["_MARKETTRACKER"]._serialized_end = 23811
-    _globals["_SIGNEREVENTSPERADDRESS"]._serialized_start = 23813
-    _globals["_SIGNEREVENTSPERADDRESS"]._serialized_end = 23929
-    _globals["_ERC20MULTISIGTOPOLOGYVERIFIED"]._serialized_start = 23932
-    _globals["_ERC20MULTISIGTOPOLOGYVERIFIED"]._serialized_end = 24188
-    _globals["_ERC20MULTISIGTOPOLOGYPENDING"]._serialized_start = 24191
-    _globals["_ERC20MULTISIGTOPOLOGYPENDING"]._serialized_end = 24507
-    _globals["_PROOFOFWORK"]._serialized_start = 24510
-    _globals["_PROOFOFWORK"]._serialized_end = 24927
-    _globals["_BANNEDPARTY"]._serialized_start = 24929
-    _globals["_BANNEDPARTY"]._serialized_end = 24986
-    _globals["_PROOFOFWORKPARAMS"]._serialized_start = 24989
-    _globals["_PROOFOFWORKPARAMS"]._serialized_end = 25377
-    _globals["_PROOFOFWORKSTATE"]._serialized_start = 25379
-    _globals["_PROOFOFWORKSTATE"]._serialized_end = 25467
-    _globals["_PROOFOFWORKBLOCKSTATE"]._serialized_start = 25470
-    _globals["_PROOFOFWORKBLOCKSTATE"]._serialized_end = 25610
-    _globals["_PROOFOFWORKPARTYSTATEFORBLOCK"]._serialized_start = 25613
-    _globals["_PROOFOFWORKPARTYSTATEFORBLOCK"]._serialized_end = 25746
-    _globals["_TRANSACTIONSATHEIGHT"]._serialized_start = 25748
-    _globals["_TRANSACTIONSATHEIGHT"]._serialized_end = 25830
-    _globals["_PROTOCOLUPGRADEPROPOSALS"]._serialized_start = 25833
-    _globals["_PROTOCOLUPGRADEPROPOSALS"]._serialized_end = 26036
-    _globals["_ACCEPTEDPROTOCOLUPGRADEPROPOSAL"]._serialized_start = 26038
-    _globals["_ACCEPTEDPROTOCOLUPGRADEPROPOSAL"]._serialized_end = 26163
+    _globals["_MARKET"]._serialized_end = 14490
+    _globals["_ORDERSATPRICE"]._serialized_start = 14492
+    _globals["_ORDERSATPRICE"]._serialized_end = 14553
+    _globals["_PRICEDSTOPORDERS"]._serialized_start = 14556
+    _globals["_PRICEDSTOPORDERS"]._serialized_end = 14708
+    _globals["_TRAILINGSTOPORDERS"]._serialized_start = 14711
+    _globals["_TRAILINGSTOPORDERS"]._serialized_end = 14907
+    _globals["_ORDERSATOFFSET"]._serialized_start = 14909
+    _globals["_ORDERSATOFFSET"]._serialized_end = 14973
+    _globals["_OFFSETSATPRICE"]._serialized_start = 14975
+    _globals["_OFFSETSATPRICE"]._serialized_end = 15073
+    _globals["_STOPORDERS"]._serialized_start = 15076
+    _globals["_STOPORDERS"]._serialized_end = 15323
+    _globals["_PEGGEDORDERS"]._serialized_start = 15325
+    _globals["_PEGGEDORDERS"]._serialized_end = 15389
+    _globals["_EXECUTIONMARKETS"]._serialized_start = 15392
+    _globals["_EXECUTIONMARKETS"]._serialized_end = 15663
+    _globals["_SUCCESSORS"]._serialized_start = 15665
+    _globals["_SUCCESSORS"]._serialized_end = 15759
+    _globals["_POSITION"]._serialized_start = 15762
+    _globals["_POSITION"]._serialized_end = 15993
+    _globals["_MARKETPOSITIONS"]._serialized_start = 15995
+    _globals["_MARKETPOSITIONS"]._serialized_end = 16099
+    _globals["_SETTLEMENTSTATE"]._serialized_start = 16102
+    _globals["_SETTLEMENTSTATE"]._serialized_end = 16340
+    _globals["_LASTSETTLEDPOSITION"]._serialized_start = 16342
+    _globals["_LASTSETTLEDPOSITION"]._serialized_end = 16428
+    _globals["_SETTLEMENTTRADE"]._serialized_start = 16431
+    _globals["_SETTLEMENTTRADE"]._serialized_end = 16579
+    _globals["_APPSTATE"]._serialized_start = 16581
+    _globals["_APPSTATE"]._serialized_end = 16684
+    _globals["_EPOCHSTATE"]._serialized_start = 16687
+    _globals["_EPOCHSTATE"]._serialized_end = 16882
+    _globals["_REWARDSPENDINGPAYOUTS"]._serialized_start = 16884
+    _globals["_REWARDSPENDINGPAYOUTS"]._serialized_end = 17007
+    _globals["_SCHEDULEDREWARDSPAYOUT"]._serialized_start = 17010
+    _globals["_SCHEDULEDREWARDSPAYOUT"]._serialized_end = 17139
+    _globals["_REWARDSPAYOUT"]._serialized_start = 17142
+    _globals["_REWARDSPAYOUT"]._serialized_end = 17394
+    _globals["_REWARDSPARTYAMOUNT"]._serialized_start = 17396
+    _globals["_REWARDSPARTYAMOUNT"]._serialized_end = 17462
+    _globals["_LIMITSTATE"]._serialized_start = 17465
+    _globals["_LIMITSTATE"]._serialized_end = 17869
+    _globals["_VOTESPAMPOLICY"]._serialized_start = 17872
+    _globals["_VOTESPAMPOLICY"]._serialized_end = 18404
+    _globals["_PARTYPROPOSALVOTECOUNT"]._serialized_start = 18406
+    _globals["_PARTYPROPOSALVOTECOUNT"]._serialized_end = 18502
+    _globals["_PARTYTOKENBALANCE"]._serialized_start = 18504
+    _globals["_PARTYTOKENBALANCE"]._serialized_end = 18571
+    _globals["_BLOCKREJECTSTATS"]._serialized_start = 18573
+    _globals["_BLOCKREJECTSTATS"]._serialized_end = 18641
+    _globals["_SPAMPARTYTRANSACTIONCOUNT"]._serialized_start = 18643
+    _globals["_SPAMPARTYTRANSACTIONCOUNT"]._serialized_end = 18714
+    _globals["_SIMPLESPAMPOLICY"]._serialized_start = 18717
+    _globals["_SIMPLESPAMPOLICY"]._serialized_end = 19039
+    _globals["_NOTARYSIGS"]._serialized_start = 19041
+    _globals["_NOTARYSIGS"]._serialized_end = 19153
+    _globals["_NOTARY"]._serialized_start = 19155
+    _globals["_NOTARY"]._serialized_end = 19226
+    _globals["_STAKEVERIFIERDEPOSITED"]._serialized_start = 19228
+    _globals["_STAKEVERIFIERDEPOSITED"]._serialized_end = 19337
+    _globals["_STAKEVERIFIERREMOVED"]._serialized_start = 19339
+    _globals["_STAKEVERIFIERREMOVED"]._serialized_end = 19442
+    _globals["_STAKEVERIFIERPENDING"]._serialized_start = 19445
+    _globals["_STAKEVERIFIERPENDING"]._serialized_end = 19706
+    _globals["_PENDINGKEYROTATION"]._serialized_start = 19709
+    _globals["_PENDINGKEYROTATION"]._serialized_end = 19864
+    _globals["_PENDINGETHEREUMKEYROTATION"]._serialized_start = 19867
+    _globals["_PENDINGETHEREUMKEYROTATION"]._serialized_end = 20051
+    _globals["_TOPOLOGY"]._serialized_start = 20054
+    _globals["_TOPOLOGY"]._serialized_end = 20659
+    _globals["_TOPLOGYSIGNATURES"]._serialized_start = 20662
+    _globals["_TOPLOGYSIGNATURES"]._serialized_end = 20884
+    _globals["_PENDINGERC20MULTISIGCONTROLSIGNATURE"]._serialized_start = 20887
+    _globals["_PENDINGERC20MULTISIGCONTROLSIGNATURE"]._serialized_end = 21066
+    _globals["_ISSUEDERC20MULTISIGCONTROLSIGNATURE"]._serialized_start = 21069
+    _globals["_ISSUEDERC20MULTISIGCONTROLSIGNATURE"]._serialized_end = 21227
+    _globals["_VALIDATORSTATE"]._serialized_start = 21230
+    _globals["_VALIDATORSTATE"]._serialized_end = 21728
+    _globals["_HEARTBEATTRACKER"]._serialized_start = 21731
+    _globals["_HEARTBEATTRACKER"]._serialized_end = 21916
+    _globals["_PERFORMANCESTATS"]._serialized_start = 21919
+    _globals["_PERFORMANCESTATS"]._serialized_end = 22200
+    _globals["_VALIDATORPERFORMANCE"]._serialized_start = 22202
+    _globals["_VALIDATORPERFORMANCE"]._serialized_end = 22310
+    _globals["_LIQUIDITYPARAMETERS"]._serialized_start = 22313
+    _globals["_LIQUIDITYPARAMETERS"]._serialized_end = 22487
+    _globals["_LIQUIDITYPENDINGPROVISIONS"]._serialized_start = 22489
+    _globals["_LIQUIDITYPENDINGPROVISIONS"]._serialized_end = 22593
+    _globals["_LIQUIDITYPARTIESLIQUIDITYORDERS"]._serialized_start = 22596
+    _globals["_LIQUIDITYPARTIESLIQUIDITYORDERS"]._serialized_end = 22724
+    _globals["_PARTYORDERS"]._serialized_start = 22726
+    _globals["_PARTYORDERS"]._serialized_end = 22798
+    _globals["_LIQUIDITYPARTIESORDERS"]._serialized_start = 22800
+    _globals["_LIQUIDITYPARTIESORDERS"]._serialized_end = 22919
+    _globals["_LIQUIDITYPROVISIONS"]._serialized_start = 22921
+    _globals["_LIQUIDITYPROVISIONS"]._serialized_end = 23048
+    _globals["_LIQUIDITYSCORES"]._serialized_start = 23051
+    _globals["_LIQUIDITYSCORES"]._serialized_end = 23211
+    _globals["_LIQUIDITYSCORE"]._serialized_start = 23213
+    _globals["_LIQUIDITYSCORE"]._serialized_end = 23278
+    _globals["_FLOATINGPOINTCONSENSUS"]._serialized_start = 23281
+    _globals["_FLOATINGPOINTCONSENSUS"]._serialized_end = 23466
+    _globals["_STATEVARINTERNALSTATE"]._serialized_start = 23469
+    _globals["_STATEVARINTERNALSTATE"]._serialized_end = 23721
+    _globals["_FLOATINGPOINTVALIDATORRESULT"]._serialized_start = 23723
+    _globals["_FLOATINGPOINTVALIDATORRESULT"]._serialized_end = 23815
+    _globals["_NEXTTIMETRIGGER"]._serialized_start = 23817
+    _globals["_NEXTTIMETRIGGER"]._serialized_end = 23931
+    _globals["_MARKETTRACKER"]._serialized_start = 23933
+    _globals["_MARKETTRACKER"]._serialized_end = 24032
+    _globals["_SIGNEREVENTSPERADDRESS"]._serialized_start = 24034
+    _globals["_SIGNEREVENTSPERADDRESS"]._serialized_end = 24150
+    _globals["_ERC20MULTISIGTOPOLOGYVERIFIED"]._serialized_start = 24153
+    _globals["_ERC20MULTISIGTOPOLOGYVERIFIED"]._serialized_end = 24409
+    _globals["_ERC20MULTISIGTOPOLOGYPENDING"]._serialized_start = 24412
+    _globals["_ERC20MULTISIGTOPOLOGYPENDING"]._serialized_end = 24728
+    _globals["_PROOFOFWORK"]._serialized_start = 24731
+    _globals["_PROOFOFWORK"]._serialized_end = 25148
+    _globals["_BANNEDPARTY"]._serialized_start = 25150
+    _globals["_BANNEDPARTY"]._serialized_end = 25207
+    _globals["_PROOFOFWORKPARAMS"]._serialized_start = 25210
+    _globals["_PROOFOFWORKPARAMS"]._serialized_end = 25598
+    _globals["_PROOFOFWORKSTATE"]._serialized_start = 25600
+    _globals["_PROOFOFWORKSTATE"]._serialized_end = 25688
+    _globals["_PROOFOFWORKBLOCKSTATE"]._serialized_start = 25691
+    _globals["_PROOFOFWORKBLOCKSTATE"]._serialized_end = 25831
+    _globals["_PROOFOFWORKPARTYSTATEFORBLOCK"]._serialized_start = 25834
+    _globals["_PROOFOFWORKPARTYSTATEFORBLOCK"]._serialized_end = 25967
+    _globals["_TRANSACTIONSATHEIGHT"]._serialized_start = 25969
+    _globals["_TRANSACTIONSATHEIGHT"]._serialized_end = 26051
+    _globals["_PROTOCOLUPGRADEPROPOSALS"]._serialized_start = 26054
+    _globals["_PROTOCOLUPGRADEPROPOSALS"]._serialized_end = 26257
+    _globals["_ACCEPTEDPROTOCOLUPGRADEPROPOSAL"]._serialized_start = 26259
+    _globals["_ACCEPTEDPROTOCOLUPGRADEPROPOSAL"]._serialized_end = 26384
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/vega_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/vega_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,187 +12,187 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import markets_pb2 as vega_dot_markets__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0fvega/vega.proto\x12\x04vega\x1a\x12vega/markets.proto"\xb8\x07\n\tStopOrder\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\x0boco_link_id\x18\x02 \x01(\tH\x01R\tocoLinkId\x88\x01\x01\x12"\n\nexpires_at\x18\x03 \x01(\x03H\x02R\texpiresAt\x88\x01\x01\x12L\n\x0f\x65xpiry_strategy\x18\x04 \x01(\x0e\x32\x1e.vega.StopOrder.ExpiryStrategyH\x03R\x0e\x65xpiryStrategy\x88\x01\x01\x12M\n\x11trigger_direction\x18\x05 \x01(\x0e\x32 .vega.StopOrder.TriggerDirectionR\x10triggerDirection\x12.\n\x06status\x18\x06 \x01(\x0e\x32\x16.vega.StopOrder.StatusR\x06status\x12\x1d\n\ncreated_at\x18\x07 \x01(\x03R\tcreatedAt\x12"\n\nupdated_at\x18\x08 \x01(\x03H\x04R\tupdatedAt\x88\x01\x01\x12\x19\n\x08order_id\x18\t \x01(\tR\x07orderId\x12\x14\n\x05party\x18\n \x01(\tR\x05party\x12\x16\n\x05price\x18\x64 \x01(\tH\x00R\x05price\x12\x38\n\x17trailing_percent_offset\x18\x65 \x01(\tH\x00R\x15trailingPercentOffset"j\n\x0e\x45xpiryStrategy\x12\x1f\n\x1b\x45XPIRY_STRATEGY_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x45XPIRY_STRATEGY_CANCELS\x10\x01\x12\x1a\n\x16\x45XPIRY_STRATEGY_SUBMIT\x10\x02"{\n\x10TriggerDirection\x12!\n\x1dTRIGGER_DIRECTION_UNSPECIFIED\x10\x00\x12!\n\x1dTRIGGER_DIRECTION_RISES_ABOVE\x10\x01\x12!\n\x1dTRIGGER_DIRECTION_FALLS_BELOW\x10\x02"\x88\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x12\n\x0eSTATUS_STOPPED\x10\x03\x12\x14\n\x10STATUS_TRIGGERED\x10\x04\x12\x12\n\x0eSTATUS_EXPIRED\x10\x05\x42\t\n\x07triggerB\x0e\n\x0c_oco_link_idB\r\n\x0b_expires_atB\x12\n\x10_expiry_strategyB\r\n\x0b_updated_at"\x17\n\x05Party\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"N\n\nRiskFactor\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05short\x18\x02 \x01(\tR\x05short\x12\x12\n\x04long\x18\x03 \x01(\tR\x04long"Z\n\x0bPeggedOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset"\x8c\x01\n\x0cIcebergOrder\x12\x1b\n\tpeak_size\x18\x01 \x01(\x04R\x08peakSize\x12\x30\n\x14minimum_visible_size\x18\x02 \x01(\x04R\x12minimumVisibleSize\x12-\n\x12reserved_remaining\x18\x03 \x01(\x04R\x11reservedRemaining"\x80\n\n\x05Order\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12\x12\n\x04size\x18\x06 \x01(\x04R\x04size\x12\x1c\n\tremaining\x18\x07 \x01(\x04R\tremaining\x12;\n\rtime_in_force\x18\x08 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12$\n\x04type\x18\t \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1d\n\ncreated_at\x18\n \x01(\x03R\tcreatedAt\x12*\n\x06status\x18\x0b \x01(\x0e\x32\x12.vega.Order.StatusR\x06status\x12\x1d\n\nexpires_at\x18\x0c \x01(\x03R\texpiresAt\x12\x1c\n\treference\x18\r \x01(\tR\treference\x12-\n\x06reason\x18\x0e \x01(\x0e\x32\x10.vega.OrderErrorH\x00R\x06reason\x88\x01\x01\x12\x1d\n\nupdated_at\x18\x0f \x01(\x03R\tupdatedAt\x12\x18\n\x07version\x18\x10 \x01(\x04R\x07version\x12\x19\n\x08\x62\x61tch_id\x18\x11 \x01(\x04R\x07\x62\x61tchId\x12\x34\n\x0cpegged_order\x18\x12 \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x34\n\x16liquidity_provision_id\x18\x13 \x01(\tR\x14liquidityProvisionId\x12\x1b\n\tpost_only\x18\x14 \x01(\x08R\x08postOnly\x12\x1f\n\x0breduce_only\x18\x15 \x01(\x08R\nreduceOnly\x12<\n\riceberg_order\x18\x16 \x01(\x0b\x32\x12.vega.IcebergOrderH\x01R\x0cicebergOrder\x88\x01\x01"\xb6\x01\n\x0bTimeInForce\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_GTC\x10\x01\x12\x15\n\x11TIME_IN_FORCE_GTT\x10\x02\x12\x15\n\x11TIME_IN_FORCE_IOC\x10\x03\x12\x15\n\x11TIME_IN_FORCE_FOK\x10\x04\x12\x15\n\x11TIME_IN_FORCE_GFA\x10\x05\x12\x15\n\x11TIME_IN_FORCE_GFN\x10\x06"O\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_LIMIT\x10\x01\x12\x0f\n\x0bTYPE_MARKET\x10\x02\x12\x10\n\x0cTYPE_NETWORK\x10\x03"\xc9\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_EXPIRED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x11\n\rSTATUS_FILLED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x12\x1b\n\x17STATUS_PARTIALLY_FILLED\x10\x07\x12\x11\n\rSTATUS_PARKED\x10\x08\x42\t\n\x07_reasonB\x10\n\x0e_iceberg_order"B\n\x1dOrderCancellationConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xa0\x01\n\x11OrderConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order\x12#\n\x06trades\x18\x02 \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x43\n\x17passive_orders_affected\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x15passiveOrdersAffected"\xd3\x01\n\x16\x41uctionIndicativeState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12)\n\x10indicative_price\x18\x02 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x03 \x01(\x04R\x10indicativeVolume\x12#\n\rauction_start\x18\x04 \x01(\x03R\x0c\x61uctionStart\x12\x1f\n\x0b\x61uction_end\x18\x05 \x01(\x03R\nauctionEnd"\xdb\x04\n\x05Trade\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12\x12\n\x04size\x18\x04 \x01(\x04R\x04size\x12\x14\n\x05\x62uyer\x18\x05 \x01(\tR\x05\x62uyer\x12\x16\n\x06seller\x18\x06 \x01(\tR\x06seller\x12(\n\taggressor\x18\x07 \x01(\x0e\x32\n.vega.SideR\taggressor\x12\x1b\n\tbuy_order\x18\x08 \x01(\tR\x08\x62uyOrder\x12\x1d\n\nsell_order\x18\t \x01(\tR\tsellOrder\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12$\n\x04type\x18\x0b \x01(\x0e\x32\x10.vega.Trade.TypeR\x04type\x12&\n\tbuyer_fee\x18\x0c \x01(\x0b\x32\t.vega.FeeR\x08\x62uyerFee\x12(\n\nseller_fee\x18\r \x01(\x0b\x32\t.vega.FeeR\tsellerFee\x12.\n\x13\x62uyer_auction_batch\x18\x0e \x01(\x04R\x11\x62uyerAuctionBatch\x12\x30\n\x14seller_auction_batch\x18\x0f \x01(\x04R\x12sellerAuctionBatch"o\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cTYPE_DEFAULT\x10\x01\x12\x1f\n\x1bTYPE_NETWORK_CLOSE_OUT_GOOD\x10\x02\x12\x1e\n\x1aTYPE_NETWORK_CLOSE_OUT_BAD\x10\x03"v\n\x03\x46\x65\x65\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"/\n\x08TradeSet\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"\xd6\x01\n\x06\x43\x61ndle\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x1a\n\x08\x64\x61tetime\x18\x02 \x01(\tR\x08\x64\x61tetime\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12*\n\x08interval\x18\x08 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval"d\n\nPriceLevel\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12(\n\x10number_of_orders\x18\x02 \x01(\x04R\x0enumberOfOrders\x12\x16\n\x06volume\x18\x03 \x01(\x04R\x06volume"\x9d\x01\n\x0bMarketDepth\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber"\xdd\x01\n\x11MarketDepthUpdate\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber\x12\x38\n\x18previous_sequence_number\x18\x05 \x01(\x04R\x16previousSequenceNumber"\xf7\x02\n\x08Position\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1f\n\x0bopen_volume\x18\x03 \x01(\x03R\nopenVolume\x12!\n\x0crealised_pnl\x18\x04 \x01(\tR\x0brealisedPnl\x12%\n\x0eunrealised_pnl\x18\x05 \x01(\tR\runrealisedPnl\x12.\n\x13\x61verage_entry_price\x18\x06 \x01(\tR\x11\x61verageEntryPrice\x12\x1d\n\nupdated_at\x18\x07 \x01(\x03R\tupdatedAt\x12:\n\x19loss_socialisation_amount\x18\x08 \x01(\tR\x17lossSocialisationAmount\x12=\n\x0fposition_status\x18\t \x01(\x0e\x32\x14.vega.PositionStatusR\x0epositionStatus"=\n\rPositionTrade\x12\x16\n\x06volume\x18\x01 \x01(\x03R\x06volume\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price"\xe4\x02\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x14.vega.Deposit.StatusR\x06status\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12-\n\x12\x63redited_timestamp\x18\x07 \x01(\x03R\x11\x63reditedTimestamp\x12+\n\x11\x63reated_timestamp\x18\x08 \x01(\x03R\x10\x63reatedTimestamp"]\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03"\xa8\x03\n\nWithdrawal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12/\n\x06status\x18\x05 \x01(\x0e\x32\x17.vega.Withdrawal.StatusR\x06status\x12\x10\n\x03ref\x18\x06 \x01(\tR\x03ref\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12+\n\x11\x63reated_timestamp\x18\t \x01(\x03R\x10\x63reatedTimestamp\x12/\n\x13withdrawn_timestamp\x18\n \x01(\x03R\x12withdrawnTimestamp\x12#\n\x03\x65xt\x18\x0b \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\\\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03J\x04\x08\x07\x10\x08"D\n\x0bWithdrawExt\x12.\n\x05\x65rc20\x18\x01 \x01(\x0b\x32\x16.vega.Erc20WithdrawExtH\x00R\x05\x65rc20B\x05\n\x03\x65xt"=\n\x10\x45rc20WithdrawExt\x12)\n\x10receiver_address\x18\x01 \x01(\tR\x0freceiverAddress"\xa3\x01\n\x07\x41\x63\x63ount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"?\n\x0f\x46inancialAmount\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset"\xb3\x01\n\x08Transfer\x12\x14\n\x05owner\x18\x01 \x01(\tR\x05owner\x12-\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x15.vega.FinancialAmountR\x06\x61mount\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId"\x84\x01\n\x10\x44ispatchStrategy\x12(\n\x10\x61sset_for_metric\x18\x01 \x01(\tR\x0e\x61ssetForMetric\x12,\n\x06metric\x18\x02 \x01(\x0e\x32\x14.vega.DispatchMetricR\x06metric\x12\x18\n\x07markets\x18\x03 \x03(\tR\x07markets"\xe6\x01\n\x0fTransferRequest\x12\x30\n\x0c\x66rom_account\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x0b\x66romAccount\x12,\n\nto_account\x18\x02 \x03(\x0b\x32\r.vega.AccountR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12&\n\x04type\x18\x07 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type"\xa7\x01\n\x0e\x41\x63\x63ountDetails\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type\x12\x19\n\x05owner\x18\x03 \x01(\tH\x00R\x05owner\x88\x01\x01\x12 \n\tmarket_id\x18\x04 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x08\n\x06_ownerB\x0c\n\n_market_id"\xb9\x02\n\x0bLedgerEntry\x12\x37\n\x0c\x66rom_account\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x0b\x66romAccount\x12\x33\n\nto_account\x18\x02 \x01(\x0b\x32\x14.vega.AccountDetailsR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12&\n\x04type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x30\n\x14\x66rom_account_balance\x18\x06 \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\x07 \x01(\tR\x10toAccountBalance"_\n\x13PostTransferBalance\x12.\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x07\x61\x63\x63ount\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"t\n\x0eLedgerMovement\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.vega.LedgerEntryR\x07\x65ntries\x12\x35\n\x08\x62\x61lances\x18\x02 \x03(\x0b\x32\x19.vega.PostTransferBalanceR\x08\x62\x61lances"\xad\x02\n\x0cMarginLevels\x12-\n\x12maintenance_margin\x18\x01 \x01(\tR\x11maintenanceMargin\x12!\n\x0csearch_level\x18\x02 \x01(\tR\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x03 \x01(\tR\rinitialMargin\x12\x38\n\x18\x63ollateral_release_level\x18\x04 \x01(\tR\x16\x63ollateralReleaseLevel\x12\x19\n\x08party_id\x18\x05 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x06 \x01(\tR\x08marketId\x12\x14\n\x05\x61sset\x18\x07 \x01(\tR\x05\x61sset\x12\x1c\n\ttimestamp\x18\x08 \x01(\x03R\ttimestamp"\x8a\x0b\n\nMarketData\x12\x1d\n\nmark_price\x18\x01 \x01(\tR\tmarkPrice\x12$\n\x0e\x62\x65st_bid_price\x18\x02 \x01(\tR\x0c\x62\x65stBidPrice\x12&\n\x0f\x62\x65st_bid_volume\x18\x03 \x01(\x04R\rbestBidVolume\x12(\n\x10\x62\x65st_offer_price\x18\x04 \x01(\tR\x0e\x62\x65stOfferPrice\x12*\n\x11\x62\x65st_offer_volume\x18\x05 \x01(\x04R\x0f\x62\x65stOfferVolume\x12\x31\n\x15\x62\x65st_static_bid_price\x18\x06 \x01(\tR\x12\x62\x65stStaticBidPrice\x12\x33\n\x16\x62\x65st_static_bid_volume\x18\x07 \x01(\x04R\x13\x62\x65stStaticBidVolume\x12\x35\n\x17\x62\x65st_static_offer_price\x18\x08 \x01(\tR\x14\x62\x65stStaticOfferPrice\x12\x37\n\x18\x62\x65st_static_offer_volume\x18\t \x01(\x04R\x15\x62\x65stStaticOfferVolume\x12\x1b\n\tmid_price\x18\n \x01(\tR\x08midPrice\x12(\n\x10static_mid_price\x18\x0b \x01(\tR\x0estaticMidPrice\x12\x16\n\x06market\x18\x0c \x01(\tR\x06market\x12\x1c\n\ttimestamp\x18\r \x01(\x03R\ttimestamp\x12#\n\ropen_interest\x18\x0e \x01(\x04R\x0copenInterest\x12\x1f\n\x0b\x61uction_end\x18\x0f \x01(\x03R\nauctionEnd\x12#\n\rauction_start\x18\x10 \x01(\x03R\x0c\x61uctionStart\x12)\n\x10indicative_price\x18\x11 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x12 \x01(\x04R\x10indicativeVolume\x12H\n\x13market_trading_mode\x18\x13 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x11marketTradingMode\x12.\n\x07trigger\x18\x14 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x15 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger\x12!\n\x0ctarget_stake\x18\x16 \x01(\tR\x0btargetStake\x12%\n\x0esupplied_stake\x18\x17 \x01(\tR\rsuppliedStake\x12S\n\x17price_monitoring_bounds\x18\x18 \x03(\x0b\x32\x1b.vega.PriceMonitoringBoundsR\x15priceMonitoringBounds\x12,\n\x12market_value_proxy\x18\x19 \x01(\tR\x10marketValueProxy\x12`\n\x1cliquidity_provider_fee_share\x18\x1a \x03(\x0b\x32\x1f.vega.LiquidityProviderFeeShareR\x19liquidityProviderFeeShare\x12\x35\n\x0cmarket_state\x18\x1b \x01(\x0e\x32\x12.vega.Market.StateR\x0bmarketState\x12-\n\x13next_mark_to_market\x18\x1c \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x1d \x01(\tR\x0flastTradedPrice\x12#\n\rmarket_growth\x18\x1e \x01(\tR\x0cmarketGrowth"\xdf\x01\n\x19LiquidityProviderFeeShare\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12*\n\x11\x65quity_like_share\x18\x02 \x01(\tR\x0f\x65quityLikeShare\x12\x36\n\x17\x61verage_entry_valuation\x18\x03 \x01(\tR\x15\x61verageEntryValuation\x12#\n\raverage_score\x18\x04 \x01(\tR\x0c\x61verageScore\x12#\n\rvirtual_stake\x18\x05 \x01(\tR\x0cvirtualStake"\xc8\x01\n\x15PriceMonitoringBounds\x12&\n\x0fmin_valid_price\x18\x01 \x01(\tR\rminValidPrice\x12&\n\x0fmax_valid_price\x18\x02 \x01(\tR\rmaxValidPrice\x12\x36\n\x07trigger\x18\x03 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger\x12\'\n\x0freference_price\x18\x04 \x01(\tR\x0ereferencePrice"Q\n\x0b\x45rrorDetail\x12\x12\n\x04\x63ode\x18\x01 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x14\n\x05inner\x18\x03 \x01(\tR\x05inner":\n\x10NetworkParameter\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\x82\x03\n\rNetworkLimits\x12,\n\x12\x63\x61n_propose_market\x18\x01 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x02 \x01(\x08R\x0f\x63\x61nProposeAsset\x12\x34\n\x16propose_market_enabled\x18\x04 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x05 \x01(\x08R\x13proposeAssetEnabled\x12%\n\x0egenesis_loaded\x18\x07 \x01(\x08R\rgenesisLoaded\x12=\n\x1bpropose_market_enabled_from\x18\x08 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\t \x01(\x03R\x17proposeAssetEnabledFromJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07"}\n\x0eLiquidityOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x1e\n\nproportion\x18\x02 \x01(\rR\nproportion\x12\x16\n\x06offset\x18\x03 \x01(\tR\x06offset"s\n\x17LiquidityOrderReference\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12=\n\x0fliquidity_order\x18\x02 \x01(\x0b\x32\x14.vega.LiquidityOrderR\x0eliquidityOrder"\xd2\x04\n\x12LiquidityProvision\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1d\n\ncreated_at\x18\x03 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x04 \x01(\x03R\tupdatedAt\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x06 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x07 \x01(\tR\x03\x66\x65\x65\x12\x33\n\x05sells\x18\x08 \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x05sells\x12\x31\n\x04\x62uys\x18\t \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x04\x62uys\x12\x18\n\x07version\x18\n \x01(\x04R\x07version\x12\x37\n\x06status\x18\x0b \x01(\x0e\x32\x1f.vega.LiquidityProvision.StatusR\x06status\x12\x1c\n\treference\x18\x0c \x01(\tR\treference"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_STOPPED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x13\n\x0fSTATUS_REJECTED\x10\x04\x12\x15\n\x11STATUS_UNDEPLOYED\x10\x05\x12\x12\n\x0eSTATUS_PENDING\x10\x06"\xd0\x03\n\x0e\x45thereumConfig\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12\x19\n\x08\x63hain_id\x18\x02 \x01(\tR\x07\x63hainId\x12Z\n\x1a\x63ollateral_bridge_contract\x18\x03 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x18\x63ollateralBridgeContract\x12$\n\rconfirmations\x18\x04 \x01(\rR\rconfirmations\x12T\n\x17staking_bridge_contract\x18\x05 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x15stakingBridgeContract\x12R\n\x16token_vesting_contract\x18\x06 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x14tokenVestingContract\x12X\n\x19multisig_control_contract\x18\x07 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x17multisigControlContract"j\n\x16\x45thereumContractConfig\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x36\n\x17\x64\x65ployment_block_height\x18\x06 \x01(\x04R\x15\x64\x65ploymentBlockHeight"\xac\x01\n\x0f\x45pochTimestamps\x12\x1d\n\nstart_time\x18\x01 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpiry_time\x18\x02 \x01(\x03R\nexpiryTime\x12\x19\n\x08\x65nd_time\x18\x03 \x01(\x03R\x07\x65ndTime\x12\x1f\n\x0b\x66irst_block\x18\x04 \x01(\x04R\nfirstBlock\x12\x1d\n\nlast_block\x18\x05 \x01(\x04R\tlastBlock"\xb0\x01\n\x05\x45poch\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x35\n\ntimestamps\x18\x02 \x01(\x0b\x32\x15.vega.EpochTimestampsR\ntimestamps\x12*\n\nvalidators\x18\x03 \x03(\x0b\x32\n.vega.NodeR\nvalidators\x12\x32\n\x0b\x64\x65legations\x18\x04 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"\x8e\x01\n\x12\x45pochParticipation\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch\x12\x18\n\x07offline\x18\x02 \x01(\x04R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x04R\x06online\x12#\n\rtotal_rewards\x18\x04 \x01(\x01R\x0ctotalRewards"S\n\tEpochData\x12\x14\n\x05total\x18\x01 \x01(\x05R\x05total\x12\x18\n\x07offline\x18\x02 \x01(\x05R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x05R\x06online"\x9b\x02\n\x0cRankingScore\x12\x1f\n\x0bstake_score\x18\x01 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12\x42\n\x0fprevious_status\x18\x03 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0epreviousStatus\x12\x31\n\x06status\x18\x04 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x06status\x12!\n\x0cvoting_power\x18\x05 \x01(\rR\x0bvotingPower\x12#\n\rranking_score\x18\x06 \x01(\tR\x0crankingScore"\xab\x02\n\x0bRewardScore\x12.\n\x13raw_validator_score\x18\x01 \x01(\tR\x11rawValidatorScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12%\n\x0emultisig_score\x18\x03 \x01(\tR\rmultisigScore\x12\'\n\x0fvalidator_score\x18\x04 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x05 \x01(\tR\x0fnormalisedScore\x12\x44\n\x10validator_status\x18\x06 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0fvalidatorStatus"\xb3\x05\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12,\n\x12staked_by_operator\x18\x07 \x01(\tR\x10stakedByOperator\x12.\n\x13staked_by_delegates\x18\x08 \x01(\tR\x11stakedByDelegates\x12!\n\x0cstaked_total\x18\t \x01(\tR\x0bstakedTotal\x12,\n\x12max_intended_stake\x18\n \x01(\tR\x10maxIntendedStake\x12#\n\rpending_stake\x18\x0b \x01(\tR\x0cpendingStake\x12.\n\nepoch_data\x18\x0c \x01(\x0b\x32\x0f.vega.EpochDataR\tepochData\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x32\n\x0b\x64\x65legations\x18\x0e \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0creward_score\x18\x0f \x01(\x0b\x32\x11.vega.RewardScoreR\x0brewardScore\x12\x37\n\rranking_score\x18\x10 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x9c\x01\n\x07NodeSet\x12\x14\n\x05total\x18\x01 \x01(\rR\x05total\x12\x1a\n\x08inactive\x18\x02 \x01(\rR\x08inactive\x12\x1a\n\x08promoted\x18\x03 \x03(\tR\x08promoted\x12\x18\n\x07\x64\x65moted\x18\x04 \x03(\tR\x07\x64\x65moted\x12\x1d\n\x07maximum\x18\x05 \x01(\rH\x00R\x07maximum\x88\x01\x01\x42\n\n\x08_maximum"\xad\x02\n\x08NodeData\x12!\n\x0cstaked_total\x18\x01 \x01(\tR\x0bstakedTotal\x12\x1f\n\x0btotal_nodes\x18\x02 \x01(\rR\ntotalNodes\x12%\n\x0einactive_nodes\x18\x03 \x01(\rR\rinactiveNodes\x12\x38\n\x10tendermint_nodes\x18\x04 \x01(\x0b\x32\r.vega.NodeSetR\x0ftendermintNodes\x12\x30\n\x0c\x65rsatz_nodes\x18\x05 \x01(\x0b\x32\r.vega.NodeSetR\x0b\x65rsatzNodes\x12\x32\n\rpending_nodes\x18\x06 \x01(\x0b\x32\r.vega.NodeSetR\x0cpendingNodes\x12\x16\n\x06uptime\x18\x07 \x01(\x02R\x06uptime"p\n\nDelegation\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"\xfb\x01\n\x06Reward\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x65poch\x18\x03 \x01(\x04R\x05\x65poch\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12.\n\x13percentage_of_total\x18\x05 \x01(\tR\x11percentageOfTotal\x12\x1f\n\x0breceived_at\x18\x06 \x01(\x03R\nreceivedAt\x12\x1b\n\tmarket_id\x18\x07 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x08 \x01(\tR\nrewardType"]\n\rRewardSummary\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x9b\x01\n\x12\x45pochRewardSummary\x12\x14\n\x05\x65poch\x18\x01 \x01(\x04R\x05\x65poch\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x04 \x01(\tR\nrewardType\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount"y\n\x12StateValueProposal\x12 \n\x0cstate_var_id\x18\x01 \x01(\tR\nstateVarId\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12&\n\x03kvb\x18\x03 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x03kvb"k\n\x0eKeyValueBundle\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x1c\n\ttolerance\x18\x02 \x01(\tR\ttolerance\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x13.vega.StateVarValueR\x05value"\xb4\x01\n\rStateVarValue\x12\x32\n\nscalar_val\x18\x01 \x01(\x0b\x32\x11.vega.ScalarValueH\x00R\tscalarVal\x12\x32\n\nvector_val\x18\x02 \x01(\x0b\x32\x11.vega.VectorValueH\x00R\tvectorVal\x12\x32\n\nmatrix_val\x18\x03 \x01(\x0b\x32\x11.vega.MatrixValueH\x00R\tmatrixValB\x07\n\x05value"#\n\x0bScalarValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value"#\n\x0bVectorValue\x12\x14\n\x05value\x18\x01 \x03(\tR\x05value"6\n\x0bMatrixValue\x12\'\n\x05value\x18\x01 \x03(\x0b\x32\x11.vega.VectorValueR\x05value*9\n\x04Side\x12\x14\n\x10SIDE_UNSPECIFIED\x10\x00\x12\x0c\n\x08SIDE_BUY\x10\x01\x12\r\n\tSIDE_SELL\x10\x02*\xb5\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x1b\n\x0eINTERVAL_BLOCK\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x10\n\x0cINTERVAL_I1M\x10<\x12\x11\n\x0cINTERVAL_I5M\x10\xac\x02\x12\x12\n\rINTERVAL_I15M\x10\x84\x07\x12\x11\n\x0cINTERVAL_I1H\x10\x90\x1c\x12\x12\n\x0cINTERVAL_I6H\x10\xe0\xa8\x01\x12\x12\n\x0cINTERVAL_I1D\x10\x80\xa3\x05*\x94\x01\n\x0ePositionStatus\x12\x1f\n\x1bPOSITION_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dPOSITION_STATUS_ORDERS_CLOSED\x10\x01\x12\x1e\n\x1aPOSITION_STATUS_CLOSED_OUT\x10\x02\x12\x1e\n\x1aPOSITION_STATUS_DISTRESSED\x10\x04*\x81\x02\n\x0e\x41uctionTrigger\x12\x1f\n\x1b\x41UCTION_TRIGGER_UNSPECIFIED\x10\x00\x12\x19\n\x15\x41UCTION_TRIGGER_BATCH\x10\x01\x12\x1b\n\x17\x41UCTION_TRIGGER_OPENING\x10\x02\x12\x19\n\x15\x41UCTION_TRIGGER_PRICE\x10\x03\x12\x1d\n\x19\x41UCTION_TRIGGER_LIQUIDITY\x10\x04\x12,\n(AUCTION_TRIGGER_LIQUIDITY_TARGET_NOT_MET\x10\x05\x12.\n*AUCTION_TRIGGER_UNABLE_TO_DEPLOY_LP_ORDERS\x10\x06*\x8b\x01\n\x0fPeggedReference\x12 \n\x1cPEGGED_REFERENCE_UNSPECIFIED\x10\x00\x12\x18\n\x14PEGGED_REFERENCE_MID\x10\x01\x12\x1d\n\x19PEGGED_REFERENCE_BEST_BID\x10\x02\x12\x1d\n\x19PEGGED_REFERENCE_BEST_ASK\x10\x03*\xc9\x10\n\nOrderError\x12\x1b\n\x17ORDER_ERROR_UNSPECIFIED\x10\x00\x12!\n\x1dORDER_ERROR_INVALID_MARKET_ID\x10\x01\x12 \n\x1cORDER_ERROR_INVALID_ORDER_ID\x10\x02\x12\x1f\n\x1bORDER_ERROR_OUT_OF_SEQUENCE\x10\x03\x12&\n"ORDER_ERROR_INVALID_REMAINING_SIZE\x10\x04\x12\x1c\n\x18ORDER_ERROR_TIME_FAILURE\x10\x05\x12\x1f\n\x1bORDER_ERROR_REMOVAL_FAILURE\x10\x06\x12+\n\'ORDER_ERROR_INVALID_EXPIRATION_DATETIME\x10\x07\x12\'\n#ORDER_ERROR_INVALID_ORDER_REFERENCE\x10\x08\x12 \n\x1cORDER_ERROR_EDIT_NOT_ALLOWED\x10\t\x12\x1d\n\x19ORDER_ERROR_AMEND_FAILURE\x10\n\x12\x19\n\x15ORDER_ERROR_NOT_FOUND\x10\x0b\x12 \n\x1cORDER_ERROR_INVALID_PARTY_ID\x10\x0c\x12\x1d\n\x19ORDER_ERROR_MARKET_CLOSED\x10\r\x12#\n\x1fORDER_ERROR_MARGIN_CHECK_FAILED\x10\x0e\x12\'\n#ORDER_ERROR_MISSING_GENERAL_ACCOUNT\x10\x0f\x12\x1e\n\x1aORDER_ERROR_INTERNAL_ERROR\x10\x10\x12\x1c\n\x18ORDER_ERROR_INVALID_SIZE\x10\x11\x12#\n\x1fORDER_ERROR_INVALID_PERSISTENCE\x10\x12\x12\x1c\n\x18ORDER_ERROR_INVALID_TYPE\x10\x13\x12\x1c\n\x18ORDER_ERROR_SELF_TRADING\x10\x14\x12.\n*ORDER_ERROR_INSUFFICIENT_FUNDS_TO_PAY_FEES\x10\x15\x12%\n!ORDER_ERROR_INCORRECT_MARKET_TYPE\x10\x16\x12%\n!ORDER_ERROR_INVALID_TIME_IN_FORCE\x10\x17\x12\x37\n3ORDER_ERROR_CANNOT_SEND_GFN_ORDER_DURING_AN_AUCTION\x10\x18\x12?\n;ORDER_ERROR_CANNOT_SEND_GFA_ORDER_DURING_CONTINUOUS_TRADING\x10\x19\x12\x34\n0ORDER_ERROR_CANNOT_AMEND_TO_GTT_WITHOUT_EXPIRYAT\x10\x1a\x12)\n%ORDER_ERROR_EXPIRYAT_BEFORE_CREATEDAT\x10\x1b\x12,\n(ORDER_ERROR_CANNOT_HAVE_GTC_AND_EXPIRYAT\x10\x1c\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_FOK_OR_IOC\x10\x1d\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_GFA_OR_GFN\x10\x1e\x12,\n(ORDER_ERROR_CANNOT_AMEND_FROM_GFA_OR_GFN\x10\x1f\x12\x34\n0ORDER_ERROR_CANNOT_SEND_IOC_ORDER_DURING_AUCTION\x10 \x12\x34\n0ORDER_ERROR_CANNOT_SEND_FOK_ORDER_DURING_AUCTION\x10!\x12#\n\x1fORDER_ERROR_MUST_BE_LIMIT_ORDER\x10"\x12"\n\x1eORDER_ERROR_MUST_BE_GTT_OR_GTC\x10#\x12\'\n#ORDER_ERROR_WITHOUT_REFERENCE_PRICE\x10$\x12\x33\n/ORDER_ERROR_BUY_CANNOT_REFERENCE_BEST_ASK_PRICE\x10%\x12\x37\n3ORDER_ERROR_OFFSET_MUST_BE_GREATER_OR_EQUAL_TO_ZERO\x10(\x12\x34\n0ORDER_ERROR_SELL_CANNOT_REFERENCE_BEST_BID_PRICE\x10)\x12\x30\n,ORDER_ERROR_OFFSET_MUST_BE_GREATER_THAN_ZERO\x10*\x12*\n&ORDER_ERROR_INSUFFICIENT_ASSET_BALANCE\x10+\x12\x45\nAORDER_ERROR_CANNOT_AMEND_PEGGED_ORDER_DETAILS_ON_NON_PEGGED_ORDER\x10,\x12.\n*ORDER_ERROR_UNABLE_TO_REPRICE_PEGGED_ORDER\x10-\x12\x35\n1ORDER_ERROR_UNABLE_TO_AMEND_PRICE_ON_PEGGED_ORDER\x10.\x12\x38\n4ORDER_ERROR_NON_PERSISTENT_ORDER_OUT_OF_PRICE_BOUNDS\x10/\x12&\n"ORDER_ERROR_TOO_MANY_PEGGED_ORDERS\x10\x30\x12+\n\'ORDER_ERROR_POST_ONLY_ORDER_WOULD_TRADE\x10\x31\x12;\n7ORDER_ERROR_REDUCE_ONLY_ORDER_WOULD_NOT_REDUCE_POSITION\x10\x32"\x04\x08&\x10&"\x04\x08\'\x10\'*\x82\x01\n\x0b\x43hainStatus\x12\x1c\n\x18\x43HAIN_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43HAIN_STATUS_DISCONNECTED\x10\x01\x12\x1a\n\x16\x43HAIN_STATUS_REPLAYING\x10\x02\x12\x1a\n\x16\x43HAIN_STATUS_CONNECTED\x10\x03*\xde\x04\n\x0b\x41\x63\x63ountType\x12\x1c\n\x18\x41\x43\x43OUNT_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41\x43\x43OUNT_TYPE_INSURANCE\x10\x01\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_SETTLEMENT\x10\x02\x12\x17\n\x13\x41\x43\x43OUNT_TYPE_MARGIN\x10\x03\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_GENERAL\x10\x04\x12$\n ACCOUNT_TYPE_FEES_INFRASTRUCTURE\x10\x05\x12\x1f\n\x1b\x41\x43\x43OUNT_TYPE_FEES_LIQUIDITY\x10\x06\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_FEES_MAKER\x10\x07\x12\x15\n\x11\x41\x43\x43OUNT_TYPE_BOND\x10\t\x12\x19\n\x15\x41\x43\x43OUNT_TYPE_EXTERNAL\x10\n\x12!\n\x1d\x41\x43\x43OUNT_TYPE_GLOBAL_INSURANCE\x10\x0b\x12\x1e\n\x1a\x41\x43\x43OUNT_TYPE_GLOBAL_REWARD\x10\x0c\x12"\n\x1e\x41\x43\x43OUNT_TYPE_PENDING_TRANSFERS\x10\r\x12\'\n#ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES\x10\x0e\x12+\n\'ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES\x10\x0f\x12(\n$ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES\x10\x10\x12(\n$ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS\x10\x11\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_HOLDING\x10\x12"\x04\x08\x08\x10\x08*\xd4\x07\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TRANSFER_TYPE_LOSS\x10\x01\x12\x15\n\x11TRANSFER_TYPE_WIN\x10\x02\x12\x1a\n\x16TRANSFER_TYPE_MTM_LOSS\x10\x04\x12\x19\n\x15TRANSFER_TYPE_MTM_WIN\x10\x05\x12\x1c\n\x18TRANSFER_TYPE_MARGIN_LOW\x10\x06\x12\x1d\n\x19TRANSFER_TYPE_MARGIN_HIGH\x10\x07\x12$\n TRANSFER_TYPE_MARGIN_CONFISCATED\x10\x08\x12\x1f\n\x1bTRANSFER_TYPE_MAKER_FEE_PAY\x10\t\x12#\n\x1fTRANSFER_TYPE_MAKER_FEE_RECEIVE\x10\n\x12(\n$TRANSFER_TYPE_INFRASTRUCTURE_FEE_PAY\x10\x0b\x12/\n+TRANSFER_TYPE_INFRASTRUCTURE_FEE_DISTRIBUTE\x10\x0c\x12#\n\x1fTRANSFER_TYPE_LIQUIDITY_FEE_PAY\x10\r\x12*\n&TRANSFER_TYPE_LIQUIDITY_FEE_DISTRIBUTE\x10\x0e\x12\x1a\n\x16TRANSFER_TYPE_BOND_LOW\x10\x0f\x12\x1b\n\x17TRANSFER_TYPE_BOND_HIGH\x10\x10\x12\x1a\n\x16TRANSFER_TYPE_WITHDRAW\x10\x12\x12\x19\n\x15TRANSFER_TYPE_DEPOSIT\x10\x13\x12\x1f\n\x1bTRANSFER_TYPE_BOND_SLASHING\x10\x14\x12\x1f\n\x1bTRANSFER_TYPE_REWARD_PAYOUT\x10\x15\x12%\n!TRANSFER_TYPE_TRANSFER_FUNDS_SEND\x10\x16\x12+\n\'TRANSFER_TYPE_TRANSFER_FUNDS_DISTRIBUTE\x10\x17\x12\x1f\n\x1bTRANSFER_TYPE_CLEAR_ACCOUNT\x10\x18\x12,\n(TRANSFER_TYPE_CHECKPOINT_BALANCE_RESTORE\x10\x19\x12\x16\n\x12TRANSFER_TYPE_SPOT\x10\x1a\x12\x1e\n\x1aTRANSFER_TYPE_HOLDING_LOCK\x10\x1b\x12!\n\x1dTRANSFER_TYPE_HOLDING_RELEASE\x10\x1c\x12.\n*TRANSFER_TYPE_SUCCESSOR_INSURANCE_FRACTION\x10\x1d"\x04\x08\x03\x10\x03"\x04\x08\x11\x10\x11*\xc7\x01\n\x0e\x44ispatchMetric\x12\x1f\n\x1b\x44ISPATCH_METRIC_UNSPECIFIED\x10\x00\x12#\n\x1f\x44ISPATCH_METRIC_MAKER_FEES_PAID\x10\x01\x12\'\n#DISPATCH_METRIC_MAKER_FEES_RECEIVED\x10\x02\x12$\n DISPATCH_METRIC_LP_FEES_RECEIVED\x10\x03\x12 \n\x1c\x44ISPATCH_METRIC_MARKET_VALUE\x10\x04*c\n\nNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15NODE_STATUS_VALIDATOR\x10\x01\x12\x1d\n\x19NODE_STATUS_NON_VALIDATOR\x10\x02*Y\n\x0b\x45pochAction\x12\x1c\n\x18\x45POCH_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x45POCH_ACTION_START\x10\x01\x12\x14\n\x10\x45POCH_ACTION_END\x10\x02*\xa7\x01\n\x13ValidatorNodeStatus\x12%\n!VALIDATOR_NODE_STATUS_UNSPECIFIED\x10\x00\x12$\n VALIDATOR_NODE_STATUS_TENDERMINT\x10\x01\x12 \n\x1cVALIDATOR_NODE_STATUS_ERSATZ\x10\x02\x12!\n\x1dVALIDATOR_NODE_STATUS_PENDING\x10\x03\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x0fvega/vega.proto\x12\x04vega\x1a\x12vega/markets.proto"\xef\x07\n\tStopOrder\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\x0boco_link_id\x18\x02 \x01(\tH\x01R\tocoLinkId\x88\x01\x01\x12"\n\nexpires_at\x18\x03 \x01(\x03H\x02R\texpiresAt\x88\x01\x01\x12L\n\x0f\x65xpiry_strategy\x18\x04 \x01(\x0e\x32\x1e.vega.StopOrder.ExpiryStrategyH\x03R\x0e\x65xpiryStrategy\x88\x01\x01\x12M\n\x11trigger_direction\x18\x05 \x01(\x0e\x32 .vega.StopOrder.TriggerDirectionR\x10triggerDirection\x12.\n\x06status\x18\x06 \x01(\x0e\x32\x16.vega.StopOrder.StatusR\x06status\x12\x1d\n\ncreated_at\x18\x07 \x01(\x03R\tcreatedAt\x12"\n\nupdated_at\x18\x08 \x01(\x03H\x04R\tupdatedAt\x88\x01\x01\x12\x19\n\x08order_id\x18\t \x01(\tR\x07orderId\x12\x19\n\x08party_id\x18\n \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x0b \x01(\tR\x08marketId\x12\x16\n\x05price\x18\x64 \x01(\tH\x00R\x05price\x12\x38\n\x17trailing_percent_offset\x18\x65 \x01(\tH\x00R\x15trailingPercentOffset"j\n\x0e\x45xpiryStrategy\x12\x1f\n\x1b\x45XPIRY_STRATEGY_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x45XPIRY_STRATEGY_CANCELS\x10\x01\x12\x1a\n\x16\x45XPIRY_STRATEGY_SUBMIT\x10\x02"{\n\x10TriggerDirection\x12!\n\x1dTRIGGER_DIRECTION_UNSPECIFIED\x10\x00\x12!\n\x1dTRIGGER_DIRECTION_RISES_ABOVE\x10\x01\x12!\n\x1dTRIGGER_DIRECTION_FALLS_BELOW\x10\x02"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x12\n\x0eSTATUS_STOPPED\x10\x03\x12\x14\n\x10STATUS_TRIGGERED\x10\x04\x12\x12\n\x0eSTATUS_EXPIRED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x42\t\n\x07triggerB\x0e\n\x0c_oco_link_idB\r\n\x0b_expires_atB\x12\n\x10_expiry_strategyB\r\n\x0b_updated_at"\x17\n\x05Party\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"N\n\nRiskFactor\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05short\x18\x02 \x01(\tR\x05short\x12\x12\n\x04long\x18\x03 \x01(\tR\x04long"Z\n\x0bPeggedOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset"\x8c\x01\n\x0cIcebergOrder\x12\x1b\n\tpeak_size\x18\x01 \x01(\x04R\x08peakSize\x12\x30\n\x14minimum_visible_size\x18\x02 \x01(\x04R\x12minimumVisibleSize\x12-\n\x12reserved_remaining\x18\x03 \x01(\x04R\x11reservedRemaining"\x80\n\n\x05Order\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12\x12\n\x04size\x18\x06 \x01(\x04R\x04size\x12\x1c\n\tremaining\x18\x07 \x01(\x04R\tremaining\x12;\n\rtime_in_force\x18\x08 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12$\n\x04type\x18\t \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1d\n\ncreated_at\x18\n \x01(\x03R\tcreatedAt\x12*\n\x06status\x18\x0b \x01(\x0e\x32\x12.vega.Order.StatusR\x06status\x12\x1d\n\nexpires_at\x18\x0c \x01(\x03R\texpiresAt\x12\x1c\n\treference\x18\r \x01(\tR\treference\x12-\n\x06reason\x18\x0e \x01(\x0e\x32\x10.vega.OrderErrorH\x00R\x06reason\x88\x01\x01\x12\x1d\n\nupdated_at\x18\x0f \x01(\x03R\tupdatedAt\x12\x18\n\x07version\x18\x10 \x01(\x04R\x07version\x12\x19\n\x08\x62\x61tch_id\x18\x11 \x01(\x04R\x07\x62\x61tchId\x12\x34\n\x0cpegged_order\x18\x12 \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x34\n\x16liquidity_provision_id\x18\x13 \x01(\tR\x14liquidityProvisionId\x12\x1b\n\tpost_only\x18\x14 \x01(\x08R\x08postOnly\x12\x1f\n\x0breduce_only\x18\x15 \x01(\x08R\nreduceOnly\x12<\n\riceberg_order\x18\x16 \x01(\x0b\x32\x12.vega.IcebergOrderH\x01R\x0cicebergOrder\x88\x01\x01"\xb6\x01\n\x0bTimeInForce\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_GTC\x10\x01\x12\x15\n\x11TIME_IN_FORCE_GTT\x10\x02\x12\x15\n\x11TIME_IN_FORCE_IOC\x10\x03\x12\x15\n\x11TIME_IN_FORCE_FOK\x10\x04\x12\x15\n\x11TIME_IN_FORCE_GFA\x10\x05\x12\x15\n\x11TIME_IN_FORCE_GFN\x10\x06"O\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_LIMIT\x10\x01\x12\x0f\n\x0bTYPE_MARKET\x10\x02\x12\x10\n\x0cTYPE_NETWORK\x10\x03"\xc9\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_EXPIRED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x11\n\rSTATUS_FILLED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x12\x1b\n\x17STATUS_PARTIALLY_FILLED\x10\x07\x12\x11\n\rSTATUS_PARKED\x10\x08\x42\t\n\x07_reasonB\x10\n\x0e_iceberg_order"B\n\x1dOrderCancellationConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xa0\x01\n\x11OrderConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order\x12#\n\x06trades\x18\x02 \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x43\n\x17passive_orders_affected\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x15passiveOrdersAffected"\xd3\x01\n\x16\x41uctionIndicativeState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12)\n\x10indicative_price\x18\x02 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x03 \x01(\x04R\x10indicativeVolume\x12#\n\rauction_start\x18\x04 \x01(\x03R\x0c\x61uctionStart\x12\x1f\n\x0b\x61uction_end\x18\x05 \x01(\x03R\nauctionEnd"\xdb\x04\n\x05Trade\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12\x12\n\x04size\x18\x04 \x01(\x04R\x04size\x12\x14\n\x05\x62uyer\x18\x05 \x01(\tR\x05\x62uyer\x12\x16\n\x06seller\x18\x06 \x01(\tR\x06seller\x12(\n\taggressor\x18\x07 \x01(\x0e\x32\n.vega.SideR\taggressor\x12\x1b\n\tbuy_order\x18\x08 \x01(\tR\x08\x62uyOrder\x12\x1d\n\nsell_order\x18\t \x01(\tR\tsellOrder\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12$\n\x04type\x18\x0b \x01(\x0e\x32\x10.vega.Trade.TypeR\x04type\x12&\n\tbuyer_fee\x18\x0c \x01(\x0b\x32\t.vega.FeeR\x08\x62uyerFee\x12(\n\nseller_fee\x18\r \x01(\x0b\x32\t.vega.FeeR\tsellerFee\x12.\n\x13\x62uyer_auction_batch\x18\x0e \x01(\x04R\x11\x62uyerAuctionBatch\x12\x30\n\x14seller_auction_batch\x18\x0f \x01(\x04R\x12sellerAuctionBatch"o\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cTYPE_DEFAULT\x10\x01\x12\x1f\n\x1bTYPE_NETWORK_CLOSE_OUT_GOOD\x10\x02\x12\x1e\n\x1aTYPE_NETWORK_CLOSE_OUT_BAD\x10\x03"v\n\x03\x46\x65\x65\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"/\n\x08TradeSet\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"\xf2\x01\n\x06\x43\x61ndle\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x1a\n\x08\x64\x61tetime\x18\x02 \x01(\tR\x08\x64\x61tetime\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12*\n\x08interval\x18\x08 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval\x12\x1a\n\x08notional\x18\t \x01(\x04R\x08notional"d\n\nPriceLevel\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12(\n\x10number_of_orders\x18\x02 \x01(\x04R\x0enumberOfOrders\x12\x16\n\x06volume\x18\x03 \x01(\x04R\x06volume"\x9d\x01\n\x0bMarketDepth\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber"\xdd\x01\n\x11MarketDepthUpdate\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber\x12\x38\n\x18previous_sequence_number\x18\x05 \x01(\x04R\x16previousSequenceNumber"\xf7\x02\n\x08Position\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1f\n\x0bopen_volume\x18\x03 \x01(\x03R\nopenVolume\x12!\n\x0crealised_pnl\x18\x04 \x01(\tR\x0brealisedPnl\x12%\n\x0eunrealised_pnl\x18\x05 \x01(\tR\runrealisedPnl\x12.\n\x13\x61verage_entry_price\x18\x06 \x01(\tR\x11\x61verageEntryPrice\x12\x1d\n\nupdated_at\x18\x07 \x01(\x03R\tupdatedAt\x12:\n\x19loss_socialisation_amount\x18\x08 \x01(\tR\x17lossSocialisationAmount\x12=\n\x0fposition_status\x18\t \x01(\x0e\x32\x14.vega.PositionStatusR\x0epositionStatus"=\n\rPositionTrade\x12\x16\n\x06volume\x18\x01 \x01(\x03R\x06volume\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price"\xe4\x02\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x14.vega.Deposit.StatusR\x06status\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12-\n\x12\x63redited_timestamp\x18\x07 \x01(\x03R\x11\x63reditedTimestamp\x12+\n\x11\x63reated_timestamp\x18\x08 \x01(\x03R\x10\x63reatedTimestamp"]\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03"\xa8\x03\n\nWithdrawal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12/\n\x06status\x18\x05 \x01(\x0e\x32\x17.vega.Withdrawal.StatusR\x06status\x12\x10\n\x03ref\x18\x06 \x01(\tR\x03ref\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12+\n\x11\x63reated_timestamp\x18\t \x01(\x03R\x10\x63reatedTimestamp\x12/\n\x13withdrawn_timestamp\x18\n \x01(\x03R\x12withdrawnTimestamp\x12#\n\x03\x65xt\x18\x0b \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\\\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03J\x04\x08\x07\x10\x08"D\n\x0bWithdrawExt\x12.\n\x05\x65rc20\x18\x01 \x01(\x0b\x32\x16.vega.Erc20WithdrawExtH\x00R\x05\x65rc20B\x05\n\x03\x65xt"=\n\x10\x45rc20WithdrawExt\x12)\n\x10receiver_address\x18\x01 \x01(\tR\x0freceiverAddress"\xa3\x01\n\x07\x41\x63\x63ount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"?\n\x0f\x46inancialAmount\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset"\xb3\x01\n\x08Transfer\x12\x14\n\x05owner\x18\x01 \x01(\tR\x05owner\x12-\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x15.vega.FinancialAmountR\x06\x61mount\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId"\x84\x01\n\x10\x44ispatchStrategy\x12(\n\x10\x61sset_for_metric\x18\x01 \x01(\tR\x0e\x61ssetForMetric\x12,\n\x06metric\x18\x02 \x01(\x0e\x32\x14.vega.DispatchMetricR\x06metric\x12\x18\n\x07markets\x18\x03 \x03(\tR\x07markets"\xe6\x01\n\x0fTransferRequest\x12\x30\n\x0c\x66rom_account\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x0b\x66romAccount\x12,\n\nto_account\x18\x02 \x03(\x0b\x32\r.vega.AccountR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12&\n\x04type\x18\x07 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type"\xa7\x01\n\x0e\x41\x63\x63ountDetails\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type\x12\x19\n\x05owner\x18\x03 \x01(\tH\x00R\x05owner\x88\x01\x01\x12 \n\tmarket_id\x18\x04 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x08\n\x06_ownerB\x0c\n\n_market_id"\xb9\x02\n\x0bLedgerEntry\x12\x37\n\x0c\x66rom_account\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x0b\x66romAccount\x12\x33\n\nto_account\x18\x02 \x01(\x0b\x32\x14.vega.AccountDetailsR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12&\n\x04type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x30\n\x14\x66rom_account_balance\x18\x06 \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\x07 \x01(\tR\x10toAccountBalance"_\n\x13PostTransferBalance\x12.\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x07\x61\x63\x63ount\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"t\n\x0eLedgerMovement\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.vega.LedgerEntryR\x07\x65ntries\x12\x35\n\x08\x62\x61lances\x18\x02 \x03(\x0b\x32\x19.vega.PostTransferBalanceR\x08\x62\x61lances"\xad\x02\n\x0cMarginLevels\x12-\n\x12maintenance_margin\x18\x01 \x01(\tR\x11maintenanceMargin\x12!\n\x0csearch_level\x18\x02 \x01(\tR\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x03 \x01(\tR\rinitialMargin\x12\x38\n\x18\x63ollateral_release_level\x18\x04 \x01(\tR\x16\x63ollateralReleaseLevel\x12\x19\n\x08party_id\x18\x05 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x06 \x01(\tR\x08marketId\x12\x14\n\x05\x61sset\x18\x07 \x01(\tR\x05\x61sset\x12\x1c\n\ttimestamp\x18\x08 \x01(\x03R\ttimestamp"\x8a\x0b\n\nMarketData\x12\x1d\n\nmark_price\x18\x01 \x01(\tR\tmarkPrice\x12$\n\x0e\x62\x65st_bid_price\x18\x02 \x01(\tR\x0c\x62\x65stBidPrice\x12&\n\x0f\x62\x65st_bid_volume\x18\x03 \x01(\x04R\rbestBidVolume\x12(\n\x10\x62\x65st_offer_price\x18\x04 \x01(\tR\x0e\x62\x65stOfferPrice\x12*\n\x11\x62\x65st_offer_volume\x18\x05 \x01(\x04R\x0f\x62\x65stOfferVolume\x12\x31\n\x15\x62\x65st_static_bid_price\x18\x06 \x01(\tR\x12\x62\x65stStaticBidPrice\x12\x33\n\x16\x62\x65st_static_bid_volume\x18\x07 \x01(\x04R\x13\x62\x65stStaticBidVolume\x12\x35\n\x17\x62\x65st_static_offer_price\x18\x08 \x01(\tR\x14\x62\x65stStaticOfferPrice\x12\x37\n\x18\x62\x65st_static_offer_volume\x18\t \x01(\x04R\x15\x62\x65stStaticOfferVolume\x12\x1b\n\tmid_price\x18\n \x01(\tR\x08midPrice\x12(\n\x10static_mid_price\x18\x0b \x01(\tR\x0estaticMidPrice\x12\x16\n\x06market\x18\x0c \x01(\tR\x06market\x12\x1c\n\ttimestamp\x18\r \x01(\x03R\ttimestamp\x12#\n\ropen_interest\x18\x0e \x01(\x04R\x0copenInterest\x12\x1f\n\x0b\x61uction_end\x18\x0f \x01(\x03R\nauctionEnd\x12#\n\rauction_start\x18\x10 \x01(\x03R\x0c\x61uctionStart\x12)\n\x10indicative_price\x18\x11 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x12 \x01(\x04R\x10indicativeVolume\x12H\n\x13market_trading_mode\x18\x13 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x11marketTradingMode\x12.\n\x07trigger\x18\x14 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x15 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger\x12!\n\x0ctarget_stake\x18\x16 \x01(\tR\x0btargetStake\x12%\n\x0esupplied_stake\x18\x17 \x01(\tR\rsuppliedStake\x12S\n\x17price_monitoring_bounds\x18\x18 \x03(\x0b\x32\x1b.vega.PriceMonitoringBoundsR\x15priceMonitoringBounds\x12,\n\x12market_value_proxy\x18\x19 \x01(\tR\x10marketValueProxy\x12`\n\x1cliquidity_provider_fee_share\x18\x1a \x03(\x0b\x32\x1f.vega.LiquidityProviderFeeShareR\x19liquidityProviderFeeShare\x12\x35\n\x0cmarket_state\x18\x1b \x01(\x0e\x32\x12.vega.Market.StateR\x0bmarketState\x12-\n\x13next_mark_to_market\x18\x1c \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x1d \x01(\tR\x0flastTradedPrice\x12#\n\rmarket_growth\x18\x1e \x01(\tR\x0cmarketGrowth"\xdf\x01\n\x19LiquidityProviderFeeShare\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12*\n\x11\x65quity_like_share\x18\x02 \x01(\tR\x0f\x65quityLikeShare\x12\x36\n\x17\x61verage_entry_valuation\x18\x03 \x01(\tR\x15\x61verageEntryValuation\x12#\n\raverage_score\x18\x04 \x01(\tR\x0c\x61verageScore\x12#\n\rvirtual_stake\x18\x05 \x01(\tR\x0cvirtualStake"\xc8\x01\n\x15PriceMonitoringBounds\x12&\n\x0fmin_valid_price\x18\x01 \x01(\tR\rminValidPrice\x12&\n\x0fmax_valid_price\x18\x02 \x01(\tR\rmaxValidPrice\x12\x36\n\x07trigger\x18\x03 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger\x12\'\n\x0freference_price\x18\x04 \x01(\tR\x0ereferencePrice"Q\n\x0b\x45rrorDetail\x12\x12\n\x04\x63ode\x18\x01 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x14\n\x05inner\x18\x03 \x01(\tR\x05inner":\n\x10NetworkParameter\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\x82\x03\n\rNetworkLimits\x12,\n\x12\x63\x61n_propose_market\x18\x01 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x02 \x01(\x08R\x0f\x63\x61nProposeAsset\x12\x34\n\x16propose_market_enabled\x18\x04 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x05 \x01(\x08R\x13proposeAssetEnabled\x12%\n\x0egenesis_loaded\x18\x07 \x01(\x08R\rgenesisLoaded\x12=\n\x1bpropose_market_enabled_from\x18\x08 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\t \x01(\x03R\x17proposeAssetEnabledFromJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07"}\n\x0eLiquidityOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x1e\n\nproportion\x18\x02 \x01(\rR\nproportion\x12\x16\n\x06offset\x18\x03 \x01(\tR\x06offset"s\n\x17LiquidityOrderReference\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12=\n\x0fliquidity_order\x18\x02 \x01(\x0b\x32\x14.vega.LiquidityOrderR\x0eliquidityOrder"\xd2\x04\n\x12LiquidityProvision\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1d\n\ncreated_at\x18\x03 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x04 \x01(\x03R\tupdatedAt\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x06 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x07 \x01(\tR\x03\x66\x65\x65\x12\x33\n\x05sells\x18\x08 \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x05sells\x12\x31\n\x04\x62uys\x18\t \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x04\x62uys\x12\x18\n\x07version\x18\n \x01(\x04R\x07version\x12\x37\n\x06status\x18\x0b \x01(\x0e\x32\x1f.vega.LiquidityProvision.StatusR\x06status\x12\x1c\n\treference\x18\x0c \x01(\tR\treference"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_STOPPED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x13\n\x0fSTATUS_REJECTED\x10\x04\x12\x15\n\x11STATUS_UNDEPLOYED\x10\x05\x12\x12\n\x0eSTATUS_PENDING\x10\x06"\xd0\x03\n\x0e\x45thereumConfig\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12\x19\n\x08\x63hain_id\x18\x02 \x01(\tR\x07\x63hainId\x12Z\n\x1a\x63ollateral_bridge_contract\x18\x03 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x18\x63ollateralBridgeContract\x12$\n\rconfirmations\x18\x04 \x01(\rR\rconfirmations\x12T\n\x17staking_bridge_contract\x18\x05 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x15stakingBridgeContract\x12R\n\x16token_vesting_contract\x18\x06 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x14tokenVestingContract\x12X\n\x19multisig_control_contract\x18\x07 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x17multisigControlContract"j\n\x16\x45thereumContractConfig\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x36\n\x17\x64\x65ployment_block_height\x18\x06 \x01(\x04R\x15\x64\x65ploymentBlockHeight"\xac\x01\n\x0f\x45pochTimestamps\x12\x1d\n\nstart_time\x18\x01 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpiry_time\x18\x02 \x01(\x03R\nexpiryTime\x12\x19\n\x08\x65nd_time\x18\x03 \x01(\x03R\x07\x65ndTime\x12\x1f\n\x0b\x66irst_block\x18\x04 \x01(\x04R\nfirstBlock\x12\x1d\n\nlast_block\x18\x05 \x01(\x04R\tlastBlock"\xb0\x01\n\x05\x45poch\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x35\n\ntimestamps\x18\x02 \x01(\x0b\x32\x15.vega.EpochTimestampsR\ntimestamps\x12*\n\nvalidators\x18\x03 \x03(\x0b\x32\n.vega.NodeR\nvalidators\x12\x32\n\x0b\x64\x65legations\x18\x04 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"\x8e\x01\n\x12\x45pochParticipation\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch\x12\x18\n\x07offline\x18\x02 \x01(\x04R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x04R\x06online\x12#\n\rtotal_rewards\x18\x04 \x01(\x01R\x0ctotalRewards"S\n\tEpochData\x12\x14\n\x05total\x18\x01 \x01(\x05R\x05total\x12\x18\n\x07offline\x18\x02 \x01(\x05R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x05R\x06online"\x9b\x02\n\x0cRankingScore\x12\x1f\n\x0bstake_score\x18\x01 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12\x42\n\x0fprevious_status\x18\x03 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0epreviousStatus\x12\x31\n\x06status\x18\x04 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x06status\x12!\n\x0cvoting_power\x18\x05 \x01(\rR\x0bvotingPower\x12#\n\rranking_score\x18\x06 \x01(\tR\x0crankingScore"\xab\x02\n\x0bRewardScore\x12.\n\x13raw_validator_score\x18\x01 \x01(\tR\x11rawValidatorScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12%\n\x0emultisig_score\x18\x03 \x01(\tR\rmultisigScore\x12\'\n\x0fvalidator_score\x18\x04 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x05 \x01(\tR\x0fnormalisedScore\x12\x44\n\x10validator_status\x18\x06 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0fvalidatorStatus"\xb3\x05\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12,\n\x12staked_by_operator\x18\x07 \x01(\tR\x10stakedByOperator\x12.\n\x13staked_by_delegates\x18\x08 \x01(\tR\x11stakedByDelegates\x12!\n\x0cstaked_total\x18\t \x01(\tR\x0bstakedTotal\x12,\n\x12max_intended_stake\x18\n \x01(\tR\x10maxIntendedStake\x12#\n\rpending_stake\x18\x0b \x01(\tR\x0cpendingStake\x12.\n\nepoch_data\x18\x0c \x01(\x0b\x32\x0f.vega.EpochDataR\tepochData\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x32\n\x0b\x64\x65legations\x18\x0e \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0creward_score\x18\x0f \x01(\x0b\x32\x11.vega.RewardScoreR\x0brewardScore\x12\x37\n\rranking_score\x18\x10 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x9c\x01\n\x07NodeSet\x12\x14\n\x05total\x18\x01 \x01(\rR\x05total\x12\x1a\n\x08inactive\x18\x02 \x01(\rR\x08inactive\x12\x1a\n\x08promoted\x18\x03 \x03(\tR\x08promoted\x12\x18\n\x07\x64\x65moted\x18\x04 \x03(\tR\x07\x64\x65moted\x12\x1d\n\x07maximum\x18\x05 \x01(\rH\x00R\x07maximum\x88\x01\x01\x42\n\n\x08_maximum"\xad\x02\n\x08NodeData\x12!\n\x0cstaked_total\x18\x01 \x01(\tR\x0bstakedTotal\x12\x1f\n\x0btotal_nodes\x18\x02 \x01(\rR\ntotalNodes\x12%\n\x0einactive_nodes\x18\x03 \x01(\rR\rinactiveNodes\x12\x38\n\x10tendermint_nodes\x18\x04 \x01(\x0b\x32\r.vega.NodeSetR\x0ftendermintNodes\x12\x30\n\x0c\x65rsatz_nodes\x18\x05 \x01(\x0b\x32\r.vega.NodeSetR\x0b\x65rsatzNodes\x12\x32\n\rpending_nodes\x18\x06 \x01(\x0b\x32\r.vega.NodeSetR\x0cpendingNodes\x12\x16\n\x06uptime\x18\x07 \x01(\x02R\x06uptime"p\n\nDelegation\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"\xfb\x01\n\x06Reward\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x65poch\x18\x03 \x01(\x04R\x05\x65poch\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12.\n\x13percentage_of_total\x18\x05 \x01(\tR\x11percentageOfTotal\x12\x1f\n\x0breceived_at\x18\x06 \x01(\x03R\nreceivedAt\x12\x1b\n\tmarket_id\x18\x07 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x08 \x01(\tR\nrewardType"]\n\rRewardSummary\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x9b\x01\n\x12\x45pochRewardSummary\x12\x14\n\x05\x65poch\x18\x01 \x01(\x04R\x05\x65poch\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x04 \x01(\tR\nrewardType\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount"y\n\x12StateValueProposal\x12 \n\x0cstate_var_id\x18\x01 \x01(\tR\nstateVarId\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12&\n\x03kvb\x18\x03 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x03kvb"k\n\x0eKeyValueBundle\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x1c\n\ttolerance\x18\x02 \x01(\tR\ttolerance\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x13.vega.StateVarValueR\x05value"\xb4\x01\n\rStateVarValue\x12\x32\n\nscalar_val\x18\x01 \x01(\x0b\x32\x11.vega.ScalarValueH\x00R\tscalarVal\x12\x32\n\nvector_val\x18\x02 \x01(\x0b\x32\x11.vega.VectorValueH\x00R\tvectorVal\x12\x32\n\nmatrix_val\x18\x03 \x01(\x0b\x32\x11.vega.MatrixValueH\x00R\tmatrixValB\x07\n\x05value"#\n\x0bScalarValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value"#\n\x0bVectorValue\x12\x14\n\x05value\x18\x01 \x03(\tR\x05value"6\n\x0bMatrixValue\x12\'\n\x05value\x18\x01 \x03(\x0b\x32\x11.vega.VectorValueR\x05value*9\n\x04Side\x12\x14\n\x10SIDE_UNSPECIFIED\x10\x00\x12\x0c\n\x08SIDE_BUY\x10\x01\x12\r\n\tSIDE_SELL\x10\x02*\xb5\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x1b\n\x0eINTERVAL_BLOCK\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x10\n\x0cINTERVAL_I1M\x10<\x12\x11\n\x0cINTERVAL_I5M\x10\xac\x02\x12\x12\n\rINTERVAL_I15M\x10\x84\x07\x12\x11\n\x0cINTERVAL_I1H\x10\x90\x1c\x12\x12\n\x0cINTERVAL_I6H\x10\xe0\xa8\x01\x12\x12\n\x0cINTERVAL_I1D\x10\x80\xa3\x05*\x94\x01\n\x0ePositionStatus\x12\x1f\n\x1bPOSITION_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dPOSITION_STATUS_ORDERS_CLOSED\x10\x01\x12\x1e\n\x1aPOSITION_STATUS_CLOSED_OUT\x10\x02\x12\x1e\n\x1aPOSITION_STATUS_DISTRESSED\x10\x04*\x81\x02\n\x0e\x41uctionTrigger\x12\x1f\n\x1b\x41UCTION_TRIGGER_UNSPECIFIED\x10\x00\x12\x19\n\x15\x41UCTION_TRIGGER_BATCH\x10\x01\x12\x1b\n\x17\x41UCTION_TRIGGER_OPENING\x10\x02\x12\x19\n\x15\x41UCTION_TRIGGER_PRICE\x10\x03\x12\x1d\n\x19\x41UCTION_TRIGGER_LIQUIDITY\x10\x04\x12,\n(AUCTION_TRIGGER_LIQUIDITY_TARGET_NOT_MET\x10\x05\x12.\n*AUCTION_TRIGGER_UNABLE_TO_DEPLOY_LP_ORDERS\x10\x06*\x8b\x01\n\x0fPeggedReference\x12 \n\x1cPEGGED_REFERENCE_UNSPECIFIED\x10\x00\x12\x18\n\x14PEGGED_REFERENCE_MID\x10\x01\x12\x1d\n\x19PEGGED_REFERENCE_BEST_BID\x10\x02\x12\x1d\n\x19PEGGED_REFERENCE_BEST_ASK\x10\x03*\xc9\x10\n\nOrderError\x12\x1b\n\x17ORDER_ERROR_UNSPECIFIED\x10\x00\x12!\n\x1dORDER_ERROR_INVALID_MARKET_ID\x10\x01\x12 \n\x1cORDER_ERROR_INVALID_ORDER_ID\x10\x02\x12\x1f\n\x1bORDER_ERROR_OUT_OF_SEQUENCE\x10\x03\x12&\n"ORDER_ERROR_INVALID_REMAINING_SIZE\x10\x04\x12\x1c\n\x18ORDER_ERROR_TIME_FAILURE\x10\x05\x12\x1f\n\x1bORDER_ERROR_REMOVAL_FAILURE\x10\x06\x12+\n\'ORDER_ERROR_INVALID_EXPIRATION_DATETIME\x10\x07\x12\'\n#ORDER_ERROR_INVALID_ORDER_REFERENCE\x10\x08\x12 \n\x1cORDER_ERROR_EDIT_NOT_ALLOWED\x10\t\x12\x1d\n\x19ORDER_ERROR_AMEND_FAILURE\x10\n\x12\x19\n\x15ORDER_ERROR_NOT_FOUND\x10\x0b\x12 \n\x1cORDER_ERROR_INVALID_PARTY_ID\x10\x0c\x12\x1d\n\x19ORDER_ERROR_MARKET_CLOSED\x10\r\x12#\n\x1fORDER_ERROR_MARGIN_CHECK_FAILED\x10\x0e\x12\'\n#ORDER_ERROR_MISSING_GENERAL_ACCOUNT\x10\x0f\x12\x1e\n\x1aORDER_ERROR_INTERNAL_ERROR\x10\x10\x12\x1c\n\x18ORDER_ERROR_INVALID_SIZE\x10\x11\x12#\n\x1fORDER_ERROR_INVALID_PERSISTENCE\x10\x12\x12\x1c\n\x18ORDER_ERROR_INVALID_TYPE\x10\x13\x12\x1c\n\x18ORDER_ERROR_SELF_TRADING\x10\x14\x12.\n*ORDER_ERROR_INSUFFICIENT_FUNDS_TO_PAY_FEES\x10\x15\x12%\n!ORDER_ERROR_INCORRECT_MARKET_TYPE\x10\x16\x12%\n!ORDER_ERROR_INVALID_TIME_IN_FORCE\x10\x17\x12\x37\n3ORDER_ERROR_CANNOT_SEND_GFN_ORDER_DURING_AN_AUCTION\x10\x18\x12?\n;ORDER_ERROR_CANNOT_SEND_GFA_ORDER_DURING_CONTINUOUS_TRADING\x10\x19\x12\x34\n0ORDER_ERROR_CANNOT_AMEND_TO_GTT_WITHOUT_EXPIRYAT\x10\x1a\x12)\n%ORDER_ERROR_EXPIRYAT_BEFORE_CREATEDAT\x10\x1b\x12,\n(ORDER_ERROR_CANNOT_HAVE_GTC_AND_EXPIRYAT\x10\x1c\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_FOK_OR_IOC\x10\x1d\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_GFA_OR_GFN\x10\x1e\x12,\n(ORDER_ERROR_CANNOT_AMEND_FROM_GFA_OR_GFN\x10\x1f\x12\x34\n0ORDER_ERROR_CANNOT_SEND_IOC_ORDER_DURING_AUCTION\x10 \x12\x34\n0ORDER_ERROR_CANNOT_SEND_FOK_ORDER_DURING_AUCTION\x10!\x12#\n\x1fORDER_ERROR_MUST_BE_LIMIT_ORDER\x10"\x12"\n\x1eORDER_ERROR_MUST_BE_GTT_OR_GTC\x10#\x12\'\n#ORDER_ERROR_WITHOUT_REFERENCE_PRICE\x10$\x12\x33\n/ORDER_ERROR_BUY_CANNOT_REFERENCE_BEST_ASK_PRICE\x10%\x12\x37\n3ORDER_ERROR_OFFSET_MUST_BE_GREATER_OR_EQUAL_TO_ZERO\x10(\x12\x34\n0ORDER_ERROR_SELL_CANNOT_REFERENCE_BEST_BID_PRICE\x10)\x12\x30\n,ORDER_ERROR_OFFSET_MUST_BE_GREATER_THAN_ZERO\x10*\x12*\n&ORDER_ERROR_INSUFFICIENT_ASSET_BALANCE\x10+\x12\x45\nAORDER_ERROR_CANNOT_AMEND_PEGGED_ORDER_DETAILS_ON_NON_PEGGED_ORDER\x10,\x12.\n*ORDER_ERROR_UNABLE_TO_REPRICE_PEGGED_ORDER\x10-\x12\x35\n1ORDER_ERROR_UNABLE_TO_AMEND_PRICE_ON_PEGGED_ORDER\x10.\x12\x38\n4ORDER_ERROR_NON_PERSISTENT_ORDER_OUT_OF_PRICE_BOUNDS\x10/\x12&\n"ORDER_ERROR_TOO_MANY_PEGGED_ORDERS\x10\x30\x12+\n\'ORDER_ERROR_POST_ONLY_ORDER_WOULD_TRADE\x10\x31\x12;\n7ORDER_ERROR_REDUCE_ONLY_ORDER_WOULD_NOT_REDUCE_POSITION\x10\x32"\x04\x08&\x10&"\x04\x08\'\x10\'*\x82\x01\n\x0b\x43hainStatus\x12\x1c\n\x18\x43HAIN_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43HAIN_STATUS_DISCONNECTED\x10\x01\x12\x1a\n\x16\x43HAIN_STATUS_REPLAYING\x10\x02\x12\x1a\n\x16\x43HAIN_STATUS_CONNECTED\x10\x03*\xb6\x05\n\x0b\x41\x63\x63ountType\x12\x1c\n\x18\x41\x43\x43OUNT_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41\x43\x43OUNT_TYPE_INSURANCE\x10\x01\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_SETTLEMENT\x10\x02\x12\x17\n\x13\x41\x43\x43OUNT_TYPE_MARGIN\x10\x03\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_GENERAL\x10\x04\x12$\n ACCOUNT_TYPE_FEES_INFRASTRUCTURE\x10\x05\x12\x1f\n\x1b\x41\x43\x43OUNT_TYPE_FEES_LIQUIDITY\x10\x06\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_FEES_MAKER\x10\x07\x12\x15\n\x11\x41\x43\x43OUNT_TYPE_BOND\x10\t\x12\x19\n\x15\x41\x43\x43OUNT_TYPE_EXTERNAL\x10\n\x12!\n\x1d\x41\x43\x43OUNT_TYPE_GLOBAL_INSURANCE\x10\x0b\x12\x1e\n\x1a\x41\x43\x43OUNT_TYPE_GLOBAL_REWARD\x10\x0c\x12"\n\x1e\x41\x43\x43OUNT_TYPE_PENDING_TRANSFERS\x10\r\x12\'\n#ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES\x10\x0e\x12+\n\'ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES\x10\x0f\x12(\n$ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES\x10\x10\x12(\n$ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS\x10\x11\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_HOLDING\x10\x12\x12"\n\x1e\x41\x43\x43OUNT_TYPE_LP_LIQUIDITY_FEES\x10\x13\x12\x32\n.ACCOUNT_TYPE_LIQUIDITY_FEES_BONUS_DISTRIBUTION\x10\x14"\x04\x08\x08\x10\x08*\xe8\t\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TRANSFER_TYPE_LOSS\x10\x01\x12\x15\n\x11TRANSFER_TYPE_WIN\x10\x02\x12\x1a\n\x16TRANSFER_TYPE_MTM_LOSS\x10\x04\x12\x19\n\x15TRANSFER_TYPE_MTM_WIN\x10\x05\x12\x1c\n\x18TRANSFER_TYPE_MARGIN_LOW\x10\x06\x12\x1d\n\x19TRANSFER_TYPE_MARGIN_HIGH\x10\x07\x12$\n TRANSFER_TYPE_MARGIN_CONFISCATED\x10\x08\x12\x1f\n\x1bTRANSFER_TYPE_MAKER_FEE_PAY\x10\t\x12#\n\x1fTRANSFER_TYPE_MAKER_FEE_RECEIVE\x10\n\x12(\n$TRANSFER_TYPE_INFRASTRUCTURE_FEE_PAY\x10\x0b\x12/\n+TRANSFER_TYPE_INFRASTRUCTURE_FEE_DISTRIBUTE\x10\x0c\x12#\n\x1fTRANSFER_TYPE_LIQUIDITY_FEE_PAY\x10\r\x12*\n&TRANSFER_TYPE_LIQUIDITY_FEE_DISTRIBUTE\x10\x0e\x12\x1a\n\x16TRANSFER_TYPE_BOND_LOW\x10\x0f\x12\x1b\n\x17TRANSFER_TYPE_BOND_HIGH\x10\x10\x12\x1a\n\x16TRANSFER_TYPE_WITHDRAW\x10\x12\x12\x19\n\x15TRANSFER_TYPE_DEPOSIT\x10\x13\x12\x1f\n\x1bTRANSFER_TYPE_BOND_SLASHING\x10\x14\x12\x1f\n\x1bTRANSFER_TYPE_REWARD_PAYOUT\x10\x15\x12%\n!TRANSFER_TYPE_TRANSFER_FUNDS_SEND\x10\x16\x12+\n\'TRANSFER_TYPE_TRANSFER_FUNDS_DISTRIBUTE\x10\x17\x12\x1f\n\x1bTRANSFER_TYPE_CLEAR_ACCOUNT\x10\x18\x12,\n(TRANSFER_TYPE_CHECKPOINT_BALANCE_RESTORE\x10\x19\x12\x16\n\x12TRANSFER_TYPE_SPOT\x10\x1a\x12\x1e\n\x1aTRANSFER_TYPE_HOLDING_LOCK\x10\x1b\x12!\n\x1dTRANSFER_TYPE_HOLDING_RELEASE\x10\x1c\x12.\n*TRANSFER_TYPE_SUCCESSOR_INSURANCE_FRACTION\x10\x1d\x12(\n$TRANSFER_TYPE_LIQUIDITY_FEE_ALLOCATE\x10\x1e\x12.\n*TRANSFER_TYPE_LIQUIDITY_FEE_NET_DISTRIBUTE\x10\x1f\x12(\n$TRANSFER_TYPE_SLA_PENALTY_BOND_APPLY\x10 \x12*\n&TRANSFER_TYPE_SLA_PENALTY_LP_FEE_APPLY\x10!\x12.\n*TRANSFER_TYPE_LIQUIDITY_FEE_UNPAID_COLLECT\x10"\x12\x32\n.TRANSFER_TYPE_SLA_PERFORMANCE_BONUS_DISTRIBUTE\x10#"\x04\x08\x03\x10\x03"\x04\x08\x11\x10\x11*\xc7\x01\n\x0e\x44ispatchMetric\x12\x1f\n\x1b\x44ISPATCH_METRIC_UNSPECIFIED\x10\x00\x12#\n\x1f\x44ISPATCH_METRIC_MAKER_FEES_PAID\x10\x01\x12\'\n#DISPATCH_METRIC_MAKER_FEES_RECEIVED\x10\x02\x12$\n DISPATCH_METRIC_LP_FEES_RECEIVED\x10\x03\x12 \n\x1c\x44ISPATCH_METRIC_MARKET_VALUE\x10\x04*c\n\nNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15NODE_STATUS_VALIDATOR\x10\x01\x12\x1d\n\x19NODE_STATUS_NON_VALIDATOR\x10\x02*Y\n\x0b\x45pochAction\x12\x1c\n\x18\x45POCH_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x45POCH_ACTION_START\x10\x01\x12\x14\n\x10\x45POCH_ACTION_END\x10\x02*\xa7\x01\n\x13ValidatorNodeStatus\x12%\n!VALIDATOR_NODE_STATUS_UNSPECIFIED\x10\x00\x12$\n VALIDATOR_NODE_STATUS_TENDERMINT\x10\x01\x12 \n\x1cVALIDATOR_NODE_STATUS_ERSATZ\x10\x02\x12!\n\x1dVALIDATOR_NODE_STATUS_PENDING\x10\x03\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.vega_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _globals["_SIDE"]._serialized_start = 14985
-    _globals["_SIDE"]._serialized_end = 15042
-    _globals["_INTERVAL"]._serialized_start = 15045
-    _globals["_INTERVAL"]._serialized_end = 15226
-    _globals["_POSITIONSTATUS"]._serialized_start = 15229
-    _globals["_POSITIONSTATUS"]._serialized_end = 15377
-    _globals["_AUCTIONTRIGGER"]._serialized_start = 15380
-    _globals["_AUCTIONTRIGGER"]._serialized_end = 15637
-    _globals["_PEGGEDREFERENCE"]._serialized_start = 15640
-    _globals["_PEGGEDREFERENCE"]._serialized_end = 15779
-    _globals["_ORDERERROR"]._serialized_start = 15782
-    _globals["_ORDERERROR"]._serialized_end = 17903
-    _globals["_CHAINSTATUS"]._serialized_start = 17906
-    _globals["_CHAINSTATUS"]._serialized_end = 18036
-    _globals["_ACCOUNTTYPE"]._serialized_start = 18039
-    _globals["_ACCOUNTTYPE"]._serialized_end = 18645
-    _globals["_TRANSFERTYPE"]._serialized_start = 18648
-    _globals["_TRANSFERTYPE"]._serialized_end = 19628
-    _globals["_DISPATCHMETRIC"]._serialized_start = 19631
-    _globals["_DISPATCHMETRIC"]._serialized_end = 19830
-    _globals["_NODESTATUS"]._serialized_start = 19832
-    _globals["_NODESTATUS"]._serialized_end = 19931
-    _globals["_EPOCHACTION"]._serialized_start = 19933
-    _globals["_EPOCHACTION"]._serialized_end = 20022
-    _globals["_VALIDATORNODESTATUS"]._serialized_start = 20025
-    _globals["_VALIDATORNODESTATUS"]._serialized_end = 20192
+    _globals["_SIDE"]._serialized_start = 15068
+    _globals["_SIDE"]._serialized_end = 15125
+    _globals["_INTERVAL"]._serialized_start = 15128
+    _globals["_INTERVAL"]._serialized_end = 15309
+    _globals["_POSITIONSTATUS"]._serialized_start = 15312
+    _globals["_POSITIONSTATUS"]._serialized_end = 15460
+    _globals["_AUCTIONTRIGGER"]._serialized_start = 15463
+    _globals["_AUCTIONTRIGGER"]._serialized_end = 15720
+    _globals["_PEGGEDREFERENCE"]._serialized_start = 15723
+    _globals["_PEGGEDREFERENCE"]._serialized_end = 15862
+    _globals["_ORDERERROR"]._serialized_start = 15865
+    _globals["_ORDERERROR"]._serialized_end = 17986
+    _globals["_CHAINSTATUS"]._serialized_start = 17989
+    _globals["_CHAINSTATUS"]._serialized_end = 18119
+    _globals["_ACCOUNTTYPE"]._serialized_start = 18122
+    _globals["_ACCOUNTTYPE"]._serialized_end = 18816
+    _globals["_TRANSFERTYPE"]._serialized_start = 18819
+    _globals["_TRANSFERTYPE"]._serialized_end = 20075
+    _globals["_DISPATCHMETRIC"]._serialized_start = 20078
+    _globals["_DISPATCHMETRIC"]._serialized_end = 20277
+    _globals["_NODESTATUS"]._serialized_start = 20279
+    _globals["_NODESTATUS"]._serialized_end = 20378
+    _globals["_EPOCHACTION"]._serialized_start = 20380
+    _globals["_EPOCHACTION"]._serialized_end = 20469
+    _globals["_VALIDATORNODESTATUS"]._serialized_start = 20472
+    _globals["_VALIDATORNODESTATUS"]._serialized_end = 20639
     _globals["_STOPORDER"]._serialized_start = 46
-    _globals["_STOPORDER"]._serialized_end = 998
-    _globals["_STOPORDER_EXPIRYSTRATEGY"]._serialized_start = 551
-    _globals["_STOPORDER_EXPIRYSTRATEGY"]._serialized_end = 657
-    _globals["_STOPORDER_TRIGGERDIRECTION"]._serialized_start = 659
-    _globals["_STOPORDER_TRIGGERDIRECTION"]._serialized_end = 782
-    _globals["_STOPORDER_STATUS"]._serialized_start = 785
-    _globals["_STOPORDER_STATUS"]._serialized_end = 921
-    _globals["_PARTY"]._serialized_start = 1000
-    _globals["_PARTY"]._serialized_end = 1023
-    _globals["_RISKFACTOR"]._serialized_start = 1025
-    _globals["_RISKFACTOR"]._serialized_end = 1103
-    _globals["_PEGGEDORDER"]._serialized_start = 1105
-    _globals["_PEGGEDORDER"]._serialized_end = 1195
-    _globals["_ICEBERGORDER"]._serialized_start = 1198
-    _globals["_ICEBERGORDER"]._serialized_end = 1338
-    _globals["_ORDER"]._serialized_start = 1341
-    _globals["_ORDER"]._serialized_end = 2621
-    _globals["_ORDER_TIMEINFORCE"]._serialized_start = 2125
-    _globals["_ORDER_TIMEINFORCE"]._serialized_end = 2307
-    _globals["_ORDER_TYPE"]._serialized_start = 2309
-    _globals["_ORDER_TYPE"]._serialized_end = 2388
-    _globals["_ORDER_STATUS"]._serialized_start = 2391
-    _globals["_ORDER_STATUS"]._serialized_end = 2592
-    _globals["_ORDERCANCELLATIONCONFIRMATION"]._serialized_start = 2623
-    _globals["_ORDERCANCELLATIONCONFIRMATION"]._serialized_end = 2689
-    _globals["_ORDERCONFIRMATION"]._serialized_start = 2692
-    _globals["_ORDERCONFIRMATION"]._serialized_end = 2852
-    _globals["_AUCTIONINDICATIVESTATE"]._serialized_start = 2855
-    _globals["_AUCTIONINDICATIVESTATE"]._serialized_end = 3066
-    _globals["_TRADE"]._serialized_start = 3069
-    _globals["_TRADE"]._serialized_end = 3672
-    _globals["_TRADE_TYPE"]._serialized_start = 3561
-    _globals["_TRADE_TYPE"]._serialized_end = 3672
-    _globals["_FEE"]._serialized_start = 3674
-    _globals["_FEE"]._serialized_end = 3792
-    _globals["_TRADESET"]._serialized_start = 3794
-    _globals["_TRADESET"]._serialized_end = 3841
-    _globals["_CANDLE"]._serialized_start = 3844
-    _globals["_CANDLE"]._serialized_end = 4058
-    _globals["_PRICELEVEL"]._serialized_start = 4060
-    _globals["_PRICELEVEL"]._serialized_end = 4160
-    _globals["_MARKETDEPTH"]._serialized_start = 4163
-    _globals["_MARKETDEPTH"]._serialized_end = 4320
-    _globals["_MARKETDEPTHUPDATE"]._serialized_start = 4323
-    _globals["_MARKETDEPTHUPDATE"]._serialized_end = 4544
-    _globals["_POSITION"]._serialized_start = 4547
-    _globals["_POSITION"]._serialized_end = 4922
-    _globals["_POSITIONTRADE"]._serialized_start = 4924
-    _globals["_POSITIONTRADE"]._serialized_end = 4985
-    _globals["_DEPOSIT"]._serialized_start = 4988
-    _globals["_DEPOSIT"]._serialized_end = 5344
-    _globals["_DEPOSIT_STATUS"]._serialized_start = 5251
-    _globals["_DEPOSIT_STATUS"]._serialized_end = 5344
-    _globals["_WITHDRAWAL"]._serialized_start = 5347
-    _globals["_WITHDRAWAL"]._serialized_end = 5771
-    _globals["_WITHDRAWAL_STATUS"]._serialized_start = 5673
-    _globals["_WITHDRAWAL_STATUS"]._serialized_end = 5765
-    _globals["_WITHDRAWEXT"]._serialized_start = 5773
-    _globals["_WITHDRAWEXT"]._serialized_end = 5841
-    _globals["_ERC20WITHDRAWEXT"]._serialized_start = 5843
-    _globals["_ERC20WITHDRAWEXT"]._serialized_end = 5904
-    _globals["_ACCOUNT"]._serialized_start = 5907
-    _globals["_ACCOUNT"]._serialized_end = 6070
-    _globals["_FINANCIALAMOUNT"]._serialized_start = 6072
-    _globals["_FINANCIALAMOUNT"]._serialized_end = 6135
-    _globals["_TRANSFER"]._serialized_start = 6138
-    _globals["_TRANSFER"]._serialized_end = 6317
-    _globals["_DISPATCHSTRATEGY"]._serialized_start = 6320
-    _globals["_DISPATCHSTRATEGY"]._serialized_end = 6452
-    _globals["_TRANSFERREQUEST"]._serialized_start = 6455
-    _globals["_TRANSFERREQUEST"]._serialized_end = 6685
-    _globals["_ACCOUNTDETAILS"]._serialized_start = 6688
-    _globals["_ACCOUNTDETAILS"]._serialized_end = 6855
-    _globals["_LEDGERENTRY"]._serialized_start = 6858
-    _globals["_LEDGERENTRY"]._serialized_end = 7171
-    _globals["_POSTTRANSFERBALANCE"]._serialized_start = 7173
-    _globals["_POSTTRANSFERBALANCE"]._serialized_end = 7268
-    _globals["_LEDGERMOVEMENT"]._serialized_start = 7270
-    _globals["_LEDGERMOVEMENT"]._serialized_end = 7386
-    _globals["_MARGINLEVELS"]._serialized_start = 7389
-    _globals["_MARGINLEVELS"]._serialized_end = 7690
-    _globals["_MARKETDATA"]._serialized_start = 7693
-    _globals["_MARKETDATA"]._serialized_end = 9111
-    _globals["_LIQUIDITYPROVIDERFEESHARE"]._serialized_start = 9114
-    _globals["_LIQUIDITYPROVIDERFEESHARE"]._serialized_end = 9337
-    _globals["_PRICEMONITORINGBOUNDS"]._serialized_start = 9340
-    _globals["_PRICEMONITORINGBOUNDS"]._serialized_end = 9540
-    _globals["_ERRORDETAIL"]._serialized_start = 9542
-    _globals["_ERRORDETAIL"]._serialized_end = 9623
-    _globals["_NETWORKPARAMETER"]._serialized_start = 9625
-    _globals["_NETWORKPARAMETER"]._serialized_end = 9683
-    _globals["_NETWORKLIMITS"]._serialized_start = 9686
-    _globals["_NETWORKLIMITS"]._serialized_end = 10072
-    _globals["_LIQUIDITYORDER"]._serialized_start = 10074
-    _globals["_LIQUIDITYORDER"]._serialized_end = 10199
-    _globals["_LIQUIDITYORDERREFERENCE"]._serialized_start = 10201
-    _globals["_LIQUIDITYORDERREFERENCE"]._serialized_end = 10316
-    _globals["_LIQUIDITYPROVISION"]._serialized_start = 10319
-    _globals["_LIQUIDITYPROVISION"]._serialized_end = 10913
-    _globals["_LIQUIDITYPROVISION_STATUS"]._serialized_start = 10756
-    _globals["_LIQUIDITYPROVISION_STATUS"]._serialized_end = 10913
-    _globals["_ETHEREUMCONFIG"]._serialized_start = 10916
-    _globals["_ETHEREUMCONFIG"]._serialized_end = 11380
-    _globals["_ETHEREUMCONTRACTCONFIG"]._serialized_start = 11382
-    _globals["_ETHEREUMCONTRACTCONFIG"]._serialized_end = 11488
-    _globals["_EPOCHTIMESTAMPS"]._serialized_start = 11491
-    _globals["_EPOCHTIMESTAMPS"]._serialized_end = 11663
-    _globals["_EPOCH"]._serialized_start = 11666
-    _globals["_EPOCH"]._serialized_end = 11842
-    _globals["_EPOCHPARTICIPATION"]._serialized_start = 11845
-    _globals["_EPOCHPARTICIPATION"]._serialized_end = 11987
-    _globals["_EPOCHDATA"]._serialized_start = 11989
-    _globals["_EPOCHDATA"]._serialized_end = 12072
-    _globals["_RANKINGSCORE"]._serialized_start = 12075
-    _globals["_RANKINGSCORE"]._serialized_end = 12358
-    _globals["_REWARDSCORE"]._serialized_start = 12361
-    _globals["_REWARDSCORE"]._serialized_end = 12660
-    _globals["_NODE"]._serialized_start = 12663
-    _globals["_NODE"]._serialized_end = 13354
-    _globals["_NODESET"]._serialized_start = 13357
-    _globals["_NODESET"]._serialized_end = 13513
-    _globals["_NODEDATA"]._serialized_start = 13516
-    _globals["_NODEDATA"]._serialized_end = 13817
-    _globals["_DELEGATION"]._serialized_start = 13819
-    _globals["_DELEGATION"]._serialized_end = 13931
-    _globals["_REWARD"]._serialized_start = 13934
-    _globals["_REWARD"]._serialized_end = 14185
-    _globals["_REWARDSUMMARY"]._serialized_start = 14187
-    _globals["_REWARDSUMMARY"]._serialized_end = 14280
-    _globals["_EPOCHREWARDSUMMARY"]._serialized_start = 14283
-    _globals["_EPOCHREWARDSUMMARY"]._serialized_end = 14438
-    _globals["_STATEVALUEPROPOSAL"]._serialized_start = 14440
-    _globals["_STATEVALUEPROPOSAL"]._serialized_end = 14561
-    _globals["_KEYVALUEBUNDLE"]._serialized_start = 14563
-    _globals["_KEYVALUEBUNDLE"]._serialized_end = 14670
-    _globals["_STATEVARVALUE"]._serialized_start = 14673
-    _globals["_STATEVARVALUE"]._serialized_end = 14853
-    _globals["_SCALARVALUE"]._serialized_start = 14855
-    _globals["_SCALARVALUE"]._serialized_end = 14890
-    _globals["_VECTORVALUE"]._serialized_start = 14892
-    _globals["_VECTORVALUE"]._serialized_end = 14927
-    _globals["_MATRIXVALUE"]._serialized_start = 14929
-    _globals["_MATRIXVALUE"]._serialized_end = 14983
+    _globals["_STOPORDER"]._serialized_end = 1053
+    _globals["_STOPORDER_EXPIRYSTRATEGY"]._serialized_start = 585
+    _globals["_STOPORDER_EXPIRYSTRATEGY"]._serialized_end = 691
+    _globals["_STOPORDER_TRIGGERDIRECTION"]._serialized_start = 693
+    _globals["_STOPORDER_TRIGGERDIRECTION"]._serialized_end = 816
+    _globals["_STOPORDER_STATUS"]._serialized_start = 819
+    _globals["_STOPORDER_STATUS"]._serialized_end = 976
+    _globals["_PARTY"]._serialized_start = 1055
+    _globals["_PARTY"]._serialized_end = 1078
+    _globals["_RISKFACTOR"]._serialized_start = 1080
+    _globals["_RISKFACTOR"]._serialized_end = 1158
+    _globals["_PEGGEDORDER"]._serialized_start = 1160
+    _globals["_PEGGEDORDER"]._serialized_end = 1250
+    _globals["_ICEBERGORDER"]._serialized_start = 1253
+    _globals["_ICEBERGORDER"]._serialized_end = 1393
+    _globals["_ORDER"]._serialized_start = 1396
+    _globals["_ORDER"]._serialized_end = 2676
+    _globals["_ORDER_TIMEINFORCE"]._serialized_start = 2180
+    _globals["_ORDER_TIMEINFORCE"]._serialized_end = 2362
+    _globals["_ORDER_TYPE"]._serialized_start = 2364
+    _globals["_ORDER_TYPE"]._serialized_end = 2443
+    _globals["_ORDER_STATUS"]._serialized_start = 2446
+    _globals["_ORDER_STATUS"]._serialized_end = 2647
+    _globals["_ORDERCANCELLATIONCONFIRMATION"]._serialized_start = 2678
+    _globals["_ORDERCANCELLATIONCONFIRMATION"]._serialized_end = 2744
+    _globals["_ORDERCONFIRMATION"]._serialized_start = 2747
+    _globals["_ORDERCONFIRMATION"]._serialized_end = 2907
+    _globals["_AUCTIONINDICATIVESTATE"]._serialized_start = 2910
+    _globals["_AUCTIONINDICATIVESTATE"]._serialized_end = 3121
+    _globals["_TRADE"]._serialized_start = 3124
+    _globals["_TRADE"]._serialized_end = 3727
+    _globals["_TRADE_TYPE"]._serialized_start = 3616
+    _globals["_TRADE_TYPE"]._serialized_end = 3727
+    _globals["_FEE"]._serialized_start = 3729
+    _globals["_FEE"]._serialized_end = 3847
+    _globals["_TRADESET"]._serialized_start = 3849
+    _globals["_TRADESET"]._serialized_end = 3896
+    _globals["_CANDLE"]._serialized_start = 3899
+    _globals["_CANDLE"]._serialized_end = 4141
+    _globals["_PRICELEVEL"]._serialized_start = 4143
+    _globals["_PRICELEVEL"]._serialized_end = 4243
+    _globals["_MARKETDEPTH"]._serialized_start = 4246
+    _globals["_MARKETDEPTH"]._serialized_end = 4403
+    _globals["_MARKETDEPTHUPDATE"]._serialized_start = 4406
+    _globals["_MARKETDEPTHUPDATE"]._serialized_end = 4627
+    _globals["_POSITION"]._serialized_start = 4630
+    _globals["_POSITION"]._serialized_end = 5005
+    _globals["_POSITIONTRADE"]._serialized_start = 5007
+    _globals["_POSITIONTRADE"]._serialized_end = 5068
+    _globals["_DEPOSIT"]._serialized_start = 5071
+    _globals["_DEPOSIT"]._serialized_end = 5427
+    _globals["_DEPOSIT_STATUS"]._serialized_start = 5334
+    _globals["_DEPOSIT_STATUS"]._serialized_end = 5427
+    _globals["_WITHDRAWAL"]._serialized_start = 5430
+    _globals["_WITHDRAWAL"]._serialized_end = 5854
+    _globals["_WITHDRAWAL_STATUS"]._serialized_start = 5756
+    _globals["_WITHDRAWAL_STATUS"]._serialized_end = 5848
+    _globals["_WITHDRAWEXT"]._serialized_start = 5856
+    _globals["_WITHDRAWEXT"]._serialized_end = 5924
+    _globals["_ERC20WITHDRAWEXT"]._serialized_start = 5926
+    _globals["_ERC20WITHDRAWEXT"]._serialized_end = 5987
+    _globals["_ACCOUNT"]._serialized_start = 5990
+    _globals["_ACCOUNT"]._serialized_end = 6153
+    _globals["_FINANCIALAMOUNT"]._serialized_start = 6155
+    _globals["_FINANCIALAMOUNT"]._serialized_end = 6218
+    _globals["_TRANSFER"]._serialized_start = 6221
+    _globals["_TRANSFER"]._serialized_end = 6400
+    _globals["_DISPATCHSTRATEGY"]._serialized_start = 6403
+    _globals["_DISPATCHSTRATEGY"]._serialized_end = 6535
+    _globals["_TRANSFERREQUEST"]._serialized_start = 6538
+    _globals["_TRANSFERREQUEST"]._serialized_end = 6768
+    _globals["_ACCOUNTDETAILS"]._serialized_start = 6771
+    _globals["_ACCOUNTDETAILS"]._serialized_end = 6938
+    _globals["_LEDGERENTRY"]._serialized_start = 6941
+    _globals["_LEDGERENTRY"]._serialized_end = 7254
+    _globals["_POSTTRANSFERBALANCE"]._serialized_start = 7256
+    _globals["_POSTTRANSFERBALANCE"]._serialized_end = 7351
+    _globals["_LEDGERMOVEMENT"]._serialized_start = 7353
+    _globals["_LEDGERMOVEMENT"]._serialized_end = 7469
+    _globals["_MARGINLEVELS"]._serialized_start = 7472
+    _globals["_MARGINLEVELS"]._serialized_end = 7773
+    _globals["_MARKETDATA"]._serialized_start = 7776
+    _globals["_MARKETDATA"]._serialized_end = 9194
+    _globals["_LIQUIDITYPROVIDERFEESHARE"]._serialized_start = 9197
+    _globals["_LIQUIDITYPROVIDERFEESHARE"]._serialized_end = 9420
+    _globals["_PRICEMONITORINGBOUNDS"]._serialized_start = 9423
+    _globals["_PRICEMONITORINGBOUNDS"]._serialized_end = 9623
+    _globals["_ERRORDETAIL"]._serialized_start = 9625
+    _globals["_ERRORDETAIL"]._serialized_end = 9706
+    _globals["_NETWORKPARAMETER"]._serialized_start = 9708
+    _globals["_NETWORKPARAMETER"]._serialized_end = 9766
+    _globals["_NETWORKLIMITS"]._serialized_start = 9769
+    _globals["_NETWORKLIMITS"]._serialized_end = 10155
+    _globals["_LIQUIDITYORDER"]._serialized_start = 10157
+    _globals["_LIQUIDITYORDER"]._serialized_end = 10282
+    _globals["_LIQUIDITYORDERREFERENCE"]._serialized_start = 10284
+    _globals["_LIQUIDITYORDERREFERENCE"]._serialized_end = 10399
+    _globals["_LIQUIDITYPROVISION"]._serialized_start = 10402
+    _globals["_LIQUIDITYPROVISION"]._serialized_end = 10996
+    _globals["_LIQUIDITYPROVISION_STATUS"]._serialized_start = 10839
+    _globals["_LIQUIDITYPROVISION_STATUS"]._serialized_end = 10996
+    _globals["_ETHEREUMCONFIG"]._serialized_start = 10999
+    _globals["_ETHEREUMCONFIG"]._serialized_end = 11463
+    _globals["_ETHEREUMCONTRACTCONFIG"]._serialized_start = 11465
+    _globals["_ETHEREUMCONTRACTCONFIG"]._serialized_end = 11571
+    _globals["_EPOCHTIMESTAMPS"]._serialized_start = 11574
+    _globals["_EPOCHTIMESTAMPS"]._serialized_end = 11746
+    _globals["_EPOCH"]._serialized_start = 11749
+    _globals["_EPOCH"]._serialized_end = 11925
+    _globals["_EPOCHPARTICIPATION"]._serialized_start = 11928
+    _globals["_EPOCHPARTICIPATION"]._serialized_end = 12070
+    _globals["_EPOCHDATA"]._serialized_start = 12072
+    _globals["_EPOCHDATA"]._serialized_end = 12155
+    _globals["_RANKINGSCORE"]._serialized_start = 12158
+    _globals["_RANKINGSCORE"]._serialized_end = 12441
+    _globals["_REWARDSCORE"]._serialized_start = 12444
+    _globals["_REWARDSCORE"]._serialized_end = 12743
+    _globals["_NODE"]._serialized_start = 12746
+    _globals["_NODE"]._serialized_end = 13437
+    _globals["_NODESET"]._serialized_start = 13440
+    _globals["_NODESET"]._serialized_end = 13596
+    _globals["_NODEDATA"]._serialized_start = 13599
+    _globals["_NODEDATA"]._serialized_end = 13900
+    _globals["_DELEGATION"]._serialized_start = 13902
+    _globals["_DELEGATION"]._serialized_end = 14014
+    _globals["_REWARD"]._serialized_start = 14017
+    _globals["_REWARD"]._serialized_end = 14268
+    _globals["_REWARDSUMMARY"]._serialized_start = 14270
+    _globals["_REWARDSUMMARY"]._serialized_end = 14363
+    _globals["_EPOCHREWARDSUMMARY"]._serialized_start = 14366
+    _globals["_EPOCHREWARDSUMMARY"]._serialized_end = 14521
+    _globals["_STATEVALUEPROPOSAL"]._serialized_start = 14523
+    _globals["_STATEVALUEPROPOSAL"]._serialized_end = 14644
+    _globals["_KEYVALUEBUNDLE"]._serialized_start = 14646
+    _globals["_KEYVALUEBUNDLE"]._serialized_end = 14753
+    _globals["_STATEVARVALUE"]._serialized_start = 14756
+    _globals["_STATEVARVALUE"]._serialized_end = 14936
+    _globals["_SCALARVALUE"]._serialized_start = 14938
+    _globals["_SCALARVALUE"]._serialized_end = 14973
+    _globals["_VECTORVALUE"]._serialized_start = 14975
+    _globals["_VECTORVALUE"]._serialized_end = 15010
+    _globals["_MATRIXVALUE"]._serialized_start = 15012
+    _globals["_MATRIXVALUE"]._serialized_end = 15066
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/wallet_pb2.py` & `vega_sim-1.2.1/vega_sim/proto/vega/wallet/v1/wallet_pb2.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/quant/quant.py` & `vega_sim-1.2.1/vega_sim/quant/quant.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent.py` & `vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO.py` & `vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent_MO.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py` & `vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_heuristic.py` & `vega_sim-1.2.1/vega_sim/reinforcement/agents/learning_agent_heuristic.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/agents/simple_agent.py` & `vega_sim-1.2.1/vega_sim/reinforcement/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/distributions.py` & `vega_sim-1.2.1/vega_sim/reinforcement/distributions.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/environments.py` & `vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/environments.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/create_csv.py` & `vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/create_csv.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py` & `vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/logdata.py` & `vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/logdata.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/strategy.py` & `vega_sim-1.2.1/vega_sim/reinforcement/full_market_sim/utils/strategy.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/helpers.py` & `vega_sim-1.2.1/vega_sim/reinforcement/helpers.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/la_market_state.py` & `vega_sim-1.2.1/vega_sim/reinforcement/la_market_state.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/networks.py` & `vega_sim-1.2.1/vega_sim/reinforcement/networks.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/plot.py` & `vega_sim-1.2.1/vega_sim/reinforcement/plot.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/run_rl_agent.py` & `vega_sim-1.2.1/vega_sim/reinforcement/run_rl_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/run_simple_agent.py` & `vega_sim-1.2.1/vega_sim/reinforcement/run_simple_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/RL.tex` & `vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/RL.tex`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL.png` & `vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/RL.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL_inv.png` & `vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/RL_inv.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo.png` & `vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/logo.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo_inv.png` & `vega_sim-1.2.1/vega_sim/reinforcement/theory_intro/images/logo_inv.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/learning_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent_MO.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/learning_agent_MO.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/puppets.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/agents/puppets.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/learning_environment.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/learning_environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Type, Optional
+from typing import Dict, Type, Optional, Union
 from dataclasses import dataclass
 from vega_sim.reinforcement.v2.agents.puppets import (
     AGENT_TYPE_TO_AGENT,
     AgentType,
     MarketOrderAction,
     Action,
     Side,
@@ -21,25 +21,32 @@
     reward: float
 
 
 class Environment:
     def __init__(
         self,
         agents: Dict[str, AgentType],
-        agent_to_reward: Dict[str, Reward],
+        agent_to_reward: Union[Reward, Dict[str, Reward]],
         agent_to_state: Dict[str, Type[State]],
         scenario: Scenario,
         reset_vega_every_n_runs: int = 100,
         funds_per_run: float = 10_000,
     ):
         self._agents = agents
-        self._agent_to_reward_enum = agent_to_reward
         self._agent_to_state = agent_to_state
+
         self._agent_to_reward: Dict[str, BaseRewarder] = {}
 
+        if isinstance(agent_to_reward, dict):
+            self._is_single_reward = False
+            self._agent_to_reward_enum = agent_to_reward
+        else:
+            self._is_single_reward = True
+            self._single_reward_base: Reward = agent_to_reward
+
         self._scenario = scenario
         self._vega = VegaServiceNull(
             warn_on_raw_data_access=False,
             run_with_console=False,
             retain_log_files=True,
             store_transactions=True,
             transactions_per_block=1000,
@@ -67,14 +74,15 @@
         for agent_name, action in actions.items():
             if action is not None:
                 self._puppets[agent_name].set_next_action(action=action)
 
         self._scenario.env.step(self._vega)
         self._vega.wait_fn(1)
         step_res = {}
+
         for agent_name, reward_gen in self._agent_to_reward.items():
             step_res[agent_name] = StepResult(
                 observation=self._extract_observation(agent_name),
                 reward=self.calculate_reward(reward_gen),
             )
         return step_res
 
@@ -129,18 +137,30 @@
                 key_name=agent_name,
                 asset=manager.asset_id,
                 amount=self._funds_per_run,
             )
 
         self._agent_to_reward = {}
 
-        for agent, reward in self._agent_to_reward_enum.items():
-            self._agent_to_reward[agent] = REWARD_ENUM_TO_CLASS[reward](
-                agent_key=agent, asset_id=manager.asset_id, market_id=manager.market_id
-            )
+        if not self._is_single_reward:
+            for agent, reward in self._agent_to_reward_enum.items():
+                self._agent_to_reward[agent] = REWARD_ENUM_TO_CLASS[reward](
+                    agent_key=agent,
+                    asset_id=manager.asset_id,
+                    market_id=manager.market_id,
+                )
+        else:
+            for agent in self._agent_to_state.keys():
+                self._agent_to_reward[agent] = REWARD_ENUM_TO_CLASS[
+                    self._single_reward_base
+                ](
+                    agent_keys=list(self._agent_to_state.keys()),
+                    asset_id=manager.asset_id,
+                    market_id=manager.market_id,
+                )
         self._market_id = manager.market_id
         self._asset_id = manager.asset_id
 
 
 if __name__ == "__main__":
     from vega_sim.scenario.registry import CurveMarketMaker
```

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/environment.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/pettingzoo/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,39 +36,41 @@
 }
 
 
 @dataclass
 class AgentConfig:
     action_type: ActionType
     state_type: Type[State]
-    reward_type: Reward
+    reward_type: Optional[Reward] = None
     terminal_reward_type: Optional[Reward] = None
 
 
 class MultiAgentVegaEnv(ParallelEnv):
     """Custom Environment that follows gym interface."""
 
     metadata = {"render.modes": ["human"]}
 
     def __init__(
         self,
         agents: List[AgentConfig],
         num_levels_state: int = 5,
         trade_volume: float = 1,
         steps_per_trading_session: int = 1000,
+        unified_reward: Optional[Reward] = None,
     ):
         super().__init__()
         self.num_levels_state = num_levels_state
         self.agent_configs = agents
         self.trade_volume = trade_volume
         self.steps_per_trading_session = steps_per_trading_session
         self.current_step = 0
         self.learner_names = {
-            str(i): "learner_{i}" for i in range(len(self.agent_configs))
+            str(i): f"learner_{i}" for i in range(len(self.agent_configs))
         }
+        self.unified_reward = unified_reward
 
         # Define action and observation space
         # They must be gym.spaces objects
         # Example when using discrete actions:
         self.action_spaces = {
             str(i): self._get_action_space(action_type=agent_config.action_type)
             for (i, agent_config) in enumerate(self.agent_configs)
@@ -98,18 +100,22 @@
         )
 
         self.env = Environment(
             agents={
                 learner_name: ACTION_TO_AGENT[self.agent_configs[int(i)].action_type]
                 for (i, learner_name) in self.learner_names.items()
             },
-            agent_to_reward={
-                learner_name: self.agent_configs[int(i)].reward_type
-                for (i, learner_name) in self.learner_names.items()
-            },
+            agent_to_reward=(
+                {
+                    learner_name: self.agent_configs[int(i)].reward_type
+                    for (i, learner_name) in self.learner_names.items()
+                }
+                if self.unified_reward is None
+                else self.unified_reward
+            ),
             agent_to_state={
                 learner_name: self.agent_configs[int(i)].state_type
                 for (i, learner_name) in self.learner_names.items()
             },
             scenario=scenario,
         )
         self.agents = list(self.learner_names.keys())
```

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/run.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/pettingzoo/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,33 +29,35 @@
 
         agents.append(DQNPolicy(model, optim))
 
     return agents
 
 
 if __name__ == "__main__":
+    env = None
     # Step 1: Load the PettingZoo environment
     try:
         agent_configs = [
             pz.AgentConfig(
                 action_type=pz.ActionType.AT_TOUCH_ONE_SIDE,
                 state_type=pz.PriceStateWithFees,
-                reward_type=pz.Reward.PNL,
-                terminal_reward_type=pz.Reward.SQ_INVENTORY_PENALTY,
+                # reward_type=pz.Reward.PNL,
+                # terminal_reward_type=pz.Reward.SQ_INVENTORY_PENALTY,
             ),
             pz.AgentConfig(
                 action_type=pz.ActionType.AT_TOUCH_ONE_SIDE,
                 state_type=pz.PriceStateWithFees,
-                reward_type=pz.Reward.PNL,
-                terminal_reward_type=pz.Reward.SQ_INVENTORY_PENALTY,
+                # reward_type=pz.Reward.PNL,
+                # terminal_reward_type=pz.Reward.SQ_INVENTORY_PENALTY,
             ),
         ]
         base_env = pz.MultiAgentVegaEnv(
             agents=agent_configs,
             steps_per_trading_session=200,
+            unified_reward=pz.Reward.UNIFIED_PNL,
         )
 
         # Step 2: Wrap the environment for Tianshou interfacing
         # env.reset()
         env = PettingZooEnv(parallel_to_aec_wrapper(base_env))
         # Step 3: Define policies for each agent
         agents = get_agents(base_env)
@@ -116,8 +118,9 @@
             # stop_fn=stop_fn,
             save_best_fn=save_best_fn,
             update_per_step=0.1,
             logger=logger,
             test_in_train=False,
         )
     finally:
-        env.close()
+        if env is not None:
+            env.close()
```

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/rewards.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/rewards.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
 from enum import Enum, auto
-from typing import Optional
+from typing import Optional, List
 
 from vega_sim.scenario.common.agents import VegaService
 
 
 class Reward(Enum):
     PNL = auto()
     SQ_INVENTORY_PENALTY = auto()
+    UNIFIED_PNL = auto()
 
 
 class BaseRewarder(ABC):
     def __init__(
         self,
         agent_key: str,
         market_id: str,
@@ -25,14 +26,57 @@
         self.last_balance = None
 
     @abstractmethod
     def get_reward(self, vega: VegaService) -> float:
         pass
 
 
+class BaseUnifiedRewarder(ABC):
+    def __init__(
+        self,
+        agent_keys: List[str],
+        market_id: str,
+        asset_id: str,
+        agent_wallets: Optional[List[str]] = None,
+    ):
+        self.agent_keys = agent_keys
+        self.agent_wallets = (
+            agent_wallets
+            if agent_wallets is not None
+            else [None for _ in range(len(self.agent_keys))]
+        )
+        self.asset_id = asset_id
+        self.market_id = market_id
+        self.last_balance = {}
+
+    @abstractmethod
+    def get_reward(self, vega: VegaService) -> float:
+        pass
+
+
+class PnlUnifiedRewarder(BaseUnifiedRewarder):
+    def get_reward(self, vega: VegaService) -> float:
+        reward = 0
+        for key, wallet in zip(self.agent_keys, self.agent_wallets):
+            balance = vega.party_account(
+                key_name=key,
+                wallet_name=wallet,
+                asset_id=self.asset_id,
+                market_id=self.market_id,
+            )
+            balance = sum(k for k in balance)
+            if self.last_balance.get(key):
+                key_reward = balance - self.last_balance.get(key)
+            else:
+                key_reward = 0
+            self.last_balance[key] = balance
+            reward += key_reward
+        return reward
+
+
 class PnlRewarder(BaseRewarder):
     def get_reward(self, vega: VegaService) -> float:
         balance = vega.party_account(
             key_name=self.agent_key,
             wallet_name=self.agent_wallet,
             asset_id=self.asset_id,
             market_id=self.market_id,
@@ -56,8 +100,9 @@
 
         return (-1 * posn.open_volume**2) if posn is not None else 0
 
 
 REWARD_ENUM_TO_CLASS = {
     Reward.PNL: PnlRewarder,
     Reward.SQ_INVENTORY_PENALTY: SquareInventoryPenalty,
+    Reward.UNIFIED_PNL: PnlUnifiedRewarder,
 }
```

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/run.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/run.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/environment.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/environment.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/run.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/run.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/states.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/stable_baselines/states.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/reinforcement/v2/states.py` & `vega_sim-1.2.1/vega_sim/reinforcement/v2/states.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/replay/replay.py` & `vega_sim-1.2.1/vega_sim/replay/replay.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/adhoc.py` & `vega_sim-1.2.1/vega_sim/scenario/adhoc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/common/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/common/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -2812,28 +2812,32 @@
                     logging.warning(
                         "Unable to record memory usage, unsupported operating system"
                     )
 
                 self.resources.append(
                     ResourceData(
                         at_time=start_time,
-                        vega_cpu_per=self.process_map["vega"].cpu_percent()
-                        if "vega" in self.process_map
-                        else 0,
+                        vega_cpu_per=(
+                            self.process_map["vega"].cpu_percent()
+                            if "vega" in self.process_map
+                            else 0
+                        ),
                         vega_mem_rss=mem_vega.rss if mem_vega is not None else 0,
                         vega_mem_vms=mem_vega.vms if mem_vega is not None else 0,
-                        datanode_cpu_per=self.process_map["data-node"].cpu_percent()
-                        if "data-node" in self.process_map
-                        else 0,
-                        datanode_mem_rss=mem_datanode.rss
-                        if mem_datanode is not None
-                        else 0,
-                        datanode_mem_vms=mem_datanode.vms
-                        if mem_datanode is not None
-                        else 0,
+                        datanode_cpu_per=(
+                            self.process_map["data-node"].cpu_percent()
+                            if "data-node" in self.process_map
+                            else 0
+                        ),
+                        datanode_mem_rss=(
+                            mem_datanode.rss if mem_datanode is not None else 0
+                        ),
+                        datanode_mem_vms=(
+                            mem_datanode.vms if mem_datanode is not None else 0
+                        ),
                     )
                 )
         if self.additional_state_fn is not None:
             self.additional_states.append(
                 self.additional_state_fn(self.vega, self.agents)
             )
 
@@ -3289,16 +3293,18 @@
             else []
         )
 
         # Check buy_order_reference and sell_order_reference are still live:
         buys = []
         sells = []
         for order in orders:
-            buys.append(order) if order.side == vega_protos.SIDE_BUY else sells.append(
-                order
+            (
+                buys.append(order)
+                if order.side == vega_protos.SIDE_BUY
+                else sells.append(order)
             )
 
         place_buy = self.current_position < self.max_position
         place_sell = self.current_position > -self.max_position
 
         if len(buys) == 0 and place_buy:
             self.buy_order_reference = self._place_order(side="SIDE_BUY")
@@ -3318,19 +3324,22 @@
             order_type="TYPE_LIMIT",
             time_in_force="TIME_IN_FORCE_GTC",
             side=side,
             volume=self.order_size,
             price=None,
             expires_at=None,
             pegged_order=PeggedOrder(
-                reference=self.buy_peg_reference
-                if side == "SIDE_BUY"
-                else self.sell_peg_reference,
+                reference=(
+                    self.buy_peg_reference
+                    if side == "SIDE_BUY"
+                    else self.sell_peg_reference
+                ),
                 offset=self.peg_offset,
             ),
+            wait=False,
         )
 
     def _cancel_order(self, orders_to_cancel):
         for order in orders_to_cancel:
             self.vega.cancel_order(
                 wallet_name=self.wallet_name,
                 trading_key=self.key_name,
```

### Comparing `vega_sim-1.2.0/vega_sim/scenario/common/utils/ideal_mm_models.py` & `vega_sim-1.2.1/vega_sim/scenario/common/utils/ideal_mm_models.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/common/utils/price_process.py` & `vega_sim-1.2.1/vega_sim/scenario/common/utils/price_process.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/comprehensive_market/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/comprehensive_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/configurable_market/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/configurable_market/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/configurable_market/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/configurable_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/curve_market_maker/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/curve_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_capsule_test.py` & `vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/run_capsule_test.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py` & `vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/fuzzed_markets/scenario.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from vega_sim.api.market import MarketConfig
 
 import argparse
 import logging
 import numpy as np
 from typing import Optional, List
 from vega_sim.scenario.common.utils.price_process import random_walk
+from collections import defaultdict
 
 from vega_sim.scenario.scenario import Scenario
 from vega_sim.environment.environment import (
     MarketEnvironmentWithState,
     NetworkEnvironment,
 )
 from vega_sim.scenario.constants import Network
@@ -21,14 +22,15 @@
     ExponentialShapedMarketMaker,
     MarketOrderTrader,
     LimitOrderTrader,
     RewardFunder,
     AtTheTouchMarketMaker,
 )
 from vega_sim.scenario.fuzzed_markets.agents import (
+    FuzzySuccessorConfigurableMarketManager,
     FuzzingAgent,
     RiskyMarketOrderTrader,
     RiskySimpleLiquidityProvider,
     FuzzyLiquidityProvider,
 )
 
 import vega_sim.proto.vega as vega_protos
@@ -176,33 +178,37 @@
         random_state: Optional[np.random.RandomState],
         **kwargs,
     ) -> List[StateAgent]:
         self.random_state = (
             random_state if random_state is not None else np.random.RandomState()
         )
 
-        market_managers = []
-        market_makers = []
-        at_touch_market_makers = []
-        auction_traders = []
-        random_traders = []
-        fuzz_traders = []
-        risky_traders = []
-        fuzz_liquidity_providers = []
-        risky_liquidity_providers = []
-        reward_funders = []
+        self.all_agents = {
+            "market_managers": [],
+            "market_makers": [],
+            "at_touch_market_makers": [],
+            "auction_traders": [],
+            "random_traders": [],
+            "fuzz_traders": [],
+            "risky_traders": [],
+            "fuzz_liquidity_providers": [],
+            "risky_liquidity_providers": [],
+            "reward_funders": [],
+        }
 
-        self.initial_asset_mint = 1e9
+        self.market_agents = {}
+        self.initial_asset_mint = 10e9
 
         for i_market in range(self.n_markets):
             # Define the market and the asset:
             market_name = f"ASSET_{str(i_market).zfill(3)}"
             asset_name = f"ASSET_{str(i_market).zfill(3)}"
             asset_dp = 18
 
+            market_agents = {}
             # Create fuzzed market config
             market_config = MarketConfig()
             market_config.set(
                 "liquidity_monitoring_parameters.target_stake_parameters.scaling_factor",
                 1e-4,
             )
             if self.fuzz_market_config is not None:
@@ -213,31 +219,34 @@
             price_process = _create_price_process(
                 random_state=self.random_state,
                 num_steps=self.num_steps,
                 decimal_places=int(market_config.decimal_places),
             )
 
             # Create fuzzed market managers
-            market_managers.append(
-                ConfigurableMarketManager(
+            market_agents["market_managers"] = [
+                FuzzySuccessorConfigurableMarketManager(
+                    proposal_wallet_name="MARKET_MANAGER",
                     proposal_key_name="PROPOSAL_KEY",
                     termination_wallet_name="MARKET_MANAGER",
                     termination_key_name="TERMINATION_KEY",
                     market_config=market_config,
                     market_name=market_name,
                     market_code=market_name,
                     asset_dp=asset_dp,
                     asset_name=asset_name,
                     settlement_price=price_process[-1],
                     stake_key=True if kwargs["network"] == Network.CAPSULE else False,
                     tag=f"MARKET_{str(i_market).zfill(3)}",
+                    market_agents=market_agents,
+                    successor_probability=0.01,
                 )
-            )
+            ]
 
-            market_makers.append(
+            market_agents["market_makers"] = [
                 ExponentialShapedMarketMaker(
                     wallet_name="MARKET_MAKERS",
                     key_name=f"MARKET_{str(i_market).zfill(3)}",
                     price_process_generator=iter(price_process),
                     initial_asset_mint=self.initial_asset_mint,
                     market_name=market_name,
                     asset_name=asset_name,
@@ -247,62 +256,68 @@
                     num_steps=self.num_steps,
                     kappa=2.4,
                     tick_spacing=0.05,
                     market_kappa=50,
                     state_update_freq=10,
                     tag=f"MARKET_{str(i_market).zfill(3)}",
                 )
-            )
+            ]
 
-            at_touch_market_makers.append(
+            market_agents["at_touch_market_makers"] = [
                 AtTheTouchMarketMaker(
                     wallet_name=f"AT_THE_TOUCH_MM",
                     key_name=f"MARKET_{str(i_market).zfill(3)}",
                     initial_asset_mint=1e5,
                     market_name=market_name,
                     asset_name=asset_name,
                     order_size=1,
                     peg_offset=0,
                     max_position=5,
                     tag=f"MARKET_{str(i_market).zfill(3)}",
                 )
-            )
+            ]
 
-            for i_agent, side in enumerate(["SIDE_BUY", "SIDE_SELL"]):
-                auction_traders.append(
-                    UncrossAuctionAgent(
-                        wallet_name=f"AUCTION_TRADERS",
-                        key_name=f"MARKET_{str(i_market).zfill(3)}_{side}",
-                        side=side,
-                        initial_asset_mint=self.initial_asset_mint,
-                        price_process=iter(price_process),
-                        market_name=market_name,
-                        asset_name=asset_name,
-                        uncrossing_size=20,
-                        tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                    )
+            market_agents["auction_traders"] = [
+                UncrossAuctionAgent(
+                    wallet_name="AUCTION_TRADERS",
+                    key_name=f"MARKET_{str(i_market).zfill(3)}_{side}",
+                    side=side,
+                    initial_asset_mint=self.initial_asset_mint,
+                    price_process=iter(price_process),
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    uncrossing_size=20,
+                    tag=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
                 )
+                for i_agent, side in enumerate(["SIDE_BUY", "SIDE_SELL"])
+            ]
 
-            for i_agent in range(5):
-                random_traders.append(
-                    MarketOrderTrader(
-                        wallet_name=f"RANDOM_TRADERS",
-                        key_name=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                        market_name=market_name,
-                        asset_name=asset_name,
-                        buy_intensity=10,
-                        sell_intensity=10,
-                        base_order_size=1,
-                        step_bias=1,
-                        tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                    )
+            market_agents["random_traders"] = [
+                MarketOrderTrader(
+                    wallet_name="RANDOM_TRADERS",
+                    key_name=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    buy_intensity=10,
+                    sell_intensity=10,
+                    base_order_size=1,
+                    step_bias=1,
+                    tag=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
                 )
+                for i_agent in range(5)
+            ]
 
             for i_agent in range(5):
-                random_traders.append(
+                market_agents["random_traders"].append(
                     LimitOrderTrader(
                         wallet_name=f"RANDOM_TRADERS",
                         key_name=f"LIMIT_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                         market_name=market_name,
                         asset_name=asset_name,
                         time_in_force_opts={"TIME_IN_FORCE_GTT": 1},
                         buy_volume=1,
@@ -316,82 +331,90 @@
                         spread=0,
                         mean=-3,
                         sigma=0.5,
                         tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
 
-            for i_agent in range(10):
-                fuzz_traders.append(
-                    FuzzingAgent(
-                        wallet_name="FUZZING_TRADERS",
-                        key_name=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                        market_name=market_name,
-                        asset_name=asset_name,
-                        output_plot_on_finalise=self.output,
-                        tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                    )
+            market_agents["fuzz_traders"] = [
+                FuzzingAgent(
+                    wallet_name="FUZZING_TRADERS",
+                    key_name=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    output_plot_on_finalise=self.output,
+                    tag=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
                 )
+                for i_agent in range(10)
+            ]
 
-            for side in ["SIDE_BUY", "SIDE_SELL"]:
-                for i_agent in range(10):
-                    risky_traders.append(
-                        RiskyMarketOrderTrader(
-                            wallet_name="risky_traders",
-                            key_name=f"MARKET_{str(i_market).zfill(3)}_SIDE_{side}_AGENT_{str(i_agent).zfill(3)}",
-                            market_name=market_name,
-                            asset_name=asset_name,
-                            side=side,
-                            initial_asset_mint=1_000,
-                            size_factor=0.5,
-                            step_bias=0.1,
-                            tag=f"MARKET_{str(i_market).zfill(3)}_SIDE_{side}_AGENT_{str(i_agent).zfill(3)}",
-                        )
-                    )
-
-            for i_agent in range(5):
-                risky_liquidity_providers.append(
-                    RiskySimpleLiquidityProvider(
-                        wallet_name="risky_liquidity_providers",
-                        key_name=f"HIGH_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                        market_name=market_name,
-                        asset_name=asset_name,
-                        initial_asset_mint=20_000,
-                        commitment_factor=0.5,
-                        step_bias=0.1,
-                        tag=f"HIGH_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                    )
+            market_agents["risky_traders"] = [
+                RiskyMarketOrderTrader(
+                    wallet_name="risky_traders",
+                    key_name=f"MARKET_{str(i_market).zfill(3)}_SIDE_{side}_AGENT_{str(i_agent).zfill(3)}",
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    side=side,
+                    initial_asset_mint=1_000,
+                    size_factor=0.5,
+                    step_bias=0.1,
+                    tag=f"MARKET_{str(i_market).zfill(3)}_SIDE_{side}_AGENT_{str(i_agent).zfill(3)}",
+                )
+                for side in ["SIDE_BUY", "SIDE_SELL"]
+                for i_agent in range(10)
+            ]
+
+            market_agents["risky_liquidity_providers"] = [
+                RiskySimpleLiquidityProvider(
+                    wallet_name="risky_liquidity_providers",
+                    key_name=f"HIGH_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    initial_asset_mint=20_000,
+                    commitment_factor=0.5,
+                    step_bias=0.1,
+                    tag=f"HIGH_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                 )
+                for i_agent in range(5)
+            ]
 
             for i_agent in range(45):
-                risky_liquidity_providers.append(
+                market_agents["risky_liquidity_providers"].append(
                     RiskySimpleLiquidityProvider(
                         wallet_name="risky_liquidity_providers",
                         key_name=f"LOW_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                         market_name=market_name,
                         asset_name=asset_name,
                         initial_asset_mint=20_000,
                         commitment_factor=0.3,
                         step_bias=0.1,
                         tag=f"LOW_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
 
-            for i_agent in range(5):
-                fuzz_liquidity_providers.append(
-                    FuzzyLiquidityProvider(
-                        wallet_name="FUZZY_LIQUIDITY_PROVIDERS",
-                        key_name=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                        market_name=market_name,
-                        asset_name=asset_name,
-                        initial_asset_mint=5_000,
-                        tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
-                    )
+            market_agents["fuzz_liquidity_providers"] = [
+                FuzzyLiquidityProvider(
+                    wallet_name="FUZZY_LIQUIDITY_PROVIDERS",
+                    key_name=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    initial_asset_mint=5_000,
+                    tag=(
+                        f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}"
+                    ),
                 )
+            ]
 
+            market_agents["reward_funders"] = []
             for i_agent, (account_type, metric) in enumerate(
                 [
                     (
                         vega_protos.vega.ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES,
                         vega_protos.vega.DISPATCH_METRIC_MAKER_FEES_PAID,
                     ),
                     (
@@ -404,43 +427,38 @@
                     ),
                     (
                         vega_protos.vega.ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS,
                         vega_protos.vega.DISPATCH_METRIC_MARKET_VALUE,
                     ),
                 ]
             ):
-                reward_funders.append(
+                market_agents["reward_funders"].append(
                     RewardFunder(
                         wallet_name="REWARD_FUNDERS",
                         key_name=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                         reward_asset_name=vega_protos.vega.DispatchMetric.Name(metric),
                         initial_mint=1e9,
                         account_type=account_type,
                         transfer_amount=100,
                         asset_for_metric_name=asset_name,
                         metric=metric,
                         market_names=[market_name],
                         stake_key=True,
                         tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
-
-        agents = (
-            market_managers
-            + market_makers
-            + at_touch_market_makers
-            + auction_traders
-            + random_traders
-            + fuzz_traders
-            + risky_traders
-            + risky_liquidity_providers
-            + fuzz_liquidity_providers
-            + reward_funders
-        )
-        return {agent.name(): agent for agent in agents}
+            self.market_agents[market_name] = market_agents
+            for agent_type, agent_list in market_agents.items():
+                self.all_agents[agent_type].extend(agent_list)
+
+        return {
+            agent.name(): agent
+            for agent_list in self.all_agents.values()
+            for agent in agent_list
+        }
 
     def configure_environment(
         self,
         vega: VegaServiceNull,
         **kwargs,
     ) -> MarketEnvironmentWithState:
         if kwargs.get("network", Network.NULLCHAIN) == Network.NULLCHAIN:
```

### Comparing `vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/hedged_market_maker/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/hedged_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/environments.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/environments.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/log_data.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/utils/log_data.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/strategy.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker/utils/strategy.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py` & `vega_sim-1.2.1/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/market_crash/price_process.py` & `vega_sim-1.2.1/vega_sim/scenario/market_crash/price_process.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/market_crash/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/market_crash/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/multi_market/agents.py` & `vega_sim-1.2.1/vega_sim/scenario/multi_market/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/multi_market/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/multi_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/parameter_experiment/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/parameter_experiment/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/realtime_market/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/realtime_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/registry.py` & `vega_sim-1.2.1/vega_sim/scenario/registry.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/scenario/scenario.py` & `vega_sim-1.2.1/vega_sim/scenario/scenario.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 from vega_sim.tools.scenario_output import (
     agents_standard_output,
     resources_standard_output,
     market_data_standard_output,
     agents_standard_output,
     assets_standard_output,
+    market_chain_standard_output,
 )
 
 import vega_sim.proto.vega as vega_protos
 
 
 class Scenario(abc.ABC):
     def __init__(
@@ -32,14 +33,18 @@
         additional_data_output_fns: Optional[Dict[str, Callable]] = None,
     ):
         self.agents = []
         self.env: Optional[MarketEnvironment] = None
         self.state_extraction_fn = state_extraction_fn
         self.additional_data_output_fns = additional_data_output_fns
 
+    def _step_end_callback(self):
+        """Called after each set of agent steps before the next loop begins."""
+        pass
+
     @abc.abstractmethod
     def configure_agents(
         self,
         vega: VegaService,
         tag: str,
         random_state: Optional[np.random.RandomState],
         **kwargs,
@@ -60,14 +65,15 @@
         self,
         pause_at_completion: bool = False,
         run_with_console: bool = False,
     ):
         result = self.env.run(
             pause_at_completion=pause_at_completion,
             run_with_console=run_with_console,
+            step_end_callback=self._step_end_callback,
         )
         return result
 
     def run_iteration(
         self,
         vega: VegaService,
         pause_at_completion: bool = False,
@@ -93,20 +99,22 @@
             vega=vega, tag=tag, random_state=random_state, **kwargs
         )
 
         outputs = self.env.run(
             pause_at_completion=pause_at_completion,
             run_with_console=run_with_console,
             log_every_n_steps=log_every_n_steps,
+            step_end_callback=self._step_end_callback,
         )
         if output_data:
             agents_standard_output(self.agents)
             resources_standard_output(self.get_resource_data())
             assets_standard_output(self.get_assets())
             market_data_standard_output(self.get_run_data())
+            market_chain_standard_output(self.get_run_data())
             if self.additional_data_output_fns is not None:
                 market_data_standard_output(
                     self.get_additional_run_data(),
                     custom_output_fns=self.additional_data_output_fns,
                 )
 
         return outputs
```

### Comparing `vega_sim-1.2.0/vega_sim/service.py` & `vega_sim-1.2.1/vega_sim/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,16 +389,16 @@
             asset,
             num_to_padded_int(amount, asset_decimals),
             faucet_url=self.faucet_url,
         )
 
         self.wait_fn(1)
         self.wait_for_total_catchup()
-        for i in range(500):
-            time.sleep(0.0005 * 1.01**i)
+        for i in range(100):
+            time.sleep(0.05 * 1.03**i)
             post_acct = self.party_account(
                 wallet_name=wallet_name,
                 asset_id=asset,
                 market_id=None,
                 key_name=key_name,
             ).general
             if post_acct > curr_acct:
@@ -482,35 +482,57 @@
         self.wait_for_thread_catchup()
 
     def create_market_from_config(
         self,
         proposal_key_name: str,
         market_config: market.MarketConfig,
         proposal_wallet_name: Optional[str] = None,
-    ):
+        vote_closing_time: Optional[datetime.datetime] = None,
+        vote_enactment_time: Optional[datetime.datetime] = None,
+        approve_proposal: bool = True,
+        forward_time_to_enactment: bool = True,
+    ) -> str:
         blockchain_time_seconds = self.get_blockchain_time(in_seconds=True)
 
+        enactment_time = (
+            blockchain_time_seconds + self.seconds_per_block * 50
+            if vote_enactment_time is None
+            else int(vote_enactment_time.timestamp())
+        )
+
         proposal_id = gov.propose_market_from_config(
             wallet=self.wallet,
             data_client=self.trading_data_client_v2,
             proposal_wallet_name=proposal_wallet_name,
             proposal_key_name=proposal_key_name,
             market_config=market_config,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
+            closing_time=(
+                blockchain_time_seconds + self.seconds_per_block * 40
+                if vote_closing_time is None
+                else int(vote_closing_time.timestamp())
+            ),
+            enactment_time=enactment_time,
             time_forward_fn=lambda: self.wait_fn(2),
         )
-        gov.approve_proposal(
-            proposal_id=proposal_id,
-            wallet=self.wallet,
-            wallet_name=proposal_wallet_name,
-            key_name=proposal_key_name,
-        )
-        self.wait_fn(60)
+        if approve_proposal:
+            gov.approve_proposal(
+                proposal_id=proposal_id,
+                wallet=self.wallet,
+                wallet_name=proposal_wallet_name,
+                key_name=proposal_key_name,
+            )
+
+        if forward_time_to_enactment:
+            time_to_enactment = enactment_time - self.get_blockchain_time(
+                in_seconds=True
+            )
+            self.wait_fn(int(time_to_enactment / self.seconds_per_block) + 1)
+
         self.wait_for_thread_catchup()
+        return proposal_id
 
     def create_simple_market(
         self,
         market_name: str,
         proposal_key: str,
         settlement_asset_id: str,
         termination_key: str,
@@ -521,15 +543,21 @@
         tau: Optional[float] = 1.0 / 365.25 / 24,
         sigma: Optional[float] = 1.0,
         price_monitoring_parameters: Optional[
             vega_protos.markets.PriceMonitoringParameters
         ] = None,
         wallet_name: Optional[str] = None,
         termination_wallet_name: Optional[str] = None,
-    ) -> None:
+        vote_closing_time: Optional[datetime.datetime] = None,
+        vote_enactment_time: Optional[datetime.datetime] = None,
+        approve_proposal: bool = True,
+        forward_time_to_enactment: bool = True,
+        parent_market_id: Optional[str] = None,
+        parent_market_insurance_pool_fraction: float = 1,
+    ) -> str:
         """Creates a simple futures market with a predefined reasonable set of parameters.
 
                 Args:
                     market_name:
                         str, name of the market
                     proposal_key:
                         str, the name of the key to use for proposing the market
@@ -548,54 +576,90 @@
                             market will drop into a price auction. If not passed defaults
                             to a very permissive setup
                             wallet_name: Optional[str] = None,
         :
                         Optional[str], name of wallet proposing market. Defaults to None.
                     termination_wallet_name:
                         Optional[str], name of wallet settling market. Defaults to None.
-
+                    vote_closing_time:
+                        Optional[datetime.datetime]: If set, decides at what time the vote will be set to
+                            close. Defaults to Now + 40 blocks
+                    vote_enactment_time:
+                        Optional[datetime.datetime]: If set, decides at what time the vote will be set to
+                            enact. Defaults to Now + 50 blocks
+                    approve_proposal:
+                        bool, default True, whether to automatically approve the proposal
+                    forward_time_to_enactment:
+                        bool, default True, whether to forward time until this proposal has already
+                            been enacted
+                    parent_market_id:
+                        Optional[str], Market to set as the parent market on the proposal
+                    parent_market_insurance_pool_fraction:
+                        float, Fraction of parent market insurance pool to carry over.
+                            defaults to 1. No-op if parent_market_id is not set.
         """
         additional_kwargs = {}
         if future_asset is not None:
             additional_kwargs["future_asset"] = future_asset
 
         blockchain_time_seconds = self.get_blockchain_time(in_seconds=True)
 
         risk_model = vega_protos.markets.LogNormalRiskModel(
             risk_aversion_parameter=risk_aversion,
             tau=tau,
             params=vega_protos.markets.LogNormalModelParams(mu=0, r=0.0, sigma=sigma),
         )
+
+        enactment_time = (
+            blockchain_time_seconds + self.seconds_per_block * 50
+            if vote_enactment_time is None
+            else int(vote_enactment_time.timestamp())
+        )
+
         proposal_id = gov.propose_future_market(
             market_name=market_name,
             wallet=self.wallet,
             wallet_name=wallet_name,
             key_name=proposal_key,
             settlement_asset_id=settlement_asset_id,
             data_client=self.trading_data_client_v2,
             termination_pub_key=self.wallet.public_key(
                 wallet_name=termination_wallet_name, name=termination_key
             ),
             position_decimals=position_decimals,
             market_decimals=market_decimals,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
+            closing_time=(
+                blockchain_time_seconds + self.seconds_per_block * 40
+                if vote_closing_time is None
+                else int(vote_closing_time.timestamp())
+            ),
+            enactment_time=enactment_time,
             risk_model=risk_model,
             time_forward_fn=lambda: self.wait_fn(2),
             price_monitoring_parameters=price_monitoring_parameters,
+            parent_market_id=parent_market_id,
+            parent_market_insurance_pool_fraction=parent_market_insurance_pool_fraction,
             **additional_kwargs,
         )
-        gov.approve_proposal(
-            proposal_id=proposal_id,
-            wallet=self.wallet,
-            wallet_name=wallet_name,
-            key_name=proposal_key,
-        )
-        self.wait_fn(60)
+        if approve_proposal:
+            gov.approve_proposal(
+                proposal_id=proposal_id,
+                wallet=self.wallet,
+                wallet_name=wallet_name,
+                key_name=proposal_key,
+            )
+
+        if forward_time_to_enactment:
+            time_to_enactment = enactment_time - self.get_blockchain_time(
+                in_seconds=True
+            )
+            self.wait_fn(int(time_to_enactment / self.seconds_per_block) + 1)
+
         self.wait_for_thread_catchup()
+        return proposal_id
 
     def submit_market_order(
         self,
         trading_key: str,
         market_id: str,
         side: Union[vega_protos.vega.Side, str],
         volume: float,
@@ -661,14 +725,16 @@
         expires_at: Optional[float] = None,
         pegged_order: Optional[PeggedOrder] = None,
         wait: bool = True,
         order_ref: Optional[str] = None,
         trading_wallet: Optional[str] = None,
         reduce_only: bool = False,
         post_only: bool = False,
+        peak_size: Optional[float] = None,
+        minimum_visible_size: Optional[float] = None,
     ) -> Optional[str]:
         """
         Submit orders as specified to required pre-existing market.
         Optionally wait for acceptance of order (raises on non-acceptance)
 
         Args:
             trading_key:
@@ -704,14 +770,18 @@
                 optional str, name of key in wallet to use
             reduce_only (bool):
                 Whether the order should only reduce a parties position. Defaults to
                 False.
             post_only (bool):
                 Whether order should be prevented from trading immediately. Defaults to
                 False.
+            peak_size:
+                optional float, size of the order that is made visible and can be traded with during the execution of a single order.
+            minimum_visible_size:
+                optional float, minimum allowed remaining size of the order before it is replenished back to its peak size
 
         Returns:
             Optional[str], If order acceptance is waited for, returns order ID.
                 Otherwise None
         """
         submit_volume = num_to_padded_int(
             volume,
@@ -736,14 +806,21 @@
         if submit_price is not None and submit_price <= 0:
             msg = "Not submitting order as price is 0 or less."
             if wait:
                 raise Exception(msg)
             else:
                 logger.debug(msg)
                 return
+        if (peak_size is None and minimum_visible_size is not None) or (
+            peak_size is not None and minimum_visible_size is None
+        ):
+            raise ValueError(
+                "Both 'peak_size' and 'minimum_visible_size' must be specified or none"
+                " at all."
+            )
 
         return trading.submit_order(
             wallet=self.wallet,
             wallet_name=trading_wallet,
             data_client=self.trading_data_client_v2,
             market_id=market_id,
             order_type=order_type,
@@ -766,14 +843,26 @@
             ),
             wait=wait,
             time_forward_fn=lambda: self.wait_fn(2),
             order_ref=order_ref,
             key_name=trading_key,
             reduce_only=reduce_only,
             post_only=post_only,
+            iceberg_opts=(
+                vega_protos.commands.v1.commands.IcebergOpts(
+                    peak_size=num_to_padded_int(
+                        peak_size, self.market_pos_decimals[market_id]
+                    ),
+                    minimum_visible_size=num_to_padded_int(
+                        minimum_visible_size, self.market_pos_decimals[market_id]
+                    ),
+                )
+                if (peak_size is not None and minimum_visible_size is not None)
+                else None
+            ),
         )
 
     def get_blockchain_time(self, in_seconds: bool = False) -> int:
         """Returns blockchain time in seconds or nanoseconds since the epoch"""
         return gov.get_blockchain_time(
             self.trading_data_client_v2, in_seconds=in_seconds
         )
```

### Comparing `vega_sim-1.2.0/vega_sim/tools/load_binaries.py` & `vega_sim-1.2.1/vega_sim/tools/load_binaries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+import argparse
 import logging
 import os
 import platform
 import shutil
 import tempfile
 import zipfile
 
 import requests
 
 import vega_sim
 
 logger = logging.getLogger(__name__)
 
 URL_BASE = "https://github.com/vegaprotocol/vega/releases/download/v{version}/"
+URL_LATEST_BASE = "https://github.com/vegaprotocol/vega/releases/latest/download/"
 DATA_NODE = "data-node-{platform}-{chipset}64.zip"
 VEGA_CORE = "vega-{platform}-{chipset}64.zip"
 VEGAWALLET = "vegawallet-{platform}-{chipset}64.zip"
 
 FILES = [DATA_NODE, VEGA_CORE, VEGAWALLET]
 
 BIN_NAMES = {
     DATA_NODE: "data-node",
     VEGA_CORE: "vega",
     VEGAWALLET: "vegawallet",
 }
 
 
-def download_binaries(force: bool = False):
+def download_binaries(force: bool = False, latest: bool = False):
     platf = platform.system().lower()
 
     # We have no Windows specific builds, so people have to use WSL to run
     platf = "linux" if platf == "windows" else platf
 
     chipset = "arm" if "arm" in platform.machine() else "amd"
 
@@ -44,23 +46,34 @@
             if (
                 not os.path.exists(
                     os.path.join(vega_sim.vega_bin_path, BIN_NAMES[remote_file])
                 )
             ) or force:
                 logger.info(f"Downloading {file_name}")
 
-                url = URL_BASE.format(version=vega_sim.VEGA_VERSION) + file_name
+                url_base = (
+                    URL_BASE.format(version=vega_sim.VEGA_VERSION)
+                    if not latest
+                    else URL_LATEST_BASE
+                )
+                url = url_base + file_name
                 res = requests.get(url)
                 file_path = os.path.join(dir, f"{file_name}")
 
                 with open(file_path, "wb") as f:
                     f.write(res.content)
                 with zipfile.ZipFile(file_path, "r") as zip_ref:
                     zip_ref.extractall(vega_sim.vega_bin_path)
 
         for bin_file in os.listdir(vega_sim.vega_bin_path):
             os.chmod(os.path.join(vega_sim.vega_bin_path, bin_file), 0o775)
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    download_binaries()
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-f", "--force", action="store_true")
+    parser.add_argument("--latest", action="store_true")
+    args = parser.parse_args()
+
+    download_binaries(force=args.force, latest=args.latest)
```

### Comparing `vega_sim-1.2.0/vega_sim/tools/scenario_output.py` & `vega_sim-1.2.1/vega_sim/tools/scenario_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from vega_sim.environment.agent import Agent, StateAgentWithWallet
 from vega_sim.scenario.common.agents import MarketHistoryData, ResourceData
 from typing import List, Callable, Optional, Dict
 import pandas as pd
 import itertools
 import os
 import os.path
+import json
 
 import vega_sim.proto.vega as vega_protos
 
 DEFAULT_PATH = "./run_logs"
 DEFAULT_RUN_NAME = "latest"
 
 AGENTS_FILE_NAME = "agents.csv"
 DATA_FILE_NAME = "market_data.csv"
 ORDER_BOOK_FILE_NAME = "depth_data.csv"
 TRADES_FILE_NAME = "trades.csv"
 ACCOUNTS_FILE_NAME = "accounts.csv"
 FUZZING_FILE_NAME = "additional_data.csv"
 RESOURCES_FILE_NAME = "resources.csv"
+ASSETS_FILE_NAME = "assets.csv"
+MARKET_CHAIN_FILE_NAME = "market_chain.json"
 
 
 def resource_data_to_row(data: ResourceData):
     return [
         {
             "time": data.at_time,
             "vega_cpu_per": data.vega_cpu_per,
@@ -30,17 +33,14 @@
             "datanode_cpu_per": data.datanode_cpu_per,
             "datanode_mem_rss": data.datanode_mem_rss,
             "datanode_mem_vms": data.datanode_mem_vms,
         }
     ]
 
 
-ASSETS_FILE_NAME = "assets.csv"
-
-
 def history_data_to_row(data: MarketHistoryData) -> List[pd.Series]:
     results = []
     for market_id in data.market_info.keys():
         market_data = data.market_data[market_id]
 
         results.append(
             {
@@ -266,14 +266,38 @@
     full_path = os.path.join(output_path, run_name)
     os.makedirs(full_path, exist_ok=True)
     pd.DataFrame.from_dict(results).set_index("id", drop=True).to_csv(
         os.path.join(full_path, ASSETS_FILE_NAME)
     )
 
 
+def market_chain_standard_output(
+    market_history_data: List[MarketHistoryData],
+    run_name: str = DEFAULT_RUN_NAME,
+    output_path: str = DEFAULT_PATH,
+):
+    run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
+    full_path = os.path.join(output_path, run_name)
+
+    market_chains: Dict[str, List[str]] = {}
+    for history_data in market_history_data:
+        for market_id, market_info in history_data.market_info.items():
+            if not market_info.parent_market_id:
+                market_chains.setdefault(market_id, [market_id])
+            else:
+                for _, market_chain in market_chains.items():
+                    if market_chain[-1] == market_info.parent_market_id:
+                        market_chain.append(market_id)
+
+    os.makedirs(output_path, exist_ok=True)
+
+    with open(os.path.join(full_path, MARKET_CHAIN_FILE_NAME), "w") as f:
+        json.dump(market_chains, f, indent=4)
+
+
 def load_agents_df(
     run_name: Optional[str] = None,
     output_path: str = DEFAULT_PATH,
 ) -> pd.DataFrame:
     run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
     return pd.read_csv(
         os.path.join(output_path, run_name, AGENTS_FILE_NAME), index_col="agent_name"
@@ -358,7 +382,21 @@
 ) -> pd.DataFrame:
     run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
     df = pd.read_csv(os.path.join(output_path, run_name, RESOURCES_FILE_NAME))
     if not df.empty:
         df["time"] = pd.to_datetime(df.time)
         df = df.set_index("time")
     return df
+
+
+def load_market_chain(
+    run_name: Optional[str] = None,
+    output_path: str = DEFAULT_PATH,
+) -> Dict[str, List[str]]:
+    run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
+    file_path = os.path.join(output_path, run_name, MARKET_CHAIN_FILE_NAME)
+    if os.path.exists(file_path):
+        with open(file_path, "r") as f:
+            market_chain = json.load(fp=f)
+    else:
+        market_chain = {}
+    return market_chain
```

### Comparing `vega_sim-1.2.0/vega_sim/tools/scenario_plots.py` & `vega_sim-1.2.1/vega_sim/tools/scenario_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import ast
 
+import itertools
 import argparse
 
 import pandas as pd
+import numpy as np
 import matplotlib.pyplot as plt
 import vega_sim.proto.vega as vega_protos
 
-from typing import Optional
+from typing import Optional, List
 from collections import defaultdict
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.markers import MarkerStyle
 from matplotlib.gridspec import GridSpec, SubplotSpec, GridSpecFromSubplotSpec
 
 from vega_sim.scenario.fuzzed_markets.agents import (
@@ -29,14 +31,15 @@
 TRADING_MODE_COLORS = {
     0: (200 / 255, 200 / 255, 200 / 255),
     1: (204 / 255, 255 / 255, 15 / 2553),
     2: (255 / 255, 204 / 255, 153 / 255),
     3: (153 / 255, 204 / 255, 244 / 255),
     4: (255 / 255, 133 / 255, 133 / 255),
     5: (255 / 255, 204 / 255, 255 / 255),
+    6: (255 / 255, 0 / 255, 0 / 255),
 }
 
 
 """
 Thoughts for plots
     - Total LP Margin positions
     - Market State
@@ -45,14 +48,15 @@
 from vega_sim.tools.scenario_output import (
     load_accounts_df,
     load_market_data_df,
     load_order_book_df,
     load_trades_df,
     load_fuzzing_df,
     load_agents_df,
+    load_market_chain,
     load_resource_df,
     load_assets_df,
 )
 
 
 def _set_xticks(ax, index, freq: int = 60):
     xaxis_ticks = index[0:-1:freq]
@@ -88,14 +92,26 @@
         .unstack(level=-1)
         .transpose()
         .sort_index(ascending=False)
         .values
     )
 
 
+def _series_df_to_single_series(
+    df: pd.DataFrame, market_series: List[str]
+) -> pd.DataFrame:
+    df_clone = df.copy().reset_index()
+    df_clone["series_ix"] = df_clone.market_id.apply(lambda x: market_series.index(x))
+    selector = df_clone.loc[df_clone.groupby("time").series_ix.idxmax()][
+        ["time", "market_id"]
+    ]
+
+    return df_clone.merge(selector, on=["time", "market_id"]).set_index("time")
+
+
 def plot_trading_summary(
     ax: Axes,
     trade_df: pd.DataFrame,
     order_book_df: pd.DataFrame,
     price_df: pd.DataFrame,
 ) -> None:
     if any(df.empty for df in (trade_df, order_book_df, price_df)):
@@ -209,21 +225,39 @@
 
 def plot_run_outputs(run_name: Optional[str] = None) -> list[Figure]:
     order_df = load_order_book_df(run_name=run_name)
     trades_df = load_trades_df(run_name=run_name)
     data_df = load_market_data_df(run_name=run_name)
     accounts_df = load_accounts_df(run_name=run_name)
 
+    market_chains = load_market_chain(run_name=run_name)
+    if not market_chains:
+        market_chains = {
+            market_id: [market_id] for market_id in data_df["market_id"].unique()
+        }
+
     figs = {}
 
-    for market_id in data_df["market_id"].unique():
-        market_order_df = order_df[order_df["market_id"] == market_id]
-        market_trades_df = trades_df[trades_df["market_id"] == market_id]
-        market_data_df = data_df[data_df["market_id"] == market_id]
-        market_accounts_df = accounts_df[accounts_df["market_id"] == market_id]
+    for market_id, market_children in market_chains.items():
+        market_order_df = _series_df_to_single_series(
+            order_df[order_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
+        market_trades_df = _series_df_to_single_series(
+            trades_df[trades_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
+        market_data_df = _series_df_to_single_series(
+            data_df[data_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
+        market_accounts_df = _series_df_to_single_series(
+            accounts_df[accounts_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
 
         market_mid_df = (
             market_order_df[market_order_df.level == 0].groupby("time")[["price"]].sum()
             / 2
         )
 
         fig = plt.figure(layout="tight", figsize=(8, 10))
@@ -370,15 +404,18 @@
 
     ep_volatility = external_price_series.var() / external_price_series.size
     mp_volatility = mark_price_series.var() / mark_price_series.size
 
     ax0.text(
         x=0.1,
         y=0.1,
-        s=f"external-price volatility = {round(ep_volatility, 1)}\nmark-price volatility = {round(mp_volatility, 1)}",
+        s=(
+            f"external-price volatility = {round(ep_volatility, 1)}\nmark-price"
+            f" volatility = {round(mp_volatility, 1)}"
+        ),
         fontsize=8,
         bbox=dict(facecolor="white", alpha=1),
         transform=ax0.transAxes,
     )
 
     ax0.set_ylabel("PRICE")
     ax0.legend(labels=["external price", "mark price"])
@@ -422,14 +459,15 @@
     ax1 = fig.add_subplot(gs[1, 0])
 
     ax0.set_title("Close Out Analysis", loc="left", fontsize=12, color=(0.3, 0.3, 0.3))
 
     insurance_pool_ds = accounts_df["balance"][
         (accounts_df["party_id"] == "network") & (accounts_df["type"] == 1)
     ]
+
     trader_close_outs_ds = fuzzing_df["trader_close_outs"]
     liquidity_provider_close_outs_ds = fuzzing_df["liquidity_provider_close_outs"]
 
     ax0r = ax0.twinx()
 
     ln0 = ax0r.plot(
         insurance_pool_ds.index,
@@ -481,21 +519,35 @@
 
 
 def fuzz_plots(run_name: Optional[str] = None) -> Figure:
     data_df = load_market_data_df(run_name=run_name)
     accounts_df = load_accounts_df(run_name=run_name)
     fuzzing_df = load_fuzzing_df(run_name=run_name)
 
-    markets = data_df.market_id.unique()
+    market_chains = load_market_chain(run_name=run_name)
+    if not market_chains:
+        market_chains = {
+            market_id: [market_id] for market_id in data_df["market_id"].unique()
+        }
 
     figs = {}
-    for market_id in markets:
-        market_data_df = data_df[data_df["market_id"] == market_id]
-        market_accounts_df = accounts_df[accounts_df["market_id"] == market_id]
-        market_fuzzing_df = fuzzing_df[fuzzing_df["market_id"] == market_id]
+    for market_id, market_children in market_chains.items():
+        market_data_df = _series_df_to_single_series(
+            data_df[data_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
+        market_accounts_df = _series_df_to_single_series(
+            accounts_df[accounts_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
+
+        market_fuzzing_df = _series_df_to_single_series(
+            fuzzing_df[fuzzing_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
 
         fig = plt.figure(figsize=[8, 10])
         fig.suptitle(
             f"Fuzz Testing Plots",
             fontsize=18,
             fontweight="bold",
             color=(0.2, 0.2, 0.2),
@@ -574,30 +626,46 @@
         axs[i].autoscale(enable=True, axis="y")
 
     return fig
 
 
 def plot_price_monitoring(run_name: Optional[str] = None):
     data_df = load_market_data_df(run_name=run_name)
-
-    market_ids = data_df.market_id.unique()
+    market_chains = load_market_chain(run_name=run_name)
+    if not market_chains:
+        market_chains = {
+            market_id: [market_id] for market_id in data_df["market_id"].unique()
+        }
 
     figs = {}
-    for market_id in market_ids:
-        market_data_df = data_df[data_df["market_id"] == market_id]
+    for market_id, market_children in market_chains.items():
+        market_data_df = _series_df_to_single_series(
+            data_df[data_df["market_id"].isin(market_children)],
+            market_series=market_children,
+        )
 
         # Extract the tightest valid prices from the price monitoring valid_prices
         valid_prices = defaultdict(lambda: [])
         for index in market_data_df.index:
-            all_bounds = ast.literal_eval(
-                market_data_df.loc[index]["price_monitoring_bounds"]
+            all_bounds = list(
+                itertools.chain(
+                    *[
+                        ast.literal_eval(
+                            bounds[0] if isinstance(bounds, np.ndarray) else bounds
+                        )
+                        for bounds in market_data_df.loc[index][
+                            ["price_monitoring_bounds"]
+                        ].values
+                    ]
+                )
             )
             valid_prices["datetime"].append(index)
             valid_prices["min_valid_price"].append(np.nan)
             valid_prices["max_valid_price"].append(np.nan)
+
             for _, individual_bound in enumerate(all_bounds):
                 valid_prices["min_valid_price"][-1] = (
                     individual_bound[0]
                     if valid_prices["min_valid_price"][-1] is np.nan
                     else max(individual_bound[0], valid_prices["min_valid_price"][-1])
                 )
                 valid_prices["max_valid_price"][-1] = (
@@ -866,14 +934,15 @@
     if args.monitoring or args.all:
         figs = plot_price_monitoring()
         for i, fig in enumerate(figs.values()):
             if args.save:
                 fig.savefig(f"{dir}/monitoring-{i}.jpg")
 
     if args.accounts or args.all:
+        print("accounting")
         fig = account_plots()
         if args.save:
             fig.savefig(f"{dir}/accounts.jpg")
 
     if args.rewards or args.all:
         fig = reward_plots()
         if args.save:
```

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/config.hcl` & `vega_sim-1.2.1/vega_sim/vegacapsule/config.hcl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/genesis.tmpl` & `vega_sim-1.2.1/vega_sim/vegacapsule/genesis.tmpl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/smart_contracts_addresses.json` & `vega_sim-1.2.1/vega_sim/vegacapsule/smart_contracts_addresses.json`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/templates/data_node_full.tmpl` & `vega_sim-1.2.1/vega_sim/vegacapsule/templates/data_node_full.tmpl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/templates/tendermint_full.tmpl` & `vega_sim-1.2.1/vega_sim/vegacapsule/templates/tendermint_full.tmpl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/templates/tendermint_validators.tmpl` & `vega_sim-1.2.1/vega_sim/vegacapsule/templates/tendermint_validators.tmpl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/templates/vega_full.tmpl` & `vega_sim-1.2.1/vega_sim/vegacapsule/templates/vega_full.tmpl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegacapsule/templates/vega_validators.tmpl` & `vega_sim-1.2.1/vega_sim/vegacapsule/templates/vega_validators.tmpl`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/config/data-node/config.toml` & `vega_sim-1.2.1/vega_sim/vegahome/config/data-node/config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
   ProfilesDir = "/tmp"
   BlockProfileRate = 0
   MutexProfileFraction = 0
 
 [SQLStore]
   Enabled = true
   WipeOnStartup = true
-  UseEmbedded = true
+  UseEmbedded = false
   [SQLStore.ConnectionConfig]
     Host = "localhost"
     Port = "TO_BE_SET"
     Username = "vega"
     Password = "vega"
     Database = "vega"
     UseTransactions = false
```

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/config/node/config.toml` & `vega_sim-1.2.1/vega_sim/vegahome/config/node/config.toml`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276` & `vega_sim-1.2.1/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758` & `vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243` & `vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067` & `vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082` & `vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124` & `vega_sim-1.2.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem` & `vega_sim-1.2.1/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem` & `vega_sim-1.2.1/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/vegahome/genesis.json` & `vega_sim-1.2.1/vega_sim/vegahome/genesis.json`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/wallet/base.py` & `vega_sim-1.2.1/vega_sim/wallet/base.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/wallet/slim_wallet.py` & `vega_sim-1.2.1/vega_sim/wallet/slim_wallet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/vega_sim/wallet/vega_wallet.py` & `vega_sim-1.2.1/vega_sim/wallet/vega_wallet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.2.0/PKG-INFO` & `vega_sim-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vega-sim
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simulator for running self-contained Vega chain on local PC
 License: MIT
 Author: Tom McLean
 Author-email: tom@vegaprotocol.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Provides-Extra: agents
 Provides-Extra: jupyter
 Provides-Extra: learning
 Provides-Extra: profile
 Requires-Dist: PyNaCl
 Requires-Dist: TA-Lib ; extra == "agents"
 Requires-Dist: deprecated
+Requires-Dist: docker
 Requires-Dist: grpcio-tools
 Requires-Dist: gymnasium ; extra == "learning"
 Requires-Dist: inflection
 Requires-Dist: ipywidgets ; extra == "jupyter"
 Requires-Dist: jupyter ; extra == "jupyter"
 Requires-Dist: jupyterlab ; extra == "jupyter"
 Requires-Dist: matplotlib ; extra == "learning" or extra == "jupyter"
@@ -31,15 +32,15 @@
 Requires-Dist: pettingzoo ; extra == "learning"
 Requires-Dist: plotly
 Requires-Dist: protoc-gen-openapiv2
 Requires-Dist: psutil
 Requires-Dist: pytest-profiling ; extra == "profile"
 Requires-Dist: python-dotenv
 Requires-Dist: requests
-Requires-Dist: sb3-contrib
+Requires-Dist: sb3-contrib (>=2.0.0a1,<3.0.0)
 Requires-Dist: scipy
 Requires-Dist: snakeviz ; extra == "profile"
 Requires-Dist: stable-baselines3 ; extra == "learning"
 Requires-Dist: tensorboard ; extra == "learning"
 Requires-Dist: tianshou ; extra == "learning"
 Requires-Dist: toml
 Requires-Dist: torch ; extra == "learning"
```

