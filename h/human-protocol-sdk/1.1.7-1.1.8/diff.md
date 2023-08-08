# Comparing `tmp/human-protocol-sdk-1.1.7.tar.gz` & `tmp/human-protocol-sdk-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human-protocol-sdk-1.1.7.tar", last modified: Tue Jul 18 15:31:30 2023, max compression
+gzip compressed data, was "human-protocol-sdk-1.1.8.tar", last modified: Tue Aug  8 13:54:03 2023, max compression
```

## Comparing `human-protocol-sdk-1.1.7.tar` & `human-protocol-sdk-1.1.8.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.927006 human-protocol-sdk-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 15:31:30.927006 human-protocol-sdk-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/access/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/access/Ownable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/access/Ownable.sol/Ownable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/access/Ownable.sol/Ownable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/IERC1967.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/IERC1967.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/IERC1822Proxiable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/IERC1822Proxiable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/ERC1967Proxy.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/ERC1967Proxy.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/ERC1967Upgrade.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/ERC1967Upgrade.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/Proxy.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/Proxy.sol/Proxy.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/Proxy.sol/Proxy.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/beacon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/beacon/IBeacon.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/beacon/IBeacon.sol/IBeacon.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/beacon/IBeacon.sol/IBeacon.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/security/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/security/ReentrancyGuard.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/security/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/security/ReentrancyGuard.sol/ReentrancyGuard.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/IERC20.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/IERC20.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/IERC20Permit.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/IERC20Permit.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/SafeERC20.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/SafeERC20.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Address.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Address.sol/Address.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Address.sol/Address.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Context.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Context.sol/Context.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Context.sol/Context.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/StorageSlot.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/StorageSlot.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.895006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/access/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/OwnableUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/OwnableUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.895006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/IERC1967Upgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/IERC1967Upgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/IERC1822ProxiableUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/IERC1822ProxiableUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.895006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.895006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/ERC1967UpgradeUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/ERC1967UpgradeUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.895006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/IBeaconUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/IBeaconUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/Initializable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/Initializable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/UUPSUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/UUPSUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/IERC20Upgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/IERC20Upgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/SafeERC20Upgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/SafeERC20Upgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.899006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/AddressUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/AddressUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/ContextUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/ContextUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.907006 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/StorageSlotUpgradeable.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/StorageSlotUpgradeable.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.911006 human-protocol-sdk-1.1.7/artifacts/build-info/
--rw-r--r--   0 runner    (1001) docker     (123)  4794001 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/build-info/247a777d02ccff4beec972355f7291e9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/Escrow.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/Escrow.sol/Escrow.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    63101 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/Escrow.sol/Escrow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/EscrowFactory.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/EscrowFactory.sol/EscrowFactory.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    89123 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/EscrowFactory.sol/EscrowFactory.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/HMToken.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/HMToken.sol/HMToken.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    37580 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/HMToken.sol/HMToken.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/KVStore.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/KVStore.sol/KVStore.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/KVStore.sol/KVStore.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/RewardPool.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/RewardPool.sol/RewardPool.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    40026 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/RewardPool.sol/RewardPool.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/Staking.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/Staking.sol/Staking.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    82634 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/Staking.sol/Staking.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/HMTokenInterface.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.915006 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IEscrow.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IEscrow.sol/IEscrow.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IEscrow.sol/IEscrow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IRewardPool.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IRewardPool.sol/IRewardPool.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IRewardPool.sol/IRewardPool.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IStaking.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IStaking.sol/IStaking.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IStaking.sol/IStaking.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/contracts/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/libs/Stakes.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/libs/Stakes.sol/Stakes.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/libs/Stakes.sol/Stakes.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/contracts/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/test/EscrowFactoryV0.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    87845 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.903006 human-protocol-sdk-1.1.7/artifacts/contracts/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/utils/Math.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/utils/Math.sol/Math.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/utils/Math.sol/Math.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/utils/SafeMath.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/utils/SafeMath.sol/SafeMath.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/utils/SafeMath.sol/SafeMath.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/artifacts/contracts/utils/SignedSafeMath.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/utils/SignedSafeMath.sol/SignedSafeMath.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/artifacts/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.919006 human-protocol-sdk-1.1.7/human_protocol_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 15:31:27.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    24652 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/escrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/legacy_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/staking.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/human_protocol_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.923006 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 15:31:30.000000 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-07-18 15:31:30.000000 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:31:30.000000 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 15:31:30.000000 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 15:31:30.000000 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:31:30.000000 human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:31:30.927006 human-protocol-sdk-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.923006 human-protocol-sdk-1.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.923006 human-protocol-sdk-1.1.7/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20063 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/e2e/test_staking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.923006 human-protocol-sdk-1.1.7/test/human_protocol_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    83787 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_escrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_legacy_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    16350 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:31:30.927006 human-protocol-sdk-1.1.7/test/human_protocol_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/utils/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-18 15:29:01.000000 human-protocol-sdk-1.1.7/test/human_protocol_sdk/utils/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.349640 human-protocol-sdk-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 13:54:03.349640 human-protocol-sdk-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/access/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/access/Ownable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/access/Ownable.sol/Ownable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/access/Ownable.sol/Ownable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/IERC1967.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/IERC1967.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/IERC1822Proxiable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/IERC1822Proxiable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/ERC1967Proxy.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/ERC1967Proxy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/ERC1967Upgrade.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/ERC1967Upgrade.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/Proxy.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/Proxy.sol/Proxy.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/Proxy.sol/Proxy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/beacon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/beacon/IBeacon.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/beacon/IBeacon.sol/IBeacon.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/beacon/IBeacon.sol/IBeacon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/security/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/security/ReentrancyGuard.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/security/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/security/ReentrancyGuard.sol/ReentrancyGuard.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/IERC20.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/IERC20.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.333639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/IERC20Permit.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/IERC20Permit.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.333639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/SafeERC20.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/SafeERC20.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.333639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Address.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Address.sol/Address.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Address.sol/Address.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.333639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Context.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Context.sol/Context.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Context.sol/Context.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.333639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/StorageSlot.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/StorageSlot.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.317639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/access/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.325640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/OwnableUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/OwnableUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.317639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.325640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/IERC1967Upgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/IERC1967Upgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/IERC1822ProxiableUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/IERC1822ProxiableUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/ERC1967UpgradeUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/ERC1967UpgradeUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/IBeaconUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/IBeaconUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/Initializable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/Initializable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/UUPSUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/UUPSUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/IERC20Upgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/IERC20Upgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/SafeERC20Upgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/SafeERC20Upgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/AddressUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/AddressUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/ContextUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/ContextUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.329640 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/StorageSlotUpgradeable.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/StorageSlotUpgradeable.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.333639 human-protocol-sdk-1.1.8/artifacts/build-info/
+-rw-r--r--   0 runner    (1001) docker     (123)  4794001 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/build-info/247a777d02ccff4beec972355f7291e9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/Escrow.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/Escrow.sol/Escrow.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63101 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/Escrow.sol/Escrow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/EscrowFactory.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/EscrowFactory.sol/EscrowFactory.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89123 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/EscrowFactory.sol/EscrowFactory.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/HMToken.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/HMToken.sol/HMToken.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37580 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/HMToken.sol/HMToken.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/KVStore.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/KVStore.sol/KVStore.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/KVStore.sol/KVStore.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/RewardPool.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/RewardPool.sol/RewardPool.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40026 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/RewardPool.sol/RewardPool.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/Staking.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/Staking.sol/Staking.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82634 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/Staking.sol/Staking.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/HMTokenInterface.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IEscrow.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IEscrow.sol/IEscrow.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IEscrow.sol/IEscrow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IRewardPool.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IRewardPool.sol/IRewardPool.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IRewardPool.sol/IRewardPool.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.337640 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IStaking.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IStaking.sol/IStaking.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IStaking.sol/IStaking.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/contracts/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.341640 human-protocol-sdk-1.1.8/artifacts/contracts/libs/Stakes.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/libs/Stakes.sol/Stakes.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/libs/Stakes.sol/Stakes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/contracts/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.341640 human-protocol-sdk-1.1.8/artifacts/contracts/test/EscrowFactoryV0.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    87845 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.321639 human-protocol-sdk-1.1.8/artifacts/contracts/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.341640 human-protocol-sdk-1.1.8/artifacts/contracts/utils/Math.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/utils/Math.sol/Math.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/utils/Math.sol/Math.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.341640 human-protocol-sdk-1.1.8/artifacts/contracts/utils/SafeMath.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/utils/SafeMath.sol/SafeMath.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/utils/SafeMath.sol/SafeMath.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.341640 human-protocol-sdk-1.1.8/artifacts/contracts/utils/SignedSafeMath.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/utils/SignedSafeMath.sol/SignedSafeMath.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/artifacts/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.341640 human-protocol-sdk-1.1.8/human_protocol_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 13:53:59.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24677 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/escrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/legacy_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/human_protocol_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.345640 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 13:54:03.000000 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-08-08 13:54:03.000000 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:54:03.000000 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 13:54:03.000000 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 13:54:03.000000 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:54:03.000000 human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:54:03.349640 human-protocol-sdk-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.345640 human-protocol-sdk-1.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.345640 human-protocol-sdk-1.1.8/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/e2e/test_staking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.345640 human-protocol-sdk-1.1.8/test/human_protocol_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83787 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_escrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_legacy_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16350 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:54:03.349640 human-protocol-sdk-1.1.8/test/human_protocol_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/utils/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 13:51:53.000000 human-protocol-sdk-1.1.8/test/human_protocol_sdk/utils/job.py
```

### Comparing `human-protocol-sdk-1.1.7/LICENSE` & `human-protocol-sdk-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/README.md` & `human-protocol-sdk-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/access/Ownable.sol/Ownable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/access/Ownable.sol/Ownable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/IERC1967.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/IERC1967.sol/IERC1967.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/IERC1822Proxiable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/interfaces/draft-IERC1822.sol/IERC1822Proxiable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/ERC1967Proxy.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Proxy.sol/ERC1967Proxy.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/ERC1967Upgrade.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/proxy/ERC1967/ERC1967Upgrade.sol/ERC1967Upgrade.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/IERC20.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/IERC20.sol/IERC20.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/IERC20Permit.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol/IERC20Permit.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/SafeERC20.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol/SafeERC20.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/Address.sol/Address.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/Address.sol/Address.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/StorageSlot.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts/utils/StorageSlot.sol/StorageSlot.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/OwnableUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/access/OwnableUpgradeable.sol/OwnableUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/IERC1967Upgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/IERC1967Upgradeable.sol/IERC1967Upgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/IERC1822ProxiableUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/interfaces/draft-IERC1822Upgradeable.sol/IERC1822ProxiableUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/ERC1967UpgradeUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/ERC1967/ERC1967UpgradeUpgradeable.sol/ERC1967UpgradeUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/IBeaconUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/beacon/IBeaconUpgradeable.sol/IBeaconUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/Initializable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol/Initializable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/UUPSUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/proxy/utils/UUPSUpgradeable.sol/UUPSUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/IERC20Upgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol/IERC20Upgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/extensions/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/SafeERC20Upgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/token/ERC20/utils/SafeERC20Upgradeable.sol/SafeERC20Upgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/AddressUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/AddressUpgradeable.sol/AddressUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/ContextUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol/ContextUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/StorageSlotUpgradeable.json` & `human-protocol-sdk-1.1.8/artifacts/@openzeppelin/contracts-upgradeable/utils/StorageSlotUpgradeable.sol/StorageSlotUpgradeable.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/build-info/247a777d02ccff4beec972355f7291e9.json` & `human-protocol-sdk-1.1.8/artifacts/build-info/247a777d02ccff4beec972355f7291e9.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/Escrow.sol/Escrow.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/Escrow.sol/Escrow.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/EscrowFactory.sol/EscrowFactory.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/EscrowFactory.sol/EscrowFactory.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/HMToken.sol/HMToken.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/HMToken.sol/HMToken.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/KVStore.sol/KVStore.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/KVStore.sol/KVStore.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/RewardPool.sol/RewardPool.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/RewardPool.sol/RewardPool.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/Staking.sol/Staking.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/Staking.sol/Staking.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IEscrow.sol/IEscrow.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IEscrow.sol/IEscrow.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IRewardPool.sol/IRewardPool.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IRewardPool.sol/IRewardPool.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/interfaces/IStaking.sol/IStaking.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/interfaces/IStaking.sol/IStaking.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/libs/Stakes.sol/Stakes.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/libs/Stakes.sol/Stakes.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/utils/Math.sol/Math.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/utils/Math.sol/Math.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/utils/SafeMath.sol/SafeMath.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/utils/SafeMath.sol/SafeMath.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/artifacts/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json` & `human-protocol-sdk-1.1.8/artifacts/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/constants.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/encryption.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/encryption.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/escrow.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/escrow.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,19 +52,19 @@
             recording_oracle_address (str): Address of the Recording Oracle
             reputation_oracle_address (str): Address of the Reputation Oracle
             recording_oracle_fee (Decimal): Fee percentage of the Recording Oracle
             reputation_oracle_fee (Decimal): Fee percentage of the Reputation Oracle
             manifest_url (str): Manifest file url
             hash (str): Manifest file hash
         """
-        if not Web3.isAddress(recording_oracle_address):
+        if not Web3.is_address(recording_oracle_address):
             raise EscrowClientError(
                 f"Invalid recording oracle address: {recording_oracle_address}"
             )
-        if not Web3.isAddress(reputation_oracle_address):
+        if not Web3.is_address(reputation_oracle_address):
             raise EscrowClientError(
                 f"Invalid reputation oracle address: {reputation_oracle_address}"
             )
         if not (0 <= recording_oracle_fee <= 100) or not (
             0 <= reputation_oracle_fee <= 100
         ):
             raise EscrowClientError("Fee must be between 0 and 100")
@@ -112,15 +112,15 @@
             and not status
             and not date_from
             and not date_to
         ):
             raise EscrowClientError(
                 "EscrowFilter class must have at least one parameter"
             )
-        if address and not Web3.isAddress(address):
+        if address and not Web3.is_address(address):
             raise EscrowClientError(f"Invalid address: {address}")
         if date_from and date_to and date_from > date_to:
             raise EscrowClientError(
                 f"Invalid dates: {date_from} must be earlier than {date_to}"
             )
 
         self.address = address
@@ -171,19 +171,19 @@
 
         Returns:
             str: The address of the escrow created
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
-        if not Web3.isAddress(token_address):
+        if not Web3.is_address(token_address):
             raise EscrowClientError(f"Invalid token address: {token_address}")
 
         for handler in trusted_handlers:
-            if not Web3.isAddress(handler):
+            if not Web3.is_address(handler):
                 raise EscrowClientError(f"Invalid handler address: {handler}")
 
         transaction_receipt = handle_transaction(
             self.w3,
             "Create Escrow",
             self.factory_contract.functions.createEscrow(
                 token_address, trusted_handlers
@@ -210,15 +210,15 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         handle_transaction(
             self.w3,
             "Setup",
             self._get_escrow_contract(escrow_address).functions.setup(
                 escrow_config.reputation_oracle_address,
@@ -268,15 +268,15 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
         if 0 >= amount:
             raise EscrowClientError("Amount must be positive")
 
         token_address = self.get_token_address(escrow_address)
 
         erc20_interface = get_erc20_interface()
@@ -300,15 +300,15 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
         if not hash:
             raise EscrowClientError("Invalid empty hash")
         if not URL(url):
             raise EscrowClientError(f"Invalid URL: {url}")
         if not self.w3.eth.default_account:
             raise EscrowClientError("You must add an account to Web3 instance")
@@ -329,15 +329,15 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         handle_transaction(
             self.w3,
             "Complete",
             self._get_escrow_contract(escrow_address).functions.complete(),
             EscrowClientError,
@@ -365,18 +365,18 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
         for recipient in recipients:
-            if not Web3.isAddress(recipient):
+            if not Web3.is_address(recipient):
                 raise EscrowClientError(f"Invalid recipient address: {recipient}")
         if len(recipients) == 0:
             raise EscrowClientError("Arrays must have any value")
         if len(recipients) != len(amounts):
             raise EscrowClientError("Arrays must have same length")
         if 0 in amounts:
             raise EscrowClientError("Amounts cannot be empty")
@@ -411,15 +411,15 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         handle_transaction(
             self.w3,
             "Cancel",
             self._get_escrow_contract(escrow_address).functions.cancel(),
             EscrowClientError,
@@ -434,15 +434,15 @@
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         handle_transaction(
             self.w3,
             "Abort",
             self._get_escrow_contract(escrow_address).functions.abort(),
             EscrowClientError,
@@ -457,18 +457,18 @@
 
         Returns:
             None
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
         for handler in handlers:
-            if not Web3.isAddress(handler):
+            if not Web3.is_address(handler):
                 raise EscrowClientError(f"Invalid handler address: {handler}")
 
         handle_transaction(
             self.w3,
             "Add Trusted Handlers",
             self._get_escrow_contract(escrow_address).functions.addTrustedHandlers(
                 handlers
@@ -485,15 +485,15 @@
         Returns:
             Decimal: Value of the balance
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return self._get_escrow_contract(escrow_address).functions.getBalance().call()
 
     def get_manifest_url(self, escrow_address: str) -> str:
         """Gets the manifest file URL.
 
@@ -503,15 +503,15 @@
         Returns:
             str: Manifest file url
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return self._get_escrow_contract(escrow_address).functions.manifestUrl().call()
 
     def get_results_url(self, escrow_address: str) -> str:
         """Gets the results file URL.
 
@@ -521,15 +521,15 @@
         Returns:
             str: Results file url
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return (
             self._get_escrow_contract(escrow_address).functions.finalResultsUrl().call()
         )
 
     def get_intermediate_results_url(self, escrow_address: str) -> str:
@@ -541,15 +541,15 @@
         Returns:
             str: Intermediate results file url
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return (
             self._get_escrow_contract(escrow_address)
             .functions.intermediateResultsUrl()
             .call()
         )
@@ -563,15 +563,15 @@
         Returns:
             str: Address of the token
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return self._get_escrow_contract(escrow_address).functions.token().call()
 
     def get_status(self, escrow_address: str) -> Status:
         """Gets the current status of the escrow.
 
@@ -581,15 +581,15 @@
         Returns:
             Status: Current status
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return Status(
             self._get_escrow_contract(escrow_address).functions.status().call()
         )
 
     def get_launched_escrows(self, requester_address: str) -> List[str]:
@@ -662,15 +662,15 @@
         Returns:
             str: Recording oracle address
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return (
             self._get_escrow_contract(escrow_address).functions.recordingOracle().call()
         )
 
     def get_reputation_oracle_address(self, escrow_address: str) -> str:
@@ -682,15 +682,15 @@
         Returns:
             str: Reputation oracle address
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return (
             self._get_escrow_contract(escrow_address)
             .functions.reputationOracle()
             .call()
         )
@@ -704,15 +704,15 @@
         Returns:
             str: Job launcher address
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return self._get_escrow_contract(escrow_address).functions.launcher().call()
 
     def get_factory_address(self, escrow_address: str) -> str:
         """Gets the escrow factory address of the escrow.
 
@@ -722,15 +722,15 @@
         Returns:
             str: Escrow factory address
 
         Raises:
             EscrowClientError: If an error occurs while checking the parameters
         """
 
-        if not Web3.isAddress(escrow_address):
+        if not Web3.is_address(escrow_address):
             raise EscrowClientError(f"Invalid escrow address: {escrow_address}")
 
         return (
             self._get_escrow_contract(escrow_address).functions.escrowFactory().call()
         )
 
     def _get_escrow_contract(self, address: str) -> contract:
```

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/kvstore.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/kvstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,11 +111,11 @@
 
         Returns:
             value (str): The value of the key-value pair if it exists
         """
 
         if not key:
             raise KVStoreClientError("Key can not be empty")
-        if not Web3.isAddress(address):
+        if not Web3.is_address(address):
             raise KVStoreClientError(f"Invalid address: {address}")
         result = self.kvstore_contract.functions.get(address, key).call()
         return result
```

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/legacy_encryption.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/legacy_encryption.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/staking.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/staking.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/storage.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/storage.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk/utils.py` & `human-protocol-sdk-1.1.8/human_protocol_sdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     hmtoken_contract: Contract, tx_receipt: Optional[TxReceipt]
 ) -> Tuple[bool, Optional[int]]:
     hmt_transferred = False
     tx_balance = None
     if not tx_receipt:
         return hmt_transferred, tx_balance
 
-    transfer_event = hmtoken_contract.events.Transfer().processReceipt(tx_receipt)
+    transfer_event = hmtoken_contract.events.Transfer().process_receipt(tx_receipt)
     logger.info(f"Transfer_event {transfer_event}.")
 
     hmt_transferred = bool(transfer_event)
 
     if hmt_transferred:
         tx_balance = transfer_event[0].get("args", {}).get("_value")
```

### Comparing `human-protocol-sdk-1.1.7/human_protocol_sdk.egg-info/SOURCES.txt` & `human-protocol-sdk-1.1.8/human_protocol_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/setup.py` & `human-protocol-sdk-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="human-protocol-sdk",
-    version="0.0.7",
+    version="0.0.8",
     author="HUMAN Protocol",
     description="A python library to launch escrow contracts to the HUMAN network.",
     url="https://github.com/humanprotocol/human-protocol/packages/sdk/python/human-protocol-sdk",
     include_package_data=True,
     exclude_package_data={"artifacts": ["*.dbg.json"]},
     zip_safe=True,
     classifiers=[
```

### Comparing `human-protocol-sdk-1.1.7/test/e2e/test_staking.py` & `human-protocol-sdk-1.1.8/test/e2e/test_staking.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         self.staking_client.stake(10)
 
         tx_hash = self.staking_client.factory_contract.functions.createEscrow(
             self.staking_client.hmtoken_contract.address,
             [self.gas_payer.address],
         ).transact()
 
-        tx_receipt = self.staking_client.w3.eth.waitForTransactionReceipt(tx_hash)
+        tx_receipt = self.staking_client.w3.eth.wait_for_transaction_receipt(tx_hash)
 
-        events = self.staking_client.factory_contract.events.Launched().processReceipt(
+        events = self.staking_client.factory_contract.events.Launched().process_receipt(
             tx_receipt
         )
         self.escrow_address = events[0].get("args", {}).get("escrow", "")
 
         escrow_interface = get_escrow_interface()
         self.escrow = self.staking_client.w3.eth.contract(
             address=self.escrow_address, abi=escrow_interface["abi"]
```

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_encryption.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_encryption.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_escrow.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_escrow.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_kvstore.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_kvstore.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,25 +141,25 @@
             kvstore.set_bulk(keys, values)
         self.assertEqual("You must add an account to Web3 instance", str(cm.exception))
 
     def test_get(self):
         mock_function = MagicMock()
         mock_function.return_value.call.return_value = "mock_value"
         self.kvstore.kvstore_contract.functions.get = mock_function
-        address = Web3.toChecksumAddress("0x1234567890123456789012345678901234567890")
+        address = Web3.to_checksum_address("0x1234567890123456789012345678901234567890")
         key = "key"
 
         result = self.kvstore.get(address, key)
 
         mock_function.assert_called_once_with(address, key)
         mock_function.return_value.call.assert_called_once_with()
         self.assertEqual(result, "mock_value")
 
     def test_get_empty_key(self):
-        address = Web3.toChecksumAddress("0x1234567890123456789012345678901234567890")
+        address = Web3.to_checksum_address("0x1234567890123456789012345678901234567890")
         key = ""
         with self.assertRaises(KVStoreClientError) as cm:
             self.kvstore.get(address, key)
         self.assertEqual("Key can not be empty", str(cm.exception))
 
     def test_get_invalid_address(self):
         address = "invalid_address"
@@ -168,15 +168,15 @@
             self.kvstore.get(address, key)
         self.assertEqual("Invalid address: invalid_address", str(cm.exception))
 
     def test_get_empty_value(self):
         mock_function = MagicMock()
         mock_function.return_value.call.return_value = ""
         self.kvstore.kvstore_contract.functions.get = mock_function
-        address = Web3.toChecksumAddress("0x1234567890123456789012345678901234567890")
+        address = Web3.to_checksum_address("0x1234567890123456789012345678901234567890")
         key = "key"
 
         result = self.kvstore.get(address, key)
 
         mock_function.assert_called_once_with(address, key)
         mock_function.return_value.call.assert_called_once_with()
         self.assertEqual(result, "")
@@ -189,15 +189,15 @@
 
         kvstore = KVStoreClient(w3)
 
         mock_function = MagicMock()
         mock_function.return_value.call.return_value = "mock_value"
         kvstore.kvstore_contract.functions.get = mock_function
 
-        address = Web3.toChecksumAddress("0x1234567890123456789012345678901234567890")
+        address = Web3.to_checksum_address("0x1234567890123456789012345678901234567890")
         key = "key"
 
         result = kvstore.get(address, key)
 
         mock_function.assert_called_once_with(address, key)
         mock_function.return_value.call.assert_called_once_with()
         self.assertEqual(result, "mock_value")
```

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_legacy_encryption.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_legacy_encryption.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_staking.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_staking.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/test_storage.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/test_storage.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.7/test/human_protocol_sdk/utils/encryption.py` & `human-protocol-sdk-1.1.8/test/human_protocol_sdk/utils/encryption.py`

 * *Files identical despite different names*

