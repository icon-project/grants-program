# SodaX - June 2026 Progress Update

## Intro
This progress report is for SodaX related development work by Venture23 Team.
The next phase of the project will focus on SodaX Phase 1 development and deployment. The report is from  1-Jun-2026 to 30-Jun-2026

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
| Hedera Spoke Contract Deployment | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/653 |
| Hedera — NOL Rebalancer Chain/Bridge Routing | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/765 |
| Solana Token-2022 Fix (xSTOCK Bridging) | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/654 |
| Orca Pool Integration for Solana | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/654 |
| Kaia — Money Market Configuration | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/585 |
| Relay DLQ Integration for Late-Payload Chains (BTC, Solana) | Completed | Relay | https://github.com/icon-project/intent-relay/issues/462 |
| Asset-to-Asset Market Making Strategy (Research + Liquidity Module + Curve) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/698 |
| Near Intents — Executor/Wallet Separation & Gas Management | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/775 |
| CCTP Bridge Integration (Stellar Enablement) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/714 |
| BTC Solver — Dockerization | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/713 |
| Auto-Scaling for Solver Executors | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/773 |
| Coordinator Dashboard — Disable Entire DEX | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/916 |
| EPIC: Shared Stateful MongoDB Migration (Multi-Phase Cutover) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/826 |
| Shared Stateful Mongo — Native TLS + mTLS + Firewall Hardening | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/860 |
| EPIC: Operator-Safe Pending-Actions & Swap Recovery Observability | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/754 |
| Oracle Price OHLC Candles + Dashboard Charts | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/845 |
| EPIC: Internal Read-Only Ops & Control Dashboard | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/586 |
| Swaps V2 API | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/533 |
| Money Market Liquidation Observability | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/702 |
| SODAX Assets Page v1 (xStocks Visibility + RWA Filter) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1392 |
| SODAX Partners Page (Case Studies, Assets Panel) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1429 |
| SODAX Brand Kit Page v1 | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1371 |
| Articles Pages (/articles + /articles/[slug]) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1433 |
| B2B World — Design System & Homepage Design | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1441 |
| Agent Readiness 100/100 (llms.txt, x402, Markdown) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1443 |
| SN Recovery Optimisation & UI Updates | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/105 |
| BTC Auto-Recovery | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/101 |


## In Progress

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| TRON-RELAY — Tron Support (Hot-Wallet Signer + Listener) | In Progress | Relay | https://github.com/icon-project/intent-relay/issues/466 |
| TRON-SOLVER — Coordinator, Executor & Liquidity Modules for Tron | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/908 |
| TRON-FRONTEND — Tron Support in Frontend + SDK | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1500 |
| TRON-BACKEND — Tron Monitor, Indexer & Solver-Balance Tracking | In Progress | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/111 |
| Hedera — Wallet SDK / DAppKit Support | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1381 |
| CCIP — Coordinator/Quote Surface, Liquidity Feeder, Executor, Ops & Docs | On hold | Solver | https://github.com/icon-project/sodax-solver-v2/issues/674 |
| Solver Observability, Dashboard Consolidation & Alerting | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/882 |
| Li.Fi — Liquidity / Bridge Adapter Integration | In Progress | Solver | https://github.com/icon-project/sodax-solver-v2/issues/784 |
| EPIC: Partner-Ready Swap Provider API (Bitcoin.com Spec) | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/740 |
| Partner API Keys + Critical Endpoint Gating | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/864 |
| Automatic Backup + Manual Restore for Shared Stateful MongoDB | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/863 |
| In-House USD Analytics Data Pipeline | In Progress | Backend | https://github.com/icon-project/sodax-backend/issues/865 |
| B2B World — Homepage Build Approach & Design System | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1507 |
| Wallet HW Support — Ledger + Trezor (EVM), Phase 1 | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1361 |
| apps/web Test Foundation + CI Test Gate | In Progress | Frontend | https://github.com/icon-project/sodax-frontend/issues/1484 |


## Sample of docs
https://github.com/icon-project/sodax-frontend
