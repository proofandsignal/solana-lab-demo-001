# Solana Lab — DEMO-001 Visual Evidence Verifier

**Public test preview only · Not an independent audit · Source-visible proprietary / All Rights Reserved.**

This isolated demonstration runs entirely in the browser. It does not connect to wallets, RPC providers or transaction execution systems. No uploaded evidence files leave the browser.

## Technology tests

1. **Run bundled test** — reconstructs an 82-byte classic SPL USDC mint account from previously captured and reported fields and checks its SHA-256 against the archived digest. The reconstructed fixture is **not** an independent second RPC capture. Four archived JSON evidence files are **PENDING** until actually provided.
2. **Run tamper test** — intentionally flips a byte to demonstrate a SHA-256 FAIL; binary field mismatch should also fail.
3. **Import real files** — select `manifest.json` plus `account.data.bin`, `account.request.json`, `account.response.json`, `genesis.request.json`, `genesis.response.json`. Files with missing/incorrect hashes are marked PENDING/FAIL. Fields are decoded directly from the actual uploaded binary file.
4. **Download .txt report** — reports the live checks, rather than hard-coded audit claims.

The source manifest is editable; digest matching verifies local consistency only. No independent historical state validation, authenticated payment intent, reserve audit, legal opinion, or issuer-safety claim.

## GitHub Pages setup

The GitHub connector does not expose Pages administration. A repository admin should navigate to **Settings → Pages → Build and deployment**, select **Deploy from a branch**, branch **main**, folder **/(root)**, and save. Publishing is limited to this standalone demo repository; the main Solana Lab repositories remain under merge/deploy hold.

Before any customer-facing claims: browser QA → evidence QA → independent review → human approval.

© Proof & Signal. All Rights Reserved. Viewing publicly does not grant commercial redistribution, copying, modification, deployment, or production-use rights.
