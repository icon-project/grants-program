# Tracker Monthly Report

This is a progress update for 3/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month we had our new frontend developer start and begin to clear out issues. He's not on full time but his primary task is clearing out the backlog and bringing improvements to some tooling related to the tracker and related resources. Besides some of the obvious cosmetic improvements (ie tools dropdown), there have been a number of issues related to the backend that need attention and will be the focus of this report. 

The backend was running relatively smoothly up until about 3 weeks ago when some interruptions started occurring resulting in some short downtime incidents summarized below. Inspecting logs revealed numerous nonsensical query strings which appeared to have malicious intent. The backend was scaled as this resulted in high memory usage and a long needed patch was put in place to automatically reject requests with these query params which improved the situation but still has not resolved the problem. We looked further into the backend and frankly, discussing DB indexing strategies are a little complicated / out of scope here but suffice to say there has been a lot of effort put in on this front which tie into long term strategies in how to effectively deliver this data over time. In the short term some additional indexes have been put in place that grew the memory footprint by ~50% on mainnet - still well within our current limits, but beginning to raise concerns. 

What is most concerning now though is we have a couple queries which frankly don't make sense to be returning sporadic 504s which after looking into the backend, are themselves expensive queries but always returning the result within the timeout window. For instance: 

https://tracker.icon.community/api/v1/transactions/address/cx622bbab73698f37dbef53955fd3decffeb0b0c16?&limit=100&skip=200

It is a little complicated to explain what is going on here but we implemented an optimization on the backend specifically for this query using common table expressions and it is optimized / should not timeout. But this is also one of the types of queries we seem to be getting hit with a lot of lately on addresses that don't exist and should not be linked in any way to an actual address on the chain. The address not existing is not overly taxing on the backend but what I am starting to think is that a firewall is being activated and filtering some of these requests before they even get to our servers. 

Long story short, this is an open issue along with uncovering what exactly the effects are on the backend with intentionally malformed queries as it is clearly having and adverse affect that needs to be dealt with. More information should be shared over a call but broadly this is what we are dealing with right now. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [437](https://github.com/sudoblockio/icon-tracker-frontend/pull/437) | chore:  limit records to 1mill in UI #436 | closed | 2024-03-29T19:49:03Z | | 
| [434](https://github.com/sudoblockio/icon-tracker-frontend/pull/434) | chore: pagination button broken in addr page #433 | closed | 2024-03-26T18:59:52Z | | 
| [433](https://github.com/sudoblockio/icon-tracker-frontend/issues/433) | Broken pagination button on address page  | closed | 2024-03-26T18:41:50Z | | 
| [431](https://github.com/sudoblockio/icon-tracker-frontend/pull/431) | chore: removed duplicate query params #429 | closed | 2024-03-22T20:00:24Z | | 
| [429](https://github.com/sudoblockio/icon-tracker-frontend/issues/429) | Remove extra query params round 2  | closed | 2024-03-22T07:34:19Z | | 
| [428](https://github.com/sudoblockio/icon-tracker-frontend/issues/428) | Tabs broken  | closed | 2024-03-20T04:11:34Z | | 
| [427](https://github.com/sudoblockio/icon-tracker-frontend/pull/427) | fix: removed debug alert #420 | closed | 2024-03-19T18:02:26Z | | 
| [425](https://github.com/sudoblockio/icon-tracker-frontend/issues/425) | Get all links for tools section  | closed | 2024-03-18T20:09:13Z | | 
| [424](https://github.com/sudoblockio/icon-tracker-frontend/pull/424) | chore(main): release 0.5.0 | closed | 2024-03-18T18:37:16Z | | 
| [423](https://github.com/sudoblockio/icon-tracker-frontend/pull/423) | fix: sort header click on common page (addresses) #361 | closed | 2024-03-14T10:18:37Z | | 
| [422](https://github.com/sudoblockio/icon-tracker-frontend/pull/422) | fix: fixed styles and added common classnames for governace page popups #408 | closed | 2024-03-13T15:41:10Z | | 
| [421](https://github.com/sudoblockio/icon-tracker-frontend/pull/421) | fix: extra query params removed #420 | closed | 2024-03-13T14:56:06Z | | 
| [420](https://github.com/sudoblockio/icon-tracker-frontend/issues/420) | Remove all extra query params from every rest call | closed | 2024-03-12T17:43:39Z | | 
| [419](https://github.com/sudoblockio/icon-tracker-frontend/pull/419) | feat: added token balance in contracts page #411 | closed | 2024-03-11T18:14:52Z | | 
| [415](https://github.com/sudoblockio/icon-tracker-frontend/pull/415) | Fix: #402 when unstaking, the target block height label is missplaced | closed | 2024-03-07T00:38:39Z | | 
| [414](https://github.com/sudoblockio/icon-tracker-frontend/issues/414) | Cache issue in lisbon | closed | 2024-03-05T17:29:41Z | | 
| [412](https://github.com/sudoblockio/icon-tracker-frontend/issues/412) | Paging broken on token transfers  | closed | 2024-03-04T17:57:56Z | | 
| [411](https://github.com/sudoblockio/icon-tracker-frontend/issues/411) | Display token balances for contracts | closed | 2024-03-04T07:49:54Z | | 
| [410](https://github.com/sudoblockio/icon-tracker-frontend/pull/410) | chore(main): release 0.4.8 | closed | 2024-03-03T05:57:34Z | | 
| [407](https://github.com/sudoblockio/icon-tracker-frontend/pull/407) | Add info popups to gov | closed | 2024-02-21T02:01:36Z | | 
| [402](https://github.com/sudoblockio/icon-tracker-frontend/issues/402) | fix position of unstaking information in the address page | closed | 2024-02-16T22:19:10Z | | 
| [389](https://github.com/sudoblockio/icon-tracker-frontend/pull/389) | feat: add initial tools drop down #373 | closed | 2024-01-29T05:59:56Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | December Sprint | closed | 2023-11-01T08:00:51Z | | 
| [237](https://github.com/sudoblockio/icon-tracker-frontend/pull/237) | Config refactor | closed | 2023-04-19T19:02:11Z | | 
| [233](https://github.com/sudoblockio/icon-tracker-frontend/pull/233) | fix: contract header cache #225 | closed | 2023-04-04T21:15:35Z | | 
| [217](https://github.com/sudoblockio/icon-tracker-frontend/pull/217) | fix: trace integration for all tx and view logs button #154 #64 | closed | 2023-03-19T07:47:19Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [439](https://github.com/sudoblockio/icon-tracker-frontend/pull/439) | Estimate step limit | open | 2024-03-30T17:29:11Z | | 
| [438](https://github.com/sudoblockio/icon-tracker-frontend/issues/438) | Debug slow load times for tokens with addresses with many tokens  | open | 2024-03-30T08:00:54Z | | 
| [436](https://github.com/sudoblockio/icon-tracker-frontend/issues/436) | Limit records in UI to a million | open | 2024-03-29T19:25:26Z | | 
| [435](https://github.com/sudoblockio/icon-tracker-frontend/issues/435) | Provide icx value input in contract explorer | open | 2024-03-27T15:10:47Z | | 
| [432](https://github.com/sudoblockio/icon-tracker-frontend/issues/432) | Create a generic error boundary page  | open | 2024-03-25T16:41:00Z | | 
| [430](https://github.com/sudoblockio/icon-tracker-frontend/pull/430) | chore: Info popup governance styling | open | 2024-03-22T18:52:07Z | | 
| [426](https://github.com/sudoblockio/icon-tracker-frontend/issues/426) | New testing strategy | open | 2024-03-18T20:18:39Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | March Sprint  | open | 2024-03-10T07:03:17Z | | 
| [417](https://github.com/sudoblockio/icon-tracker-frontend/issues/417) | Change balance in address view to RPC call | open | 2024-03-10T06:41:26Z | | 
| [416](https://github.com/sudoblockio/icon-tracker-frontend/issues/416) | Tabs broken when used as link | open | 2024-03-10T06:31:47Z | | 
| [413](https://github.com/sudoblockio/icon-tracker-frontend/issues/413) | Get contract data showing for berlin   | open | 2024-03-05T17:29:13Z | | 
| [409](https://github.com/sudoblockio/icon-tracker-frontend/issues/409) | Estimate step for contract calls on Tracker | open | 2024-02-26T11:34:39Z | | 
| [408](https://github.com/sudoblockio/icon-tracker-frontend/issues/408) | Add pop-ups to governance page  | open | 2024-02-21T02:04:25Z | | 
| [373](https://github.com/sudoblockio/icon-tracker-frontend/issues/373) | Tools drop down  | open | 2024-01-10T19:01:52Z | | 
| [361](https://github.com/sudoblockio/icon-tracker-frontend/issues/361) | Address tab not sorting on number of transactions  | open | 2023-12-22T19:37:24Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [47](https://github.com/sudoblockio/icon-go-api/pull/47) | chore(main): release 0.5.3 | closed | 2024-03-26T22:57:40Z | | 
| [46](https://github.com/sudoblockio/icon-go-api/pull/46) | chore(main): release 0.5.2 | closed | 2024-03-26T22:21:07Z | | 
| [44](https://github.com/sudoblockio/icon-go-api/pull/44) | chore(main): release 0.5.1 | closed | 2023-11-10T11:22:41Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [41](https://github.com/sudoblockio/icon-governance/pull/41) | chore(main): release 0.8.0 | closed | 2024-03-20T20:49:22Z | | 
| [40](https://github.com/sudoblockio/icon-governance/pull/40) | chore(main): release 0.7.6 | closed | 2024-03-10T08:41:14Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [43](https://github.com/sudoblockio/icon-governance/pull/43) | chore(main): release 0.8.1 | open | 2024-03-24T15:06:23Z | | 
| [42](https://github.com/sudoblockio/icon-governance/issues/42) | Update DB connection to fail | open | 2024-03-24T15:04:32Z | |

## Downtime Incidents

We had about 5 days of downtime on one cluster due to an error with the cloud. Long chain of issues until the issue on their side was resolved. Complained / demanded compensation which they seemed to have applied some credit for on but completely over dealing with them as the new solution is in place. Their quality of service has been unacceptable and looking forward to the new solution.  

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| March 7th | 15 | Operator error when doing migration | nothing | 
| March 11th | 15 | Backend crash due to influx of requests | Scale backend | 
| March 12th | 15 | Backend crash due to influx of requests | Scale backend | 
| March 28th | 15 | As soon as alarms went off and arriving at site no problem was seen. This has happened only a couple times in the past but everything is being disected now so chalking this up to the suspected firewall issue. | 


> Report generated with [tackle](https://github.com/robcxyz/tackle-box)
