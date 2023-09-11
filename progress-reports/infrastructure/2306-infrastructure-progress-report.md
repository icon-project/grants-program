# Tracker Monthly Report

This is a progress update for 5/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month was largely occupied with dev ops tasks still preparing for the migration which is taking longer than anticipated. One cluster was down for roughly 10 days resulting in no downtime but was also the focus of attention for this period. Further details given in the Ops and Migration sections.

As part of the migration and contract code generator, issues with tackle have been identified and fixed. A new tackle release is being drafted with those fixes and other features needed to build a general purpose block extraction tool. This next version will be promoted with an article with uses cases in ICON, contract code generation, dev ops, report generation, etc, being highlighted.

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [258](https://github.com/sudoblockio/icon-tracker-frontend/pull/258) | chores: added 'expand' button on contract tab | closed | 2023-05-24T13:44:01Z | | 
| [257](https://github.com/sudoblockio/icon-tracker-frontend/pull/257) | update: added support for icxCall and sendTransaction methods on custom networks | closed | 2023-05-21T21:52:18Z | | 
| [256](https://github.com/sudoblockio/icon-tracker-frontend/pull/256) | multiple chores done | closed | 2023-05-19T23:44:44Z | | 
| [255](https://github.com/sudoblockio/icon-tracker-frontend/pull/255) | WIP: Contract explorer single page | closed | 2023-05-06T17:56:49Z | | 
| [251](https://github.com/sudoblockio/icon-tracker-frontend/issues/251) | Setup e2e with coverage in CI  | closed | 2023-04-23T19:26:19Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [262](https://github.com/sudoblockio/icon-tracker-frontend/issues/262) | On address and contract lists, the sort is reset when going back a page  | open | 2023-05-28T12:42:03Z | | 
| [261](https://github.com/sudoblockio/icon-tracker-frontend/issues/261) | Update prep functionalities with button css from contract tab  | open | 2023-05-24T18:32:37Z | | 
| [260](https://github.com/sudoblockio/icon-tracker-frontend/issues/260) | Change network on the bottom right when in a testnet  | open | 2023-05-24T18:12:39Z | | 
| [259](https://github.com/sudoblockio/icon-tracker-frontend/issues/259) | Add tool tip to proposal status  | open | 2023-05-24T15:30:18Z | | 
| [193](https://github.com/sudoblockio/icon-tracker-frontend/issues/193) | EPIC: Contract Write Meta  | open | 2023-03-08T12:19:25Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [75](https://github.com/sudoblockio/icon-transformer/pull/75) | chore(main): release 0.3.4 | closed | 2023-03-18T10:07:11Z | | 
| [65](https://github.com/sudoblockio/icon-transformer/issues/65) | Missing BTP contracts (internal) in tokens list | closed | 2023-01-20T13:58:47Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [37](https://github.com/sudoblockio/icon-go-api/pull/37) | chore(main): release 0.4.5 | closed | 2023-04-22T03:44:08Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [5](https://github.com/sudoblockio/icon-contracts/pull/5) | chore(main): release 0.2.0 | closed | 2023-01-13T09:27:02Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [13](https://github.com/sudoblockio/icon-governance/pull/13) | chore(main): release 0.3.1 | closed | 2023-04-26T11:06:49Z | | 
| [9](https://github.com/sudoblockio/icon-governance/issues/9) | Delegation under counting  | closed | 2023-03-18T09:27:04Z | | 
| [6](https://github.com/sudoblockio/icon-governance/issues/6) | Delegation out of sync with some addresses that have un-delegated  | closed | 2023-03-03T12:29:33Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [15](https://github.com/sudoblockio/icon-governance/issues/15) | Add historical penalties  | open | 2023-05-02T22:17:35Z | | 

### [icon-tracker](https://github.com/sudoblockio/icon-tracker)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [76](https://github.com/sudoblockio/icon-tracker/pull/76) | Fix the Governance link | closed | 2023-04-29T05:34:14Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [67](https://github.com/sudoblockio/icon-tracker/pull/67) | chore(main): release 1.0.0 | open | 2022-11-18T20:17:38Z | | 

### [tackle-icon-contract](https://github.com/sudoblockio/tackle-icon-contract)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [9](https://github.com/sudoblockio/tackle-icon-contract/issues/9) | Clarification on import  | open | 2023-05-17T15:19:00Z | | 

## Ops 

Last reporting cycle a downtime incident happened on lisbon for a day where the tracker was not syncing. The root cause of this instigated a number of deep looks into the cluster which culminated in needing to upgrade to the latest kubernetes version. Beyond just being good practice and recommended potential solution to the prior downtime, this was also going to prepare us for the migration since most applications prefer to be run on a version within the last year. 

The endpoints were prepared for a little expected downtime (ie running one cluster) and the upgrade started which ended up causing numerous mission critical services to fail. After talking with support and bringing in a consultant, the issue was understood to be on the application level. Fixes were identified which then helped address a downtime incident on the actual production cluster described below. This downtime was due to the same cause that initiated all this work in the first place. All clusters are now upgraded with the only major issue being disk space issue where some backup plans are being put in place in case the migration isn't ready to start by mid July. 

While fixing the issues above, the entire API gateway configuration was rebuilt which addressed some issues we were having with SSL and unstable API access. Instead of using both cloudflare and letsencrypt certs, we are only using cloudflare now which handles an issue we had with cert validation not working last month. This would have taken down the cluster if the in a couple weeks if it had not been handled. 

## Migration 

The migration as mentioned last month is harder than anticipated. Doing this setup right is in sudoblock's interest and thus we are bringing in a number of qualified consultants to assist that most of this next month's dev budget is being allocated to. It is important this is done right though and thus the utmost care is being given. 

Plan is to still reduce costs in the long term but we might start running a node on the new cloud soon and turning off nodes on the old cloud. Depending on negotiations for cloud costs, this could result in a minor increase for the first month which will be credited in subsequent months. Details will be shared for approval at the appropriate time.  

## Downtime Incidents

| Date | Total Downtime             | Cause                                                                                                                                         | Resolution                                                      |
|------|----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| 5/28 | 6 days on testnet trackers | The same issues which caused a cluster to go down for 10 days fixed this issue, albeit on a different cluster and resulting in real downtime. | Upgrading several operators and rolling numerous cluster certs. |

> Note: This was a major downtime incident that would have been alerted on if the exporter had not crashed. Nonetheless, we should have had a rule alerting us on that condition and not just relying on the data coming out of the exporter to trigger the alarm. Updates to the alerting rules have been put in place to get alarms on this in the future.  

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)