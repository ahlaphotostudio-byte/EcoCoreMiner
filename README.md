# EcoCoreMiner / EcoMine369

EcoCoreMiner **0.1.0-preview** is a standalone mining engine under development. EcoMine369 **1.22.0** provides the desktop interface and eight simple coin profiles.

- [Product page](https://369apps.studio/ecocoreminer/)
- [Standalone EcoCoreMiner ZIP](https://369apps.studio/ecocoreminer/releases/EcoCoreMiner-0.1.0-preview.zip) — Windows / Linux x64; Python 3.10+ required; explicit ERG module setup downloads approximately 19 MB from the checksum-verified EcoMine distribution.
- [EcoMine369 Windows ZIP](https://369apps.studio/ecomine/EcoMine369-1.22.0.zip) — includes Python and the standalone CLI.
- [Russian instructions](INSTALL-RU.md), [native modules and readiness](NATIVE-RU.md), [fees](FEES-RU.md), [checksums](SHA256SUMS.txt).

Own-engine fee: **2%**. External engines managed through EcoMine: **3%**, plus their own miner and pool fees. Automatic mining-time collection is implemented for **ERG / Autolykos2**, with explicit terms. BTC/ASIC collection is not connected because no BTC fee recipient is configured. No wallet balance is debited.

Autolykos2 and a new SHA256d implementation have binary modules. Bitcoin has a Stratum v1 adapter and an experimental one-device ASIC gateway. Other native algorithms are **planned**, not implemented. Hardware acceptance, actual pool shares, Windows execution, performance and energy efficiency remain unverified. This is not a completed commercial release or a claim of universal hardware support.

The public repository contains distribution documentation and update metadata. Computational source and build tools remain in a separate private development repository. Downloads are hosted on the product website; this commit does not create GitHub Release binary assets. Existing MIT and third-party notices remain applicable.
