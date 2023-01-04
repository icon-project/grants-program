# Tracker Monthly Report

This is a progress update for 01/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month saw a lot of work happening on all sides of the stack from several improvements to the frontend, backend, and movement towards a new version of the infrastructure deployment. 

Things of note:

- Added a couple features on the frontend along with bugs fixes (more details below).
- Had to rework some of the CI which failed in the middle of the month. That spawned a rotation of tokens and having to modify the github actions across a number of repos. 
- Got to the bottom of a couple bugs in the backend finally get some help on stack overflow after initially not getting any 
- Added a couple options needed to support features in the frontend like sorting of columns and others 
- Started working on a new infra deployment focusing first on improving the current logging setup. 
  - Work on this will continue over the coming months as we make efforts to drive down costs and increase reliability.
  - Hired contractor and getting him up to speed for assisting with this work. 
- While not directly related to tracker, did build [smart contract code generator POC](https://github.com/sudoblockio/tackle-icon-sc-poc)
- Created two projects for Devera Hackathon


### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

Some fixes were put in place for some regressions that occurred from pushes in Oct / Nov. A feature was put in place that allows for some tables such as contracts, addresses, and tokens to have some coloumns sortable. Before, the default sort on contract name, balance, and token name was the only option. Now you can sort on balance and number of transactions in multiple orders. Some other minor things were added such as including `method` in transaction tables. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [99](https://github.com/sudoblockio/icon-tracker-frontend/pull/99) | feat: added method column to contract tx table #88 | closed | 2022-12-29T23:27:06Z | | 
| [98](https://github.com/sudoblockio/icon-tracker-frontend/pull/98) | feat: added sorting and filterable columns to addresses, contract and tokens #46 | closed | 2022-12-29T23:12:18Z | | 
| [97](https://github.com/sudoblockio/icon-tracker-frontend/pull/97) | fix: address missing tabs chained api calls and tab onclick | closed | 2022-12-22T19:13:39Z | | 
| [96](https://github.com/sudoblockio/icon-tracker-frontend/pull/96) | feat: added method column in transactions table #88 | closed | 2022-12-20T18:53:58Z | | 
| [95](https://github.com/sudoblockio/icon-tracker-frontend/pull/95) | fix: token transfer details not showing up #92 | closed | 2022-12-14T09:56:26Z | | 
| [92](https://github.com/sudoblockio/icon-tracker-frontend/issues/92) | Token transfer details not show up in transaction anymore | closed | 2022-12-06T22:21:16Z | | 
| [91](https://github.com/sudoblockio/icon-tracker-frontend/issues/91) | Community is missing a lot of tabs for Prep wallets | closed | 2022-12-06T18:46:05Z | | 


#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [100](https://github.com/sudoblockio/icon-tracker-frontend/issues/100) | Move Method column  | open | 2022-12-30T15:30:40Z | | 
| [94](https://github.com/sudoblockio/icon-tracker-frontend/issues/94) | Remove multiple requests /address/{}  | open | 2022-12-07T17:16:22Z | | 
| [93](https://github.com/sudoblockio/icon-tracker-frontend/issues/93) | December sprint | open | 2022-12-07T12:12:37Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

Not mentioned in these issues were some fixes related to getting the right count for total contracts and others that was made apparent with implementing the sorting in the frontend feature. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [64](https://github.com/sudoblockio/icon-transformer/pull/64) | chore(main): release 0.3.1 | closed | 2022-12-20T19:34:22Z | | 
| [61](https://github.com/sudoblockio/icon-transformer/issues/61) | Update CI  | closed | 2022-12-09T21:58:24Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [62](https://github.com/sudoblockio/icon-transformer/issues/62) | Fix contract `status` which seems to be overwritten by transformer somewhere  | open | 2022-12-19T06:56:16Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [28](https://github.com/sudoblockio/icon-go-api/pull/28) | chore(main): release 0.4.1 | closed | 2022-12-20T15:06:54Z | | 
| [25](https://github.com/sudoblockio/icon-go-api/issues/25) | /transactions returning empty for method | closed | 2022-12-13T15:37:30Z | | 
| [24](https://github.com/sudoblockio/icon-go-api/pull/24) | chore(main): release 0.4.0 | closed | 2022-12-13T09:00:11Z | | 
| [23](https://github.com/sudoblockio/icon-go-api/pull/23) | Add sort to addresses/contracts #18 | closed | 2022-12-10T00:56:00Z | | 
| [21](https://github.com/sudoblockio/icon-go-api/issues/21) | Update CI | closed | 2022-12-09T21:58:09Z | | 
| [20](https://github.com/sudoblockio/icon-go-api/issues/20) | In /addresses api, '+' is not working in sort query params. | closed | 2022-12-08T17:47:05Z | | 
| [19](https://github.com/sudoblockio/icon-go-api/issues/19) | Addresses limit and sort exclusive  | closed | 2022-12-08T17:09:13Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [27](https://github.com/sudoblockio/icon-go-api/issues/27) | in /addresses api, negative sort (sort = -paramName) does not return the right data | open | 2022-12-16T18:59:41Z | | 
| [26](https://github.com/sudoblockio/icon-go-api/issues/26) | In /addresses/contracts API, 'status' query param not working  | open | 2022-12-14T16:24:09Z | | 
| [22](https://github.com/sudoblockio/icon-go-api/pull/22) | Add parameterized count to transactions #9 | open | 2022-12-10T00:45:33Z | | 

## Downtime Incidents

| Date       | Total Downtime | Cause                       | Resolution                                                                                                                |
|------------|----------------|-----------------------------|---------------------------------------------------------------------------------------------------------------------------|
| 6/12/2023 | 0 | Governance page was not updating | Restarted service. Never seen a worker silently fail like that and looking into way of alerting on this failure scenario. |  
| 27/12/2023 | 0              | Lost connection to API server | Got cloud provider to fix it. Not my doing.                                                                               |


> Report generated with [tackle](https://github.com/robcxyz/tackle-box)
