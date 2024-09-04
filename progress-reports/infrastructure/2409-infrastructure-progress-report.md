# Tracker Monthly Report

This is a progress update for 8/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

Our work can be summarized relating to infrastructure and rebuilding of the tracker.  

##### Infrastructure 

1. We have clusters up and operational now with CI pipelines being migrated to run the core tracker components on
2. Advertising public endpoints running over our acquired IP blocks via BGP 
3. Able to bootstrap clusters in less than 2 hours from OS install on bare metal machines to k8s running services. All configuration with ansible and bootstrapping of VMs in terraform. There is almost no component of our stack that is not automated. 
4. Complete observability suite with multiple logging tools shipping logs from every component in our stack

Next month we hope to have one cluster migrated and turning components off on the cloud. 

##### Tracker Rebuild 

We worked on two sides of the rebuild, the extraction of chain data and transformation side into the appropriate indexes. On the extraction side which we'll be mainly focussing on for the next couple months, we built a new client which is able to be extended into multiple chains with typed returns (as compared to untyped dicts / objects). Plan is to code generate those interfaces on the next iteration but for now just manually writing them along with the transformers needed to index all parts of the chain. This will replace the extractor written in go and form the basis for merging all the repos we manage in ICON into a single service. It works with multiple chains and plan is to have a single client that can access all the chains. 

On the transformation side, we have been doing a lot of research on this best left to a conversation but have POCed out the components needed to join streams of data from multiple chains. This would be ideal for indexing both sides of a BTP transaction where the join key might be from event logs on the source and destination chains. The components we are using are high performance and could do full indexes on streams of data from multiple chains. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [481](https://github.com/sudoblockio/icon-tracker-frontend/pull/481) | chore: events pagination empty data bug | closed | 2024-09-02T08:41:01Z | | 
| [480](https://github.com/sudoblockio/icon-tracker-frontend/pull/480) | Wallet tooling | closed | 2024-09-01T12:25:55Z | | 
| [479](https://github.com/sudoblockio/icon-tracker-frontend/pull/479) | chore: process/browser webpack config | closed | 2024-08-21T14:30:53Z | | 
| [476](https://github.com/sudoblockio/icon-tracker-frontend/pull/476) | chore: prep update popup close button | closed | 2024-08-08T09:21:02Z | | 
| [470](https://github.com/sudoblockio/icon-tracker-frontend/pull/470) | Wallet tooling | closed | 2024-07-20T06:58:09Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [482](https://github.com/sudoblockio/icon-tracker-frontend/pull/482) | Contract view | open | 2024-09-03T11:53:07Z | | 
| [478](https://github.com/sudoblockio/icon-tracker-frontend/issues/478) | add support to identify payable methods in an arbitrary contract and add an extra field called "value" to add the amount of ICX to be transferred | open | 2024-08-16T04:38:27Z | | 
| [477](https://github.com/sudoblockio/icon-tracker-frontend/issues/477) | Signing registerPRep method of chain contract on the tracker fails due to invalid registration fee | open | 2024-08-16T04:21:52Z | | 
| [475](https://github.com/sudoblockio/icon-tracker-frontend/issues/475) | bonding issue | open | 2024-08-06T19:33:00Z | | 
| [472](https://github.com/sudoblockio/icon-tracker-frontend/pull/472) | chore(main): release 0.6.0 | open | 2024-07-25T08:46:21Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [45](https://github.com/sudoblockio/icon-governance/pull/45) | chore(main): release 0.9.0 | closed | 2024-07-31T15:08:41Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [65](https://github.com/balancednetwork/balanced-backend/pull/65) | chore(main): release 0.7.0 | closed | 2024-08-26T02:08:56Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [64](https://github.com/balancednetwork/balanced-backend/issues/64) | Additional collateral and loan charts for BTC | open | 2024-08-01T15:59:06Z | | 
| [61](https://github.com/balancednetwork/balanced-backend/issues/61) | Estimate for cross-chain collateral deposit breakdown | open | 2024-07-22T10:21:40Z | | 

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 8/28 | 5 min * ~3 | Memory filling up - missed some vacuums. Result was sluggish performance breifly on the backend over about 36 hours. | More aggressive vacuuming + removal of a couple of manually created indexes to free up some space. | 
| 8/19 | 15 min  | Expired certificate in backend caused an issue with the API gateway | Rolled certs and everything was resolved. |

Because of the issue on 8/28, some bad data was cached which resulted in some white screens as reported by a couple users. We cleared the cache in cloudflare and have since not received a single complaint on the backend. 

We also lost a couple of volumes on the message queue which needed to be recovered. Thankfully we run this in HA so recovery was possible without losing data. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)