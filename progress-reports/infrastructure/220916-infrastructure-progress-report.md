## Intro

This is a progress update for infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem for the period from August 1st to September 17th.

## Summary

Rebuilt backend resulting in an increase in ~500x performance increase. Code has dramatically been reduced in size due to the use of generics for CRUD (create read update delete) logic. Testing patterns are now in place to get much better coverage and allow test driven development.

## Deliverables

### Accomplished this cycle

| Name | Development State | Notes | Source / location |
| ---- |-------------------| ----- | ----------------- |
| NFT token indexes | Beta | Added indexes to cover token transfers for IRC3/31 tokens which initially took to long to sync prompting a rebuild of the CRUD and other core components of the icon-transformer repo | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Selective syncing | Beta | Added selective syncing capability to allow syncing individual indexes at a time. Prior to this feature, a resync required updating all the indexes at the same time which is much slower than syncing a single index as syncs are very IO bound on the DB. Also most indexes are very sparse so if one of those indexes needs to be synced, it can read / ignore the majority of the data and only upsert targetted data.   | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Buffered loader channels | Beta | Added a buffered channel to do all CRUD operations allowing a transformer to read and process data in a non-blocking way. This allows batches of data to be upserted into the DB which is far more efficient than upserting individual records at a time. Within the buffered loader channels, upserts are tunable so that there is a sleep step that happens allowing the buffer to fill up so that batches of records can be upserted into the DB. This process has increased performance of syncs by roughly 500x. Berlin now can be synced on a laptop within ~2 hours for all indexes. For a lean individual index (<500k records), syncs take ~5-10 min. Prior to the change, syncs took over a day. On mainnet, a full sync hasn't been done yet but initial benchmarks show lean indexes syncing in roughly 30 min. Prior to change, a full resync was taking over a week.  | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Generic crud interfaces | Beta | Created generic CRUD interfaces that are shared along all transformers. Before there was an enourmous amount of boilerplate for CRUD. Now, using features from Go 1.18 (ie generics), there is a single CRUD struct whose interfaces are able to provide CRUD operations for all the transformers. This allowed the removal of roughly 4k lines of code.  | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Retry logic | Beta | Added retry logic for DB operations that are shared along all transformers. Prior to this retry logic, any lapse in DB connections caused a crash which when doing resyncs forced applying the resync from scratch. Now lapses in DB connections are non-disruptive and they recover on their own. | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Improved testing patterns | Beta | Added new testing pattern whereby individual block records are saved as json fixtures and can be read / run through transformer and result is asserted as being correct. This is a major improvement as now test driven development can be applied to all the transformers.  | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Updated / cron routines | Beta | Applied new CRUD logic to cron jobs which initially had some bugs but have since been worked out and are passing QC checks. Syncs now require a per record transform plus a cron job sync to get fully up to date. Cron job runs for about 15 min on Berlin and 1.5 hours on mainnet. Was observed that prior cron jobs was causing disruptions by overloading the DB which has since been worked out with the new CRUD pattern.   | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) | 
| Contracts created by contracts | WIP | Began rework of indexes for BTP contracts that are created within contracts. Initial work was done on parsing the traces of specific methods on specific contracts that created other contracts but now the plan is to use RPC methods to index these new contracts.  | [PR](https://github.com/sudoblockio/icon-transformer/pull/42) |

### Projected for next cycle

| Name | Development State | Notes |
| ---- | ----------------- | ----- |
| Add guaranteed once delivery | Not started | [Issue](https://github.com/sudoblockio/icon-transformer/issues/43) | 
| Hire DO engineer | Interviews in progress | Have interviewed ~20 candidates |

### Downtime Incidents 

All downtime incidents can be found at [icon-status-page](https://github.com/sudoblockio/icon-status-page/issues?q=)

| Date | Downtime | Cause | Notes |
| ---- | ----- | ----- | ----- |
| 9/18 | 10 min | DB Crash | DB server crashed and still investigating cause. Suspecting issue with file handlers / dropped connections. Hoping new backend will solve the issue but will still need to do a deep dive to truly uncover cause. Switched DNS to backup tracker while dealing with issue. Restarted DB server which solved issue. | 

### Instructions to run tests

In every repo, tests can be run with `make test`.

Alternatively look at the logs from the CI pipeline for results of tests.
