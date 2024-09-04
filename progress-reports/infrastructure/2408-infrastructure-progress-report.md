# Tracker Monthly Report

This is a progress update for 7/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month was mainly working on infrastructure migrations. Details coming in following report. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [474](https://github.com/sudoblockio/icon-tracker-frontend/pull/474) | chore: prep update modal revert debugging code | closed | 2024-07-29T07:39:48Z | | 
| [473](https://github.com/sudoblockio/icon-tracker-frontend/pull/473) | UI polish | closed | 2024-07-29T07:21:03Z | | 
| [471](https://github.com/sudoblockio/icon-tracker-frontend/pull/471) | Event parser | closed | 2024-07-25T08:37:16Z | | 
| [470](https://github.com/sudoblockio/icon-tracker-frontend/pull/470) | Wallet tooling | closed | 2024-07-20T06:58:09Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [472](https://github.com/sudoblockio/icon-tracker-frontend/pull/472) | chore(main): release 0.6.0 | open | 2024-07-25T08:46:21Z | | 
| [469](https://github.com/sudoblockio/icon-tracker-frontend/issues/469) | Using sentry for frontend logs | open | 2024-07-16T19:14:12Z | | 
| [468](https://github.com/sudoblockio/icon-tracker-frontend/issues/468) | Redesign Code tab in contracts view | open | 2024-07-03T15:29:16Z | | 
| [467](https://github.com/sudoblockio/icon-tracker-frontend/issues/467) | Updated json viewer for code section  | open | 2024-07-03T15:27:57Z | | 
| [466](https://github.com/sudoblockio/icon-tracker-frontend/issues/466) | Sectioned ABI view  | open | 2024-07-03T15:25:34Z | | 
| [465](https://github.com/sudoblockio/icon-tracker-frontend/issues/465) | Change login flow + add options drop down  | open | 2024-07-03T15:17:43Z | | 
| [464](https://github.com/sudoblockio/icon-tracker-frontend/issues/464) | Clean up old testing cruft + make tests run  | open | 2024-07-03T14:55:29Z | | 
| [463](https://github.com/sudoblockio/icon-tracker-frontend/issues/463) | Review M2  | open | 2024-07-03T14:44:11Z | | 
| [462](https://github.com/sudoblockio/icon-tracker-frontend/issues/462) | Last page doesn't work in contract view | open | 2024-07-03T14:42:51Z | | 
| [461](https://github.com/sudoblockio/icon-tracker-frontend/issues/461) | Pick base libraries for openapi docs  | open | 2024-07-03T14:24:16Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

We dealt with some issues with migrations that we thought were causing some issues but ended up getting root caused to another issue with us running multiple transformers and there being a deadlock issue that caused some outages in one cluster before. That was resolved though and since then have not had any issues with the core transformer. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [78](https://github.com/sudoblockio/icon-transformer/pull/78) | fix: update protoc gorm | closed | 2024-06-28T03:45:05Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [79](https://github.com/sudoblockio/icon-transformer/pull/79) | Update Protoc Gorm Generation | open | 2024-07-15T05:22:06Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [45](https://github.com/sudoblockio/icon-governance/pull/45) | chore(main): release 0.9.0 | closed | 2024-07-31T15:08:41Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [44](https://github.com/sudoblockio/icon-governance/issues/44) | Add sort to preps endpoint | open | 2024-07-31T15:07:32Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [63](https://github.com/balancednetwork/balanced-backend/pull/63) | chore(main): release 0.6.4 | closed | 2024-07-22T21:53:11Z | | 
| [60](https://github.com/balancednetwork/balanced-backend/pull/60) | chore(main): release 0.6.3 | closed | 2024-07-19T00:16:52Z | | 
| [59](https://github.com/balancednetwork/balanced-backend/pull/59) | chore(main): release 0.6.2 | closed | 2024-07-04T00:35:41Z | | 
| [57](https://github.com/balancednetwork/balanced-backend/issues/57) | Sync the name of renamed USDC token contract | closed | 2024-07-01T09:55:04Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [62](https://github.com/balancednetwork/balanced-backend/issues/62) | Address with no transactions causing issues in backend  | open | 2024-07-22T21:51:28Z | | 
| [61](https://github.com/balancednetwork/balanced-backend/issues/61) | Estimate for cross-chain collateral deposit breakdown | open | 2024-07-22T10:21:40Z | | 
| [58](https://github.com/balancednetwork/balanced-backend/issues/58) | Confirm pool changes  | open | 2024-07-04T00:33:31Z | | 

## Downtime Incidents

None to report. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)
