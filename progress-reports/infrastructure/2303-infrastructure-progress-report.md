# Tracker Monthly Report

This is a progress update for 03/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

During the last reporting period we worked on all sides of the stack. Summarized in bullets:

- Rebuilt balanced backend
  - This was a ticking time bomb as the old version was unsyncable and was only a matter of time till it crashed. We hence had to rebuild it and make it maintainable. 
  - Those data feeds now support any token / pool traded on balanced and the data will be integrated into the tracker. Contemplating various designs so that different tokens can be linked to via the tracker. 
- Submitted CPS 
  - CPS proposal for adding numerous transaction submission features to the tracker was submitted. This addresses the agreed supplemental funding via CPS. 

The rest of the work is summarized in the corresponding sections. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

All the major issues have been dealt with now. As part of this grant we'll be working on some requests to allow sorting and filtering of Txs based on method and other parameters for the next couple cycles along with general maintenance. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [188](https://github.com/sudoblockio/icon-tracker-frontend/pull/188) | fix: token dropdown sort in addr info #153 | closed | 2023-03-04T09:04:01Z | | 
| [187](https://github.com/sudoblockio/icon-tracker-frontend/pull/187) | chore(main): release 0.2.14 | closed | 2023-03-03T15:19:22Z | | 
| [186](https://github.com/sudoblockio/icon-tracker-frontend/pull/186) | fix: proposals page pagination #181 | closed | 2023-03-03T15:17:38Z | | 
| [185](https://github.com/sudoblockio/icon-tracker-frontend/pull/185) | fix: address delegation tabs #184 | closed | 2023-03-02T08:52:28Z | | 
| [183](https://github.com/sudoblockio/icon-tracker-frontend/pull/183) | fix: info summary market cap loading & api #87 | closed | 2023-02-23T11:51:04Z | | 
| [184](https://github.com/sudoblockio/icon-tracker-frontend/issues/184) | Delegations Tab is not (always) working. | closed | 2023-02-22T16:49:11Z | | 
| [182](https://github.com/sudoblockio/icon-tracker-frontend/pull/182) | fix: missing tabs in network proposals #176 | closed | 2023-02-22T10:33:31Z | | 
| [180](https://github.com/sudoblockio/icon-tracker-frontend/pull/180) | chore(main): release 0.2.13 | closed | 2023-02-16T16:09:07Z | | 
| [179](https://github.com/sudoblockio/icon-tracker-frontend/pull/179) | fix: removed decimals in token vote value in network proposal #177 | closed | 2023-02-16T14:37:05Z | | 
| [178](https://github.com/sudoblockio/icon-tracker-frontend/pull/178) | fix: added method column to internal tx tables #160 | closed | 2023-02-16T14:13:26Z | | 
| [177](https://github.com/sudoblockio/icon-tracker-frontend/issues/177) | Fix decimals in `Network Proposals` | closed | 2023-02-14T12:00:55Z | | 
| [176](https://github.com/sudoblockio/icon-tracker-frontend/issues/176) | Missing tab in `Network Proposals`  | closed | 2023-02-14T11:57:32Z | | 
| [175](https://github.com/sudoblockio/icon-tracker-frontend/pull/175) | fix: block navigation selector grey out fix #164 | closed | 2023-02-14T10:34:34Z | | 
| [174](https://github.com/sudoblockio/icon-tracker-frontend/pull/174) | fix: network proposal date fix #85 | closed | 2023-02-13T13:57:01Z | | 
| [173](https://github.com/sudoblockio/icon-tracker-frontend/pull/173) | fix: token dropdown undefined #169 | closed | 2023-02-09T16:10:41Z | | 
| [172](https://github.com/sudoblockio/icon-tracker-frontend/pull/172) | chore(main): release 0.2.12 | closed | 2023-02-09T13:44:06Z | | 
| [171](https://github.com/sudoblockio/icon-tracker-frontend/pull/171) | fix: token-tx-quantity-value #168 | closed | 2023-02-09T12:59:28Z | | 
| [170](https://github.com/sudoblockio/icon-tracker-frontend/issues/170) | Right arrow button on block view is greyed out but shouldn't be | closed | 2023-02-08T23:33:31Z | | 
| [169](https://github.com/sudoblockio/icon-tracker-frontend/issues/169) | Token drop down showing `undefined` for name  | closed | 2023-02-08T10:45:03Z | | 
| [168](https://github.com/sudoblockio/icon-tracker-frontend/issues/168) | Token transfer `Quantity` not showing properly  | closed | 2023-02-07T09:18:29Z | | 
| [164](https://github.com/sudoblockio/icon-tracker-frontend/issues/164) | Block up / down selector not working properly  | closed | 2023-02-04T12:16:07Z | | 
| [163](https://github.com/sudoblockio/icon-tracker-frontend/pull/163) | chore(main): release 0.2.11 | closed | 2023-02-04T10:57:40Z | | 
| [162](https://github.com/sudoblockio/icon-tracker-frontend/pull/162) | fix: api not being called on address change #161 | closed | 2023-02-04T10:04:46Z | | 
| [161](https://github.com/sudoblockio/icon-tracker-frontend/issues/161) | Cache issue when on an address  | closed | 2023-02-01T06:32:12Z | | 


#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [189](https://github.com/sudoblockio/icon-tracker-frontend/pull/189) | chore(main): release 0.2.15 | open | 2023-03-04T17:02:21Z | | 
| [181](https://github.com/sudoblockio/icon-tracker-frontend/issues/181) | Paginate proposals page | open | 2023-02-22T07:19:00Z | | 
| [167](https://github.com/sudoblockio/icon-tracker-frontend/issues/167) | Update build scripts  | open | 2023-02-04T17:00:54Z | | 
| [166](https://github.com/sudoblockio/icon-tracker-frontend/issues/166) | Update readme with new build instructions  | open | 2023-02-04T17:00:38Z | | 
| [165](https://github.com/sudoblockio/icon-tracker-frontend/issues/165) | February Sprint | open | 2023-02-04T13:16:37Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [73](https://github.com/sudoblockio/icon-transformer/pull/73) | chore(main): release 0.3.3 | closed | 2023-03-01T14:20:01Z | | 
| [72](https://github.com/sudoblockio/icon-transformer/pull/72) | Sort token transfers | closed | 2023-03-01T14:16:15Z | | 
| [71](https://github.com/sudoblockio/icon-transformer/issues/71) | Sort output in token transfers based on transaction and log index  | closed | 2023-02-20T03:30:27Z | | 
| [67](https://github.com/sudoblockio/icon-transformer/pull/67) | chore(main): release 0.3.2 | closed | 2023-02-07T16:20:08Z | | 
| [66](https://github.com/sudoblockio/icon-transformer/issues/66) | Add new migration script for custom index  | closed | 2023-02-07T14:47:52Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [70](https://github.com/sudoblockio/icon-transformer/issues/70) | Add additional columns for filters on `*_by_address` | open | 2023-02-14T12:17:27Z | | 
| [69](https://github.com/sudoblockio/icon-transformer/issues/69) | Create index of ABIs over time  | open | 2023-02-13T18:12:34Z | | 
| [68](https://github.com/sudoblockio/icon-transformer/issues/68) | Unpack event logs into map  | open | 2023-02-12T21:10:55Z | |

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

Merged feature where we are performing counts on arbitrary `/transactions` endpoint requests. This was non-trivial as these requests are frequent and could return >100k records which are expensive to count. Thus we put a timeout on the count and revert to the total count if the query takes longer than 1 second. Count is also done in parallel with the actual query. This was a highly requested feature from several members of the community. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [35](https://github.com/sudoblockio/icon-go-api/pull/35) | chore(main): release 0.4.3 | closed | 2023-03-01T14:19:34Z | | 
| [33](https://github.com/sudoblockio/icon-go-api/pull/33) | chore(main): release 0.4.2 | closed | 2023-02-14T12:38:52Z | |

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [34](https://github.com/sudoblockio/icon-go-api/issues/34) | Timeout on /transactions/icx/<address> and internal | open | 2023-02-18T11:50:27Z | | 
| [32](https://github.com/sudoblockio/icon-go-api/issues/32) | Add filter for `method` for internal transactions  | open | 2023-02-14T12:32:18Z | | 
| [31](https://github.com/sudoblockio/icon-go-api/pull/31) | Add block param to transactions/token-transfers/address/{address} | open | 2023-02-14T12:05:57Z | | 
| [30](https://github.com/sudoblockio/icon-go-api/issues/30) | Add block start / end query param to token transfers  | open | 2023-02-13T11:59:48Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

An issue with BTP contracts not showing up in the `Tokens` drop down was found and a fix should be in place in the next few days. 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [6](https://github.com/sudoblockio/icon-contracts/issues/6) | Zipbomb check failing test  | open | 2023-02-08T16:41:23Z | | 
| [5](https://github.com/sudoblockio/icon-contracts/pull/5) | chore(main): release 0.2.0 | open | 2023-01-13T09:27:02Z | | 
| [4](https://github.com/sudoblockio/icon-contracts/issues/4) | Add sort parameter to /contracts api | open | 2022-12-08T17:37:05Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

Issues with peer discovery are in progress which will be dealth with as part of the upcoming CPS proposal. 

#### Open Issues

| Number | Name | Status | Created | Notes                          |
| --- | --- | --- | --- |--------------------------------| 
| [6](https://github.com/sudoblockio/icon-governance/issues/6) | Delegation out of sync with some addresses that have un-delegated  | open | 2023-03-03T12:29:33Z | Triaged and will be fixed soon | 
| [5](https://github.com/sudoblockio/icon-governance/issues/5) | Add missed blocks to cron  | open | 2023-02-13T08:01:08Z |                                | 
| [4](https://github.com/sudoblockio/icon-governance/issues/4) | Move cron to apscheduler | open | 2023-02-13T07:59:30Z | WIP                            | 

### [icon-extractor](https://github.com/sudoblockio/icon-extractor)

This is currently being rebuilt to support multiple chains. Time spent on this upgrade not considered part of the grant and part of broader sudoblock efforts but will benefit ICON nonetheless. 

## Infrastructure 

Preparation is underway for a migration. OVH Cloud is the leading candidate for the migration. Instead of running kubernetes directly on the host's OS, it was advised to run it inside VMs using a tool called [Harvester](https://github.com/harvester/harvester). Initial trials are underway with the tool which will allow for better resource segregation and more easily being able to run upgrades. 

We are also currently dealing with issues with our API Gateway / reverse proxy and are talking directly to support of [Emissary Ingress](https://github.com/emissary-ingress/emissary) to resolve them. This issue has led to several intermittent outages where the reverse proxies run out of memory and crash. These proxies shouldn't consume much memory at all though by inspecting logs and the admin console, we can see errors that could explain the memory issue. Long term, we are considering a new reverse proxy as we need to have certain features such as rate limiting and auth baked in which is only available in their enterprise plan that is likely out of our price range. Kubernetes just released a new spec called [Gateway API](https://gateway-api.sigs.k8s.io/) which standardizes how API Gateways are configured similar to ingress controllers. We're evaluating new API Gateways that will conform to this spec and give us the features we need. 

### Downtime Incidents

| Date | Total Downtime | Cause                               | Resolution                                |
|------|----------------|-------------------------------------|-------------------------------------------|
| 2023-02-20 | < 5 min        | Aforementioned reverse proxy issue. | Resolved itself when containers restarted |
| 2023-02-28 | < 1 min | Node failure | Pods rebalanced. Contacted support and new node was added to cluster. | 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)