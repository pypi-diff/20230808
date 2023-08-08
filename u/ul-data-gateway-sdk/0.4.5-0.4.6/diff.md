# Comparing `tmp/ul-data-gateway-sdk-0.4.5.tar.gz` & `tmp/ul-data-gateway-sdk-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-gateway-sdk-0.4.5.tar", last modified: Thu Jun 22 13:26:07 2023, max compression
+gzip compressed data, was "ul-data-gateway-sdk-0.4.6.tar", last modified: Tue Aug  8 10:55:15 2023, max compression
```

## Comparing `ul-data-gateway-sdk-0.4.5.tar` & `ul-data-gateway-sdk-0.4.6.tar`

### file list

```diff
@@ -1,177 +1,179 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.985847 ul-data-gateway-sdk-0.4.5/
--rw-r--r--   0 root         (0) root         (0)    13358 2023-06-22 13:26:07.985847 ul-data-gateway-sdk-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12799 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.945845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.945845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/__tests__/test_encryption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.945845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.945845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.945845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3510 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py
--rw-rw-rw-   0 root         (0) root         (0)     6855 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py
--rw-rw-rw-   0 root         (0) root         (0)   132363 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin
--rw-rw-rw-   0 root         (0) root         (0)    14821 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/crypto_aes.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py
--rw-rw-rw-   0 root         (0) root         (0)     4405 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/crypto_xtea.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.949845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/extensions/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/extensions/type_alias.py
--rw-rw-rw-   0 root         (0) root         (0)    18714 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/device_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/device_data_encryption.py
--rw-rw-rw-   0 root         (0) root         (0)     4983 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/device_data_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.949845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/messages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/messages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/messages/input_bs_http_nero_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/nero_bs_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.949845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.949845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.949845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49906 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     2574 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     2602 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/smp_device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     5911 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/water5_device_packet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.953845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.953845 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11930 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py
--rw-rw-rw-   0 root         (0) root         (0)    14061 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)    10020 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     4736 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/nero_bs_packet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.961846 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.969846 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20286 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)    20421 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py
--rw-rw-rw-   0 root         (0) root         (0)    41491 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py
--rw-rw-rw-   0 root         (0) root         (0)    10024 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6432 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py
--rw-rw-rw-   0 root         (0) root         (0)     3748 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py
--rw-rw-rw-   0 root         (0) root         (0)     6627 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py
--rw-rw-rw-   0 root         (0) root         (0)    24530 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)    24665 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py
--rw-rw-rw-   0 root         (0) root         (0)     8394 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)   381664 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    21659 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)    10076 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)   127594 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py
--rw-rw-rw-   0 root         (0) root         (0)     9461 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     3003 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py
--rw-rw-rw-   0 root         (0) root         (0)   166938 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)   394524 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     8151 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)     8010 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py
--rw-rw-rw-   0 root         (0) root         (0)    13400 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     6164 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py
--rw-rw-rw-   0 root         (0) root         (0)    33661 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py
--rw-rw-rw-   0 root         (0) root         (0)    12807 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    12806 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    12787 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    19267 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py
--rw-rw-rw-   0 root         (0) root         (0)    17974 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py
--rw-rw-rw-   0 root         (0) root         (0)    30002 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py
--rw-rw-rw-   0 root         (0) root         (0)    10857 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)    10814 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py
--rw-rw-rw-   0 root         (0) root         (0)     7648 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    15770 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     8485 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     4409 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     4815 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     4815 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)    10998 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     5553 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py
--rw-rw-rw-   0 root         (0) root         (0)     9258 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py
--rw-rw-rw-   0 root         (0) root         (0)    13713 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    16361 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.973846 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.973846 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py
--rw-rw-rw-   0 root         (0) root         (0)     5542 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.977846 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.981846 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_magnet.py
--rw-rw-rw-   0 root         (0) root         (0)     3930 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py
--rw-rw-rw-   0 root         (0) root         (0)     8688 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     8271 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     8892 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2491 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     2483 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     2547 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     4063 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     4697 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     3493 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3564 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     3555 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.985847 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.985847 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1387 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/__tests__/timestamp_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/buf_ref.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/days_ago_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/packet.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/timestamp_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/true_round.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 13:26:07.985847 ul-data-gateway-sdk-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1251 2023-06-22 13:25:55.000000 ul-data-gateway-sdk-0.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:26:07.985847 ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13358 2023-06-22 13:26:06.000000 ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10247 2023-06-22 13:26:06.000000 ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 13:26:06.000000 ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-22 13:26:06.000000 ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-22 13:26:06.000000 ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.792660 ul-data-gateway-sdk-0.4.6/
+-rw-r--r--   0 root         (0) root         (0)    13358 2023-08-08 10:55:15.792660 ul-data-gateway-sdk-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12799 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.760659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.760659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/__tests__/test_encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.760659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.760659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.760659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6855 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py
+-rw-rw-rw-   0 root         (0) root         (0)   132363 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin
+-rw-rw-rw-   0 root         (0) root         (0)    14821 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/crypto_aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py
+-rw-rw-rw-   0 root         (0) root         (0)     4405 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/crypto_xtea.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.760659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/extensions/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/extensions/type_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)    18714 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/device_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/device_data_encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)     5162 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/device_data_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.764659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/messages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/messages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/messages/input_bs_http_nero_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/nero_bs_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.764659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.764659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.764659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49906 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/smp_device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     6194 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/water5_device_packet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.764659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.764659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11930 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)    14061 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)    12271 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     4736 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/nero_bs_packet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.768659 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.784660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20286 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)    20421 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)    41491 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    10024 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6432 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3748 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py
+-rw-rw-rw-   0 root         (0) root         (0)     6627 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py
+-rw-rw-rw-   0 root         (0) root         (0)    24530 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)    24665 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)     8394 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)   381664 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)  5475148 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_group_meter_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    21659 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10076 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)   127594 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     9461 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     3003 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)   166938 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)   394524 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8151 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)     8010 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)    13400 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     6164 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    33661 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    12806 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    12787 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    19267 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py
+-rw-rw-rw-   0 root         (0) root         (0)    17974 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py
+-rw-rw-rw-   0 root         (0) root         (0)    30002 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10857 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)    10814 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)     7648 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    15770 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    87832 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_group_meter_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     9190 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     4409 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4815 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4815 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10998 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     9258 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    13713 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    16361 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.784660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.784660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py
+-rw-rw-rw-   0 root         (0) root         (0)     5542 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.784660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.788660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_magnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3930 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     8688 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     8271 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     8892 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2491 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     2483 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2547 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4333 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     4063 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3493 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3564 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3555 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.792660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.792660 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/__tests__/timestamp_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/buf_ref.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/days_ago_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/timestamp_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/true_round.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 10:55:15.792660 ul-data-gateway-sdk-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-08-08 10:55:09.000000 ul-data-gateway-sdk-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:55:15.792660 ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13358 2023-08-08 10:55:15.000000 ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10403 2023-08-08 10:55:15.000000 ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 10:55:15.000000 ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-08-08 10:55:15.000000 ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-08 10:55:15.000000 ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-gateway-sdk-0.4.5/PKG-INFO` & `ul-data-gateway-sdk-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-gateway-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Data gateway sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-gateway-sdk-0.4.5/README.md` & `ul-data-gateway-sdk-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/__tests__/test_encryption.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/__tests__/test_encryption.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/crypto_aes.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/crypto_aes.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/crypto_xtea.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/crypto_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/crypto_algorithms/extensions/errors.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/crypto_algorithms/extensions/errors.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/device_data.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/device_data.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/device_data_encryption.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/device_data_encryption.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/device_data_protocol.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/device_data_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from data_gateway_sdk.errors import DataGatewayDeviceProtocolParsingError
 from data_gateway_sdk.protocols.device_packet.device_packet import DevicePacket
 from data_gateway_sdk.protocols.device_packet.ncp_smp_device_packet import NcpSmpV0DevicePacket
 from data_gateway_sdk.protocols.device_packet.smp_device_packet import SmpV0DevicePacket
 from data_gateway_sdk.protocols.device_packet.smpm_device_packet import SmpMGasMeterV0DevicePacket, \
     SmpMEnergyMeterV0DevicePacket, SmpMJupiter08BV0DevicePacket, SmpMJupiter12BV0DevicePacket, \
     SmpMWaterMeter08BV0DevicePacket, SmpMWaterMeter12BV0DevicePacket, SmpMWaterMeter04BV0DevicePacket, SmpMJupiter16BV0DevicePacket, SmpMWaterMeter16BV0DevicePacket, \
-    SmpMInternalInfoDataV0DevicePacket, SmpMHeatProxyMeter16BV0DevicePacket
+    SmpMInternalInfoDataV0DevicePacket, SmpMHeatProxyMeter16BV0DevicePacket, SmpMHeatGroupMeterV0DevicePacket
 from data_gateway_sdk.protocols.device_packet.water5_device_packet import Water5NeroV0DevicePacket, \
     Water5JupiterFreeScaleV0DevicePacket, Water5JupiterSTMV0DevicePacket, Water5FluoSTMV0DevicePacket, \
     Water5FluoFreeScaleV0DevicePacket, Water5FluoAV0DevicePacket, Water5GasV0DevicePacket, \
     Water5JupiterLoraV0DevicePacket, Water5FluoSV0DevicePacket
 
 
 @unique
@@ -26,14 +26,15 @@
     SMP_M_JUPITER_12B_V0 = 'SMP_M_JUPITER_12B_V0'
     SMP_M_JUPITER_16B_V0 = 'SMP_M_JUPITER_16B_V0'
     SMP_M_WATER_METER_04B_V0 = 'SMP_M_WATER_METER_04B_V0'
     SMP_M_WATER_METER_08B_V0 = 'SMP_M_WATER_METER_08B_V0'
     SMP_M_WATER_METER_12B_V0 = 'SMP_M_WATER_METER_12B_V0'
     SMP_M_WATER_METER_16B_V0 = 'SMP_M_WATER_METER_16B_V0'
     SMP_M_HEAT_PROXY_METER_16B_V0 = 'SMP_M_HEAT_PROXY_METER_16B_V0'
+    SMP_M_HEAT_GROUP_METER_V0 = 'SMP_M_HEAT_GROUP_METER_V0'
     WATER5_V_JUPITER_FREESCALE_V0 = 'WATER5_V_JUPITER_FREESCALE_V0'
     WATER5_V_JUPITER_STM_V0 = 'WATER5_V_JUPITER_STM_V0'
     WATER5_V_FLUO_STM_V0 = 'WATER5_V_FLUO_STM_V0'
     WATER5_V_FLUO_FREESCALE_V0 = 'WATER5_V_FLUO_FREESCALE_V0'
     WATER5_V_FLUO_A_V0 = 'WATER5_V_FLUO_A_V0'
     WATER5_V_FLUO_S_V0 = 'WATER5_V_FLUO_S_V0'
     WATER5_V_GAS_V0 = 'WATER5_V_GAS_V0'
@@ -63,15 +64,17 @@
     DeviceProtocolType.SMP_M_JUPITER_08B_V0: SmpMJupiter08BV0DevicePacket,
     DeviceProtocolType.SMP_M_JUPITER_12B_V0: SmpMJupiter12BV0DevicePacket,
     DeviceProtocolType.SMP_M_JUPITER_16B_V0: SmpMJupiter16BV0DevicePacket,
     DeviceProtocolType.SMP_M_WATER_METER_04B_V0: SmpMWaterMeter04BV0DevicePacket,
     DeviceProtocolType.SMP_M_WATER_METER_08B_V0: SmpMWaterMeter08BV0DevicePacket,
     DeviceProtocolType.SMP_M_WATER_METER_12B_V0: SmpMWaterMeter12BV0DevicePacket,
     DeviceProtocolType.SMP_M_WATER_METER_16B_V0: SmpMWaterMeter16BV0DevicePacket,
+
     DeviceProtocolType.SMP_M_HEAT_PROXY_METER_16B_V0: SmpMHeatProxyMeter16BV0DevicePacket,
+    DeviceProtocolType.SMP_M_HEAT_GROUP_METER_V0: SmpMHeatGroupMeterV0DevicePacket,
 
     DeviceProtocolType.WATER5_V_JUPITER_FREESCALE_V0: Water5JupiterFreeScaleV0DevicePacket,
     DeviceProtocolType.WATER5_V_JUPITER_STM_V0: Water5JupiterSTMV0DevicePacket,
     DeviceProtocolType.WATER5_V_FLUO_STM_V0: Water5FluoSTMV0DevicePacket,
     DeviceProtocolType.WATER5_V_FLUO_FREESCALE_V0: Water5FluoFreeScaleV0DevicePacket,
     DeviceProtocolType.WATER5_V_FLUO_A_V0: Water5FluoAV0DevicePacket,
     DeviceProtocolType.WATER5_V_FLUO_S_V0: Water5FluoSV0DevicePacket,
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/nero_bs_protocol.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/nero_bs_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/device_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/smp_device_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/smp_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_energy_16b_profile_8h_pqs import SmpmUlDeviceEnergy16BProfile8HPqsData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_energy_16b_tariff_consumed import \
     SmpmUlDeviceEnergy16BTariffConsumedData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_energy_16b_tariff_generated import \
     SmpmUlDeviceEnergy16BTariffGeneratedData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_gaz_flow_08b_daily import SmpmUlDeviceGazFlow08BDailyData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_gaz_flow_16b_daily import SmpmUlDeviceGazFlow16BDailyData
+from data_gateway_sdk.protocols.smpm.smpm_ul_device_heat_group_meter_daily import SmpmUlDeviceHeatGroupMeterDailyData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_heat_proxy_meter_16b_daily import SmpmUlDeviceHeatProxyMeter16BDailyData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_internal_info import SmpmUlDeviceInternalInfoData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_jupiter_08b_counter import SmpmUlDeviceJupiter08BCounterData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_jupiter_08b_counter_ch1 import SmpmUlDeviceJupiter08BCounterCh1Data
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_jupiter_08b_counter_ch2 import SmpmUlDeviceJupiter08BCounterCh2Data
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_jupiter_12b_counter import SmpmUlDeviceJupiter12BCounterData
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_jupiter_16b_counter import SmpmUlDeviceJupiter16BCounterData
@@ -109,11 +110,17 @@
 
 class SmpMHeatProxyMeter16BV0DevicePacket(DevicePacketTyped):
     _SUPPORTED_PACKETS: Tuple[Type[Packet], ...] = (
         SmpmUlDeviceHeatProxyMeter16BDailyData,
     )
 
 
+class SmpMHeatGroupMeterV0DevicePacket(DevicePacketTyped):
+    _SUPPORTED_PACKETS: Tuple[Type[Packet], ...] = (
+        SmpmUlDeviceHeatGroupMeterDailyData,
+    )
+
+
 class SmpMInternalInfoDataV0DevicePacket(DevicePacketTyped):
     _SUPPORTED_PACKETS: Tuple[Type[Packet], ...] = (
         SmpmUlDeviceInternalInfoData,
     )
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/device_packet/water5_device_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/device_packet/water5_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 import re
 from datetime import datetime
 from enum import Enum, unique
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
+from data_aggregator_sdk.constants.enums import SignalModulation, DownlinkTaskType
 from data_aggregator_sdk.integration_message import IntegrationV0MessageMeta, IntegrationV0MessageMetaBSChannelProtocol, \
     IntegrationV0MessageMetaBSHttp
 from pydantic import BaseModel, Extra, validator
 
 from data_gateway_sdk.errors import DataGatewayBSProtocolParsingError
 from data_gateway_sdk.protocols.nero_bs_packet.nero_bs_packet import NeroBsPacket
 
@@ -263,34 +264,109 @@
     debug = 'debug'
     info = 'info'
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}.{self.name}'
 
 
+@unique
+class BsDownlinkCommandNameEnum(Enum):
+    sync_downlink_tasks = "sync_downlink_tasks"
+    add_downlink_task = "add_downlink_task"
+    delete_downlink_task = "delete_downlink_task"
+    get_active_downlink_task_ids = "get_active_downlink_task_ids"
+
+    def __repr__(self) -> str:
+        return f'{type(self).__name__}.{self.name}'
+
+
+class DataAddDownlinkTaskResponseInvalidTasks(BaseModel):
+    id: UUID
+    reason: str
+
+
+class DataAddDownlinkTaskResponse(BaseModel):
+    accepted_ids: List[UUID]
+    already_exist_ids: List[UUID]
+    invalid: List[DataAddDownlinkTaskResponseInvalidTasks]
+
+
+class DataDeleteDownlinkTaskResponse(BaseModel):
+    deleted_ids: List[UUID]
+
+
+class DataGetActiveDownlinkTaskIDSResponse(BaseModel):
+    active_ids: List[UUID]
+
+
+class BsDownlinkTaskExecutionsSignalParams(BaseModel):
+    freq: int
+    power: int
+    baudrate: int
+    modulation: SignalModulation
+
+
+class BsDownlinkTaskExecutionsDataUnbpMessage(BaseModel):
+    ...
+
+
+class BsDownlinkTaskExecutionsDataTimeSync(BaseModel):
+    dt: datetime
+
+
 class BaseStationLogs(BaseModel):
     type: BaseStationLogsTypeEnum
     mdl: Optional[str]
     dt: datetime
     text: str
 
     @validator('mdl', 'text')
     def validate_mac(cls, value: str) -> str:
         return value.strip()
 
     # TODO: strip content of mdl
     # TODO: strip content of text
 
 
+class BsDownlinkCommandRequests(BaseModel):
+    command: BsDownlinkCommandNameEnum
+
+
+class BsDownlinkCommandResponse(BaseModel):
+    dt: datetime
+    id: UUID
+    status_ok: bool
+    command: BsDownlinkCommandNameEnum
+    data_add_downlink_task: Optional[DataAddDownlinkTaskResponse] = None
+    data_delete_downlink_tasks: Optional[DataDeleteDownlinkTaskResponse] = None
+    data_get_active_downlink_task_ids: Optional[DataGetActiveDownlinkTaskIDSResponse] = None
+
+
+class BsDownlinkTaskExecutions(BaseModel):
+    task_id: UUID
+    execution_start_dt: datetime
+    execution_end_dt: datetime
+    status_ok: bool
+    status_message: str
+    mac: int
+    signal_params: Optional[BsDownlinkTaskExecutionsSignalParams] = None
+    type: DownlinkTaskType
+    data_unbp_message: Optional[BsDownlinkTaskExecutionsDataUnbpMessage] = None
+    data_time_sync: Optional[BsDownlinkTaskExecutionsDataTimeSync] = None
+
+
 class HttpV0NeroBsPacket(NeroBsPacket):
     data: List[DevicePackage]
     base_station_environment_info: Optional[List[BaseStationEnvironmentInfo]] = None
     base_station_info: BaseStationInfo
     base_station_additional_info: BaseStationAdditionalInfo
     base_station_logs: Optional[List[BaseStationLogs]] = None
+    command_requests: Optional[List[BsDownlinkCommandRequests]] = None
+    commands_responses: Optional[List[BsDownlinkCommandResponse]] = None
+    downlink_task_executions: Optional[List[BsDownlinkTaskExecutions]] = None
 
     def to_integration_meta(self, *, bs_id: UUID, packet: DevicePackage, **kwargs: Any) -> IntegrationV0MessageMeta:  # type: ignore
         assert packet.sdr_info is not None
         return IntegrationV0MessageMeta(
             bs_http=IntegrationV0MessageMetaBSHttp(
                 freq=packet.sdr_info.freq,
                 freq_channel=packet.sdr_info.freq_channel,
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,104 +1,104 @@
 from data_gateway_sdk.protocols.smpm.smpm_ul_device_heat_proxy_meter_16b_daily import SmpmUlDeviceHeatProxyMeter16BDailyData
 from data_gateway_sdk.utils.buf_ref import BufRef
 
 
 def test_smpm_ul_device_heat_proxy_meter_16b_daily() -> None:
-    case_serialized = bytes.fromhex("8464c81900300000286dba1400000000")
+    case_serialized = bytes.fromhex("84640000e40c0000030080524d970200")
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=3.3, uptime_min=3, meter_battery_volts=3.3, capacitor_volts=3.33, radio_proxy_battery_volts=3.31, error_meter_sync=False, error_reset=False) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(value=3.3, uptime_min=3, meter_battery_volts=3.3, capacitor_volts=3.33, radio_proxy_battery_volts=3.31, error_meter_sync=False, error_reset=False))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("84640000000000000000f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000000000fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07006000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00000c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fc07f07f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07f00fe0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=0.0, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=0.0, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f80f6000000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f80f6000000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f80f6000000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f80f6000000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f8ff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f8ff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f8ff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("846400000000000000f8ff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("846400000000000000000000ffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=0.0, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=0.0, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcff0f6000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcff0f6000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcff0f6000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcff0f6000000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fff010c00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=0.0, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=0.0, uptime_min=8388608, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcffff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=0, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcffff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=0, value=268435.456))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcffff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=0.0))  # noqa: E501
-    case_serialized = bytes.fromhex("8464000000000000fcffff7f00000000")  # overflow
+    case_serialized = bytes.fromhex("84640000000000000000c07fffff0f00")  # overflow
     assert SmpmUlDeviceHeatProxyMeter16BDailyData(value=0.0, uptime_min=0, meter_battery_volts=5.11, capacitor_volts=5.11, radio_proxy_battery_volts=5.11, error_meter_sync=True, error_reset=True) == SmpmUlDeviceHeatProxyMeter16BDailyData.parse(BufRef(case_serialized))  # noqa: E501
     assert case_serialized == SmpmUlDeviceHeatProxyMeter16BDailyData.serialize(SmpmUlDeviceHeatProxyMeter16BDailyData(capacitor_volts=5.11, error_meter_sync=True, error_reset=True, meter_battery_volts=5.11, radio_proxy_battery_volts=5.11, uptime_min=8388608, value=268435.456))  # noqa: E501
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 # profile.5.point          u13                                          13           5                                  0000000000101
 # profile.6.point          u13                                          13           6                     0000000000110
 # profile.7.point          u13                                          13           7        0000000000111
 # point_factor             uf6p1                                         6          50  110010
 
 @unique
 class SmpmUlDeviceEnergy16bProfile8h1EnergyType(IntEnum):
-    ENERGY_GENERATED_ACTIVE = 0  # ENERGY_A_P 0
-    ENERGY_GENERATED_REACTIVE = 1  # ENERGY_R_P 1
-    ENERGY_CONSUMED_ACTIVE = 2  # ENERGY_A_N 2
-    ENERGY_CONSUMED_REACTIVE = 3  # ENERGY_R_N 3
+    ENERGY_GENERATED_ACTIVE = 0  # ENERGY_A_N 0
+    ENERGY_GENERATED_REACTIVE = 1  # ENERGY_R_N 1
+    ENERGY_CONSUMED_ACTIVE = 2  # ENERGY_A_P 2
+    ENERGY_CONSUMED_REACTIVE = 3  # ENERGY_R_P 3
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}.{self.name}'
 
 
 PROFILE_MAP = {
-    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_GENERATED_ACTIVE: ProfileKind.ENERGY_A_P,
-    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_GENERATED_REACTIVE: ProfileKind.ENERGY_R_P,
-    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_CONSUMED_ACTIVE: ProfileKind.ENERGY_A_N,
-    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_CONSUMED_REACTIVE: ProfileKind.ENERGY_R_N,
+    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_GENERATED_ACTIVE: ProfileKind.ENERGY_A_N,
+    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_GENERATED_REACTIVE: ProfileKind.ENERGY_R_N,
+    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_CONSUMED_ACTIVE: ProfileKind.ENERGY_A_P,
+    SmpmUlDeviceEnergy16bProfile8h1EnergyType.ENERGY_CONSUMED_REACTIVE: ProfileKind.ENERGY_R_P,
 }
 
 
 class SmpmUlDeviceEnergy16BProfile8H1EnergyData(Packet):
     type: SmpmUlDeviceEnergy16bProfile8h1EnergyType
     point_factor_multiplier: int
     days_ago: timedelta
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 # profile.5.point          u13                                          13           5                                  0000000000101
 # profile.6.point          u13                                          13           6                     0000000000110
 # profile.7.point          u13                                          13           7        0000000000111
 # point_factor             uf6p1                                         6          50  110010
 
 @unique
 class SmpmUlDeviceEnergy16bProfile8h2EnergyType(IntEnum):
-    ENERGY_GENERATED_ACTIVE = 0  # ENERGY_A_P 0
-    ENERGY_GENERATED_REACTIVE = 1  # ENERGY_R_P 1
-    ENERGY_CONSUMED_ACTIVE = 2  # ENERGY_A_N 2
-    ENERGY_CONSUMED_REACTIVE = 3  # ENERGY_R_N 3
+    ENERGY_GENERATED_ACTIVE = 0  # ENERGY_A_N 0
+    ENERGY_GENERATED_REACTIVE = 1  # ENERGY_R_N 1
+    ENERGY_CONSUMED_ACTIVE = 2  # ENERGY_A_P 2
+    ENERGY_CONSUMED_REACTIVE = 3  # ENERGY_R_P 3
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}.{self.name}'
 
 
 PROFILE_MAP = {
-    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_GENERATED_ACTIVE: ProfileKind.ENERGY_A_P,
-    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_GENERATED_REACTIVE: ProfileKind.ENERGY_R_P,
-    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_CONSUMED_ACTIVE: ProfileKind.ENERGY_A_N,
-    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_CONSUMED_REACTIVE: ProfileKind.ENERGY_R_N,
+    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_GENERATED_ACTIVE: ProfileKind.ENERGY_A_N,
+    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_GENERATED_REACTIVE: ProfileKind.ENERGY_R_N,
+    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_CONSUMED_ACTIVE: ProfileKind.ENERGY_A_P,
+    SmpmUlDeviceEnergy16bProfile8h2EnergyType.ENERGY_CONSUMED_REACTIVE: ProfileKind.ENERGY_R_P,
 }
 
 
 class SmpmUlDeviceEnergy16BProfile8H2EnergyData(Packet):
     type: SmpmUlDeviceEnergy16bProfile8h2EnergyType
     point_factor_multiplier: int
     days_ago: timedelta
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 # profile.5.point          u13                                          13           5                                  0000000000101
 # profile.6.point          u13                                          13           6                     0000000000110
 # profile.7.point          u13                                          13           7        0000000000111
 # point_factor             uf6p1                                         6          50  110010
 
 @unique
 class SmpmUlDeviceEnergy16bProfile8h3EnergyType(IntEnum):
-    ENERGY_GENERATED_ACTIVE = 0  # ENERGY_A_P 0
-    ENERGY_GENERATED_REACTIVE = 1  # ENERGY_R_P 1
-    ENERGY_CONSUMED_ACTIVE = 2  # ENERGY_A_N 2
-    ENERGY_CONSUMED_REACTIVE = 3  # ENERGY_R_N 3
+    ENERGY_GENERATED_ACTIVE = 0  # ENERGY_A_N 0
+    ENERGY_GENERATED_REACTIVE = 1  # ENERGY_R_N 1
+    ENERGY_CONSUMED_ACTIVE = 2  # ENERGY_A_P 2
+    ENERGY_CONSUMED_REACTIVE = 3  # ENERGY_R_P 3
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}.{self.name}'
 
 
 PROFILE_MAP = {
-    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_GENERATED_ACTIVE: ProfileKind.ENERGY_A_P,
-    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_GENERATED_REACTIVE: ProfileKind.ENERGY_R_P,
-    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_CONSUMED_ACTIVE: ProfileKind.ENERGY_A_N,
-    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_CONSUMED_REACTIVE: ProfileKind.ENERGY_R_N,
+    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_GENERATED_ACTIVE: ProfileKind.ENERGY_A_N,
+    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_GENERATED_REACTIVE: ProfileKind.ENERGY_R_N,
+    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_CONSUMED_ACTIVE: ProfileKind.ENERGY_A_P,
+    SmpmUlDeviceEnergy16bProfile8h3EnergyType.ENERGY_CONSUMED_REACTIVE: ProfileKind.ENERGY_R_P,
 }
 
 
 class SmpmUlDeviceEnergy16BProfile8H3EnergyData(Packet):
     type: SmpmUlDeviceEnergy16bProfile8h3EnergyType
     point_factor_multiplier: int
     days_ago: timedelta
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from datetime import datetime, tzinfo
 from typing import Any, Dict, List
 
 from data_aggregator_sdk.constants.enums import IntegrationV0MessageEvent
 from data_aggregator_sdk.integration_message import IntegrationV0MessageData, IntegrationV0MessageCurrentBatteryLevel, IntegrationV0MessageConsumption, CounterType, ResourceType, \
-    BatteryId
+    BatteryId, IntegrationV0MessageUptime
 
 from data_gateway_sdk.utils.buf_ref import BufRef
 from data_gateway_sdk.utils.packet import Packet
 
 
 # PACKET (128 bits)   smpm_ul_device_heat_proxy_meter_16b_daily
 #
-# RESULT int:        6415075874691670917692023940
-# RESULT bin:  MSB   00000000 00000000 00000000 00000000 00010100 10111010 01101101 00101000 00000000 00000000 00110000 00000000 00011001 11001000 01100100 10000100   LSB
-# RESULT hex:  LE    84 64 c8 19 00 30 00 00 28 6d ba 14 00 00 00 00
+# RESULT int:        13453363668248021446286294801998980
+# RESULT bin:  MSB   00000000 00000010 10010111 01001101 01010010 10000000 00000000 00000011 00000000 00000000 00001100 11100100 00000000 00000000 01100100 10000100   LSB
+# RESULT hex:  LE    84 64 00 00 e4 0c 00 00 03 00 80 52 4d 97 02 00
 #
-# name                       type    size  value(int)                                                                                                                        data(bits) # noqa: E501
-# -------------------------  ------  ----  ----------  -------------------------------------------------------------------------------------------------------------------------------- # noqa: E501
-# packet_type_id.0.VAL       u7         7           4                                                                                                                           0000100 # noqa: E501
+# name                       type    size  value(int)                                                                                                                        data(bits)     # noqa: E501
+# -------------------------  ------  ----  ----------  --------------------------------------------------------------------------------------------------------------------------------     # noqa: E501
+# packet_type_id.0.VAL       u7         7           4                                                                                                                           0000100     # noqa: E501
 # packet_type_id.0.DFF       bool       1           1                                                                                                                          1
 # packet_type_id.1.VAL       u2         2           0                                                                                                                        00
 # packet_type_id.1.DFF       bool       1           1                                                                                                                       1
 # packet_type_id.2.VAL       u2         2           0                                                                                                                     00
 # packet_type_id.2.DFF       bool       1           1                                                                                                                    1
 # packet_type_id.3.VAL       u2         2           1                                                                                                                  01
 # packet_type_id.3.DFF       bool       1           0                                                                                                                 0
-# value                      uf27p3    27        3300                                                                                      000000000000000110011100100
-# uptime_min                 u22       22           3                                                                0000000000000000000011
-# meter_battery_volts        uf9p2      9         330                                                       101001010
-# capacitor_volts            uf9p2      9         333                                              101001101
-# radio_proxy_battery_volts  uf9p2      9         331                                     101001011
-# error_meter_sync           bool       1           0                                    0
-# error_reset                bool       1           0                                   0
-# RESERVED                   u33       33           0  000000000000000000000000000000000
+# UNUSED                     -         15           0                                                                                                  000000000000000
+# value                      uf27p3    27        3300                                                                       000000000000000110011100100
+# UNUSED                     -          5           0                                                                  00000
+# uptime_min                 u22       22           3                                            0000000000000000000011
+# meter_battery_volts        uf9p2      9         330                                   101001010
+# UNUSED                     -          1           0                                  0
+# capacitor_volts            uf9p2      9         333                         101001101
+# radio_proxy_battery_volts  uf9p2      9         331                101001011
+# error_meter_sync           bool       1           0               0
+# error_reset                bool       1           0              0
+# RESERVED                   u12       12           0  000000000000
 
 
 class SmpmUlDeviceHeatProxyMeter16BDailyData(Packet):
     value: float
     uptime_min: int
     meter_battery_volts: float
     capacitor_volts: float
@@ -60,23 +63,29 @@
         size += 2
         result |= ((1) & (2 ** (1) - 1)) << size
         size += 1
         result |= ((1) & (2 ** (2) - 1)) << size
         size += 2
         result |= ((0) & (2 ** (1) - 1)) << size
         size += 1
+        result |= ((0) & (2 ** (15) - 1)) << size
+        size += 15
         assert isinstance(data.value, (int, float))
         result |= ((int(round(float(data.value) * 1000.0, 0)) & 134217727) & (2 ** (27) - 1)) << size
         size += 27
+        result |= ((0) & (2 ** (5) - 1)) << size
+        size += 5
         assert isinstance(data.uptime_min, int)
         result |= (((data.uptime_min) & 4194303) & (2 ** (22) - 1)) << size
         size += 22
         assert isinstance(data.meter_battery_volts, (int, float))
         result |= ((int(round(max(min(5.11, float(data.meter_battery_volts)), 0.0) * 100.0, 0))) & (2 ** (9) - 1)) << size
         size += 9
+        result |= ((0) & (2 ** (1) - 1)) << size
+        size += 1
         assert isinstance(data.capacitor_volts, (int, float))
         result |= ((int(round(max(min(5.11, float(data.capacitor_volts)), 0.0) * 100.0, 0))) & (2 ** (9) - 1)) << size
         size += 9
         assert isinstance(data.radio_proxy_battery_volts, (int, float))
         result |= ((int(round(max(min(5.11, float(data.radio_proxy_battery_volts)), 0.0) * 100.0, 0))) & (2 ** (9) - 1)) << size
         size += 9
         assert isinstance(data.error_meter_sync, bool)
@@ -102,23 +111,26 @@
             raise ValueError("packet_type_id: buffer doesn't match value")
         if 1 != buf.shift(1):
             raise ValueError("packet_type_id: buffer doesn't match value")
         if 1 != buf.shift(2):
             raise ValueError("packet_type_id: buffer doesn't match value")
         if 0 != buf.shift(1):
             raise ValueError("packet_type_id: buffer doesn't match value")
+        buf.shift(15)
         result__el_tmp1["value"] = round(buf.shift(27) / 1000.0, 3)
+        buf.shift(5)
         result__el_tmp1["uptime_min"] = buf.shift(22) + 0
         result__el_tmp1["meter_battery_volts"] = round(buf.shift(9) / 100.0, 2)
+        buf.shift(1)
         result__el_tmp1["capacitor_volts"] = round(buf.shift(9) / 100.0, 2)
         result__el_tmp1["radio_proxy_battery_volts"] = round(buf.shift(9) / 100.0, 2)
         result__el_tmp1["error_meter_sync"] = bool(buf.shift(1))
         result__el_tmp1["error_reset"] = bool(buf.shift(1))
         result = SmpmUlDeviceHeatProxyMeter16BDailyData(**result__el_tmp1)
-        buf.shift(33)
+        buf.shift(12)
         return result
 
     def to_integration_data(self, received_at: datetime, device_tz: tzinfo, **kwargs: Any) -> List[IntegrationV0MessageData]:
         return [
             IntegrationV0MessageData(
                 dt=received_at,
                 battery=[
@@ -135,9 +147,14 @@
                         overloading_value=134217.727,
                     ),
                 ],
                 events=[
                     *([IntegrationV0MessageEvent.ERROR_RESET] if self.error_reset else []),
                     *([IntegrationV0MessageEvent.ERROR_METER_SYNC] if self.error_meter_sync else []),
                 ],
+                uptime=[
+                    IntegrationV0MessageUptime(
+                        uptime_s=self.uptime_min * 60,
+                    ),
+                ],
             ),
         ]
```

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/__tests__/timestamp_calculation.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/__tests__/timestamp_calculation.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/buf_ref.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/buf_ref.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/packet.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/data_gateway_sdk/utils/timestamp_calculation.py` & `ul-data-gateway-sdk-0.4.6/data_gateway_sdk/utils/timestamp_calculation.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/PKG-INFO` & `ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-gateway-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Data gateway sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-gateway-sdk-0.4.5/ul_data_gateway_sdk.egg-info/SOURCES.txt` & `ul-data-gateway-sdk-0.4.6/ul_data_gateway_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py
+data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_group_meter_daily.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py
 data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py
@@ -80,14 +81,15 @@
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py
+data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_group_meter_daily.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py
 data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py
```

