# Releases

## 1.19.0 / EcoMine 3 (0.3.0) — 2026-10-18

- Separate native execution variant; original EcoMine binaries and profiles preserved.
- Per-kernel CUDA launch selection, cached job/functions, blocking CPU waits.
- Optional interruptible 70% active-time pacing, including dataset building; no fixed watt-saving claim.
- One-click preparation of three sequential comparison profiles; efficiency, energy and temperature in results/CSV.
- Same algorithm, pool, wallet and device enforced for comparisons.
- CPU/reference, mock-driver contracts, pacing, guard and distribution checks passed. Real GPU, Windows execution, live-pool shares and performance remain unvalidated.
- Native tariff remains 1.5%; external tariff 2%. Automatic collection remains disabled.


## 1.18.0 / EcoMine native 0.2.0 — 2026-10-18

- Own computing engine is now named **EcoMine**.
- NVIDIA / ERG native binary runtime and nine-field Ergo Stratum connection.
- Mandatory CPU/GPU self-test, every share rechecked on CPU, stale-job and session isolation.
- Full or partial VRAM cache, bounded batches and configured-pool reconnects.
- Integrated existing process containment and mandatory temperature monitoring.
- 160 desktop tests passed, including 18 native/reference/protocol checks; no physical GPU or real-pool performance claim.
- Binary-only computational release; private source remains private.
- Native 1.5% / external 2% tariffs unchanged; automatic deduction remains disabled.
- Download available on the website. Existing GitHub release assets are retained.

## 1.17.0 — 2026-10-18

- Own engine and component-management branding: EcoCoreMiner.
- Native tariff: 1.5%; managed external engines: 2% service fee.
- Shared fee policy for website, desktop previews, ERG invoices, gateway invoices and prepared managed-payout calculations.
- Exact integer/decimal arithmetic and updated payment consent policy.
- Existing invoice amounts remain unchanged; a pool payout cannot be invoiced twice.
- Public release repository and separate private development repository.
- GPU source and intermediate-code checks remain mandatory before publication.
- Existing profiles, wallets and history are preserved by the updater.

Automatic deduction and native pool mining are not enabled in this release. The production desktop still runs the selected external engine under its own name.

