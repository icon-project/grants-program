# SodaX - October 2026 Progress Update

## Intro
This progress report is for SodaX related development work by Venture23 Team.
The next phase of the project will focus on SodaX Phase 1 development and deployment. The report is from  1-Oct-2026 to 31-Oct-2026

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
Milestone 1 - SodaX Mainnet - Completed


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| TRON-RELAY — Tron Support (Hot-Wallet Signer + Listener) | Completed | Relay | https://github.com/icon-project/intent-relay/issues/466 |
| Relay Hub-Paused Guard (Relay Stops When Hub Is Paused) | Completed | Relay | https://github.com/icon-project/intent-relay/issues/496 |
| BTC Verifier — connSn On-Demand Derivation + Freshness Enforcement | Completed | Relay | https://github.com/icon-project/intent-relay/issues/504 |
| BTC Verifier — schnorr.verify Await Fix (RadFi Co-Signature) | Completed | Relay | https://github.com/icon-project/intent-relay/issues/497 |
| BTC MuSig Signer — Validate Every PSBT Output Before Signing | Completed | Relay | https://github.com/icon-project/intent-relay/issues/503 |
| BTC Verifier Update | Completed | Relay | https://github.com/icon-project/intent-relay/issues/419 |
| SUI Rate-Limits Package Pointer Hardening | Completed | Relay | https://github.com/icon-project/intent-relay/issues/498 |
| ICXSwap — Admin Approval Queue for ICX→SODA Migration | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/727 |
| Audit Fix — MMLiquidator Intent Deadline Bound (MML-M-1 Bypass) | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/750 |
| Audit Fix — ProtocolIntents Escrow Orphan + Unauthorized createIntentAutoSwap | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/749 |
| TRON-SOLVER — Coordinator, Executor & Liquidity Modules | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/908 |
| Cardano Solver Integration | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1140 |
| Project X (HyperEVM) — Concentrated-Liquidity Source | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/921 |
| Balancer V3 — Liquidity Source (Feeder + Curve + Executor) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/840 |
| Solver Dashboard Consolidation | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/882 |
| DEX Registry in Liquidity Curve (Track All Liquidity Feeders) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/814 |
| PRIME Routing — Drop Shortcut Machinery, BFS over Full Graph | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/644 |
| Solver Accounts for Relay Gas Fees | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/746 |
| Solana Feeder RPC Call Reduction | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/891 |
| Security Fixes — Dashboard Auth, OAuth XSS, Unsafe Agent Instructions | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1159 |
| STACKS Verifications | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/575 |
| EPIC: Partner-Ready Swap Provider API (Bitcoin.com Spec) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/740 |
| EPIC: Backend Roadmap — Partner API Keys, Shared-Mongo, DB Backups, In-House Analytics | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/862 |
| Partner Portal — Per-Org & Per-Key Volume + Intent Lifecycle | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1364 |
| Partner Analytics Dashboard (Overview, Swap Activity Log, Key Health) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1360 |
| Org-Scoped Partner Volume for Partner Portal | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1366 |
| Slack Alerts — Readable Triage Cards + Per-Channel On/Off Switches | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1421 |
| SODA Burn Tracking API & Stats Dashboard Tab | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/434 |
| intent_tokens Collection — Lazy ERC-20 Metadata for Intent-Touched Tokens | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/552 |
| Per-IP Rate Limiting on Public Endpoints | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1371 |
| Record Portal User Terms Acceptance | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1393 |
| Transformator Frontier Check — logIndex-Aware (Same-Block Completeness) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/661 |
| Dev Portal — Sign-In Page | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1975 |
| SODA Exchange — One-Way ICX Migration UI | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1911 |
| Case Studies — Full Epic (Modal, Categories, CMS, llms.txt, Content Optimisation) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1947 |
| SODAX Homepage — Hero Live Activity v1.2 + Built-With SODAX Slider | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1892 |
| SODAX Website — Mobile Contact Drawer | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1970 |
| Integration CTAs Pointing to Free API Key Portal | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2024 |
| Swaps API Terms Published at /terms | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2027 |
| Pre-Signature Preview Modal (Drainer Defence) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1632 |
| Email Provider Wallet Connectivity (SDK v2) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1069 |
| Agentic Skills (Open-Source Code-Based) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1585 |
| SDK Bump to 2.3.0-rc.2 | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/2020 |
| Security & Dependency Fixes (zod, uuid, undici, sanitize-html, OSV scanner) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1977 |
| Per-Asset Configurable Money Market Utilisation Alert Thresholds | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/182 |
| Pause-All-Spokes Feature | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/165 |
| MPC Alerts Integration | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/146 |
| Monitor Behind Pangolin (Auth Hardening) | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/166 |
| Fix Missing-SN OOM Kill (Unbounded Gap Enumeration) | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/180 |


## In Progress

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| TRON-FRONTEND — Tron Support in Frontend + SDK | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1500 |
| TRON-BACKEND — Tron Monitor, Indexer & Solver-Balance Tracking | In Progress | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/111 |
| XRP Integration — Solver (Executor, Liquidity Pools, MPC Relayer) | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1033 |
| 0G Chain — Intent Relay / MPC-Relay Support | In Progress | Relay | https://github.com/icon-project/intent-relay/issues/455 |
| 0G Chain — Backend Indexing & Data Support | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/716 |
| CCIP — Coordinator, Executor, Ops & Docs (Full Integration) | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/674 |
| Meteora (DLMM + DAMM v2) — Solana Liquidity Source | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/841 |
| Li.Fi — Liquidity / Bridge Adapter Integration | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/784 |
| In-House USD Analytics Data Pipeline | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/865 |
| SODAX Website — Full Redesign (Homepage, Developers, Assets, About) | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1916 |
| Wallet HW Support — Ledger + Trezor (EVM), Phase 1 | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1361 |
| apps/web Test Foundation + CI Test Gate | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1484 |


## Sample of docs
https://github.com/icon-project/sodax-frontend
