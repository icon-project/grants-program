# Tracker Monthly Report

This is a progress update for 7/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month saw the completion of the migration to larger servers where separate discussions will take place about future directions. The focus of this report is thus on some of the upgrades happening in the tracker frontend where we are in the middle of upgrading to a modern react. 

Little background on the tracker frontend, it was originally generated from create-react-app over 5 years ago with basically no major changes to the tool chain. This has led to some build issues in the past and is projected to only get worse as we are using versions of packages that are no longer supported. Additionally it prevents us from using packages that are needed for ledger integration which is blocked by using a old version of webpack. We've always been wanting to upgrade the tool chain but were hesitant considering the size of the change. 

We are happy to report though that we have upgraded the tracker using the create react app version 5 template [in a branch](https://github.com/sudoblockio/icon-tracker-frontend/tree/cra5-update) keeping a [worklog of the changes](https://github.com/sudoblockio/icon-tracker-frontend/blob/cra5-update/UPDATE_ISSUES.md). So far we still have some issues with the e2e tests which might need to be updated but in general it is currently working with minor issues to be fixed. This is a big win thanks to Fidel requiring moving all the old code into the new template. So far about 50 dependencies have been removed and 7 new dependencies added. In general though, this will make the tracker far more maintainable and set the table for additional long term house keeping tasks that we have been contemplating such as: 

- Upgrading to react 18
- Refactoring much of the code from class based to functional components 
- Updating the CSS to reflect the wireframes we built in the last CPS grant 

A potential discussion offline could be had about the long term plans for the tracker. 

It also should be noted we brought on an additional dev on the frontend. Fidel will be working on broader changes where as the new dev will be handling day to day issues.  

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

We did a lot of issue house keeping this month so a lot of old issues were closed. Several bugs were dealt with along with features brought over from the Rhizome tracker. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [298](https://github.com/sudoblockio/icon-tracker-frontend/pull/298) | Cra5 update | closed | 2023-07-31T11:59:17Z | | 
| [296](https://github.com/sudoblockio/icon-tracker-frontend/pull/296) | fix: make contracts that stake clickable #278 | closed | 2023-07-27T16:23:08Z | | 
| [295](https://github.com/sudoblockio/icon-tracker-frontend/pull/295) | chore: add ICX per day to governance #271 | closed | 2023-07-25T15:02:13Z | | 
| [294](https://github.com/sudoblockio/icon-tracker-frontend/pull/294) | chore(main): release 0.2.20 | closed | 2023-07-25T14:34:54Z | | 
| [293](https://github.com/sudoblockio/icon-tracker-frontend/pull/293) | fix: add reward column to governance table #271 | closed | 2023-07-25T14:28:18Z | | 
| [292](https://github.com/sudoblockio/icon-tracker-frontend/pull/292) | chore: added "Bonded %" to governance tab #270 | closed | 2023-07-24T17:52:08Z | | 
| [289](https://github.com/sudoblockio/icon-tracker-frontend/pull/289) | chore: fix #288 | closed | 2023-07-24T11:09:44Z | | 
| [288](https://github.com/sudoblockio/icon-tracker-frontend/issues/288) | frontend breaks when entering contract tab on specific contract | closed | 2023-07-24T11:00:52Z | | 
| [287](https://github.com/sudoblockio/icon-tracker-frontend/pull/287) | chore: linked address opens in new tab | closed | 2023-07-22T12:06:02Z | | 
| [283](https://github.com/sudoblockio/icon-tracker-frontend/pull/283) | chore(main): release 0.2.19 | closed | 2023-07-04T07:36:50Z | | 
| [281](https://github.com/sudoblockio/icon-tracker-frontend/issues/281) | Update footer to right repo | closed | 2023-06-29T13:49:32Z | | 
| [279](https://github.com/sudoblockio/icon-tracker-frontend/issues/279) | Make sortable tables more clear | closed | 2023-06-21T19:11:55Z | | 
| [278](https://github.com/sudoblockio/icon-tracker-frontend/issues/278) | Make contracts that stake clickable   | closed | 2023-06-21T19:04:35Z | | 
| [275](https://github.com/sudoblockio/icon-tracker-frontend/issues/275) | Clicking on delegations address is opening in new tab | closed | 2023-06-21T11:44:23Z | | 
| [273](https://github.com/sudoblockio/icon-tracker-frontend/issues/273) | Update bonded logic / update form  | closed | 2023-06-15T12:54:28Z | | 
| [271](https://github.com/sudoblockio/icon-tracker-frontend/issues/271) | Add ICX per day to governance  | closed | 2023-06-14T11:47:42Z | | 
| [270](https://github.com/sudoblockio/icon-tracker-frontend/issues/270) | Add "Bonded %" to governance tab  | closed | 2023-06-14T11:46:14Z | | 
| [263](https://github.com/sudoblockio/icon-tracker-frontend/issues/263) | Pre-populate bonders with existing bonders  | closed | 2023-06-09T10:49:46Z | | 
| [261](https://github.com/sudoblockio/icon-tracker-frontend/issues/261) | Update prep functionalities with button css from contract tab  | closed | 2023-05-24T18:32:37Z | | 
| [260](https://github.com/sudoblockio/icon-tracker-frontend/issues/260) | Change network on the bottom right when in a testnet  | closed | 2023-05-24T18:12:39Z | | 
| [252](https://github.com/sudoblockio/icon-tracker-frontend/issues/252) | Refactor tests into convention  | closed | 2023-04-23T19:28:35Z | | 
| [244](https://github.com/sudoblockio/icon-tracker-frontend/issues/244) | Setting up bonder list page  | closed | 2023-04-22T22:29:29Z | | 
| [243](https://github.com/sudoblockio/icon-tracker-frontend/issues/243) | Setting up vote page  | closed | 2023-04-22T22:29:14Z | | 
| [242](https://github.com/sudoblockio/icon-tracker-frontend/issues/242) | Setting up proposals full page  | closed | 2023-04-22T22:29:01Z | | 
| [241](https://github.com/sudoblockio/icon-tracker-frontend/issues/241) | Setting up full page contract  | closed | 2023-04-22T22:28:06Z | | 
| [238](https://github.com/sudoblockio/icon-tracker-frontend/issues/238) | Cleanout all references to configJson | closed | 2023-04-21T18:21:23Z | | 
| [232](https://github.com/sudoblockio/icon-tracker-frontend/issues/232) | April Sprint | closed | 2023-04-03T16:20:36Z | | 
| [230](https://github.com/sudoblockio/icon-tracker-frontend/issues/230) | popup window for updating bonders list | closed | 2023-03-27T12:27:13Z | | 
| [229](https://github.com/sudoblockio/icon-tracker-frontend/issues/229) | popup window for updating prep details | closed | 2023-03-27T12:25:35Z | | 
| [223](https://github.com/sudoblockio/icon-tracker-frontend/issues/223) | Prep functionalities and forms functionalities  | closed | 2023-03-21T23:30:26Z | | 
| [222](https://github.com/sudoblockio/icon-tracker-frontend/issues/222) | Proposals wireframes  | closed | 2023-03-21T23:30:07Z | | 
| [219](https://github.com/sudoblockio/icon-tracker-frontend/issues/219) | Modify `config.js` so that we can run locally on each network  | closed | 2023-03-20T16:03:32Z | | 
| [213](https://github.com/sudoblockio/icon-tracker-frontend/pull/213) | Fixed broken commits due to dependencies bugs | closed | 2023-03-16T03:32:56Z | | 
| [209](https://github.com/sudoblockio/icon-tracker-frontend/pull/209) | fix to #200 | closed | 2023-03-10T23:57:01Z | | 
| [208](https://github.com/sudoblockio/icon-tracker-frontend/issues/208) | Bonded address opens in new tab  | closed | 2023-03-10T11:43:42Z | | 
| [194](https://github.com/sudoblockio/icon-tracker-frontend/issues/194) | Add new full pages for proposal and contract write  | closed | 2023-03-08T12:30:07Z | | 
| [193](https://github.com/sudoblockio/icon-tracker-frontend/issues/193) | EPIC: Contract Write Meta  | closed | 2023-03-08T12:19:25Z | | 
| [192](https://github.com/sudoblockio/icon-tracker-frontend/issues/192) | Initial wireframes  | closed | 2023-03-08T12:18:26Z | | 
| [167](https://github.com/sudoblockio/icon-tracker-frontend/issues/167) | Update build scripts  | closed | 2023-02-04T17:00:54Z | | 
| [166](https://github.com/sudoblockio/icon-tracker-frontend/issues/166) | Update readme with new build instructions  | closed | 2023-02-04T17:00:38Z | | 
| [165](https://github.com/sudoblockio/icon-tracker-frontend/issues/165) | February Sprint | closed | 2023-02-04T13:16:37Z | | 
| [103](https://github.com/sudoblockio/icon-tracker-frontend/issues/103) | January Sprint | closed | 2023-01-04T12:52:24Z | | 
| [102](https://github.com/sudoblockio/icon-tracker-frontend/issues/102) | Design new contracts read tab setting up for write tab | closed | 2023-01-04T12:52:14Z | | 
| [93](https://github.com/sudoblockio/icon-tracker-frontend/issues/93) | December sprint | closed | 2022-12-07T12:12:37Z | | 
| [72](https://github.com/sudoblockio/icon-tracker-frontend/issues/72) | Update the Read Contract section  | closed | 2022-10-18T04:20:41Z | | 
| [71](https://github.com/sudoblockio/icon-tracker-frontend/issues/71) | November Sprint | closed | 2022-10-18T04:13:54Z | | 
| [58](https://github.com/sudoblockio/icon-tracker-frontend/issues/58) | Sort bonder list and formatting | closed | 2022-07-25T20:15:43Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [301](https://github.com/sudoblockio/icon-tracker-frontend/pull/301) | fix: "read contract" tab in tokens not working #284 | open | 2023-08-03T18:28:40Z | | 
| [300](https://github.com/sudoblockio/icon-tracker-frontend/issues/300) | Tools section | open | 2023-08-03T15:21:14Z | | 
| [299](https://github.com/sudoblockio/icon-tracker-frontend/issues/299) | Tx trace logsfor failed txs doesn't work - no error msg | open | 2023-07-31T14:30:27Z | | 
| [297](https://github.com/sudoblockio/icon-tracker-frontend/pull/297) | chore(main): release 0.2.21 | open | 2023-07-27T16:29:13Z | | 
| [291](https://github.com/sudoblockio/icon-tracker-frontend/pull/291) | Added light and dark mode | open | 2023-07-24T11:26:01Z | | 
| [290](https://github.com/sudoblockio/icon-tracker-frontend/issues/290) | Empty abi produces weird output  | open | 2023-07-24T11:15:35Z | | 
| [285](https://github.com/sudoblockio/icon-tracker-frontend/issues/285) | Bonded tab shows by default  | open | 2023-07-14T14:00:10Z | | 
| [284](https://github.com/sudoblockio/icon-tracker-frontend/issues/284) | "Read Contract" tab in tokens not working  | open | 2023-07-09T11:03:01Z | | 
| [282](https://github.com/sudoblockio/icon-tracker-frontend/issues/282) | July Sprint | open | 2023-07-01T09:06:19Z | | 
| [205](https://github.com/sudoblockio/icon-tracker-frontend/issues/205) | In `/token/<>` there is no transactions tab  | open | 2023-03-09T10:36:32Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | open | 2023-03-08T20:34:13Z | | 
| [83](https://github.com/sudoblockio/icon-tracker-frontend/issues/83) | Show events tab in token detail view  | open | 2022-11-16T18:14:01Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [8](https://github.com/sudoblockio/icon-contracts/issues/8) | Contract code is not updated in community tracker | open | 2023-07-15T18:45:31Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [17](https://github.com/sudoblockio/icon-governance/pull/17) | chore(main): release 0.4.0 | closed | 2023-06-29T13:47:58Z | | 
| [16](https://github.com/sudoblockio/icon-governance/issues/16) | Add cron to update `grade` of prep | closed | 2023-06-29T12:46:31Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [20](https://github.com/sudoblockio/icon-governance/issues/20) | Add alert manifold  | open | 2023-07-01T14:44:11Z | | 
| [19](https://github.com/sudoblockio/icon-governance/issues/19) | Put prep icons in bucket | open | 2023-07-01T13:14:53Z | | 
| [18](https://github.com/sudoblockio/icon-governance/issues/18) | Add ICX per day calculation | open | 2023-07-01T09:56:08Z | | 

## Dev Ops 

The migration is now complete to new servers. Too many issues to lay out in this report to outline what happened to get here but suffice to say it was a major endeavor. DBs though are now on machines that will be able to run through 2024. Discussion offline will be around a more cost effective / higher capacity solution. 

Currently fighting some DB tuning issues as I am getting an inordinate amount of cache misses / slow queries. Doesn't seem to impact user experience much but can see effects when doing cache recovery operations. 

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution                                          |
|------|--------------------------------------|------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| 8/2  | 15 min of keeping at head on indexer | DB needed a restart due to nearing free disk space (did not exceed it but for some reason hung up one block because of this. | Switched off zone, restarted DB, brought back zone. |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)