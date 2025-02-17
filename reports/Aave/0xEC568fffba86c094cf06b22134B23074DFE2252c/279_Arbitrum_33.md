## Arbitrum

- Simulation: [https://dashboard.tenderly.co/me/simulator/806b6d99-222c-4833-8668-0ae1d9fbae42](https://dashboard.tenderly.co/me/simulator/806b6d99-222c-4833-8668-0ae1d9fbae42)

### Checks

#### Reports all state changes from the proposal ✅ Passed

Info:

- State changes:

```diff
# InitializableImmutableAdminUpgradeabilityProxy at `0x794a61358D6845594F94dc1DB02A252b5b4814aD`
@@ `_reserves` key `0x3f56e0c36d275367b8c502090edf38289b3dea0d`.configuration.data @@
- 789842187514178900234390916618697834629975824831871252692900334111038796
+ 65820182292848241686204476293091843982498351104381157829614586399038796

# decoded configuration.data for key `0x3f56e0c36d275367b8c502090edf38289b3dea0d` (symbol: MAI)
@@ configuration.data.borrowCap @@
- 2400000
+ 250000
@@ configuration.data.supplyCap @@
- 4800000
+ 325000
@@ configuration.data.debtCeiling @@
- 120000000
+ 10000000

```

```diff
# ArbitrumBridgeExecutor at `0x7d9103572bE58FfE99dc390E8246f02dcAe6f611`
@@ `_queuedActions` key `0x25829da8039192178bce8b8d1352b5c60971834199ca1df37bd0b915edb424a2` @@
- true
+ false

@@ `_actionsSets` key `"33"`.executed @@
- false
+ true

```

```diff
# unknown contract name at `0xA4b05FffffFffFFFFfFFfffFfffFFfffFfFfFFFf`
@@ Slot `0xa9f6f085d78d1d37c5819e5c16c9e03198bd14e08cd1f6f8191bc6207b9e9706` @@
- "0x0000000000000000000000000000000000000000000000000000000001a66413"
+ "0x0000000000000000000000000000000000000000000000000000000001a66f4f"
@@ Slot `0xa9f6f085d78d1d37c5819e5c16c9e03198bd14e08cd1f6f8191bc6207b9e970b` @@
- "0x00000000000000000000000000000000000000000000000028281b77d9f74d5c"
+ "0x0000000000000000000000000000000000000000000000002828363c97c0a05c"
```

#### Check stack trace of the proposal ✅ Passed

Info:

- There is no SELFDESTRUCT inside of delegated call

#### Reports all events emitted from the proposal ✅ Passed

Info:

- Events Emitted:
  - InitializableImmutableAdminUpgradeabilityProxy at `0x8145eddDf43f50276641b55bd3AD95944510021E`
    - `CollateralConfigurationChanged(asset: 0x3f56e0c36d275367b8c502090edf38289b3dea0d, ltv: 7500, liquidationThreshold: 8000, liquidationBonus: 10500)`
    - `DebtCeilingChanged(asset: 0x3f56e0c36d275367b8c502090edf38289b3dea0d, oldDebtCeiling: 120000000, newDebtCeiling: 10000000)`
    - `SupplyCapChanged(asset: 0x3f56e0c36d275367b8c502090edf38289b3dea0d, oldSupplyCap: 4800000, newSupplyCap: 325000)`
    - `BorrowCapChanged(asset: 0x3f56e0c36d275367b8c502090edf38289b3dea0d, oldBorrowCap: 2400000, newBorrowCap: 250000)`
  - ArbitrumBridgeExecutor at `0x7d9103572bE58FfE99dc390E8246f02dcAe6f611`
    - `ActionsSetExecuted(id: 33, initiatorExecution: 0xd73a92be73efbfcf3854433a5fcbabf9c1316073, returnedData: 0x)`

#### Check all targets are verified on Etherscan ✅ Passed

Info:

- Targets:
  - 0x4449A4d0C1cA7C0EA218F11C8a84DD9b8e633D43: Contract (not verified)

#### Check all touched contracts are verified on Etherscan ✅ Passed

Info:

- Touched address:
  - 0xd73a92be73efbfcf3854433a5fcbabf9c1316073: EOA (verification not applicable)
  - 0x7d9103572be58ffe99dc390e8246f02dcae6f611: Contract (verified) (ArbitrumBridgeExecutor)
  - 0x4449a4d0c1ca7c0ea218f11c8a84dd9b8e633d43: Contract (not verified)
  - 0x0efdfc1a940de4e7e6acc9bb801481f81b17fd20: Contract (verified) (AaveV3ConfigEngine)
  - 0x794a61358d6845594f94dc1db02a252b5b4814ad: Contract (verified) (InitializableImmutableAdminUpgradeabilityProxy)
  - 0xbcb167bdcf14a8f791d6f4a6edd964aed2f8813b: Contract (verified) (L2Pool)
  - 0x8145edddf43f50276641b55bd3ad95944510021e: Contract (verified) (InitializableImmutableAdminUpgradeabilityProxy)
  - 0x04a8d477ee202adce1682f5902e1160455205b12: Contract (verified) (PoolConfigurator)
  - 0xa97684ead0e402dc232d5a977953df7ecbab3cdb: Contract (verified) (PoolAddressesProvider)
  - 0xa72636cbcaa8f5ff95b2cc47f3cdee83f3294a0b: Contract (verified) (ACLManager)

#### Runs solc against the verified contracts ✅ Passed

Info:

-

<details>
<summary>View Details</summary>
<details>
<summary>View warnings for PoolConfigurator at `0x04a8D477eE202aDCE1682F5902e1160455205b12`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for AaveV3ConfigEngine at `0x0EfdfC1A940DE4E7E6acC9Bb801481f81B17fd20`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for InitializableImmutableAdminUpgradeabilityProxy at `0x794a61358D6845594F94dc1DB02A252b5b4814aD`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for ArbitrumBridgeExecutor at `0x7d9103572bE58FfE99dc390E8246f02dcAe6f611`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for InitializableImmutableAdminUpgradeabilityProxy at `0x8145eddDf43f50276641b55bd3AD95944510021E`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for ACLManager at `0xa72636CbcAa8F5FF95B2cc47F3CDEe83F3294a0B`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for PoolAddressesProvider at `0xa97684ead0e402dC232d5A977953DF7ECBaB3CDb`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for L2Pool at `0xbCb167bDCF14a8F791d6f4A6EDd964aed2F8813B`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

</details>

#### Runs slither against the verified contracts ✅ Passed

Info:

-

<details>
<summary>View Details</summary>

<details>
<summary>Slither report for PoolConfigurator at `0x04a8D477eE202aDCE1682F5902e1160455205b12`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0x04a8d477ee202adce1682f5902e1160455205b12
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for AaveV3ConfigEngine at `0x0EfdfC1A940DE4E7E6acC9Bb801481f81B17fd20`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0x0efdfc1a940de4e7e6acc9bb801481f81b17fd20
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for InitializableImmutableAdminUpgradeabilityProxy at `0x794a61358D6845594F94dc1DB02A252b5b4814aD`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0x794a61358d6845594f94dc1db02a252b5b4814ad
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for ArbitrumBridgeExecutor at `0x7d9103572bE58FfE99dc390E8246f02dcAe6f611`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0x7d9103572be58ffe99dc390e8246f02dcae6f611
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for InitializableImmutableAdminUpgradeabilityProxy at `0x8145eddDf43f50276641b55bd3AD95944510021E`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0x8145edddf43f50276641b55bd3ad95944510021e
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for ACLManager at `0xa72636CbcAa8F5FF95B2cc47F3CDEe83F3294a0B`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0xa72636cbcaa8f5ff95b2cc47f3cdee83f3294a0b
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for PoolAddressesProvider at `0xa97684ead0e402dC232d5A977953DF7ECBaB3CDb`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0xa97684ead0e402dc232d5a977953df7ecbab3cdb
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

<details>
<summary>Slither report for L2Pool at `0xbCb167bDCF14a8F791d6f4A6EDd964aed2F8813B`</summary>

```
Source code not available, try to fetch the bytecode only
ERROR:SlitherSolcParsing:crytic-compile returned an empty AST. If you are trying to analyze a contract from etherscan or similar make sure it has source code available.
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''
ERROR:root:Error in 0xbcb167bdcf14a8f791d6f4a6edd964aed2f8813b
ERROR:root:Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 115, in __init__
    self.add_source_code(path)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/core/slither_core.py", line 172, in add_source_code
    with open(path, encoding="utf8", newline="") as f:
FileNotFoundError: [Errno 2] No such file or directory: ''

```

</details>

</details>
