# Tracker Monthly Report

This is a progress update for 11/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month saw work on all sides of the stack. Improvements to the governance service were put in to build the backend for stats pages. Some small fixes were put in on the frontend with many only surfacing from completing the one-click custom tracker including additional issues in the indexer and transformer. All is working with the local tracker though which is [passing tests in CI](https://github.com/sudoblockio/gochain-local-community/actions/runs/7112621095/job/19362911829).

In preparation for the move to bare metal, we have begun working on both the software side on the migration and procurement. On the SW side, we are working out details of our new API gateway which has passed initial validation. We built an auth layer tied to a user service. Next month we'll be working on setting up health checking. On the procurement side, we started purchasing the servers required and expect to be able to perform the install by roughly new years with clusters coming online within a couple months from then after testing. Selecting the right server configurations has been a significant amount of work trying to keep costs as low as possible.   

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [357](https://github.com/sudoblockio/icon-tracker-frontend/issues/357) | BUG - query parameters error | closed | 2023-11-20T12:58:34Z | | 
| [346](https://github.com/sudoblockio/icon-tracker-frontend/issues/346) | Change data source for getting contract ABI in `Contract` tab to rpc  | closed | 2023-10-19T13:20:40Z | | 
| [345](https://github.com/sudoblockio/icon-tracker-frontend/issues/345) | Validate governance statistics  | closed | 2023-10-16T02:50:02Z | | 
| [334](https://github.com/sudoblockio/icon-tracker-frontend/issues/334) | Make contracts that delegate linkable  | closed | 2023-09-30T06:58:54Z | | 
| [323](https://github.com/sudoblockio/icon-tracker-frontend/issues/323) | October Sprint | closed | 2023-09-17T09:02:23Z | | 
| [284](https://github.com/sudoblockio/icon-tracker-frontend/issues/284) | "Read Contract" tab in tokens not working  | closed | 2023-07-09T11:03:01Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [358](https://github.com/sudoblockio/icon-tracker-frontend/issues/358) | Feature Request : Integrate ONS to enhance the display of users’ addresses. | open | 2023-11-22T14:47:12Z | | 
| [356](https://github.com/sudoblockio/icon-tracker-frontend/issues/356) | Cleanup all queries with additional parameters  | open | 2023-11-10T15:09:44Z | | 
| [355](https://github.com/sudoblockio/icon-tracker-frontend/pull/355) | Add ability to set backend based on search parameters - #354 | open | 2023-11-02T08:56:15Z | | 
| [354](https://github.com/sudoblockio/icon-tracker-frontend/issues/354) | Ability to modify backend sources | open | 2023-11-01T14:43:08Z | | 
| [353](https://github.com/sudoblockio/icon-tracker-frontend/issues/353) | Remove everything sejong related  | open | 2023-11-01T08:12:52Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | November Sprint | open | 2023-11-01T08:00:51Z | | 
| [337](https://github.com/sudoblockio/icon-tracker-frontend/issues/337) | Expand e2e tests to include paging in tx list views | open | 2023-10-06T11:51:38Z | | 
| [305](https://github.com/sudoblockio/icon-tracker-frontend/issues/305) | New governance stat - Staking APY | open | 2023-08-09T02:12:07Z | | 
| [304](https://github.com/sudoblockio/icon-tracker-frontend/issues/304) | Adding functionality to apply network proposals | open | 2023-08-07T16:17:00Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [43](https://github.com/sudoblockio/icon-go-api/issues/43) | Coin gecko mkt cap call failing locally  | closed | 2023-11-10T11:21:43Z | | 
| [40](https://github.com/sudoblockio/icon-go-api/pull/40) | chore(main): release 0.5.0 | closed | 2023-09-20T13:30:39Z | | 
| [38](https://github.com/sudoblockio/icon-go-api/pull/38) | 🐛 Fix fluid typing issue with query parameters | closed | 2023-06-21T08:04:46Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [45](https://github.com/sudoblockio/icon-go-api/issues/45) | Make queries stricter  | open | 2023-11-10T15:09:33Z | | 
| [44](https://github.com/sudoblockio/icon-go-api/pull/44) | chore(main): release 0.5.1 | open | 2023-11-10T11:22:41Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [25](https://github.com/sudoblockio/icon-governance/issues/25) | Add APY over time | closed | 2023-11-06T08:18:09Z | | 
| [24](https://github.com/sudoblockio/icon-governance/pull/24) | chore(main): release 0.5.2 | closed | 2023-11-05T04:58:41Z | | 
| [23](https://github.com/sudoblockio/icon-governance/issues/23) | Some prep details failing - blocked by cloudflare   | closed | 2023-11-05T04:57:19Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [31](https://github.com/sudoblockio/icon-governance/issues/31) | apy time crashing in testnets  | open | 2023-12-08T13:00:48Z | | 
| [30](https://github.com/sudoblockio/icon-governance/issues/30) | Update CPS rpc calls  | open | 2023-11-15T16:54:30Z | | 
| [29](https://github.com/sudoblockio/icon-governance/issues/29) | Add bonders and stakers to preps  | open | 2023-11-15T13:20:21Z | | 
| [28](https://github.com/sudoblockio/icon-governance/pull/28) | chore(main): release 0.6.0 | open | 2023-11-06T08:23:15Z | | 
| [27](https://github.com/sudoblockio/icon-governance/issues/27) | Total delegators endpoint | open | 2023-11-06T08:20:51Z | | 
| [26](https://github.com/sudoblockio/icon-governance/issues/26) | Add current APY Endpoint? | open | 2023-11-06T08:18:59Z | |

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 11/29 | 5 min | Cluster had a node down which didn't disrupt service but when the maintenance was done on it which involved upgrading the k8s version, a misset DNS record caused about 5 min of downtime as it was wrongly assumed a safe to perform the maintenance. | Resolved itself. | 

The above incident generated a lot of complaints oddly. Three users who I assume were using the tracker at the time had to do a hard refresh to get it to work again. Very add as the total downtime as only about 5 minutes. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)