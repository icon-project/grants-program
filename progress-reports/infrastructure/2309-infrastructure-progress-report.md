# Tracker Monthly Report

This is a progress update for 8/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month's activities were focused on frontend and dev ops work. On the frontend we integrated ledger support which required upgrading to the newest create react app version 5.0. This was a major change and needed for long term sustainability of the frontend. We are waiting to merge that change along with other PRs / closing of issues which is reflected in the large number of open issues from this month. Lot of these issues are addresses but until the big update has happened, we're leaving them open as there will need to be a forced push to get the new changes in place. 

On the backend, we have been dealing with some issues with the cloud provider which per the notes on the bottom of the report are nearing resolution. We're also building a new health checking system which will prevent issues like this coming up in the future. Backend work has also started on a complete new design but it is too early to report on that. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [309](https://github.com/sudoblockio/icon-tracker-frontend/issues/309) | Transaction fails but logs says successful | closed | 2023-08-23T18:59:03Z | | 
| [307](https://github.com/sudoblockio/icon-tracker-frontend/pull/307) | Ledger integration | closed | 2023-08-18T19:30:32Z | | 
| [306](https://github.com/sudoblockio/icon-tracker-frontend/pull/306) | progress: refactoring to add support to ledger | closed | 2023-08-18T19:28:50Z | | 
| [303](https://github.com/sudoblockio/icon-tracker-frontend/issues/303) | Misleading Info on Network Proposal EndBlockHeight | closed | 2023-08-07T16:12:51Z | | 
| [298](https://github.com/sudoblockio/icon-tracker-frontend/pull/298) | Cra5 update | closed | 2023-07-31T11:59:17Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [312](https://github.com/sudoblockio/icon-tracker-frontend/issues/312) | Fix tests per the CRA 5 update  | open | 2023-08-29T05:00:17Z | | 
| [311](https://github.com/sudoblockio/icon-tracker-frontend/issues/311) | Paginate ledger addresses  | open | 2023-08-29T04:59:02Z | | 
| [310](https://github.com/sudoblockio/icon-tracker-frontend/pull/310) | Ledger integration complete | open | 2023-08-28T14:42:11Z | | 
| [308](https://github.com/sudoblockio/icon-tracker-frontend/pull/308) | Ledger integration  | open | 2023-08-18T19:34:07Z | | 
| [305](https://github.com/sudoblockio/icon-tracker-frontend/issues/305) | New governance stat - Staking APY | open | 2023-08-09T02:12:07Z | | 
| [304](https://github.com/sudoblockio/icon-tracker-frontend/issues/304) | Adding functionality to apply network proposals | open | 2023-08-07T16:17:00Z | | 
| [302](https://github.com/sudoblockio/icon-tracker-frontend/issues/302) | Date in proposals says UTC but it displays in local time  | open | 2023-08-07T16:08:43Z | | 
| [301](https://github.com/sudoblockio/icon-tracker-frontend/pull/301) | fix: "read contract" tab in tokens not working #284 and fix: In /token/<> there is no transactions tab #205 | open | 2023-08-03T18:28:40Z | | 
| [300](https://github.com/sudoblockio/icon-tracker-frontend/issues/300) | Tools section | open | 2023-08-03T15:21:14Z | | 
| [299](https://github.com/sudoblockio/icon-tracker-frontend/issues/299) | Tx trace logsfor failed txs doesn't work - no error msg | open | 2023-07-31T14:30:27Z | | 
| [282](https://github.com/sudoblockio/icon-tracker-frontend/issues/282) | July Sprint | open | 2023-07-01T09:06:19Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [18](https://github.com/sudoblockio/icon-governance/issues/18) | Add ICX per day calculation | closed | 2023-07-01T09:56:08Z | | 

## Downtime Incidents

We one downtime incident for two and a half hours this month on both testnets which had two root causes, one of them relating to the cloud provider which was then exacerbated by a configuration error. Without the configuration error, the outage would have only lasted 10 minutes but with that issue, the outage lasted longer. Configuration issue has since been resolved. The cloud provider issue on the other hand is systemic relating to a single node which had a long issue open for the past two months which I finally was able to convince them was on their side. They are now saying they need to replace a network cable and will resolve it soon. I'll be asking for credit for this node which if it is given will be reflected as a discount on next month's cloud bill. Last month's cloud spend was $500 less than previous months and is reflected in the invoice. 

Also it should be noted that the downtime incident didn't take down the trackers but delayed the indexing of blocks by up to 20 minutes. Blocks still get indexed but at a slower rate. Need to look into this more but suspecting it is from the load balancer now only having two nodes to load balance against. In the past when we had more less powerful nodes, losing a node didn't cause these types of issues. Now losing a node severly impacts the system. Working on a solution to load balance only on healthy nodes with a custom health checker, something equivalent to the reverse proxies used by Infura.  

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)