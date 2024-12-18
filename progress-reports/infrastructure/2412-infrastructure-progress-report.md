# Tracker Monthly Report

This is a progress update for 11/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month we saw a lot of activity on both the development side and infrastructure. On dev we worked through a major upgrade of the core packages that back all of our tooling including ORMs, webservers, and other core tooling. This caused changes across all of our repos but was needed as some incompatibilities were showing up. On the infrastructure side we finally completed the migration to bare metal and are now shutting off one of the cloud clusters. The other will remain on until new years after we do an upgrade to the nodes (add ram) and then the final migration will be complete.

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [512](https://github.com/sudoblockio/icon-tracker-frontend/pull/512) | chore: unregistered prep in voting | closed | 2024-12-03T11:52:49Z | | 
| [511](https://github.com/sudoblockio/icon-tracker-frontend/issues/511) | Allow unstaking from preps that have left the network - ie Rhizome | closed | 2024-12-03T11:15:13Z | | 
| [510](https://github.com/sudoblockio/icon-tracker-frontend/pull/510) | chore: WIP, added value field if payable | closed | 2024-12-03T07:12:56Z | | 
| [509](https://github.com/sudoblockio/icon-tracker-frontend/pull/509) | chore: udpate btp2 links and contract write []string bug fix #508 && … | closed | 2024-11-27T15:29:17Z | | 
| [508](https://github.com/sudoblockio/icon-tracker-frontend/issues/508) | update btp2 monitors links | closed | 2024-11-27T15:26:37Z | | 
| [506](https://github.com/sudoblockio/icon-tracker-frontend/pull/506) | chore(main): release 0.6.3 | closed | 2024-11-07T06:27:56Z | | 
| [499](https://github.com/sudoblockio/icon-tracker-frontend/issues/499) | Remove "Explorer (Coming)" and change "Stats (Coming)" to "Stats" with link | closed | 2024-09-23T06:28:58Z | | 
| [468](https://github.com/sudoblockio/icon-tracker-frontend/issues/468) | Redesign Code tab in contracts view | closed | 2024-07-03T15:29:16Z | | 
| [467](https://github.com/sudoblockio/icon-tracker-frontend/issues/467) | Updated json viewer for code section  | closed | 2024-07-03T15:27:57Z | | 
| [463](https://github.com/sudoblockio/icon-tracker-frontend/issues/463) | Review M2  | closed | 2024-07-03T14:44:11Z | | 
| [461](https://github.com/sudoblockio/icon-tracker-frontend/issues/461) | Pick base libraries for openapi docs  | closed | 2024-07-03T14:24:16Z | | 
| [458](https://github.com/sudoblockio/icon-tracker-frontend/issues/458) | Staking feedback turn #1  | closed | 2024-06-12T15:21:39Z | | 
| [457](https://github.com/sudoblockio/icon-tracker-frontend/issues/457) | Ability logout with wallet  | closed | 2024-06-12T15:12:38Z | | 
| [454](https://github.com/sudoblockio/icon-tracker-frontend/issues/454) | Update styling of wallet login  | closed | 2024-05-15T07:18:27Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | April Sprint  | closed | 2024-03-10T07:03:17Z | | 
| [417](https://github.com/sudoblockio/icon-tracker-frontend/issues/417) | Change balance in address view to RPC call | closed | 2024-03-10T06:41:26Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [507](https://github.com/sudoblockio/icon-tracker-frontend/issues/507) | Modify the the config to accept more backends  | open | 2024-11-20T06:12:20Z | | 
| [505](https://github.com/sudoblockio/icon-tracker-frontend/issues/505) | Estimate Fee breaking voting + bonding + others  | open | 2024-11-01T07:57:28Z | | 
| [502](https://github.com/sudoblockio/icon-tracker-frontend/issues/502) | Prioritized Backlog | open | 2024-10-06T09:40:07Z | | 
| [496](https://github.com/sudoblockio/icon-tracker-frontend/issues/496) | Empty event objects in contract event logs | open | 2024-09-19T09:28:19Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [54](https://github.com/sudoblockio/icon-go-api/pull/54) | chore(main): release 0.5.7 | closed | 2024-11-18T04:32:33Z | | 
| [53](https://github.com/sudoblockio/icon-go-api/pull/53) | fix: address doc string | closed | 2024-11-14T13:28:20Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [15](https://github.com/sudoblockio/icon-contracts/pull/15) | bump sqlmodel / pydantic / fastapi | closed | 2024-11-10T12:26:09Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [16](https://github.com/sudoblockio/icon-contracts/pull/16) | chore(main): release 0.2.6 | open | 2024-11-20T04:59:00Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [57](https://github.com/sudoblockio/icon-governance/pull/57) | Bump pydantic and fix concurrency issue | closed | 2024-11-28T13:07:47Z | | 
| [55](https://github.com/sudoblockio/icon-governance/pull/55) | bump sqlmodel / pydantic / fastapi | closed | 2024-11-09T07:52:42Z | | 
| [54](https://github.com/sudoblockio/icon-governance/pull/54) | bump sqlmodel / pydantic / fastapi | closed | 2024-11-09T07:36:11Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [56](https://github.com/sudoblockio/icon-governance/pull/56) | chore(main): release 0.10.6 | open | 2024-11-14T11:27:06Z | | 
| [53](https://github.com/sudoblockio/icon-governance/pull/53) | Bump pydantic | open | 2024-11-09T06:15:58Z | | 
| [52](https://github.com/sudoblockio/icon-governance/issues/52) | Update sqlmodel / pydantic / fastapi / sqlalchemy so that alembic does not create a diff  | open | 2024-11-08T07:07:12Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [77](https://github.com/balancednetwork/balanced-backend/pull/77) | chore(main): release 0.8.3 | closed | 2024-11-12T08:40:29Z | | 
| [76](https://github.com/balancednetwork/balanced-backend/pull/76) | chore(main): release 0.8.2 | closed | 2024-11-11T11:55:50Z | | 
| [75](https://github.com/balancednetwork/balanced-backend/pull/75) | chore(main): release 0.8.1 | closed | 2024-11-11T09:18:44Z | | 
| [74](https://github.com/balancednetwork/balanced-backend/issues/74) | Batch commits | closed | 2024-11-08T02:47:16Z | | 
| [67](https://github.com/balancednetwork/balanced-backend/pull/67) | chore(main): release 0.8.0 | closed | 2024-09-17T07:35:18Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [79](https://github.com/balancednetwork/balanced-backend/issues/79) | Fix XLM Token Symbol | open | 2024-11-26T04:52:17Z | | 
| [78](https://github.com/balancednetwork/balanced-backend/pull/78) | chore(main): release 0.8.4 | open | 2024-11-21T09:16:44Z | | 
| [73](https://github.com/balancednetwork/balanced-backend/issues/73) | Async RPC Calls | open | 2024-11-08T02:43:19Z | | 
| [72](https://github.com/balancednetwork/balanced-backend/issues/72) | Cache price graph | open | 2024-11-08T02:36:01Z | | 
| [71](https://github.com/balancednetwork/balanced-backend/issues/71) | Move time-series data to TimescaleDB | open | 2024-11-08T02:18:15Z | | 
| [61](https://github.com/balancednetwork/balanced-backend/issues/61) | Estimate for cross-chain collateral deposit breakdown | open | 2024-07-22T10:21:40Z | | 

### [icon-stats](https://github.com/sudoblockio/icon-stats)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [21](https://github.com/sudoblockio/icon-stats/pull/21) | updated sa_coloumn to only coloumn fixing failing api tests | closed | 2024-12-01T17:12:20Z | | 
| [17](https://github.com/sudoblockio/icon-stats/pull/17) | chore(main): release 0.2.6 | closed | 2024-11-18T04:33:11Z | | 
| [16](https://github.com/sudoblockio/icon-stats/pull/16) | fix: remove get merge openapi spec path | closed | 2024-11-14T13:35:33Z | | 
| [15](https://github.com/sudoblockio/icon-stats/pull/15) | bump sqlmodel / pydantic / fastapi | closed | 2024-11-10T14:14:34Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [20](https://github.com/sudoblockio/icon-stats/issues/20) | sqla update - Passing primary_key is not supported when also passing a sa_column | open | 2024-12-01T07:32:46Z | | 
| [19](https://github.com/sudoblockio/icon-stats/pull/19) | Bump pydantic | open | 2024-11-30T08:53:20Z | | 
| [18](https://github.com/sudoblockio/icon-stats/pull/18) | chore(main): release 0.2.7 | open | 2024-11-30T06:09:52Z | | 


## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 12/12 | 10 min | Operator error misconfiguring a load balancer | Fix the issue as soon as the alarm came in. |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)