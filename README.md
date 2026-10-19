# EcoMine

Official programs, instructions and updates for **EcoMine**, distributed in the **EcoMine369** desktop application. This repository keeps its existing URL so installed links continue to work.

[Download EcoMine369 1.20.0](https://369apps.studio/ecomine/EcoMine369-1.20.0.zip) · [Website](https://369apps.studio/ecomine/) · [Installation](INSTALL-RU.md) · [Native engine](NATIVE-RU.md) · [Fee policy](FEES-RU.md)

## Current release

**Desktop 1.20.0 / EcoMine 0.2.0 + EcoMine 3 (0.4.0) — device-validation release.**

EcoMine contains its own compiled Autolykos2 computations and an Ergo Stratum adapter for NVIDIA on Windows/Linux x64. It verifies the package and GPU calculations before connecting to the configured pool. Every reported GPU solution is recomputed on CPU before submission. Existing profiles continue to use their selected engine.

EcoMine 3 adds Economy (70%), Balance (85%), Speed (100%) and a custom 50–100% active-time ceiling. Optional thermal adaptation reduces workload before the stop threshold and gradually recovers it after cooling. It fails closed on missing temperature feedback. These are duty-cycle settings, not watt limits or guaranteed savings.

The native host measures GPU block sizes in two passes with a stable-baseline check, retains the driver's occupancy choice when evidence is insufficient, and reuses allocated dataset memory across compatible jobs. Consensus CUBINs and the original EcoMine host are unchanged.

The own-engine comparison measures workloads 100/85/70/50%, repeats the selected candidate and baseline, and ranks by efficiency, balanced throughput or speed. Applying a confirmed result saves a device/driver/core-bound profile without starting mining. Hashrate per watt, kWh, temperature and accepted/rejected solutions are shown and exportable. Original profiles remain available.

Control vectors, CPU reference comparisons, partial-cache logic, a simulated local pool with reconnects and controller protection were tested. Physical GPU execution, Windows execution, accepted shares from a real pool and performance have not been validated in the build environment. Do not infer that every listed architecture is hardware-tested.

| Computing engine | Service tariff |
| --- | ---: |
| EcoMine / EcoMine 3 native engines, once connected to the settlement path | 1.5% |
| External engines managed through EcoMine | 2% |

Automatic deduction is disabled. This native release does not switch mining to a developer wallet or send payments. Pool fees and an external miner's developer fee are separate.

## Distribution

The new downloadable client is available from the website; older GitHub release assets remain available in [Releases](https://github.com/ahlaphotostudio-byte/EcoCoreMiner/releases). Check [release.json](release.json) and [SHA256SUMS.txt](SHA256SUMS.txt).

This public repository contains documentation and release metadata. Computational development source remains in the separate private repository. GitHub's automatically generated Source code ZIP/TAR files contain only this repository's files, not the GPU engine source. The installer includes binary computational modules and the existing MIT controller.

No seed phrase or private wallet key is needed. Existing MIT notices remain valid; see [notices](NOTICES.md).

