# Comparing `tmp/argrelay-0.1.0.dev4.tar.gz` & `tmp/argrelay-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argrelay-0.1.0.dev4.tar", last modified: Sun Aug  6 10:44:22 2023, max compression
+gzip compressed data, was "argrelay-0.1.0.dev5.tar", last modified: Sun Aug  6 11:51:18 2023, max compression
```

## Comparing `argrelay-0.1.0.dev4.tar` & `argrelay-0.1.0.dev5.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.180954 argrelay-0.1.0.dev4/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.1.0.dev4/LICENSE
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-08-06 10:44:22.180954 argrelay-0.1.0.dev4/PKG-INFO
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.157954 argrelay-0.1.0.dev4/docs/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.158954 argrelay-0.1.0.dev4/docs/dev_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      538 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/argrelay_env_var_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5522 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/bootstrap_procedure.1.project_creation.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2508 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1716 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2506 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/code_style.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/completion_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5991 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/completion_perf_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4799 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/how_search_works.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1289 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/mongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/plugin_development.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/plugin_interaction.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7764 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/query_perf_10_x_more_data_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7125 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/query_perf_cache_vs_no_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4264 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/query_perf_mongomock_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8339 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/query_perf_pymongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/release_procedure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      729 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/screencast_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/scripts_summary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      357 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/semver_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1964 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/term_dictionary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      904 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/testing_guidelines.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10550 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/top_todos.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/dev_notes/ui_tests_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1637 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/dev_notes/version_format.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.161954 argrelay-0.1.0.dev4/docs/feature_stories/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1922 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1486 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1256 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1685 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      545 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3030 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_29_54_67_86.dir_structure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1239 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_31_70_49_15.search_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      392 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1184 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1251 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_46_96_59_05.init_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1478 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_55_57_45_04.demo_logic.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      564 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_58_61_77_69.dev_shell.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      372 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1454 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_62_25_92_06.assigned_context.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      599 2023-08-06 08:14:16.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_67_16_61_97.git_plugin.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1316 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_71_87_33_52.help_hint.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1485 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_72_40_53_00.fill_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2072 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      473 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_88_66_66_73.intercept_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1385 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/FS_94_30_49_28.help_doc.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/feature_stories/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.161954 argrelay-0.1.0.dev4/docs/known_issues/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1032 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      962 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      325 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/known_issues/KI_99_81_19_25.no_space_in_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/docs/known_issues/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      668 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.162954 argrelay-0.1.0.dev4/docs/test_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      694 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/docs/test_data/TD_38_03_48_51.large_data_set.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      386 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9497 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/docs/test_data/TD_63_37_05_36.demo_services_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/test_data/TD_70_69_38_46.no_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      398 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev4/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/docs/test_data/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev4/pyproject.toml
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15811 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2023-08-06 10:44:22.180954 argrelay-0.1.0.dev4/setup.cfg
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3849 2023-08-06 10:41:32.000000 argrelay-0.1.0.dev4/setup.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.155954 argrelay-0.1.0.dev4/src/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.162954 argrelay-0.1.0.dev4/src/argrelay/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.162954 argrelay-0.1.0.dev4/src/argrelay/client_command_local/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1642 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_local/AbstractLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      876 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_local/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.163954 argrelay-0.1.0.dev4/src/argrelay/client_command_remote/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2252 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      845 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/client_command_remote/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.164954 argrelay-0.1.0.dev4/src/argrelay/custom_integ/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      282 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/DemoInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      828 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/DemoInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1364 2023-08-06 09:30:09.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2899 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1506 2023-08-06 09:05:26.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10066 2023-08-06 09:58:24.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2023-08-06 09:44:56.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      713 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8041 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      188 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    59593 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      835 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      209 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ/value_constants.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.165954 argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6779 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/argrelay_rc.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    20152 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/dev_shell.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1875 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/init_shell_env.bash
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.166954 argrelay-0.1.0.dev4/src/argrelay/enum_desc/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1158 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/ArgSource.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2701 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/CompType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      568 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/GlobalArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/InterpStep.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      191 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/PluginType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      151 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/ReservedArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      164 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/ReservedEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1163 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/RunMode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/SpecialChar.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      106 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/SpecialFunc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      685 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/TermColor.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/TokenType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/enum_desc/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.166954 argrelay-0.1.0.dev4/src/argrelay/handler_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1691 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/handler_request/AbstractServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1242 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      943 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2949 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/handler_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.166954 argrelay-0.1.0.dev4/src/argrelay/handler_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      177 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/handler_response/AbstractClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      716 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      446 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/handler_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.167954 argrelay-0.1.0.dev4/src/argrelay/misc_helper/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1308 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/misc_helper/AbstractPlugin.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1738 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/misc_helper/ElapsedTime.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      950 2023-08-06 08:40:16.000000 argrelay-0.1.0.dev4/src/argrelay/misc_helper/TypeDesc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1360 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/misc_helper/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.167954 argrelay-0.1.0.dev4/src/argrelay/mongo_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2389 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoClientWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      450 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1732 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoServerWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev4/src/argrelay/mongo_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.168954 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4136 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/AbstractDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1670 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/ErrorDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      807 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5330 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/HelpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2732 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/InterceptDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1214 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/InvocationInput.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1077 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/NoopDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.169954 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1444 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/AbstractInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      351 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/AbstractInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      646 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FirstArgInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1948 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FirstArgInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      940 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12638 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FuncArgsInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2524 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FuncArgsInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      833 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/NoopInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      666 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/NoopInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/TreePathInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      911 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/TreePathInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.169954 argrelay-0.1.0.dev4/src/argrelay/plugin_loader/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_loader/AbstractLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1587 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_loader/HelpLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1675 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_loader/InterceptLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_loader/NoopLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/plugin_loader/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.170954 argrelay-0.1.0.dev4/src/argrelay/relay_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/AbstractClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/AbstractClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/AbstractClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1290 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/LocalClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2204 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/LocalClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/RemoteClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1546 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/RemoteClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2180 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_client/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.171954 argrelay-0.1.0.dev4/src/argrelay/relay_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4665 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/CustomFlaskApp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/GuiBannerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1419 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/HelpHintCache.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5700 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/LocalServer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/QueryCacheConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5872 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/QueryEngine.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      562 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/QueryResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.171954 argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_static/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27871 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_static/argrelay_client.js
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4505 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_static/argrelay_style.css
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_static/external_link.svg
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.171954 argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_templates/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5567 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_templates/argrelay_main.html
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5438 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/route_api.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      922 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/relay_server/route_gui.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.172954 argrelay-0.1.0.dev4/src/argrelay/runtime_context/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5451 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/EnvelopeContainer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/InitControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2875 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/InputContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10161 2023-08-06 09:30:09.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/InterpContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5871 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/ParsedContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/RequestContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2179 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/SearchControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_context/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.172954 argrelay-0.1.0.dev4/src/argrelay/runtime_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/AssignedValue.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      247 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/ClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/ConnectionConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      289 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/PluginEntry.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2162 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/ServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      604 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/StaticData.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/runtime_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.172954 argrelay-0.1.0.dev4/src/argrelay/sample_conf/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/sample_conf/argrelay.client.json
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11172 2023-08-06 09:56:37.000000 argrelay-0.1.0.dev4/src/argrelay/sample_conf/argrelay.server.yaml
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.173954 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1347 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_client/ClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1056 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_client/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.173954 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      852 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1621 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/MongoConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1196 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3999 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/ServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1570 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/StaticDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.174954 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3942 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1088 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1035 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/InitControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2047 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/SearchControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.174954 argrelay-0.1.0.dev4/src/argrelay/schema_config_plugin/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2598 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_plugin/PluginEntrySchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/schema_config_plugin/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.174954 argrelay-0.1.0.dev4/src/argrelay/schema_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3257 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_request/RequestContextSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/schema_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.175954 argrelay-0.1.0.dev4/src/argrelay/schema_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      706 2023-05-07 13:37:37.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/ArgValuesSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1742 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/AssignedValueSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3026 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/EnvelopeContainerSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      856 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/FilteredDict.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1207 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/InterpResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2126 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/InterpResultSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3250 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/InvocationInputSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev4/src/argrelay/schema_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.175954 argrelay-0.1.0.dev4/src/argrelay/server_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1543 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/server_spec/DescribeLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1268 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/server_spec/ProposeArgValuesSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1325 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/server_spec/RelayLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev4/src/argrelay/server_spec/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      772 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/server_spec/const_int.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3031 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/server_spec/server_data_schema.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.175954 argrelay-0.1.0.dev4/src/argrelay/test_helper/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    20113 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/test_helper/EnvMockBuilder.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4046 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/test_helper/InOutTestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      684 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev4/src/argrelay/test_helper/OpenFileMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1892 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev4/src/argrelay/test_helper/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 10:44:22.162954 argrelay-0.1.0.dev4/src/argrelay.egg-info/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-08-06 10:44:22.000000 argrelay-0.1.0.dev4/src/argrelay.egg-info/PKG-INFO
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27812 2023-08-06 10:44:22.000000 argrelay-0.1.0.dev4/src/argrelay.egg-info/SOURCES.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2023-08-06 10:44:22.000000 argrelay-0.1.0.dev4/src/argrelay.egg-info/dependency_links.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      148 2023-08-06 10:44:22.000000 argrelay-0.1.0.dev4/src/argrelay.egg-info/requires.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2023-08-06 10:44:22.000000 argrelay-0.1.0.dev4/src/argrelay.egg-info/top_level.txt
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.339182 argrelay-0.1.0.dev5/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.1.0.dev5/LICENSE
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-08-06 11:51:18.339182 argrelay-0.1.0.dev5/PKG-INFO
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.315182 argrelay-0.1.0.dev5/docs/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.317182 argrelay-0.1.0.dev5/docs/dev_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      538 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/argrelay_env_var_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5522 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/bootstrap_procedure.1.project_creation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2508 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1716 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2506 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/code_style.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/completion_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5991 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/completion_perf_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4799 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/how_search_works.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1289 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/mongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/plugin_development.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/plugin_interaction.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7764 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/query_perf_10_x_more_data_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7125 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/query_perf_cache_vs_no_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4264 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/query_perf_mongomock_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8339 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/query_perf_pymongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/release_procedure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      729 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/screencast_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/scripts_summary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      357 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/semver_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1964 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/term_dictionary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      904 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/testing_guidelines.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10582 2023-08-06 11:03:24.000000 argrelay-0.1.0.dev5/docs/dev_notes/top_todos.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/dev_notes/ui_tests_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1637 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/dev_notes/version_format.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.319182 argrelay-0.1.0.dev5/docs/feature_stories/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1922 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1486 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1256 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1685 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      545 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3030 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_29_54_67_86.dir_structure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1239 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_31_70_49_15.search_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      392 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1184 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1251 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_46_96_59_05.init_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1478 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_55_57_45_04.demo_logic.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      564 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_58_61_77_69.dev_shell.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      372 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1454 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_62_25_92_06.assigned_context.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      599 2023-08-06 08:14:16.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_67_16_61_97.git_plugin.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1316 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_71_87_33_52.help_hint.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1485 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_72_40_53_00.fill_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2072 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      473 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_88_66_66_73.intercept_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1385 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/FS_94_30_49_28.help_doc.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/feature_stories/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.320182 argrelay-0.1.0.dev5/docs/known_issues/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1032 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      962 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      325 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/known_issues/KI_99_81_19_25.no_space_in_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/docs/known_issues/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      668 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.320182 argrelay-0.1.0.dev5/docs/test_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      694 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/docs/test_data/TD_38_03_48_51.large_data_set.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      386 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9497 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/docs/test_data/TD_63_37_05_36.demo_services_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/test_data/TD_70_69_38_46.no_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      398 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev5/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/docs/test_data/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15811 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2023-08-06 11:51:18.339182 argrelay-0.1.0.dev5/setup.cfg
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3849 2023-08-06 11:47:58.000000 argrelay-0.1.0.dev5/setup.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.313182 argrelay-0.1.0.dev5/src/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.320182 argrelay-0.1.0.dev5/src/argrelay/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.321182 argrelay-0.1.0.dev5/src/argrelay/client_command_local/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1642 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_local/AbstractLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      876 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_local/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.322182 argrelay-0.1.0.dev5/src/argrelay/client_command_remote/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2252 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      845 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/client_command_remote/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.323182 argrelay-0.1.0.dev5/src/argrelay/custom_integ/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      282 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/DemoInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      828 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/DemoInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1428 2023-08-06 11:41:59.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3003 2023-08-06 11:31:43.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1506 2023-08-06 09:05:26.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10489 2023-08-06 11:45:29.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2023-08-06 09:44:56.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      713 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8041 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      188 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    59593 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      835 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      209 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ/value_constants.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.323182 argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6779 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/argrelay_rc.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    20152 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/dev_shell.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1875 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/init_shell_env.bash
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.324182 argrelay-0.1.0.dev5/src/argrelay/enum_desc/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1158 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/ArgSource.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2701 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/CompType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      568 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/GlobalArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/InterpStep.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      191 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/PluginType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      151 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/ReservedArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      164 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/ReservedEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1163 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/RunMode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/SpecialChar.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      106 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/SpecialFunc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      685 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/TermColor.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/TokenType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/enum_desc/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.325182 argrelay-0.1.0.dev5/src/argrelay/handler_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1691 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/handler_request/AbstractServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1242 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      943 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2949 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/handler_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.325182 argrelay-0.1.0.dev5/src/argrelay/handler_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      177 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/handler_response/AbstractClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      716 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      446 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/handler_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.326182 argrelay-0.1.0.dev5/src/argrelay/misc_helper/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1308 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/misc_helper/AbstractPlugin.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1738 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/misc_helper/ElapsedTime.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      950 2023-08-06 08:40:16.000000 argrelay-0.1.0.dev5/src/argrelay/misc_helper/TypeDesc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1360 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/misc_helper/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.326182 argrelay-0.1.0.dev5/src/argrelay/mongo_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2389 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoClientWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      450 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1732 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoServerWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev5/src/argrelay/mongo_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.327182 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4136 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/AbstractDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1670 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/ErrorDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      807 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5330 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/HelpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2732 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/InterceptDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1214 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/InvocationInput.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1077 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/NoopDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.328182 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1444 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/AbstractInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      351 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/AbstractInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      646 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FirstArgInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1948 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FirstArgInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      940 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12638 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FuncArgsInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2524 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FuncArgsInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      833 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/NoopInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      666 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/NoopInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5734 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/TreePathInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      911 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/TreePathInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.328182 argrelay-0.1.0.dev5/src/argrelay/plugin_loader/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_loader/AbstractLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1587 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_loader/HelpLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1675 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_loader/InterceptLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_loader/NoopLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/plugin_loader/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.328182 argrelay-0.1.0.dev5/src/argrelay/relay_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/AbstractClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/AbstractClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/AbstractClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1290 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/LocalClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2204 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/LocalClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/RemoteClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1546 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/RemoteClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2180 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_client/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.329182 argrelay-0.1.0.dev5/src/argrelay/relay_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4665 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/CustomFlaskApp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/GuiBannerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1419 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/HelpHintCache.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5700 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/LocalServer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/QueryCacheConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5872 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/QueryEngine.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      562 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/QueryResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.330182 argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_static/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27871 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_static/argrelay_client.js
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4505 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_static/argrelay_style.css
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_static/external_link.svg
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.330182 argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_templates/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5567 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_templates/argrelay_main.html
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5438 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/route_api.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      922 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/relay_server/route_gui.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.330182 argrelay-0.1.0.dev5/src/argrelay/runtime_context/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5451 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/EnvelopeContainer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/InitControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2875 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/InputContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10161 2023-08-06 09:30:09.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/InterpContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5871 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/ParsedContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/RequestContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2179 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/SearchControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_context/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.331182 argrelay-0.1.0.dev5/src/argrelay/runtime_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/AssignedValue.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      247 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/ClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/ConnectionConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      289 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/PluginEntry.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2162 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/ServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      604 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/StaticData.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/runtime_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.331182 argrelay-0.1.0.dev5/src/argrelay/sample_conf/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/sample_conf/argrelay.client.json
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11172 2023-08-06 11:47:07.000000 argrelay-0.1.0.dev5/src/argrelay/sample_conf/argrelay.server.yaml
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.331182 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1347 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_client/ClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1056 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_client/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.332182 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      852 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1621 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/MongoConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1196 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3999 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/ServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1570 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/StaticDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.332182 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3942 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1088 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1035 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/InitControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2047 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/SearchControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.332182 argrelay-0.1.0.dev5/src/argrelay/schema_config_plugin/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2598 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_plugin/PluginEntrySchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/schema_config_plugin/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.332182 argrelay-0.1.0.dev5/src/argrelay/schema_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3257 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_request/RequestContextSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/schema_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.333182 argrelay-0.1.0.dev5/src/argrelay/schema_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      706 2023-05-07 13:37:37.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/ArgValuesSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1742 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/AssignedValueSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3026 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/EnvelopeContainerSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      856 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/FilteredDict.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1207 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/InterpResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2126 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/InterpResultSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3250 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/InvocationInputSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev5/src/argrelay/schema_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.333182 argrelay-0.1.0.dev5/src/argrelay/server_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1543 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/server_spec/DescribeLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1268 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/server_spec/ProposeArgValuesSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1325 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/server_spec/RelayLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev5/src/argrelay/server_spec/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      772 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/server_spec/const_int.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3031 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/server_spec/server_data_schema.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.334182 argrelay-0.1.0.dev5/src/argrelay/test_helper/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    20113 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/test_helper/EnvMockBuilder.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4046 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/test_helper/InOutTestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      684 2023-08-06 08:09:50.000000 argrelay-0.1.0.dev5/src/argrelay/test_helper/OpenFileMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1892 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev5/src/argrelay/test_helper/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-08-06 11:51:18.321182 argrelay-0.1.0.dev5/src/argrelay.egg-info/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-08-06 11:51:18.000000 argrelay-0.1.0.dev5/src/argrelay.egg-info/PKG-INFO
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27812 2023-08-06 11:51:18.000000 argrelay-0.1.0.dev5/src/argrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2023-08-06 11:51:18.000000 argrelay-0.1.0.dev5/src/argrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      148 2023-08-06 11:51:18.000000 argrelay-0.1.0.dev5/src/argrelay.egg-info/requires.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2023-08-06 11:51:18.000000 argrelay-0.1.0.dev5/src/argrelay.egg-info/top_level.txt
```

### Comparing `argrelay-0.1.0.dev4/LICENSE` & `argrelay-0.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/PKG-INFO` & `argrelay-0.1.0.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Tab-completion & data search server - total recall
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Environment :: Console
```

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/argrelay_env_var_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/argrelay_env_var_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/bootstrap_procedure.1.project_creation.md` & `argrelay-0.1.0.dev5/docs/dev_notes/bootstrap_procedure.1.project_creation.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md` & `argrelay-0.1.0.dev5/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md` & `argrelay-0.1.0.dev5/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/code_style.md` & `argrelay-0.1.0.dev5/docs/dev_notes/code_style.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/completion_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/completion_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/completion_perf_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/completion_perf_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/how_search_works.md` & `argrelay-0.1.0.dev5/docs/dev_notes/how_search_works.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/mongo_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/mongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/query_perf_10_x_more_data_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/query_perf_10_x_more_data_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/query_perf_cache_vs_no_cache.md` & `argrelay-0.1.0.dev5/docs/dev_notes/query_perf_cache_vs_no_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/query_perf_mongomock_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/query_perf_mongomock_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/query_perf_pymongo_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/query_perf_pymongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/release_procedure.md` & `argrelay-0.1.0.dev5/docs/dev_notes/release_procedure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/screencast_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/screencast_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/scripts_summary.md` & `argrelay-0.1.0.dev5/docs/dev_notes/scripts_summary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/term_dictionary.md` & `argrelay-0.1.0.dev5/docs/dev_notes/term_dictionary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/testing_guidelines.md` & `argrelay-0.1.0.dev5/docs/dev_notes/testing_guidelines.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/top_todos.md` & `argrelay-0.1.0.dev5/docs/dev_notes/top_todos.md`

 * *Files 1% similar despite different names*

```diff
@@ -162,18 +162,19 @@
 
 *   Enable debug in all bootstrap scripts.
 
 *   There is constant need to distinguish:
     *   project_dir - the path to special dir (where venv is configured via relative path, artifacts generated, config files, etc.)
     *   package_dir - the path to useful artifacts (where known after venv is sourced)
 
-*   Split `argrelay.server.yaml` into: `argrelay.common.yaml` and `argrelay.server.yaml`.
-    Or at least make it less confusing (because client-side still uses `argrelay.server.yaml`).
-    Maybe instead of "common", it should be called `argrelay.plugins.yaml` which is exactly the part seen and
-    reused by both server and client?
+*   Split `argrelay.server.yaml` into: `argrelay.plugins.yaml` and `argrelay.server.yaml`.
+    Or at least make it less confusing
+    (because client-side still uses `argrelay.server.yaml` to use plugin configuration on server response).
+    It should be called `argrelay.plugins.yaml` which is exactly the part seen and
+    reused by both server and client, right?
 
 *   Make it possible to override location of `@/conf/` via env var
     (to allow experimental development co-exists).
     See `FS_16_07_78_84.conf_dir_priority.md` - is it done?
 
 *   Make yaml config composable (to reduce chances of merging):
     allow loading external config which should plug itself into existing config.
```

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/ui_tests_notes.md` & `argrelay-0.1.0.dev5/docs/dev_notes/ui_tests_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/dev_notes/version_format.md` & `argrelay-0.1.0.dev5/docs/dev_notes/version_format.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_06_99_43_60.list_arg_value.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_06_99_43_60.list_arg_value.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_29_54_67_86.dir_structure.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_29_54_67_86.dir_structure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_31_70_49_15.search_control.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_31_70_49_15.search_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_55_57_45_04.demo_logic.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_55_57_45_04.demo_logic.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_58_61_77_69.dev_shell.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_58_61_77_69.dev_shell.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_62_25_92_06.assigned_context.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_62_25_92_06.assigned_context.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_67_16_61_97.git_plugin.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_67_16_61_97.git_plugin.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_71_87_33_52.help_hint.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_71_87_33_52.help_hint.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_72_40_53_00.fill_control.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_72_40_53_00.fill_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md` & `argrelay-0.1.0.dev5/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md` & `argrelay-0.1.0.dev5/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md` & `argrelay-0.1.0.dev5/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/readme.md` & `argrelay-0.1.0.dev5/docs/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md` & `argrelay-0.1.0.dev5/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/test_data/TD_63_37_05_36.demo_services_data.md` & `argrelay-0.1.0.dev5/docs/test_data/TD_63_37_05_36.demo_services_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/docs/test_data/TD_70_69_38_46.no_data.md` & `argrelay-0.1.0.dev5/docs/test_data/TD_70_69_38_46.no_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/readme.md` & `argrelay-0.1.0.dev5/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/setup.py` & `argrelay-0.1.0.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # All paths start with `top_dir_path`:
     return file_paths
 
 
 setuptools.setup(
     name = "argrelay",
     # See `docs/dev_notes/version_format.md`:
-    version = "0.1.0.dev4",
+    version = "0.1.0.dev5",
     author = "uvsmtid",
     author_email = "uvsmtid@gmail.com",
     description = "Tab-completion & data search server - total recall",
     long_description = """
 See: https://github.com/argrelay/argrelay
     """,
     long_description_content_type = "text/markdown",
```

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_local/AbstractLocalClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_local/AbstractLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py` & `argrelay-0.1.0.dev5/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/DemoInterpFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/DemoInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoArgType.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoArgType.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,19 +7,22 @@
     """
     Envelope arg types (properties) used by `GitRepoLoader`.
     """
 
     # Short name for a repo (to avoid specifying its `GitRepoRootRelPath`):
     GitRepoAlias = auto()
 
-    # Git root path relative to `GitRepoRootAbsOath`:
+    # Git root path relative to `GitRepoRootAbsPath`:
     GitRepoRootRelPath = auto()
 
     # Absolute path common to multiple Git repos - what `GitRepoRootRelPath` are relative to:
-    GitRepoRootAbsOath = auto()
+    GitRepoRootAbsPath = auto()
+
+    # Git root dir base name:
+    GitRepoRootBaseName = auto()
 
     # Categorize repo content: conf, code, ...
     GitRepoContentType = auto()
 
     # TODO: FS_06_99_43_60: this is experimental:
     # Path component leading to Git repo root path (e.g. ["qwer", "asdf", "zxcv"] of "zxcv/qwer/asdf"):
     GitRepoPathComp = auto()
```

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoDelegator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import subprocess
+from __future__ import annotations
 
+import subprocess
 from argrelay.custom_integ.value_constants import goto_repo_func_, desc_commit_func_
 from argrelay.misc_helper import eprint
 from argrelay.plugin_delegator.AbstractDelegator import AbstractDelegator, get_data_envelopes
 from argrelay.plugin_delegator.InvocationInput import InvocationInput
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.runtime_context.InterpContext import InterpContext, function_envelope_ipos_
 from argrelay.schema_config_interp.DataEnvelopeSchema import envelope_payload_, envelope_id_, instance_data_
@@ -48,22 +49,25 @@
         )
         return invocation_input
 
     @staticmethod
     def invoke_action(invocation_input: InvocationInput):
         if invocation_input.data_envelopes[function_envelope_ipos_][envelope_id_] == goto_repo_func_:
             repo_envelope = invocation_input.data_envelopes[repo_envelope_ipos_]
-            abs_repo_path = repo_envelope[envelope_payload_]["abs_repo_path"]
-            eprint(f"INFO: starting subshell in: {abs_repo_path}")
+            repo_root_abs_path = repo_envelope[envelope_payload_][repo_root_abs_path_]
+            eprint(f"INFO: starting subshell in: {repo_root_abs_path}")
             # List Git repo dir:
             subproc = subprocess.run(
                 [
                     "bash",
                     "-l",
                 ],
-                cwd = abs_repo_path
+                cwd = repo_root_abs_path
             )
             ret_code = subproc.returncode
             if ret_code != 0:
                 raise RuntimeError
         if invocation_input.data_envelopes[function_envelope_ipos_][envelope_id_] == desc_commit_func_:
             raise RuntimeError("not implemented")
+
+
+repo_root_abs_path_: str = "repo_root_abs_path"
```

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoLoader.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import os
 import subprocess
 
 from git import Repo
 
 from argrelay.custom_integ.GitRepoArgType import GitRepoArgType
-from argrelay.custom_integ.GitRepoDelegator import GitRepoDelegator
+from argrelay.custom_integ.GitRepoDelegator import GitRepoDelegator, repo_root_abs_path_
 from argrelay.custom_integ.GitRepoEntryConfigSchema import (
     repo_rel_path_,
     envelope_properties_,
     is_repo_enabled_,
 )
 from argrelay.custom_integ.GitRepoEnvelopeClass import GitRepoEnvelopeClass
 from argrelay.custom_integ.GitRepoLoaderConfigSchema import (
@@ -34,16 +34,14 @@
 )
 from argrelay.schema_config_interp.FunctionEnvelopeInstanceDataSchema import (
     delegator_plugin_instance_id_,
     search_control_list_,
 )
 from argrelay.schema_config_interp.SearchControlSchema import keys_to_types_list_, envelope_class_
 
-repo_root_abs_path_: str = "repo_root_abs_path"
-
 
 class GitRepoLoader(AbstractLoader):
     """
     Implements FS_67_16_61_97 git_plugin.
     """
 
     def __init__(
@@ -88,20 +86,21 @@
 
             repo_entries = self.config_dict[repo_entries_][repo_base_abs_path]
             repo_base_abs_path = os.path.expanduser(repo_base_abs_path)
 
             # Process repo entries collecting `repo_root_rel_path` and `repo_root_abs_path`:
             for repo_entry in repo_entries:
 
-                if not repo_entry[is_repo_enabled_]:
-                    continue
-
                 repo_root_rel_path = repo_entry[repo_rel_path_]
                 repo_root_abs_path = os.path.join(repo_base_abs_path, repo_root_rel_path)
 
+                if not repo_entry[is_repo_enabled_]:
+                    eprint(f"INFO: disabled repo: {repo_root_abs_path}")
+                    continue
+
                 # Deduplicate Git root paths:
                 if repo_root_abs_path not in repo_root_abs_paths:
                     # Register `repo_root_abs_path`:
                     repo_root_abs_paths.append(repo_root_abs_path)
                 else:
                     eprint(f"ERROR: duplicate Git repo: {repo_root_abs_path}")
                     raise RuntimeError
@@ -122,14 +121,16 @@
                 if ret_code == 0:
                     pass
                 else:
                     eprint(f"ERROR: not a Git repo: {repo_root_abs_path}")
                     # Walked into dir outside of Git repo:
                     continue
 
+                repo_root_base_name = os.path.basename(repo_root_abs_path)
+
                 # Produce path component list, for example, if:
                 # repo_root_rel_path = "rel/path/to/git/repo.git/"
                 # then:
                 # path_comp_list = [ "rel", "path", "to", "git", "repo" ]
                 path_comp_list = []
                 for rel_git_path_comp in repo_root_rel_path.split(os.sep)[:-1]:
                     if rel_git_path_comp not in path_comp_list:
@@ -144,15 +145,16 @@
                     envelope_id_: repo_root_abs_path,
                     envelope_payload_: {
                         repo_root_abs_path_: repo_root_abs_path,
                     },
                     ReservedArgType.EnvelopeClass.name: GitRepoEnvelopeClass.ClassGitRepo.name,
                     GlobalArgType.ObjectSelector.name: "repo",
                     GitRepoArgType.GitRepoRootRelPath.name: repo_root_rel_path,
-                    GitRepoArgType.GitRepoRootAbsOath.name: repo_root_abs_path,
+                    GitRepoArgType.GitRepoRootAbsPath.name: repo_root_abs_path,
+                    GitRepoArgType.GitRepoRootBaseName.name: repo_root_base_name,
                     GitRepoArgType.GitRepoPathComp.name: path_comp_list,
                 })
                 print(repo_envelope)
                 data_envelopes.append(repo_envelope)
 
                 if not self.config_dict[load_repo_commits_]:
                     continue
@@ -167,15 +169,16 @@
                     commit_envelope.update({
                         envelope_id_: f"{repo_root_abs_path}:{git_commit.hexsha}",
                         envelope_payload_: {
                         },
                         ReservedArgType.EnvelopeClass.name: GitRepoEnvelopeClass.ClassGitCommit.name,
                         GlobalArgType.ObjectSelector.name: "commit",
                         GitRepoArgType.GitRepoRootRelPath.name: repo_root_rel_path,
-                        GitRepoArgType.GitRepoRootAbsOath.name: repo_root_abs_path,
+                        GitRepoArgType.GitRepoRootAbsPath.name: repo_root_abs_path,
+                        GitRepoArgType.GitRepoRootBaseName.name: repo_root_base_name,
                         GitRepoArgType.GitRepoPathComp.name: path_comp_list,
                         GitRepoArgType.GitRepoCommitId.name: git_commit.hexsha,
                         GitRepoArgType.GitRepoCommitAuthorName.name: git_commit.author.name,
                         GitRepoArgType.GitRepoCommitAuthorEmail.name: git_commit.author.email,
                         GitRepoArgType.GitRepoCommitMessage.name: git_commit.message,
                     })
                     data_envelopes.append(commit_envelope)
@@ -191,25 +194,27 @@
         # functions
 
         repo_search_control = {
             envelope_class_: GitRepoEnvelopeClass.ClassGitRepo.name,
             keys_to_types_list_: [
                 {"alias": GitRepoArgType.GitRepoAlias.name},
                 {"content": GitRepoArgType.GitRepoContentType.name},
+                {"name": GitRepoArgType.GitRepoRootBaseName.name},
                 {"path": GitRepoArgType.GitRepoRootRelPath.name},
-                {"base": GitRepoArgType.GitRepoRootAbsOath.name},
+                {"base": GitRepoArgType.GitRepoRootAbsPath.name},
                 {"part": GitRepoArgType.GitRepoPathComp.name},
             ],
         }
 
         commit_search_control = {
             envelope_class_: GitRepoEnvelopeClass.ClassGitCommit.name,
             keys_to_types_list_: [
+                {"name": GitRepoArgType.GitRepoRootBaseName.name},
                 {"path": GitRepoArgType.GitRepoRootRelPath.name},
-                {"base": GitRepoArgType.GitRepoRootAbsOath.name},
+                {"base": GitRepoArgType.GitRepoRootAbsPath.name},
                 {"email": GitRepoArgType.GitRepoCommitAuthorEmail.name},
                 {"hex": GitRepoArgType.GitRepoCommitId.name},
             ],
         }
 
         given_function_envelope = {
             envelope_id_: goto_repo_func_,
```

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceArgType.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceLoader.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/argrelay_rc.bash` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/argrelay_rc.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/bootstrap_dev_env.bash` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/bootstrap_dev_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/dev_shell.bash` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/dev_shell.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/custom_integ_res/init_shell_env.bash` & `argrelay-0.1.0.dev5/src/argrelay/custom_integ_res/init_shell_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/enum_desc/ArgSource.py` & `argrelay-0.1.0.dev5/src/argrelay/enum_desc/ArgSource.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/enum_desc/CompType.py` & `argrelay-0.1.0.dev5/src/argrelay/enum_desc/CompType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/enum_desc/GlobalArgType.py` & `argrelay-0.1.0.dev5/src/argrelay/enum_desc/GlobalArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/enum_desc/RunMode.py` & `argrelay-0.1.0.dev5/src/argrelay/enum_desc/RunMode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/enum_desc/TermColor.py` & `argrelay-0.1.0.dev5/src/argrelay/enum_desc/TermColor.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/enum_desc/TokenType.py` & `argrelay-0.1.0.dev5/src/argrelay/enum_desc/TokenType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/handler_request/AbstractServerRequestHandler.py` & `argrelay-0.1.0.dev5/src/argrelay/handler_request/AbstractServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py` & `argrelay-0.1.0.dev5/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py` & `argrelay-0.1.0.dev5/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py` & `argrelay-0.1.0.dev5/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py` & `argrelay-0.1.0.dev5/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py` & `argrelay-0.1.0.dev5/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/misc_helper/AbstractPlugin.py` & `argrelay-0.1.0.dev5/src/argrelay/misc_helper/AbstractPlugin.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/misc_helper/ElapsedTime.py` & `argrelay-0.1.0.dev5/src/argrelay/misc_helper/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/misc_helper/TypeDesc.py` & `argrelay-0.1.0.dev5/src/argrelay/misc_helper/TypeDesc.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/misc_helper/__init__.py` & `argrelay-0.1.0.dev5/src/argrelay/misc_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoClientWrapper.py` & `argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoClientWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/mongo_data/MongoServerWrapper.py` & `argrelay-0.1.0.dev5/src/argrelay/mongo_data/MongoServerWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/AbstractDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/AbstractDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/ErrorDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/ErrorDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/HelpDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/HelpDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/InterceptDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/InterceptDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/InvocationInput.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/InvocationInput.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_delegator/NoopDelegator.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_delegator/NoopDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/AbstractInterp.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/AbstractInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FirstArgInterp.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FirstArgInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FirstArgInterpFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FirstArgInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FuncArgsInterp.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FuncArgsInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/FuncArgsInterpFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/FuncArgsInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/NoopInterp.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/NoopInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/NoopInterpFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/NoopInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/TreePathInterp.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/TreePathInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/TreePathInterpFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/TreePathInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_loader/HelpLoader.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_loader/HelpLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/plugin_loader/InterceptLoader.py` & `argrelay-0.1.0.dev5/src/argrelay/plugin_loader/InterceptLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/AbstractClient.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/AbstractClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/AbstractClientCommandFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/AbstractClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/LocalClient.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/LocalClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/LocalClientCommandFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/LocalClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/RemoteClient.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/RemoteClientCommandFactory.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/RemoteClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_client/__main__.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_client/__main__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/CustomFlaskApp.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/CustomFlaskApp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/HelpHintCache.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/HelpHintCache.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/LocalServer.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/LocalServer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/QueryEngine.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/QueryEngine.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/QueryResult.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/QueryResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_static/argrelay_client.js` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_static/argrelay_client.js`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_static/argrelay_style.css` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_static/argrelay_style.css`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/gui_templates/argrelay_main.html` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/gui_templates/argrelay_main.html`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/route_api.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/route_api.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/relay_server/route_gui.py` & `argrelay-0.1.0.dev5/src/argrelay/relay_server/route_gui.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_context/EnvelopeContainer.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_context/EnvelopeContainer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_context/InputContext.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_context/InputContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_context/InterpContext.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_context/InterpContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_context/ParsedContext.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_context/ParsedContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_context/SearchControl.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_context/SearchControl.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_data/ServerConfig.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_data/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/runtime_data/StaticData.py` & `argrelay-0.1.0.dev5/src/argrelay/runtime_data/StaticData.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/sample_conf/argrelay.server.yaml` & `argrelay-0.1.0.dev5/src/argrelay/sample_conf/argrelay.server.yaml`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_client/ClientConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_client/ClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/MongoConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/MongoConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/ServerConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/ServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_core_server/StaticDataSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_core_server/StaticDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/DataEnvelopeSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/DataEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/InitControlSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/InitControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_interp/SearchControlSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_interp/SearchControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_config_plugin/PluginEntrySchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_config_plugin/PluginEntrySchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_request/RequestContextSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_request/RequestContextSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/ArgValuesSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/ArgValuesSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/AssignedValueSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/AssignedValueSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/EnvelopeContainerSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/EnvelopeContainerSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/FilteredDict.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/FilteredDict.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/InterpResult.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/InterpResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/InterpResultSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/InterpResultSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/schema_response/InvocationInputSchema.py` & `argrelay-0.1.0.dev5/src/argrelay/schema_response/InvocationInputSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/server_spec/DescribeLineArgsSpec.py` & `argrelay-0.1.0.dev5/src/argrelay/server_spec/DescribeLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/server_spec/ProposeArgValuesSpec.py` & `argrelay-0.1.0.dev5/src/argrelay/server_spec/ProposeArgValuesSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/server_spec/RelayLineArgsSpec.py` & `argrelay-0.1.0.dev5/src/argrelay/server_spec/RelayLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/server_spec/const_int.py` & `argrelay-0.1.0.dev5/src/argrelay/server_spec/const_int.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/server_spec/server_data_schema.py` & `argrelay-0.1.0.dev5/src/argrelay/server_spec/server_data_schema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/test_helper/EnvMockBuilder.py` & `argrelay-0.1.0.dev5/src/argrelay/test_helper/EnvMockBuilder.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/test_helper/InOutTestCase.py` & `argrelay-0.1.0.dev5/src/argrelay/test_helper/InOutTestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/test_helper/OpenFileMock.py` & `argrelay-0.1.0.dev5/src/argrelay/test_helper/OpenFileMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay/test_helper/__init__.py` & `argrelay-0.1.0.dev5/src/argrelay/test_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.1.0.dev4/src/argrelay.egg-info/PKG-INFO` & `argrelay-0.1.0.dev5/src/argrelay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Tab-completion & data search server - total recall
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Environment :: Console
```

### Comparing `argrelay-0.1.0.dev4/src/argrelay.egg-info/SOURCES.txt` & `argrelay-0.1.0.dev5/src/argrelay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

