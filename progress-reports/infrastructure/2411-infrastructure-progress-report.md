# Tracker Monthly Report

This is a progress update for 10/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month was focused on balanced, infra, and various dev items. 

On balanced, what seemed like a complicated but not too difficult issue exploded into a huge amount of work due to issues with outdated core dependencies which every service uses. These needed to be updated and the issue itself took 4x longer than anticipated. Also with all the pools now, roughly 75 atm, the backend is not particularly fast and some stats are delayed by 5 min or so when some updates are being done. There are various optimizations and fixes but generally speaking the whole backend should be upgraded to do jobs async which would broadly solve this issue and allow for more jobs to be added without the worry of them slowing everything else down. 

On the infra side, we hit 2 rough patches which has spawned on some rebuild of the extractor service. First issue was with postgres which is too technical to explain but had an instance backup go in a loop and sent Tbs of data to s3 which was then somehow replicated numerous times peaking out at an $900/day cost. We had a couple issues but snoozing on an issue a little over a day cost us 2k and after syncing mainnet crashed the DB. So from that we had to start over this time fixing the root cause. Second issue was with some slow sync times we can't get into. After all this, effort is now being put into rebuilding the extractor tool, again reasons out of scope of this report. 

Despite this, on the infra side we are operating over 10 icon nodes right now on each network which we believe is stable after hitting these nodes with load. We have a full observability suite setup with traces from gateways which we built dashboards and alarms off of. Every node is centrally logged and monitored with alarms activated. Only thing holding up the infra side is syncs which had to be redone. 

As for dev work, we touched most services this month as we are upgrading the API docs to have an on-brand consistent feeling. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [504](https://github.com/sudoblockio/icon-tracker-frontend/pull/504) | chore(main): release 0.6.2 | closed | 2024-10-24T04:43:22Z | | 
| [503](https://github.com/sudoblockio/icon-tracker-frontend/pull/503) | Bugs | closed | 2024-10-23T20:09:58Z | | 
| [501](https://github.com/sudoblockio/icon-tracker-frontend/pull/501) | chore(main): release 0.6.1 | closed | 2024-10-02T19:38:34Z | | 
| [500](https://github.com/sudoblockio/icon-tracker-frontend/pull/500) | fix: removed iconex mention | closed | 2024-10-02T19:37:54Z | | 
| [498](https://github.com/sudoblockio/icon-tracker-frontend/issues/498) | Remove "Connected to ICONex" icon  | closed | 2024-09-23T06:26:30Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | April Sprint  | closed | 2024-03-10T07:03:17Z | | 
| [405](https://github.com/sudoblockio/icon-tracker-frontend/issues/405) | Add `auto-vote` feature | closed | 2024-02-18T23:04:53Z | | 
| [404](https://github.com/sudoblockio/icon-tracker-frontend/issues/404) | Add `voting` feature  | closed | 2024-02-18T23:03:42Z | | 
| [403](https://github.com/sudoblockio/icon-tracker-frontend/issues/403) | Add `staking` feature   | closed | 2024-02-18T22:51:08Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | December Sprint | closed | 2023-11-01T08:00:51Z | | 
| [349](https://github.com/sudoblockio/icon-tracker-frontend/issues/349) | Decode event logs based on ABI  | closed | 2023-10-21T10:34:23Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [506](https://github.com/sudoblockio/icon-tracker-frontend/pull/506) | chore(main): release 0.6.3 | open | 2024-11-07T06:27:56Z | | 
| [505](https://github.com/sudoblockio/icon-tracker-frontend/issues/505) | Estimate Fee breaking voting + bonding + others  | open | 2024-11-01T07:57:28Z | | 
| [502](https://github.com/sudoblockio/icon-tracker-frontend/issues/502) | Prioritized Backlog | open | 2024-10-06T09:40:07Z | | 
| [490](https://github.com/sudoblockio/icon-tracker-frontend/issues/490) | contract method with param of type []string fail when trying to call on the the tracker | open | 2024-09-13T20:36:22Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [79](https://github.com/sudoblockio/icon-transformer/pull/79) | Update Protoc Gorm Generation | closed | 2024-07-15T05:22:06Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [52](https://github.com/sudoblockio/icon-go-api/pull/52) | chore(main): release 0.5.6 | closed | 2024-10-15T13:34:13Z | | 
| [51](https://github.com/sudoblockio/icon-go-api/pull/51) | fix: transactions and address doc string | closed | 2024-10-15T13:20:21Z | | 
| [50](https://github.com/sudoblockio/icon-go-api/pull/50) | chore(main): release 0.5.5 | closed | 2024-10-15T12:57:32Z | | 
| [49](https://github.com/sudoblockio/icon-go-api/pull/49) | fix: update doc string for stats | closed | 2024-10-15T12:35:43Z | | 


### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [14](https://github.com/sudoblockio/icon-contracts/pull/14) | chore(main): release 0.2.5 | closed | 2024-10-14T11:14:30Z | | 
| [13](https://github.com/sudoblockio/icon-contracts/pull/13) | chore(main): release 0.2.4 | closed | 2024-10-14T09:21:01Z | | 
| [12](https://github.com/sudoblockio/icon-contracts/pull/12) | chore(main): release 0.2.3 | closed | 2024-10-11T08:43:01Z | | 
| [10](https://github.com/sudoblockio/icon-contracts/pull/10) | chore(main): release 0.2.2 | closed | 2024-10-06T15:00:06Z | | 
| [9](https://github.com/sudoblockio/icon-contracts/pull/9) | chore(main): release 0.2.1 | closed | 2024-10-06T11:54:41Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [11](https://github.com/sudoblockio/icon-contracts/issues/11) | Had to snub test_get_first_tx tests - find cause  | open | 2024-10-07T22:31:50Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [51](https://github.com/sudoblockio/icon-governance/pull/51) | chore(main): release 0.10.5 | closed | 2024-10-14T09:00:51Z | | 
| [50](https://github.com/sudoblockio/icon-governance/pull/50) | chore(main): release 0.10.4 | closed | 2024-10-11T08:46:41Z | | 
| [49](https://github.com/sudoblockio/icon-governance/pull/49) | chore(main): release 0.10.3 | closed | 2024-10-06T14:53:05Z | | 
| [48](https://github.com/sudoblockio/icon-governance/pull/48) | chore(main): release 0.10.2 | closed | 2024-10-06T11:50:37Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [69](https://github.com/balancednetwork/balanced-backend/issues/69) | Fix price charts | closed | 2024-10-07T07:06:46Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [70](https://github.com/balancednetwork/balanced-backend/issues/70) | New collateral tokens loan charts | open | 2024-10-11T07:21:08Z | | 
| [68](https://github.com/balancednetwork/balanced-backend/issues/68) | Stability fund collateral series shows hyTB balance only | open | 2024-10-04T12:31:55Z | | 
| [67](https://github.com/balancednetwork/balanced-backend/pull/67) | chore(main): release 0.8.0 | open | 2024-09-17T07:35:18Z | | 

### [icon-stats](https://github.com/sudoblockio/icon-stats)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [14](https://github.com/sudoblockio/icon-stats/pull/14) | chore(main): release 0.2.5 | closed | 2024-10-18T08:15:22Z | | 
| [13](https://github.com/sudoblockio/icon-stats/pull/13) | chore(main): release 0.2.4 | closed | 2024-10-11T11:37:22Z | | 
| [12](https://github.com/sudoblockio/icon-stats/pull/12) | chore(main): release 0.2.3 | closed | 2024-10-11T08:41:45Z | | 
| [11](https://github.com/sudoblockio/icon-stats/pull/11) | chore(main): release 0.2.2 | closed | 2024-09-30T11:12:05Z | | 



## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| ~10/15 | 30 min on Berlin | Seemed node related - just a node going out of sync | Took node off the LB | 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)