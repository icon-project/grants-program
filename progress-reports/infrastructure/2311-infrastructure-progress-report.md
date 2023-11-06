# Tracker Monthly Report

This is a progress update for 10/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month was saw the final release of the new frontend with ledger support (last month dev work was done - this month  was a few more issues that were included before pushing to the cluster), some work on rebuilding the backend (stats service along with general improvements), and starting on some major backend changes needed for increased stability, tools section, and other features. 

### [icon-tracker](https://github.com/sudoblockio/icon-tracker)

Working on making this one-click for interfacing with custom backend. Main issue is in the frontend which sets the backend based on the host it is running on (ie tracker.icon.community -> mainnet etc). There is currently no way to run a custom backend unless you build the tracker from source which is not an ideal way of operating it. It should generally be one-click and the whole stack potentially integrated into DIVE since that is where efforts to deply custom networks in the ecosystem have gone. Before that though, we'll be in charge of the docker-compose side (DIVE team / others can translate the docker-compose to starlark / kurtosis) which is blocked by [icon-tracker-frontend/issues/354](https://github.com/sudoblockio/icon-tracker-frontend/issues/354). As a summary, instead of having to build the frontend again with environment variables pointing to the backend, user should be able override the logic which sets the source based on location with either filling out a form or adding parameters to the path. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

New react version has been deployed and now going through backlog. Most things have been addressed and so priority now is on above issue (custom backends) and then looking at charts which the backend is being developed for right now. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [350](https://github.com/sudoblockio/icon-tracker-frontend/pull/350) | fix: change out ABI request from backend to RPC for contracts #346 | closed | 2023-10-22T17:17:04Z | | 
| [348](https://github.com/sudoblockio/icon-tracker-frontend/pull/348) | chore(main): release 0.3.3 | closed | 2023-10-21T10:10:32Z | | 
| [347](https://github.com/sudoblockio/icon-tracker-frontend/pull/347) | fix: events tab in token view and date in proposals #83 #302 | closed | 2023-10-21T07:40:05Z | | 
| [346](https://github.com/sudoblockio/icon-tracker-frontend/issues/346) | Change data source for getting contract ABI in `Contract` tab to rpc  | closed | 2023-10-19T13:20:40Z | | 
| [345](https://github.com/sudoblockio/icon-tracker-frontend/issues/345) | Validate governance statistics  | closed | 2023-10-16T02:50:02Z | | 
| [344](https://github.com/sudoblockio/icon-tracker-frontend/pull/344) | fixed #336 and implemented #304 | closed | 2023-10-13T12:06:49Z | | 
| [343](https://github.com/sudoblockio/icon-tracker-frontend/pull/343) | chore(main): release 0.3.2 | closed | 2023-10-12T10:27:20Z | | 
| [342](https://github.com/sudoblockio/icon-tracker-frontend/pull/342) | fix: Bring back rewards into governance view #341 and Make contracts that delegate linkable #334 | closed | 2023-10-12T07:54:25Z | | 
| [341](https://github.com/sudoblockio/icon-tracker-frontend/issues/341) | Bring back rewards into governance view  | closed | 2023-10-09T01:31:34Z | | 
| [339](https://github.com/sudoblockio/icon-tracker-frontend/pull/339) | chore(main): release 0.3.1 | closed | 2023-10-07T12:03:10Z | | 
| [338](https://github.com/sudoblockio/icon-tracker-frontend/pull/338) | fix: pagination button on tx list view | closed | 2023-10-07T12:01:02Z | | 
| [336](https://github.com/sudoblockio/icon-tracker-frontend/issues/336) | Proposal vote step limit | closed | 2023-10-06T02:14:03Z | | 
| [335](https://github.com/sudoblockio/icon-tracker-frontend/issues/335) | Bug-Pagination Issue | closed | 2023-10-05T06:30:25Z | |

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [354](https://github.com/sudoblockio/icon-tracker-frontend/issues/354) | Ability to modify backend sources | open | 2023-11-01T14:43:08Z | | 
| [353](https://github.com/sudoblockio/icon-tracker-frontend/issues/353) | Remove everything sejong related  | open | 2023-11-01T08:12:52Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | November Sprint | open | 2023-11-01T08:00:51Z | | 
| [351](https://github.com/sudoblockio/icon-tracker-frontend/issues/351) | Token sending tab in token / address view  | open | 2023-10-31T14:38:50Z | | 
| [349](https://github.com/sudoblockio/icon-tracker-frontend/issues/349) | Decode event logs based on ABI  | open | 2023-10-21T10:34:23Z | | 
| [340](https://github.com/sudoblockio/icon-tracker-frontend/issues/340) | Add feature to support an address book | open | 2023-10-08T11:20:42Z | | 
| [337](https://github.com/sudoblockio/icon-tracker-frontend/issues/337) | Exxpand e2e tests to include paging in tx list views | open | 2023-10-06T11:51:38Z | | 
| [305](https://github.com/sudoblockio/icon-tracker-frontend/issues/305) | New governance stat - Staking APY | open | 2023-08-09T02:12:07Z | | 
| [304](https://github.com/sudoblockio/icon-tracker-frontend/issues/304) | Adding functionality to apply network proposals | open | 2023-08-07T16:17:00Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | open | 2023-03-08T20:34:13Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

Started working on overhauling the cron scheduler with a proper framework. Will be done next month or month after. This is needed for building out stats within this service. Decision is still be considered which stats to put here or in other services such as the newly developed icon-stats service. 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

CSV outputs have been deployed for the tools section but likely be a 2024 goal after we migrate to a new API gateway which will allow rate limits. The tools section which outputs CSV will have ability to bulk output large record sets similar to etherscan (ie download 5k+ transactions in single query) which unless we have rate limiting in place will surely be abused and cause backend problems. New API Gateway development discussed below. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [40](https://github.com/sudoblockio/icon-go-api/pull/40) | chore(main): release 0.5.0 | closed | 2023-09-20T13:30:39Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [42](https://github.com/sudoblockio/icon-go-api/issues/42) | Duplicate in token-holders  | open | 2023-10-03T12:25:50Z | | 

### [icon-stats](https://github.com/sudoblockio/icon-stats)

Built a new service to give stats that will fuel the charts in the tracker. This got held up by many small bugs as we transition to the followin upgrades: 

1. Using all asyncio calls in both the backend (schedulers / client)
2. Upgrade pydantic 2.0 / sqlalchemy 2.0 using edge non-official edge releases
- Needed since all new work we are doing is based on pydantic 2.0 which is in the process of being upgraded across all dependencies so might as well use it while the edge version is available and working 
3. Upgrade associated DB clients to async (asyncpg vs psycopg2) along with migration tooling 
- Included being able to use custom schemas as current DB management is a major pain across multiple services 
- Future versions of the stack will expose configuration settings for DB allowing multiple DBs (hard), multiple schemas (easier - need to run one SQL setup script), or a single DB (will require a little more tooling but this is the easiest approach)

This was all a lot of work with many other smaller improvements coming along with. While in the short term this was probably a little too much effort to put into this one service, in the long term it will pay-off with better manageability as we look to migrate parts of the backend into a simpler / easier to manage monolithic application.  

### Infrastructure Updates 

We've started working on a major change to the infrastructure namely in replacing our current API Gateway (Ambassador) with a new one which will allow rate limiting, active health checking, and authentication. There is a lot of technical details here that are best left for an offline discussion but in general this will get us near feature parity with Alchemy. 

## Downtime Incidents

| Date  | Total Downtime | Cause                                            | Resolution                                      |
|-------|----------------|--------------------------------------------------|-------------------------------------------------|
| 10/29 | 10 min         | Loss of network connectivity from cloud provider | Restarted node which resolved issue immediately |

This incident is emblematic of working with this cloud provider. Hope is that after migration issues like this will no longer happen. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)