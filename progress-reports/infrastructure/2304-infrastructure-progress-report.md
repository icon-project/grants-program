# Tracker Monthly Report

This is a progress update for 3/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month efforts were made on all sides of the stack 

- Faced a regression in the frontend from a dependency forcing us to upgrade Node 2 major versions (12 to 16 - long time coming). Upgrade was successful but set off a whole string of issues. 
- Added a more clear route to the trace screen regardless of the transaction success 
- Fixed some long standing issue with the cache not getting fully updated affecting transaction counts and other params 
- Fixed governance service finding preps IP and maintaining a count of it's penalties, missed blocks, and node status every 30 seconds.
- Almost done fixing long standing issue of not getting contracts service to propeerly emit data for internal contract creation events.
- Patched backend error where reverse proxies were crashing causing SSL errors
- Making some progress with the migration of the backend 
- Continued working on smart contract code generator with outputs from CPS Grant 
- Started CPS grant. Most issues removed from this report as these endeavors are separate (CPS is enhancement)

[Brief summary of month's progress]

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [217](https://github.com/sudoblockio/icon-tracker-frontend/pull/217) | fix: trace integration for all tx and view logs button #154 #64 | closed | 2023-03-19T07:47:19Z | | 
| [213](https://github.com/sudoblockio/icon-tracker-frontend/pull/213) | Fixed broken commits due to dependencies bugs | closed | 2023-03-16T03:32:56Z | | 
| [210](https://github.com/sudoblockio/icon-tracker-frontend/pull/210) | chore(main): release 0.2.16 | closed | 2023-03-13T18:30:20Z | | 
| [209](https://github.com/sudoblockio/icon-tracker-frontend/pull/209) | fix to #200 | closed | 2023-03-10T23:57:01Z | | 
| [207](https://github.com/sudoblockio/icon-tracker-frontend/pull/207) | fix: voters address were opening on new tab #201 | closed | 2023-03-09T21:53:13Z | | 
| [206](https://github.com/sudoblockio/icon-tracker-frontend/pull/206) | fix #202 | closed | 2023-03-09T17:55:41Z | | 
| [202](https://github.com/sudoblockio/icon-tracker-frontend/issues/202) | Bonded tab is broken  | closed | 2023-03-08T20:32:05Z | | 
| [201](https://github.com/sudoblockio/icon-tracker-frontend/issues/201) | Voters address link opens up new tab  | closed | 2023-03-08T20:30:06Z | | 
| [200](https://github.com/sudoblockio/icon-tracker-frontend/issues/200) | Broken link in Bonders tab  | closed | 2023-03-08T20:29:30Z | | 
| [191](https://github.com/sudoblockio/icon-tracker-frontend/issues/191) | Setup testing framework  | closed | 2023-03-07T18:10:27Z | | 
| [190](https://github.com/sudoblockio/icon-tracker-frontend/issues/190) | List of types of proposals along with their schema for value  | closed | 2023-03-07T18:05:11Z | | 
| [189](https://github.com/sudoblockio/icon-tracker-frontend/pull/189) | chore(main): release 0.2.15 | closed | 2023-03-04T17:02:21Z | | 
| [188](https://github.com/sudoblockio/icon-tracker-frontend/pull/188) | fix: token dropdown sort in addr info #153 | closed | 2023-03-04T09:04:01Z | | 
| [187](https://github.com/sudoblockio/icon-tracker-frontend/pull/187) | chore(main): release 0.2.14 | closed | 2023-03-03T15:19:22Z | | 
| [186](https://github.com/sudoblockio/icon-tracker-frontend/pull/186) | fix: proposals page pagination #181 | closed | 2023-03-03T15:17:38Z | | 
| [185](https://github.com/sudoblockio/icon-tracker-frontend/pull/185) | fix: address delegation tabs #184 | closed | 2023-03-02T08:52:28Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [228](https://github.com/sudoblockio/icon-tracker-frontend/issues/228) | Validate the reward rate on P-Rep List view  | open | 2023-03-27T09:30:52Z | | 
| [225](https://github.com/sudoblockio/icon-tracker-frontend/issues/225) | Header Data caches and does not refresh when using the magnifier search feature | open | 2023-03-23T19:35:43Z | | 
| [218](https://github.com/sudoblockio/icon-tracker-frontend/pull/218) | chore(main): release 0.2.17 | open | 2023-03-19T19:48:50Z | | 
| [216](https://github.com/sudoblockio/icon-tracker-frontend/pull/216) | chore: update dockerfile | open | 2023-03-18T15:09:10Z | | 
| [215](https://github.com/sudoblockio/icon-tracker-frontend/issues/215) | Make debug trace steps collapsable  | open | 2023-03-18T14:05:01Z | | 
| [214](https://github.com/sudoblockio/icon-tracker-frontend/issues/214) | Disappearing mouse on `Status` field  | open | 2023-03-18T14:00:37Z | | 
| [212](https://github.com/sudoblockio/icon-tracker-frontend/pull/212) | E2e tests | open | 2023-03-15T08:59:56Z | | 
| [211](https://github.com/sudoblockio/icon-tracker-frontend/pull/211) | Node 18 upgrade | open | 2023-03-15T02:03:57Z | | 
| [208](https://github.com/sudoblockio/icon-tracker-frontend/issues/208) | Bonded address opens in new tab  | open | 2023-03-10T11:43:42Z | | 
| [205](https://github.com/sudoblockio/icon-tracker-frontend/issues/205) | `/token/<>` is missing transactions tab  | open | 2023-03-09T10:36:32Z | | 
| [204](https://github.com/sudoblockio/icon-tracker-frontend/issues/204) | Transaction / token transfer finder  | open | 2023-03-09T10:28:14Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | open | 2023-03-08T20:34:13Z | | 
| [199](https://github.com/sudoblockio/icon-tracker-frontend/issues/199) | Excessive blocking calls on preps page  | open | 2023-03-08T20:18:11Z | | 
| [198](https://github.com/sudoblockio/icon-tracker-frontend/issues/198) | Ledger wallet integration  | open | 2023-03-08T13:49:15Z | | 
| [197](https://github.com/sudoblockio/icon-tracker-frontend/issues/197) | Main page mobile - stack cards so it is 2 x 2  | open | 2023-03-08T13:24:44Z | | 
| [196](https://github.com/sudoblockio/icon-tracker-frontend/issues/196) | Main page mobile - blocks on top of transactions  | open | 2023-03-08T13:24:19Z | | 
| [195](https://github.com/sudoblockio/icon-tracker-frontend/issues/195) | Fix some footer for mobile  | open | 2023-03-08T13:19:13Z | | 
| [194](https://github.com/sudoblockio/icon-tracker-frontend/issues/194) | Add new full pages for proposal and contract write  | open | 2023-03-08T12:30:07Z | | 
| [192](https://github.com/sudoblockio/icon-tracker-frontend/issues/192) | Initial wireframes  | open | 2023-03-08T12:18:26Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [73](https://github.com/sudoblockio/icon-transformer/pull/73) | chore(main): release 0.3.3 | closed | 2023-03-01T14:20:01Z | | 
| [72](https://github.com/sudoblockio/icon-transformer/pull/72) | Sort token transfers | closed | 2023-03-01T14:16:15Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [75](https://github.com/sudoblockio/icon-transformer/pull/75) | chore(main): release 0.3.4 | open | 2023-03-18T10:07:11Z | | 
| [74](https://github.com/sudoblockio/icon-transformer/issues/74) | Token address balance not including right decimals  | open | 2023-03-18T10:05:43Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [36](https://github.com/sudoblockio/icon-go-api/pull/36) | chore(main): release 0.4.4 | closed | 2023-03-14T10:57:16Z | | 
| [35](https://github.com/sudoblockio/icon-go-api/pull/35) | chore(main): release 0.4.3 | closed | 2023-03-01T14:19:34Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

Major issue in this service traxcked in transformer. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [7](https://github.com/sudoblockio/icon-contracts/issues/7) | ABI failing to show up  | closed | 2023-03-16T13:53:14Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [10](https://github.com/sudoblockio/icon-governance/pull/10) | chore(main): release 0.3.0 | closed | 2023-03-21T09:40:40Z | | 
| [8](https://github.com/sudoblockio/icon-governance/issues/8) | Make stats call async  | closed | 2023-03-08T19:29:52Z | | 
| [7](https://github.com/sudoblockio/icon-governance/pull/7) | chore(main): release 0.2.0 | closed | 2023-03-08T19:12:11Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [9](https://github.com/sudoblockio/icon-governance/issues/9) | Delegation under counting  | open | 2023-03-18T09:27:04Z | | 
| [6](https://github.com/sudoblockio/icon-governance/issues/6) | Delegation out of sync with some addresses that have un-delegated  | open | 2023-03-03T12:29:33Z | | 

### [icon-tracker](https://github.com/sudoblockio/icon-tracker)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [75](https://github.com/sudoblockio/icon-tracker/issues/75) | Link to Transformer and Go-API docs invalid | closed | 2023-03-15T18:45:45Z | | 
| [74](https://github.com/sudoblockio/icon-tracker/issues/74) | Status Page has NET::ERR_CERT_COMMON_NAME_INVALID | closed | 2023-03-15T18:43:00Z | | 
| [69](https://github.com/sudoblockio/icon-tracker/issues/69) | Problem with the showing number of voters | closed | 2023-01-12T11:00:33Z | | 


### [icon-extractor](https://github.com/sudoblockio/icon-extractor)

This is being rebuilt. 

### [tackle-icon-contract](https://github.com/sudoblockio/tackle-icon-contract)

This issue is being mentioned here as it has still to be funded. Working on this to derisk any funding an know exactly what is needed to make this successful. Generator works. Need to pull out some features and make a post about it and how people can contribute. Has been ready for funding  for a while and  it should be time to pull thee trigger on that soon. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [6](https://github.com/sudoblockio/tackle-icon-contract/pull/6) | Made IRC2 and Contract Module compile successfully | closed | 2023-03-30T10:26:10Z | | 
| [5](https://github.com/sudoblockio/tackle-icon-contract/pull/5) | Made IRC3/IRC31 compile successfully | closed | 2023-03-26T04:43:11Z | | 
| [4](https://github.com/sudoblockio/tackle-icon-contract/pull/4) | Changed contract folder link | closed | 2023-03-24T19:57:36Z | | 
| [2](https://github.com/sudoblockio/tackle-icon-contract/issues/2) | contract generation issue | closed | 2023-03-18T10:48:14Z | | 
| [3](https://github.com/sudoblockio/tackle-icon-contract/issues/3) | Make contracts compile  | closed | 2023-03-24T12:47:00Z | |

## Downtime Incidents

Major issue with reverse proxies was dealt with. Issue was with resources which were spiking up beyond reasonable expectations. Root cause is still being worked out with vendors. Still working on migration planning. 

- [Incidents](https://github.com/sudoblockio/icon-status-page/issues?page=1&q=)

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)