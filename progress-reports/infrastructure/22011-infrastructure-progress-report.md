## Intro

This is a progress update for 10/2022 and part of 9/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

After rebuilding the backend, the past month was mostly focused on deploying this new backend, dealing with QC issues, and small bug fixes that had been put off since before the new backend was built. The new backend is able to sync ~100x faster than the old one on full syncs along with being able to sync individual attributes, something not possible with the old one, which realized a >500x improvement depending on how rich the attribute is. The importance of this performance increase cannot be overstated as it makes implementing improvements orders of magnitude easier along with recovery operations feasible in the worst case scenario that a cluster is lost. Many bugs were introduced with this new backend though that were very difficult to diagnose and solve originating from using multi-threading and batching. These issues have been dealt with and the backend is now passing all the QC checks. Many bugs were put off to be handled with the new backend including indexing contracts that are created within contracts and other frontend issues. 

## Repos 

### icon-tracker-frontend

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [74](https://github.com/sudoblockio/icon-tracker-frontend/issues/74) | "btp-0x61.bsc-BNB" token name displayed as "undefined" on lisbon tracker | closed | 2022-10-20T19:15:54Z | | 
| [66](https://github.com/sudoblockio/icon-tracker-frontend/issues/66) | Community Tracker does not display Token Symbols | closed | 2022-08-23T18:57:26Z | | 
| [51](https://github.com/sudoblockio/icon-tracker-frontend/issues/51) | Fix bonded list  | closed | 2022-07-21T00:36:16Z | | 
| [50](https://github.com/sudoblockio/icon-tracker-frontend/issues/50) | Fix bonders list  | closed | 2022-07-20T19:17:01Z | | 
| [49](https://github.com/sudoblockio/icon-tracker-frontend/issues/49) | Formatting ICX amount in address page  | closed | 2022-07-20T18:26:07Z | | 
| [44](https://github.com/sudoblockio/icon-tracker-frontend/issues/44) | Fix pagination in `Tokens` and `Contracts` pages | closed | 2022-07-14T05:44:55Z | | 
| [25](https://github.com/sudoblockio/icon-tracker-frontend/issues/25) | Add contract type to tokens page  | closed | 2022-06-30T06:35:10Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [75](https://github.com/sudoblockio/icon-tracker-frontend/issues/75) | Fix contract verification  | open | 2022-10-25T13:54:58Z | Slated for upcoming month. | 
| [73](https://github.com/sudoblockio/icon-tracker-frontend/issues/73) | Fix token holders list view  | open | 2022-10-18T04:21:43Z | This is fixed and waiting for a merge. | 
| [72](https://github.com/sudoblockio/icon-tracker-frontend/issues/72) | Update the Read Contract section  | open | 2022-10-18T04:20:41Z | This is from an edge case of contracts created by contracts where the contract only has internal Txs. Will be updating backend service shortly to index these rare contracts. | 
| [70](https://github.com/sudoblockio/icon-tracker-frontend/issues/70) | Reduce number of getTotalSupply calls in token holders list view and Addresses list  | open | 2022-10-18T04:10:56Z | This is fixed and waiting for a merge. | 
| [69](https://github.com/sudoblockio/icon-tracker-frontend/issues/69) | Fix decimals for non-e18 tokens  | open | 2022-10-04T12:32:32Z | This is fixed and waiting for a merge. | 
| [68](https://github.com/sudoblockio/icon-tracker-frontend/issues/68) | Fix pagination for events  | open | 2022-09-22T13:09:28Z | This is fixed and waiting for a merge. | 
| [67](https://github.com/sudoblockio/icon-tracker-frontend/issues/67) | Ranking information unavailable beyond top 25 for IRC-2 tokens other than ICX | open | 2022-09-14T00:29:49Z | This should be fixed very soon (days). | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [56](https://github.com/sudoblockio/icon-transformer/issues/56) | Some token transfers missing | closed | 2022-10-26T12:40:22Z | Batching issue that has been fixed. | 
| [50](https://github.com/sudoblockio/icon-transformer/issues/50) | Fix contracts information when they're deployed by another contract | Closed | 2022-10-13T20:45:46Z | | 
| [48](https://github.com/sudoblockio/icon-transformer/issues/48) | Fix getGormError returning null  | closed | 2022-10-03T20:27:05Z | | 
| [47](https://github.com/sudoblockio/icon-transformer/issues/47) | Random crashes on backfill  | closed | 2022-10-03T16:56:43Z | Batching issue that has been fixed. | 
| [39](https://github.com/sudoblockio/icon-transformer/issues/39) | Replace counting logic  | closed | 2022-08-15T06:14:10Z | | 
| [38](https://github.com/sudoblockio/icon-transformer/issues/38) | Replace crud methods with generic functions  | closed | 2022-08-15T06:10:31Z | | 
| [37](https://github.com/sudoblockio/icon-transformer/issues/37) | Add batch upserter  | closed | 2022-08-15T06:06:22Z | | 
| [33](https://github.com/sudoblockio/icon-transformer/issues/33) | Classify Txs for contract creation / update / approval events  | closed | 2022-06-16T00:14:29Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [57](https://github.com/sudoblockio/icon-transformer/issues/57) | Insert transaction for internally created contracts marking contract created  | open | 2022-11-01T11:17:53Z | This is for the prior mentioned edge case of internally created contracts | 
| [55](https://github.com/sudoblockio/icon-transformer/issues/55) | Transformer getting stuck on blocks  | open | 2022-10-22T15:56:52Z | There are what seems to be 3 blocks in whole chain that are causing issues. Suspecting from range where chain was spam attacked but still looking into it. Low priority. | 
| [54](https://github.com/sudoblockio/icon-transformer/issues/54) | Missing blocks not completing crud | open | 2022-10-20T11:00:23Z | Same as #55 | 
| [53](https://github.com/sudoblockio/icon-transformer/issues/53) | Problem blocks 4070001 - OOM transformer  | open | 2022-10-17T20:58:07Z | Suspecting same as #55 | 
| [51](https://github.com/sudoblockio/icon-transformer/issues/51) | Speed up DB  | open | 2022-10-14T12:31:25Z | This could be a non-issue but certain queries aren't performing as well as they should. They aren't exposed in API though so likely not an issue. | 
| [49](https://github.com/sudoblockio/icon-transformer/issues/49) | Add decimals for tokens  | open | 2022-10-04T12:30:33Z | Solved for FE but should still index it in backend. | 
| [46](https://github.com/sudoblockio/icon-transformer/issues/46) | Add callback functions into crud  | open | 2022-09-28T10:49:31Z | Side stepped with another solution but should implement general one. | 
| [43](https://github.com/sudoblockio/icon-transformer/issues/43) | Update consumer to guaranteed once delivery  | open | 2022-09-17T21:50:58Z | Long term, will fix but not a near term issue. | 

## Downtime Incidents

| Date | Total Downtime    | Cause                        | Resolution                                |
|------|-------------------|------------------------------|-------------------------------------------|
| 10/28 | 10 min            | DB crash                     | Switched DNS, restart, brought back online |
| 10/8 | 30 min (non-prod) | Cloud provider network issue | Yelled at customer support                |

All downtime incidents can be found at [icon-status-page](https://github.com/sudoblockio/icon-status-page/issues?q=)

### Projected for next cycle

| Name             | Development State        | Notes                           |
|------------------|--------------------------|---------------------------------|
| Hire DO engineer | Interviews in progress   | Have interviewed ~30 candidates |
| Hire Sr Go dev   | Hired Jr, looking for Sr | Have interviewed ~10 candidates |
| Logging          | Partially completed      | Working through bugs            |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)
