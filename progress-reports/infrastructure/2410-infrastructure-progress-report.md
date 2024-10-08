# Tracker Monthly Report

This is a progress update for 9/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month was mainly focused on redeploying the tracker on our new bare metal servers and rebuilding the backend focussing on building a new client for making RPC calls. 

On the infra side, all the major hurdles are over with respect to routing, and deployments. We synced Berlin in roughly 8 hours from extraction of events from the chain to inserting the records in a DB. This is a major improvement on our prior sync times and only using a fraction of the resources we have available. Ran into a couple issues with deployment of mainnet which were recently unstuck but should be starting that imminently. We also have a new observability stack working where we are getting much more granular metrics, logs, and traces from our entire stack which are being instrumented with alarms. 

On the rebuilding of the backend, we built what we consider a very idiomatic RPC client for multiple chains including eth, cosmos, polkadot, and sui. The client is currently only in python but we have plans to expand it into each major language. It supports both async and sync calls along with batching. There is also a middleware layer for things like metrics, logs, caching, retries, and load balancing that can be applied to every chain the client ends up supporting. We're now working on extracting OpenRPC specs from it which will then be used to create API documentation and code generation for building new clients in each language. For building the backend itself, we're still in design phase but the clients will make it so indexing all the chains will be based on the same core design.  

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

We recently got sentry working with the frontend and are now getting alerts on various crashes. Further instrumentation can be done to then find potential issues with the backend from the frontend which we'll be exploring more in the future. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [501](https://github.com/sudoblockio/icon-tracker-frontend/pull/501) | chore(main): release 0.6.1 | closed | 2024-10-02T19:38:34Z | | 
| [500](https://github.com/sudoblockio/icon-tracker-frontend/pull/500) | fix: removed iconex mention | closed | 2024-10-02T19:37:54Z | | 
| [498](https://github.com/sudoblockio/icon-tracker-frontend/issues/498) | Remove "Connected to ICONex" icon  | closed | 2024-09-23T06:26:30Z | | 
| [494](https://github.com/sudoblockio/icon-tracker-frontend/pull/494) | chore: empty events table | closed | 2024-09-18T14:12:57Z | | 
| [493](https://github.com/sudoblockio/icon-tracker-frontend/pull/493) | chore: bonding dropdown | closed | 2024-09-18T12:47:29Z | | 
| [492](https://github.com/sudoblockio/icon-tracker-frontend/pull/492) | chore: event log input parsing bug | closed | 2024-09-17T20:11:23Z | | 
| [489](https://github.com/sudoblockio/icon-tracker-frontend/pull/489) | chore: breadcrubms onClick & style | closed | 2024-09-11T10:17:14Z | | 
| [488](https://github.com/sudoblockio/icon-tracker-frontend/pull/488) | Wallet tooling | closed | 2024-09-11T09:37:42Z | | 
| [487](https://github.com/sudoblockio/icon-tracker-frontend/pull/487) | chore: voting table toFixed bug | closed | 2024-09-10T12:18:55Z | | 
| [486](https://github.com/sudoblockio/icon-tracker-frontend/pull/486) | chore: updated hearder dropdown view | closed | 2024-09-10T11:37:18Z | | 
| [485](https://github.com/sudoblockio/icon-tracker-frontend/pull/485) | chore: sentry setup | closed | 2024-09-09T08:31:08Z | | 
| [484](https://github.com/sudoblockio/icon-tracker-frontend/pull/484) | chore: contract abi json collapse fix | closed | 2024-09-07T10:38:04Z | | 
| [483](https://github.com/sudoblockio/icon-tracker-frontend/pull/483) | chore: abi table style | closed | 2024-09-05T09:55:38Z | | 
| [482](https://github.com/sudoblockio/icon-tracker-frontend/pull/482) | Contract view | closed | 2024-09-03T11:53:07Z | | 
| [481](https://github.com/sudoblockio/icon-tracker-frontend/pull/481) | chore: events pagination empty data bug | closed | 2024-09-02T08:41:01Z | | 
| [480](https://github.com/sudoblockio/icon-tracker-frontend/pull/480) | Wallet tooling | closed | 2024-09-01T12:25:55Z | | 
| [475](https://github.com/sudoblockio/icon-tracker-frontend/issues/475) | bonding issue | closed | 2024-08-06T19:33:00Z | | 
| [472](https://github.com/sudoblockio/icon-tracker-frontend/pull/472) | chore(main): release 0.6.0 | closed | 2024-07-25T08:46:21Z | | 
| [466](https://github.com/sudoblockio/icon-tracker-frontend/issues/466) | Sectioned ABI view  | closed | 2024-07-03T15:25:34Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [499](https://github.com/sudoblockio/icon-tracker-frontend/issues/499) | Remove "Explorer (Coming)" and change "Stats (Coming)" to "Stats" with link | open | 2024-09-23T06:28:58Z | | 
| [497](https://github.com/sudoblockio/icon-tracker-frontend/issues/497) | Delay in opening bonding popup | open | 2024-09-19T09:29:42Z | | 
| [496](https://github.com/sudoblockio/icon-tracker-frontend/issues/496) | Empty event objects in contract event logs | open | 2024-09-19T09:28:19Z | | 
| [495](https://github.com/sudoblockio/icon-tracker-frontend/issues/495) | Transaction events | open | 2024-09-19T09:26:52Z | | 
| [491](https://github.com/sudoblockio/icon-tracker-frontend/issues/491) | Duplicate synchronous REST API calls /governance/preps in governance page | open | 2024-09-17T15:54:24Z | | 
| [490](https://github.com/sudoblockio/icon-tracker-frontend/issues/490) | contract method with param of type []string fail when trying to call on the the tracker | open | 2024-09-13T20:36:22Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

Facing some deadlock issues with this service that we're hoping to avert fixing by rebuilding the backend. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [79](https://github.com/sudoblockio/icon-transformer/pull/79) | Update Protoc Gorm Generation | closed | 2024-07-15T05:22:06Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [47](https://github.com/sudoblockio/icon-governance/pull/47) | chore(main): release 0.10.1 | closed | 2024-09-04T03:40:21Z | | 
| [46](https://github.com/sudoblockio/icon-governance/pull/46) | chore(main): release 0.10.0 | closed | 2024-08-20T02:30:14Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [65](https://github.com/balancednetwork/balanced-backend/pull/65) | chore(main): release 0.7.0 | closed | 2024-08-26T02:08:56Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [67](https://github.com/balancednetwork/balanced-backend/pull/67) | chore(main): release 0.8.0 | open | 2024-09-17T07:35:18Z | | 
| [66](https://github.com/balancednetwork/balanced-backend/issues/66) | Add stability fund liquidity to token list | open | 2024-09-04T07:20:47Z | | 

### [icon-stats](https://github.com/sudoblockio/icon-stats)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [7](https://github.com/sudoblockio/icon-stats/pull/7) | OpenAPI merger endpoint | closed | 2024-09-29T12:28:20Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [11](https://github.com/sudoblockio/icon-stats/pull/11) | chore(main): release 0.2.2 | open | 2024-09-30T11:12:05Z | | 
| [10](https://github.com/sudoblockio/icon-stats/issues/10) | OpenAPI Merger Meta | open | 2024-09-29T12:38:19Z | | 
| [9](https://github.com/sudoblockio/icon-stats/issues/9) | Fix outputs of merger - anyOf missing types  | open | 2024-09-29T12:38:11Z | | 
| [8](https://github.com/sudoblockio/icon-stats/issues/8) | Setup OpenAPI merger  | open | 2024-09-29T12:36:51Z | | 


## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 9/10 | 15 min | The page cache for the DBs was not big enough for vacuums to proceed so auto-vacuum was failing which ended up causing a lot of issues. | Page cache was increased and then after successful vacuums the response times and time outs decreased / went away. | 

We're generally dealing with issues surrounding a large amount of memory usage. We contacted a consultant to do some index optimizations but haven't met with them yet as doing the remediation step from above has temporarily fixed the issue. Moving to the new servers which have .5tb of memory will again solve the issue but in general we need to do some index optimizations / likely figuring out a better way of indexing transactions which consume the most memory. Considering a number of options but as we are also rebuilding the backend, the timing of the rebuilding of indexes would be best if they to coincided with the rebuild of the backend.  

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)