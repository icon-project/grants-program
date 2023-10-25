# Tracker Monthly Report

This is a progress update for 9/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month saw the final release of the upgrading of the react version along with the ability to support ledger to sign transactions along. The upgrading of react version, while required to support ledger, was a ticking time bomb on the tracker and needed to get done as prior versions were more frequently facing build errors from outdated dependencies and thus sets us up well to maintain the tracker into the future. We also cleared out a number of bugs particularly in the token view page. In the upgrade, we found many bugs with the newly built e2e tests which additionally needed maintenance but proved their worth. 

On the backend, we added the ability to export data in csv format but have some issues worth discussing to fully be able to support the tools section as mention in [#330](https://github.com/sudoblockio/icon-tracker-frontend/issues/300) but the API related development has been completed. For stats related to [321](https://github.com/sudoblockio/icon-tracker-frontend/issues/321), discussions have started with frontend developers to do this. For the backend, a new solution will need to be built to get it into a production which we will be begin discussions soon. 

We also faced a really bad situation with the cloud provider which is summarized in the infrastructure section with a longer term resolution still being discussed with our representative. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [333](https://github.com/sudoblockio/icon-tracker-frontend/pull/333) | chore: fixed #330 and #331 | closed | 2023-09-30T05:37:43Z | | 
| [332](https://github.com/sudoblockio/icon-tracker-frontend/pull/332) | Chore: fixed #327 | closed | 2023-09-29T15:51:27Z | | 
| [331](https://github.com/sudoblockio/icon-tracker-frontend/issues/331) | Remove `Token Transfers` tab from /contract/cx... view  | closed | 2023-09-29T02:18:01Z | | 
| [330](https://github.com/sudoblockio/icon-tracker-frontend/issues/330) | Contract tab in token view not showing  | closed | 2023-09-26T11:51:15Z | | 
| [329](https://github.com/sudoblockio/icon-tracker-frontend/pull/329) | chore: e2e Test cases fails for view list count scenarios #315 | closed | 2023-09-22T12:16:40Z | | 
| [328](https://github.com/sudoblockio/icon-tracker-frontend/issues/328) | Missing 25 option from pagination selector in drop down  | closed | 2023-09-20T01:26:49Z | | 
| [327](https://github.com/sudoblockio/icon-tracker-frontend/issues/327) | Transactions tab the same as token transfers tab in token detail view  | closed | 2023-09-20T01:24:47Z | | 
| [326](https://github.com/sudoblockio/icon-tracker-frontend/issues/326) | Pagination broken for contracts and tokens list view | closed | 2023-09-20T01:23:02Z | | 
| [325](https://github.com/sudoblockio/icon-tracker-frontend/pull/325) | Cra5 update | closed | 2023-09-20T01:06:23Z | | 
| [324](https://github.com/sudoblockio/icon-tracker-frontend/pull/324) | fix: e2e Test cases fails for view list count scenarios #315 | closed | 2023-09-19T12:18:31Z | | 
| [320](https://github.com/sudoblockio/icon-tracker-frontend/pull/320) | chore: add test cases for token view contract tab | closed | 2023-09-15T09:34:17Z | | 
| [319](https://github.com/sudoblockio/icon-tracker-frontend/issues/319) | Token list contract tab doesn't show any data | closed | 2023-09-15T08:38:46Z | | 
| [317](https://github.com/sudoblockio/icon-tracker-frontend/issues/317) | Update e2e tests on /token/ view  | closed | 2023-09-14T20:41:24Z | | 
| [316](https://github.com/sudoblockio/icon-tracker-frontend/pull/316) | fix: Replace "Read Contract" tab in /token/* view with "Contract" #314 | closed | 2023-09-14T20:25:05Z | | 
| [315](https://github.com/sudoblockio/icon-tracker-frontend/issues/315) | e2e Test cases fails for view list count scenarios | closed | 2023-09-14T05:36:58Z | | 
| [314](https://github.com/sudoblockio/icon-tracker-frontend/issues/314) | Replace "Read Contract" tab in /token/* view with "Contract" | closed | 2023-09-13T15:20:33Z | | 
| [313](https://github.com/sudoblockio/icon-tracker-frontend/pull/313) | Test v2 | closed | 2023-09-06T07:34:07Z | | 
| [312](https://github.com/sudoblockio/icon-tracker-frontend/issues/312) | Fix tests per the CRA 5 update  | closed | 2023-08-29T05:00:17Z | | 
| [310](https://github.com/sudoblockio/icon-tracker-frontend/pull/310) | Ledger integration complete | closed | 2023-08-28T14:42:11Z | | 
| [308](https://github.com/sudoblockio/icon-tracker-frontend/pull/308) | Ledger integration  | closed | 2023-08-18T19:34:07Z | | 
| [301](https://github.com/sudoblockio/icon-tracker-frontend/pull/301) | fix: "read contract" tab in tokens not working #284 and fix: In /token/<> there is no transactions tab #205 | closed | 2023-08-03T18:28:40Z | | 
| [299](https://github.com/sudoblockio/icon-tracker-frontend/issues/299) | Tx trace logsfor failed txs doesn't work - no error msg | closed | 2023-07-31T14:30:27Z | | 
| [297](https://github.com/sudoblockio/icon-tracker-frontend/pull/297) | chore(main): release 0.3.0 | closed | 2023-07-27T16:29:13Z | |
| [312](https://github.com/sudoblockio/icon-tracker-frontend/issues/312) | Fix tests per the CRA 5 update  | closed | 2023-08-29T05:00:17Z | | 
| [138](https://github.com/sudoblockio/icon-tracker-frontend/issues/138) | Update react version  | closed | 2023-01-20T14:06:01Z | | 
| [104](https://github.com/sudoblockio/icon-tracker-frontend/issues/104) | Update CI to include version update on release  | closed | 2023-01-04T14:11:29Z | | 


### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

CSV feature missed in code gen but is [here](https://github.com/sudoblockio/icon-go-api/issues/39). Respond to header but right now we have a hard limit on 100 entries in the API. This is due to limitations on the DB which  struggles for being hit with lots of large requests. In etherscan, exports of 5k records are supported so we have some options that interract with timelines that should be discussed offline. 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [42](https://github.com/sudoblockio/icon-go-api/issues/42) | Duplicate in token-holders  | open | 2023-10-03T12:25:50Z | | 


## Downtime Incidents

No material downtime incidents to report this month though we did have issues with a cluster that was down for multiple days. It was outside of the load balancer at the time due to an issue dealt with just prior to the downtime from last month. When the issue was seen, it was immediately raised with support who after 20 interactions / 3 days finally restored the cluster since the issue was entirely on their end. Have meeting planned with cloud provider where I will fully explain the unacceptable nature of their response. The issue before that originally had the cluster outside of the load balancer was raised and resulted in a little over $100 in credit that is reflected in the invoice. The last incident described that did not result in actual downtime we'll again be pushing for credit. Further discussions will happen to make sure that we can get better support and avert this in the future. 

This, to put it mildly, was a struggle but I think we need to chalk it up to the cost of doing business with a lower tier cloud provider. This is the sort of stuff you are going to get but how we're also able to get considerable savings compared to the likes of AWS. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)