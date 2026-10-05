# SodaX - September 2026 Progress Update

## Intro
This progress report is for SodaX related development work by Venture23 Team.
The next phase of the project will focus on SodaX Phase 1 development and deployment. The report is from  1-Sep-2026 to 30-Sep-2026

## Summary
For more details please see : <br>

https://github.com/icon-project/intent-relay<br>
https://github.com/icon-project/sodax-contracts<br>
https://github.com/icon-project/sodax-frontend<br>
https://github.com/icon-project/sodax-solver-v2<br>
https://github.com/icon-project/sodax-backend<br>
https://github.com/icon-project/go-sodax-monitor-be<br>
https://github.com/icon-project/intent-contracts


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| Bounded Oracle Prices | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/713 |
| Whitelisted Executors | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/712 |
| FeeM Upgrades | Completed | Contracts | https://github.com/icon-project/sodax-contracts/issues/301 |
| TON Chain Integration — Solver | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1073 |
| Monad Chain Integration — Solver | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1071 |
| Zcash (ZEC) Chain Integration — Solver | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1072 |
| Velodrome / Aerodrome Slipstream CL on Optimism | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1095 |
| Cetus Aggregator API Integration | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1057 |
| Robinhood Chain — Tokenised Stocks, ETFs & Commodity ETPs as Liquidity Source | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1076 |
| Hedera & Stellar Stock Token Deployment | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1088 |
| EPIC: SODA Market Making Strategy (Research + Kraken Integration) | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1052 |
| New Token Support Expansion | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1063 |
| Quoting API — Distinct Error Codes per Quote Service Error | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1105 |
| Hops Limitation | Completed | Solver | https://github.com/icon-project/sodax-solver-v2/issues/1097 |
| API Keys per Registered Partner + Critical Endpoint Gating | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/864 |
| DEX Volumes + Intent Volumes Dashboard Pages | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1249 |
| GET /amm/volume — Windowed DEX Volume, KPIs & Per-Pool Series | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1248 |
| AMM Swap USD Pricing at Ingest | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1246 |
| Reproducible Shared USD Price Lookup (Oracle Tier Ladder) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1245 |
| Time-Ranged Partner Volume & Fee Metrics | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1177 |
| RadFi / Bound Backend HMAC Auth + Allowance Reset Tx | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1090 |
| Oracle Candle Catalog — Operator Curation via Dashboard | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1275 |
| Stocks Rate Limiters on All Chains | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1261 |
| Backfill Historical Oracle Price Candles for SODA | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1121 |
| WAF IP Rate-Limit Incident Fix (Relay Packet Fetch Blocked) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1283 |
| CORS Fix — x-api-key Header for Browser SDK Calls | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1212 |
| Leverage-Yield /approve — Return Reset Tx (USDT Holders Unblocked) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1276 |
| Data-Transformator Stability (Watermark Guard, AMM Candle Double-Count Fix) | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1168 |
| AMM USD Pricing — Bind to Token Address not ERC-20 Symbol | Completed | Backend | https://github.com/icon-project/sodax-backend/issues/1269 |
| Frontend Security Hardening (CSP, CMS Sanitizer, Rate Limits, Credential Revocation, CI Scanners) | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1836 |
| SODAX Homepage — Hero Intro Video + Live SodaxScan Activity | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1818 |
| SODAX Homepage — Hero API Badge, CTA Updates | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1736 |
| SODAX Website — Footer Redesign | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1765 |
| SODAX Website — Mobile Modals as Drawers | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1823 |
| Holders Page — Exchange Bar Driven from Notion | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1774 |
| SODAX Brand Page — Face Lift | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1873 |
| SDK Playground / Widget | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1651 |
| Swaps API Example Page in Demo App | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1570 |
| SDK Upgrade to 2.2.0-rc.6 | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1871 |
| SODAX Solana Page — Post-Giveaway Hero + Contact Modal | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1793 |
| Partner Portal Update | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1117 |
| Swap — Show $1 Minimum Instead of "Quote Unavailable" | Completed | Frontend | https://github.com/icon-project/sodax-frontend/issues/1869 |
| Spoke Auto-Pause Error Fixes | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/157 |
| SUI — Upgrade to gRPC | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/147 |
| Investigate & Verify SN Missed-Message Auto-Recovery (Sonic→Arbitrum Bridge) | Completed | Monitor | https://github.com/icon-project/go-sodax-monitor-be/issues/164 |


## Sample of docs
https://github.com/icon-project/sodax-frontend
