# EcoCoreMiner

Official downloads, instructions and release notes for EcoCoreMiner, distributed through the **EcoMine369** desktop application.

[Download and updates](https://github.com/ahlaphotostudio-byte/EcoCoreMiner/releases) · [Website](https://369apps.studio/ecomine/) · [Fee policy](FEES-RU.md) · [Installation](INSTALL-RU.md)

## Current release

**EcoMine369 1.17.0 — EcoCoreMiner branding and fee policy.** The application manages installed third-party miners. Existing profiles, wallets and history are preserved when using its updater.

The separate native EcoCoreMiner Autolykos2 GPU engine is in development. Its CUDA/OpenCL sources and unpublished binaries are not distributed here. This release does not claim a production native pool miner or automatic fee deduction.

| Actual computing engine | Service tariff |
| --- | ---: |
| Native EcoCoreMiner, when released and connected to payouts | 1.5% |
| SRBMiner, lolMiner, Rigel, XMRig, PeakMiner or a custom external engine managed through EcoMine | 2% |

The external engine's own developer fee and the pool's fee are separate. Selecting the EcoCoreMiner management interface does not turn an external engine into a native one or reduce its tariff.

## Distribution model

This public repository contains documentation, release manifests and downloadable programs. Development takes place in a separate private repository. GitHub's automatically generated **Source code** ZIP/TAR archives contain only the files in this public repository, not the GPU engine implementation.

Use release assets or the website for installation. Check the published SHA-256 before running a download. No seed phrase or wallet private key is needed to configure mining.

Existing MIT components retain their license. See [notices](NOTICES.md).
