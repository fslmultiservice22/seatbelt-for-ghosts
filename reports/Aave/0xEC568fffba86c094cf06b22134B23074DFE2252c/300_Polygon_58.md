## Polygon

- Simulation: [https://dashboard.tenderly.co/me/simulator/d7dbe7e8-864f-40cf-a9d4-ce6972dbd3ed](https://dashboard.tenderly.co/me/simulator/d7dbe7e8-864f-40cf-a9d4-ce6972dbd3ed)

### Checks

#### Reports all state changes from the proposal ✅ Passed

Info:

- State changes:

```diff
# InitializableImmutableAdminUpgradeabilityProxy at `0x794a61358D6845594F94dc1DB02A252b5b4814aD` with implementation Pool at `0xb77fc84a549ecc0b410d6fa15159C2df207545a3`
@@ `_reserves` key `0x3a58a54c066fdc0f2d55fc9c89f0415c92ebf3c4`.configuration.data @@
- 759706823178139962631042604402753306546605517968264
+ 759706824590444708152515719363048308094471629968264

# decoded configuration.data for key `0x3a58a54c066fdc0f2d55fc9c89f0415c92ebf3c4` (symbol: stMATIC)
@@ configuration.data.supplyCap @@
- 40000000
+ 57000000

```

```diff
# PolygonBridgeExecutor at `0xdc9A35B16DB4e126cFeDC41322b3a36454B1F772`
@@ `_actionsSets` key `"58"`.executed @@
- false
+ true

@@ `_queuedActions` key `0xc8bd066296a72f493d5bf57f23a212d5ff18d65134db16513f782a561121167c` @@
- true
+ false

```

#### Check stack trace of the proposal ✅ Passed

Info:

- There is no SELFDESTRUCT inside of delegated call

#### Reports all events emitted from the proposal ✅ Passed

Info:

- Events Emitted:
  - InitializableImmutableAdminUpgradeabilityProxy at `0x8145eddDf43f50276641b55bd3AD95944510021E` with implementation PoolConfigurator at `0xADf86b537eF08591c2777E144322E8b0Ca7E82a7`
    - `SupplyCapChanged(asset: 0x3a58a54c066fdc0f2d55fc9c89f0415c92ebf3c4, oldSupplyCap: 40000000, newSupplyCap: 57000000)`
  - PolygonBridgeExecutor at `0xdc9A35B16DB4e126cFeDC41322b3a36454B1F772`
    - `ActionsSetExecuted(id: 58, initiatorExecution: 0xd73a92be73efbfcf3854433a5fcbabf9c1316073, returnedData: 0x)`

#### Check all targets are verified on Etherscan ✅ Passed

Info:

- Targets:
  - 0xF28E5a2f04B6B74741579DaEE1fc164978D2d646: Contract (not verified)

#### Check all touched contracts are verified on Etherscan ✅ Passed

Info:

- Touched address:
  - 0xd73a92be73efbfcf3854433a5fcbabf9c1316073: EOA (verification not applicable)
  - 0xdc9a35b16db4e126cfedc41322b3a36454b1f772: Contract (verified) (PolygonBridgeExecutor)
  - 0xf28e5a2f04b6b74741579daee1fc164978d2d646: Contract (verified) (AaveV3PolygonSupplyCapStmatic_20230810)
  - 0xe202f2fc4b6a37ba53cfd15be42a762a645fca07: Contract (verified) (AaveV3ConfigEngine)
  - 0x8145edddf43f50276641b55bd3ad95944510021e: Contract (verified) (InitializableImmutableAdminUpgradeabilityProxy)
  - 0xadf86b537ef08591c2777e144322e8b0ca7e82a7: Contract (verified) (PoolConfigurator)
  - 0xa97684ead0e402dc232d5a977953df7ecbab3cdb: Contract (verified) (PoolAddressesProvider)
  - 0xa72636cbcaa8f5ff95b2cc47f3cdee83f3294a0b: Contract (verified) (ACLManager)
  - 0x794a61358d6845594f94dc1db02a252b5b4814ad: Contract (verified) (InitializableImmutableAdminUpgradeabilityProxy)
  - 0xb77fc84a549ecc0b410d6fa15159c2df207545a3: Contract (verified) (Pool)

#### Runs solc against the verified contracts ✅ Passed

Info:

-

<details>
<summary>View Details</summary>
<details>
<summary>View warnings for InitializableImmutableAdminUpgradeabilityProxy at `0x794a61358D6845594F94dc1DB02A252b5b4814aD` with implementation Pool at `0xb77fc84a549ecc0b410d6fa15159C2df207545a3`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for InitializableImmutableAdminUpgradeabilityProxy at `0x8145eddDf43f50276641b55bd3AD95944510021E` with implementation PoolConfigurator at `0xADf86b537eF08591c2777E144322E8b0Ca7E82a7`</summary>

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
<summary>View warnings for PoolConfigurator at `0xADf86b537eF08591c2777E144322E8b0Ca7E82a7`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for Pool at `0xb77fc84a549ecc0b410d6fa15159C2df207545a3`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for PolygonBridgeExecutor at `0xdc9A35B16DB4e126cFeDC41322b3a36454B1F772`</summary>

```
INFO:CryticCompile:Source code not available, try to fetch the bytecode only
```

</details>

<details>
<summary>View warnings for AaveV3ConfigEngine at `0xE202F2fc4b6A37Ba53cfD15bE42a762A645FCA07`</summary>

```
INFO:CryticCompile:'solc --standard-json --allow-paths /home/runner/work/seatbelt-for-ghosts/seatbelt-for-ghosts/crytic-export/etherscan-contracts/0xe202f2fc4b6a37ba53cfd15be42a762a645fca07-AaveV3ConfigEngine' running
```

</details>

<details>
<summary>View warnings for AaveV3PolygonSupplyCapStmatic_20230810 at `0xF28E5a2f04B6B74741579DaEE1fc164978D2d646`</summary>

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
<summary>Slither report for InitializableImmutableAdminUpgradeabilityProxy at `0x794a61358D6845594F94dc1DB02A252b5b4814aD` with implementation Pool at `0xb77fc84a549ecc0b410d6fa15159C2df207545a3`</summary>

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
<summary>Slither report for InitializableImmutableAdminUpgradeabilityProxy at `0x8145eddDf43f50276641b55bd3AD95944510021E` with implementation PoolConfigurator at `0xADf86b537eF08591c2777E144322E8b0Ca7E82a7`</summary>

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
<summary>Slither report for PoolConfigurator at `0xADf86b537eF08591c2777E144322E8b0Ca7E82a7`</summary>

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
ERROR:root:Error in 0xadf86b537ef08591c2777e144322e8b0ca7e82a7
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
<summary>Slither report for Pool at `0xb77fc84a549ecc0b410d6fa15159C2df207545a3`</summary>

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
ERROR:root:Error in 0xb77fc84a549ecc0b410d6fa15159c2df207545a3
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
<summary>Slither report for PolygonBridgeExecutor at `0xdc9A35B16DB4e126cFeDC41322b3a36454B1F772`</summary>

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
ERROR:root:Error in 0xdc9a35b16db4e126cfedc41322b3a36454b1f772
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
<summary>Slither report for AaveV3ConfigEngine at `0xE202F2fc4b6A37Ba53cfD15bE42a762A645FCA07`</summary>

```
'solc --standard-json --allow-paths /home/runner/work/seatbelt-for-ghosts/seatbelt-for-ghosts/crytic-export/etherscan-contracts/0xe202f2fc4b6a37ba53cfd15be42a762a645fca07-AaveV3ConfigEngine' running
Traceback (most recent call last):
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 814, in main_impl
    ) = process_all(filename, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 102, in process_all
    ) = process_single(compilation, args, detector_classes, printer_classes)
  File "/home/runner/.local/lib/python3.10/site-packages/slither/__main__.py", line 80, in process_single
    slither = Slither(target, ast_format=ast, **vars(args))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 135, in __init__
    self._init_parsing_and_analyses(kwargs.get("skip_analyze", False))
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 145, in _init_parsing_and_analyses
    raise e
  File "/home/runner/.local/lib/python3.10/site-packages/slither/slither.py", line 141, in _init_parsing_and_analyses
    parser.parse_contracts()
  File "/home/runner/.local/lib/python3.10/site-packages/slither/solc_parsing/slither_compilation_unit_solc.py", line 447, in parse_contracts
    raise InheritanceResolutionError(
slither.solc_parsing.slither_compilation_unit_solc.InheritanceResolutionError: Could not resolve contract inheritance. This is likely caused by an import renaming that collides with existing names (see https://github.com/crytic/slither/issues/1758).
 Try changing `contract IACLManager` (lib/aave-address-book/src/AaveV3.sol#75-87) to a unique name.
ERROR:root:Error:
ERROR:root:Could not resolve contract inheritance. This is likely caused by an import renaming that collides with existing names (see https://github.com/crytic/slither/issues/1758).
 Try changing `contract IACLManager` (lib/aave-address-book/src/AaveV3.sol#75-87) to a unique name.
ERROR:root:Please report an issue to https://github.com/crytic/slither/issues
```

</details>

<details>
<summary>Slither report for AaveV3PolygonSupplyCapStmatic_20230810 at `0xF28E5a2f04B6B74741579DaEE1fc164978D2d646`</summary>

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
ERROR:root:Error in 0xf28e5a2f04b6b74741579daee1fc164978d2d646
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
