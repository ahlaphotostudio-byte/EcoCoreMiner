# EcoMine

Official programs, instructions and updates for **EcoMine**, distributed in the **EcoMine369** desktop application. This repository keeps its existing URL so installed links continue to work.

[Download EcoMine369 1.19.0](https://369apps.studio/ecomine/EcoMine369-1.19.0.zip) · [Website](https://369apps.studio/ecomine/) · [Installation](INSTALL-RU.md) · [Native engine](NATIVE-RU.md) · [Fee policy](FEES-RU.md)

## Current release

**Desktop 1.19.0 / EcoMine 0.2.0 + EcoMine 3 (0.3.0) — device-validation release.**

EcoMine contains its own compiled Autolykos2 computations and an Ergo Stratum adapter for NVIDIA on Windows/Linux x64. It verifies the package and GPU calculations before connecting to the configured pool. Every reported GPU solution is recomputed on CPU before submission. Existing profiles continue to use their selected engine.

EcoMine 3 is a separate execution variant: per-kernel driver occupancy selection, cached functions/job data and blocking CPU waits. It shares the unchanged compiled Autolykos2 kernels with the baseline. Its optional economy mode paces GPU batches to a nominal 70% active time; that is not a watt limit or a guarantee of savings. The comparison screen prepares three new profiles and shows hashrate per watt, energy, temperature and shares. Original profiles are preserved.

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

