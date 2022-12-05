# Tracker Monthly Report

This is a progress update for 11/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

November was mainly focused on integrating a number of fixes from the tracker backend into the frontend. Several bugs dealing with the counting of records were handled in the backend and changes brought forward. Also some bugs were dealt with having to do with batch processing and conflicts in the CRUD logic. Had been working with two different frontend engineers, the first being relatively inexperienced and being replaced by the second who will be continuing work through the new year. 

On the infrastructure side of things, a redeployment of Berlin took place due to the network being reset. Also, significant effort is being put into the infra deployment process. The plan is to update the infra to a new pattern which will be cleaner / more maintainable by the devops engineers who will be brought on within the next few months with interviews in progress.  

Also while not directly having to do with the tracker, some POCs were put together for improving BTP deployments. 

### [icon-tracker](https://github.com/sudoblockio/icon-tracker)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [65](https://github.com/sudoblockio/icon-tracker/issues/65) | API in README is dead link | closed | 2022-11-08T00:06:07Z | | 
| [63](https://github.com/sudoblockio/icon-tracker/issues/63) | Update this repo or archive  | closed | 2022-07-07T04:06:40Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [68](https://github.com/sudoblockio/icon-tracker/issues/68) | API links are dead | open | 2022-11-29T16:45:27Z | | 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [89](https://github.com/sudoblockio/icon-tracker-frontend/pull/89) | fix: fixed home page recent block listing and sorting | closed | 2022-11-29T20:38:49Z | | 
| [84](https://github.com/sudoblockio/icon-tracker-frontend/pull/84) | fix: pagination issues | closed | 2022-11-17T15:58:37Z | | 
| [82](https://github.com/sudoblockio/icon-tracker-frontend/issues/82) | Counts not being shown appropriately in transaction bottom | closed | 2022-11-16T14:08:14Z | | 
| [81](https://github.com/sudoblockio/icon-tracker-frontend/issues/81) | the data is not rendered properly due to invalid URL | closed | 2022-11-15T16:33:37Z | | 
| [80](https://github.com/sudoblockio/icon-tracker-frontend/pull/80) | fix #79; Events not getting populated after reload issue is fixed | closed | 2022-11-09T16:20:29Z | | 
| [79](https://github.com/sudoblockio/icon-tracker-frontend/issues/79) | Events not getting populated after reload | closed | 2022-11-07T16:35:29Z | | 
| [78](https://github.com/sudoblockio/icon-tracker-frontend/pull/78) | fix #62; Add QR code to adresses issue is fixed. | closed | 2022-11-06T12:08:59Z | | 
| [77](https://github.com/sudoblockio/icon-tracker-frontend/pull/77) | fix #73; Token holder view is fixed. | closed | 2022-11-01T16:53:45Z | | 
| [73](https://github.com/sudoblockio/icon-tracker-frontend/issues/73) | Fix token holders list view  | closed | 2022-10-18T04:21:43Z | | 
| [70](https://github.com/sudoblockio/icon-tracker-frontend/issues/70) | Reduce number of getTotalSupply calls in token holders list view and Addresses list | closed | 2022-10-18T04:10:56Z | | 
| [69](https://github.com/sudoblockio/icon-tracker-frontend/issues/69) | Fix decimals for non-e18 tokens  | closed | 2022-10-04T12:32:32Z | | 
| [68](https://github.com/sudoblockio/icon-tracker-frontend/issues/68) | Fix pagination for events  | closed | 2022-09-22T13:09:28Z | | 
| [67](https://github.com/sudoblockio/icon-tracker-frontend/issues/67) | Ranking information unavailable beyond top 25 for IRC-2 tokens other than ICX | closed | 2022-09-14T00:29:49Z | | 
| [62](https://github.com/sudoblockio/icon-tracker-frontend/issues/62) | Add QR code to addresses | closed | 2022-08-08T18:54:37Z | | 
| [52](https://github.com/sudoblockio/icon-tracker-frontend/issues/52) | Fix decimals for token transfers and supply  | closed | 2022-07-21T06:16:07Z | | 
| [24](https://github.com/sudoblockio/icon-tracker-frontend/issues/24) | Enforce sort order on websockets output for blocks  | closed | 2022-06-30T06:32:19Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [88](https://github.com/sudoblockio/icon-tracker-frontend/issues/88) | [feature request] add a 'method' column in the transaction table | open | 2022-11-25T18:28:45Z | | 
| [87](https://github.com/sudoblockio/icon-tracker-frontend/issues/87) | Swap endpoints for market_cap and circulating_supply  | open | 2022-11-25T17:38:40Z | | 
| [86](https://github.com/sudoblockio/icon-tracker-frontend/issues/86) | Add search to transaction pages | open | 2022-11-19T20:41:37Z | | 
| [83](https://github.com/sudoblockio/icon-tracker-frontend/issues/83) | Show transactions tab in token detail view  | open | 2022-11-16T18:14:01Z | | 
| [85](https://github.com/sudoblockio/icon-tracker-frontend/issues/85) | Frontend changes for displaying Network Proposals on Community Tracker | open | 2022-11-15T20:00:28Z | | 
| [71](https://github.com/sudoblockio/icon-tracker-frontend/issues/71) | November Sprint | open | 2022-10-18T04:13:54Z | | 
| [60](https://github.com/sudoblockio/icon-tracker-frontend/issues/60) | Testing for how the tracker can possibly return faulty data  | open | 2022-08-03T04:46:17Z | | 
| [46](https://github.com/sudoblockio/icon-tracker-frontend/issues/46) | Add sortable / filterable columns to `Addresses`, `Contracts`, and `Tokens` pages  | open | 2022-07-14T06:40:46Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [50](https://github.com/sudoblockio/icon-transformer/issues/50) | Fix contracts information when they're deployed by another contract | closed | 2022-10-13T20:45:46Z | | 
| [48](https://github.com/sudoblockio/icon-transformer/issues/48) | Fix getGormError returning null  | closed | 2022-10-03T20:27:05Z | | 
| [47](https://github.com/sudoblockio/icon-transformer/issues/47) | Random crashes on backfill  | closed | 2022-10-03T16:56:43Z | | 
| [39](https://github.com/sudoblockio/icon-transformer/issues/39) | Replace counting logic  | closed | 2022-08-15T06:14:10Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [60](https://github.com/sudoblockio/icon-transformer/issues/60) | Create contracts transformer  | open | 2022-11-19T19:21:11Z | | 
| [59](https://github.com/sudoblockio/icon-transformer/issues/59) | Create contracts transformer  | open | 2022-11-19T19:21:05Z | | 
| [58](https://github.com/sudoblockio/icon-transformer/issues/58) | Internal Tx / log counts not showing up properly | open | 2022-11-16T15:49:15Z | | 
| [57](https://github.com/sudoblockio/icon-transformer/issues/57) | Insert transaction for internally created contracts marking contract created  | open | 2022-11-01T11:17:53Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [16](https://github.com/sudoblockio/icon-go-api/pull/16) | chore(main): release 0.2.0 | closed | 2022-11-24T12:23:09Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [18](https://github.com/sudoblockio/icon-go-api/issues/18) | Add sort to /addresses/contracts on tx count and balance | open | 2022-11-28T19:22:18Z | | 
| [17](https://github.com/sudoblockio/icon-go-api/pull/17) | chore(main): release 0.3.0 | open | 2022-11-25T17:35:14Z | | 
| [15](https://github.com/sudoblockio/icon-go-api/issues/15) | Integrate with transformer  | open | 2022-11-19T19:22:06Z | | 
| [14](https://github.com/sudoblockio/icon-go-api/issues/14) | Slow query with low number of results and low LIMIT | open | 2022-11-17T19:29:27Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [3](https://github.com/sudoblockio/icon-contracts/issues/3) | Live API docs link is dead | closed | 2022-11-29T16:46:07Z | | 
| [1](https://github.com/sudoblockio/icon-contracts/issues/1) | librdkafka breaking on backfill  | closed | 2022-05-31T16:21:54Z | |

## Downtime Incidents

No major downtime incidents recorded besides some disruption on Berlin due to the network being reset. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box) with templates located in the [icon-tracker](https://github.com/sudoblockio/icon-tracker/blob/main/planning/tackle.yaml).
