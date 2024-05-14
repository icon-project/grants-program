# Tracker Monthly Report

This is a progress update for 4/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month we cleared out the majority of the impending backlog on the frontend along with working on migrating servers off the cloud. The latter has been an enormous amount of work dealing with networking consultants to build a fault-tolerant networking setup. This is done now and servers are installed in their respective locations giving ping. Details are out of scope of this report. 

We also spent some time on query optimizations on the DB which after dealing with some issues have realized need to be looked at by a consultant. This will happen this month and unless it turns into a serious endeavor, will be handled internally under our budget. Long term we need to figure out what are sane rate limits and how to limit some expensive queries which seem to be choking up the DB. This is most appropriately done during migration though so holding off till then.

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [451](https://github.com/sudoblockio/icon-tracker-frontend/pull/451) | chore: target blockheight readded | closed | 2024-05-13T13:34:08Z | | 
| [448](https://github.com/sudoblockio/icon-tracker-frontend/pull/448) | chore: fixed empty contract events #447 | closed | 2024-05-10T10:37:34Z | | 
| [447](https://github.com/sudoblockio/icon-tracker-frontend/issues/447) | Contract Events is always empty | closed | 2024-05-10T10:36:41Z | | 
| [445](https://github.com/sudoblockio/icon-tracker-frontend/pull/445) | chore(main): release 0.5.2 | closed | 2024-04-24T19:01:37Z | | 
| [444](https://github.com/sudoblockio/icon-tracker-frontend/issues/444) | Change % of bond calculation | closed | 2024-04-17T10:53:21Z | | 
| [442](https://github.com/sudoblockio/icon-tracker-frontend/pull/442) | chore(main): release 0.5.1 | closed | 2024-04-05T21:25:54Z | | 
| [441](https://github.com/sudoblockio/icon-tracker-frontend/pull/441) | fix: tokens loading slowly, refactor #438 | closed | 2024-04-05T21:22:40Z | | 
| [440](https://github.com/sudoblockio/icon-tracker-frontend/pull/440) | chore: contract broken tabs #416 | closed | 2024-04-02T20:36:23Z | | 
| [439](https://github.com/sudoblockio/icon-tracker-frontend/pull/439) | Estimate step limit | closed | 2024-03-30T17:29:11Z | | 
| [438](https://github.com/sudoblockio/icon-tracker-frontend/issues/438) | Debug slow load times for tokens with addresses with many tokens  | closed | 2024-03-30T08:00:54Z | | 
| [436](https://github.com/sudoblockio/icon-tracker-frontend/issues/436) | Limit records in UI to a million | closed | 2024-03-29T19:25:26Z | | 
| [416](https://github.com/sudoblockio/icon-tracker-frontend/issues/416) | Tabs broken when used as link | closed | 2024-03-10T06:31:47Z | | 
| [373](https://github.com/sudoblockio/icon-tracker-frontend/issues/373) | Tools drop down  | closed | 2024-01-10T19:01:52Z | | 
| [361](https://github.com/sudoblockio/icon-tracker-frontend/issues/361) | Address tab not sorting on number of transactions  | closed | 2023-12-22T19:37:24Z | | 
| [356](https://github.com/sudoblockio/icon-tracker-frontend/issues/356) | Cleanup all queries with additional parameters  | closed | 2023-11-10T15:09:44Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | December Sprint | closed | 2023-11-01T08:00:51Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [452](https://github.com/sudoblockio/icon-tracker-frontend/pull/452) | fix: blockheight fix commit #451 | open | 2024-05-13T17:52:32Z | | 
| [450](https://github.com/sudoblockio/icon-tracker-frontend/issues/450) | Nested contract calls not showing properly  | open | 2024-05-12T17:59:43Z | | 
| [449](https://github.com/sudoblockio/icon-tracker-frontend/issues/449) | Make site title dynamic according to the page | open | 2024-05-12T05:25:13Z | | 
| [446](https://github.com/sudoblockio/icon-tracker-frontend/issues/446) | Scrub "P-Rep" from tracker and replace with "Validator" | open | 2024-05-03T18:56:31Z | | 
| [443](https://github.com/sudoblockio/icon-tracker-frontend/issues/443) | Estimated blockheight not shown in tracker while unstaking | open | 2024-04-13T13:17:57Z | | 
| [435](https://github.com/sudoblockio/icon-tracker-frontend/issues/435) | Provide icx value input in contract explorer | open | 2024-03-27T15:10:47Z | | 
| [426](https://github.com/sudoblockio/icon-tracker-frontend/issues/426) | New testing strategy | open | 2024-03-18T20:18:39Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | April Sprint  | open | 2024-03-10T07:03:17Z | | 
| [417](https://github.com/sudoblockio/icon-tracker-frontend/issues/417) | Change balance in address view to RPC call | open | 2024-03-10T06:41:26Z | | 
| [413](https://github.com/sudoblockio/icon-tracker-frontend/issues/413) | Get contract data showing for berlin   | open | 2024-03-05T17:29:13Z | | 
| [411](https://github.com/sudoblockio/icon-tracker-frontend/issues/411) | Display token balances for contracts | open | 2024-03-04T07:49:54Z | | 
| [403](https://github.com/sudoblockio/icon-tracker-frontend/issues/403) | Add `staking` feature   | open | 2024-02-18T22:51:08Z | | 
| [355](https://github.com/sudoblockio/icon-tracker-frontend/pull/355) | Add ability to set backend based on search parameters - #354 | open | 2023-11-02T08:56:15Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [77](https://github.com/sudoblockio/icon-transformer/issues/77) | Deadlock on cron  | open | 2024-05-05T02:23:12Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [45](https://github.com/sudoblockio/icon-go-api/issues/45) | Make queries stricter  | closed | 2023-11-10T15:09:33Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [43](https://github.com/sudoblockio/icon-governance/pull/43) | chore(main): release 0.8.1 | closed | 2024-03-24T15:06:23Z | |

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 4/23 | 2 min | Did not determine - focused on migration | Recovered | 

There is a major issue in one of the clusters that has been root caused and will be getting more attention during migration. Issue causes a deadlock on the transactions table in DB until processes are cleaned. We have brought in a consultant to debug and start some query optimizations which the bug came up during initially.  

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)