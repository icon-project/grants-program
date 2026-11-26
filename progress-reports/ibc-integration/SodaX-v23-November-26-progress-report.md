# SodaX - November 2026 Progress Update

## Intro
This progress report is for SodaX related development work by Venture23 Team.
The next phase of the project will focus on SodaX Phase 1 development and deployment. The report is from  1-Nov-2026 to 30-Nov-2026

## Summary
For more details please see : <br>

https://github.com/icon-project/intent-relay<br>
https://github.com/icon-project/sodax-contracts<br>
https://github.com/icon-project/sodax-frontend<br>
https://github.com/icon-project/sodax-solver-v2<br>
https://github.com/icon-project/sodax-backend<br>
https://github.com/icon-project/go-sodax-monitor-be<br>
https://github.com/icon-project/intent-contracts

## Milestones
Milestone 1 - SodaX Mainnet - Phase1 - TBD


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| Executor Destination Allowlist (Delivery Signing Guard) | Completed | Relay | https://github.com/icon-project/intent-relay/issues/502 |
| NEAR Connection — bind recv_message to Signed Destination | Completed | Relay | https://github.com/icon-project/intent-relay/issues/501 |
| LI.FI Filler Contract (Enclave-Signed Fills via Gas Wallet) | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/730 |
| LI.FI Vault Order Guard | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/765 |
| SignerRegistry — Rotate Enclave Signer Across All EVM Chains | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/738 |
| NEAR Asset Manager — Accept Deposits from NEAR Intents (intents.near) | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/736 |
| MarketMakingStrategy — Gas-Wallet Relayed + Signer-Authorised Ops | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/728 |
| ICXSwap Redirect + BalnSwap Lock Transfer for Compromised Recipients | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/754 |
| Robinhood Stocks & ETFs as Money Market Supply Assets (All Spoke Chains) | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/758 |
| Stellar Hooks Improvements | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/707 |
| Meteora (DLMM + DAMM v2) — Solana Liquidity Source | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/841 |
| Li.Fi — Liquidity / Bridge Adapter Integration | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/784 |
| Ramses (HyperEVM) — Concentrated-Liquidity Source | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/922 |
| Camelot V3 (Algebra Integral) on Arbitrum | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1062 |
| PancakeSwap V3 on Solana — Second Solana CLMM Source | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1005 |
| SUI AMM Integrations | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/301 |
| Asset-to-Asset Swap Filler (Executor — Borrow + Holdings) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/697 |
| Robinhood Chain — Next Wave Tokenised Stocks as Liquidity Source | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1103 |
| ANT (Anthropic Token on Robinhood) Added as Swappable Asset | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1234 |
| New Token Support — Round 2 | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1127 |
| Unified Logging — Solver Producer (NATS Structured Events) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1181 |
| Orderbook /execute — Process All Intents in a Multi-Intent Tx | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1215 |
| 0G Chain — Backend Indexing & Data Support | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/716 |
| EPIC: Partner Portal Admin View + Org Plans (Staff Access, Plan Tiers, Invite Links, Expiry Emails) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1442 |
| EPIC: Observability Section in Backend Dashboard (Grafana — Log Pulse, Error Explorer, Edge Health) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1538 |
| Unified Logging Infrastructure (OTel Collector + ClickHouse + Grafana) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1397 |
| Unified Logging — Backend Producer (OTLP Transport) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1401 |
| Per-Org Tier Rate Limits at HAProxy (Synced from API-Auth Keyset) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1372 |
| Swaps from and to MPC-Relay Chains | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1471 |
| Stellar Sponsored-Account Support (Sign Endpoint + Revoke Sweep) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/983 |
| EPIC: Fake Swap Submission Hardening (Spam Probing of submit-tx) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1519 |
| Swaps API — Self-Clearing Triage (Auto-Address Provable On-Chain Outcomes) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1161 |
| Swaps API — Junk EVM & Stellar Submit-Tx Row Auto-Clear | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1586 |
| Swaps API — Strict txHash Validation for Tron, XRP, TON, ZCash, Cardano | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1592 |
| Backend as Sole Oracle Consumer (Cache + Shield Non-Production Solver) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/874 |
| USD-Stamp Protocol Revenue at Ingest (P0.1) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1507 |
| Partner Portal Widget — Apply Partner Fee from API Key | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1384 |
| Widget Partner Fee via appId + Locked Widget Tier | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1489 |
| Stateful API Hardening (Signature in Responses, CORS, Swagger, 500 on Bad Input) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1482 |
| NEAR Contract State Balance Alert (80% Threshold) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1374 |
| Oracle Candle Tracked-Asset Manage & One-Click Add | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/846 |
| Portal Database Consolidation (Three DBs → One) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1504 |
| SODAX Website — Developers Page (Design + Build + Animated Infographics) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2131 |
| SODAX Website — Plans Page (Wireframe + Build) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2083 |
| SODAX Website — New Footer & Navbar (SODA Token Moved to Footer) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2138 |
| Developer Portal — Onboarding Flow (Terms, Privacy, Sign-Up Steps) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1989 |
| Site Search — Cmd+K Command Menu | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2051 |
| SDK, API & MCP Partner Pages | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2210 |
| Case Studies — Replace SDK Module Cards with SODAX API Callout | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2130 |
| SODAX Homepage — API Fit Infographic | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2212 |
| SODAX Homepage — Hero Partner Strip + Activity Logos & Stocks | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2200 |
| SODA Exchange — xSODA Move from Wallet to Staking (Sonic) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2066 |
| Frontend Security Audit — All 22 Findings Resolved (2026-08 Audit) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1861 |
| Whole-Repo Security Audit — 5 Medium Findings Closed (2026-07 Audit) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1621 |
| SDK Bump to 2.3.0-rc.4 | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2213 |
| Alert Organising & Drill-Down Discovery | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/179 |


## In Progress

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| TRON-FRONTEND — Tron Support in Frontend + SDK | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1500 |
| TRON-BACKEND — Tron Monitor, Indexer & Solver-Balance Tracking | In Progress | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/111 |
| XRP Integration — Solver (Executor, Liquidity Pools, MPC Relayer) | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1033 |
| 0G Chain — Intent Relay / MPC-Relay Support | In Progress | Relay | https://github.com/icon-project/intent-relay/issues/455 |
| CCIP — Coordinator, Executor, Ops & Docs (Full Integration) | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/674 |
| In-House USD Analytics Data Pipeline | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/865 |
| SODAX Website — Full Redesign (Homepage, Assets, About) | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1916 |
| Dev Portal — Dashboard Design & Build | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/2187 |
| Wallet HW Support — Ledger + Trezor (EVM), Phase 1 | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1361 |
| apps/web Test Foundation + CI Test Gate | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1484 |


## Sample of docs
https://github.com/icon-project/sodax-frontend
