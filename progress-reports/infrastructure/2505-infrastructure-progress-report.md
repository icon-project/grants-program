# Tracker Monthly Report

This is a progress update for 4/2025 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

On the frontend we started scoping out wallet connect and what we need to do on the frontend and in Hanna to support the protocol. On the backend, we're still doing migrations from last month + further optimizations needed to run many applications on the same system without so called noisy neighbor issues where adjacent workloads could interfere with others. Finally after working through this we can say we are working with all the available knobs to tune our systems and get the most performance - something that has been a long learning experience. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [561](https://github.com/sudoblockio/icon-tracker-frontend/pull/561) | fix: added apr column in voting page #560 | closed | 2025-04-19T11:35:50Z | | 
| [560](https://github.com/sudoblockio/icon-tracker-frontend/issues/560) | APR in voting page | closed | 2025-04-19T11:35:01Z | | 
| [556](https://github.com/sudoblockio/icon-tracker-frontend/pull/556) | chore: added logging for Sentry ErrorBoundary | closed | 2025-02-18T15:08:06Z | | 
| [544](https://github.com/sudoblockio/icon-tracker-frontend/issues/544) | When staking in the tracker you need to leave a small amount for the Tx fee | closed | 2025-02-06T18:30:28Z | | 
| [541](https://github.com/sudoblockio/icon-tracker-frontend/issues/541) | Show APR/APY values for validators | closed | 2025-02-05T13:57:39Z | | 
| [525](https://github.com/sudoblockio/icon-tracker-frontend/issues/525) | Validate that the new global bond rate value is reflected in the governance page | closed | 2025-01-20T13:18:08Z | | 
| [513](https://github.com/sudoblockio/icon-tracker-frontend/issues/513) | Display projected voter APR on tracker | closed | 2024-12-09T14:35:28Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [563](https://github.com/sudoblockio/icon-tracker-frontend/pull/563) | feat: added total available voted amt in voting page #552 | open | 2025-04-21T12:19:47Z | | 
| [562](https://github.com/sudoblockio/icon-tracker-frontend/pull/562) | chore(main): release 0.6.8 | open | 2025-04-21T11:52:11Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [60](https://github.com/sudoblockio/icon-governance/issues/60) | Update bond_percent formula | open | 2025-02-01T19:34:34Z | |

### Infrastructure

- Still working on migration figuring out new way to operate nodes to get another ~30% performance 
  - Each VM running all the applications is currently being migrated again 
- After this will need one last migration potentially at the end of the year to upgrade some components but that should be it 
- As a result of these migrations we believe we have de-bottlenecked everything we can allowing us to run roughly 2 times more workloads and push at least 5 times as many requests per second as before the optimizations 

## Downtime Incidents

| Date | Total DoCrash in wntime | Cause | Resolution |
| --- | --- | --- | --- |
| 4/29 | ~5-10 minutes | Kernel crash on node running many VMs | Understood original issue better - came up during some maintentance / migration - Fixed procedure so issue won't happen again. |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)