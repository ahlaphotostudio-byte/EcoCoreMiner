# EcoMine

Official programs, instructions and updates for **EcoMine**, distributed in the **EcoMine369** desktop application. This repository keeps its existing URL so installed links continue to work.

[Download EcoMine369 1.21.0](https://369apps.studio/ecomine/EcoMine369-1.21.0.zip) · [Website](https://369apps.studio/ecomine/) · [Installation](INSTALL-RU.md) · [Native engine](NATIVE-RU.md) · [Fee policy](FEES-RU.md)

## Current release

**Desktop 1.21.0 / EcoMine 0.2.0 + EcoMine 3 (0.4.0) — device-validation release.**

EcoMine contains its own compiled Autolykos2 computations and an Ergo Stratum adapter for NVIDIA on Windows/Linux x64. It verifies the package and GPU calculations before connecting to the configured pool. Every reported GPU solution is recomputed on CPU before submission. Existing profiles continue to use their selected engine.

EcoMine 3 adds Economy (70%), Balance (85%), Speed (100%) and a custom 50–100% active-time ceiling. Optional thermal adaptation reduces workload before the stop threshold and gradually recovers it after cooling. It fails closed on missing temperature feedback. These are duty-cycle settings, not watt limits or guaranteed savings.

The native host measures GPU block sizes in two passes with a stable-baseline check, retains the driver's occupancy choice when evidence is insufficient, and reuses allocated dataset memory across compatible jobs. Consensus CUBINs and the original EcoMine host are unchanged.

The own-engine comparison measures workloads 100/85/70/50%, repeats the selected candidate and baseline, and ranks by efficiency, balanced throughput or speed. Applying a confirmed result saves a device/driver/core-bound profile without starting mining. Hashrate per watt, kWh, temperature and accepted/rejected solutions are shown and exportable. Original profiles remain available.

Control vectors, CPU reference comparisons, partial-cache logic, a simulated local pool with reconnects and controller protection were tested. Physical GPU execution, Windows execution, accepted shares from a real pool and performance have not been validated in the build environment. Do not infer that every listed architecture is hardware-tested.

## Optional ERG mining-time fee

| Computing engine | Target share of observed mining time |
| --- | ---: |
| EcoMine / EcoMine 3 | 1.5% (54 seconds per 3600 counted seconds) |
| Rigel / lolMiner / SRBMiner, ERG only | 2% (72 seconds per 3600 counted seconds) |

Version 1.21.0 adds explicit consent per job and bounded switching to the published EcoMine recipient at `stratum+ssl://erg.2miners.com:18888`. Positive hashrate observations must be fresh. Restart/warm-up costs reduce throughput; mining-time share is not an exact share of coins. Failed fee attempts return to the original user command without debt. Checkpoints preserve user progress. Benchmarks do not collect this fee, and updating does not enable it in existing jobs. See [full terms](FEES-RU.md).

Pool payouts go separately to each address according to pool thresholds. No wallet balance is debited or transaction signed. Pool fees and the external miner's developer fee are additional. Other coins and managed payout deduction remain unconnected. The switching behavior was tested with harmless local processes; real GPU/pool execution and payouts still require device validation.

## Distribution

The new downloadable client is available from the website; older GitHub release assets remain available in [Releases](https://github.com/ahlaphotostudio-byte/EcoCoreMiner/releases). Check [release.json](release.json) and [SHA256SUMS.txt](SHA256SUMS.txt).

This public repository contains documentation and release metadata. Computational development source remains in the separate private repository. GitHub's automatically generated Source code ZIP/TAR files contain only this repository's files, not the GPU engine source. The installer includes binary computational modules and the existing MIT controller.

No seed phrase or private wallet key is needed. Existing MIT notices remain valid; see [notices](NOTICES.md).

