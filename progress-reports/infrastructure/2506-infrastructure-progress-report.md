# Tracker Monthly Report

This is a progress update for 5/2025 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month was very busy on the ops side as we figured out solutions to several bottlenecks which required redeploying every service we are running on our cluster. This included rolling several k8s clusters and every blockchain VM and at this time is almost finished. While the tracker itself doesn't need the newly gained performance, because of these changes we saw a decrease in memory usage of about 25% or 50gb which is helpful when we are running 4 copies of the tracker (prod/dev environments with backups). Most notably though this has allowed us to run the ICON nodes much more efficiently and of course every other chain we might run. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [566](https://github.com/sudoblockio/icon-tracker-frontend/pull/566) | fix: monthly inflation box overflow in Governance page #565 | closed | 2025-05-22T09:03:36Z | | 
| [563](https://github.com/sudoblockio/icon-tracker-frontend/pull/563) | feat: added total available voted amt in voting page #552 | closed | 2025-04-21T12:19:47Z | | 
| [562](https://github.com/sudoblockio/icon-tracker-frontend/pull/562) | chore(main): release 0.7.0 | closed | 2025-04-21T11:52:11Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [565](https://github.com/sudoblockio/icon-tracker-frontend/issues/565) | Governance page style | open | 2025-05-22T08:59:18Z | | 
| [564](https://github.com/sudoblockio/icon-tracker-frontend/issues/564) | Modify  | open | 2025-05-16T10:25:32Z | | 
| [524](https://github.com/sudoblockio/icon-tracker-frontend/issues/524) | Jan Sprint | open | 2025-01-20T12:11:35Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [60](https://github.com/sudoblockio/icon-governance/issues/60) | Update bond_percent formula | closed | 2025-02-01T19:34:34Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [62](https://github.com/sudoblockio/icon-governance/pull/62) | chore(main): release 0.10.7 | open | 2025-02-13T08:11:01Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [83](https://github.com/balancednetwork/balanced-backend/pull/83) | fix: add skip on wETH address which does not exist #82 | closed | 2025-05-09T10:04:52Z | | 
| [78](https://github.com/balancednetwork/balanced-backend/pull/78) | chore(main): release 0.8.4 | closed | 2024-11-21T09:16:44Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [84](https://github.com/balancednetwork/balanced-backend/issues/84) | getTotalCollateral missing at non-near head block heights for loans contract | open | 2025-05-18T10:28:26Z | | 
| [82](https://github.com/balancednetwork/balanced-backend/issues/82) | wETH has non-existant address | open | 2025-05-09T09:59:30Z | | 

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 5/14 | 11 min | Upstream issue with BGP | Ordered a second cross-connect and added redundant peer |
| 5/20 | No downtime but over 8 hours saw about 10% of requests failing | We forgot to remove 2 nodes from a LB pool which normally is ok for 1 node but 2 caused issues | Do the right config |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)