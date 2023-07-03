# Tracker Monthly Report

This is a progress update for 6/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month's focus was split between normal development activities and infrastructure work. Main things of note:

- Features lost from Rhizome will now be integrated into the tracker. Backend work is done for that and frontend work will start soon. 
- The CPS grant was finished which has setup a lot of work which will be covered through this grant and some that is out of scope such as major CSS changes across the tracker 
- Tackle improvements done that unblock a number of activities. At least 2 articles planned featuring applications in ICON. 
- Status page restored 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

Note: Many issues from the CPS proposal are mixed into this report. Main improvements made outside of CPS were in internal configuration setting management within the repo that prevented running on custom networks easily. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [281](https://github.com/sudoblockio/icon-tracker-frontend/issues/281) | Update footer to right repo | closed | 2023-06-29T13:49:32Z | | 
| [273](https://github.com/sudoblockio/icon-tracker-frontend/issues/273) | Update bonded logic / update form  | closed | 2023-06-15T12:54:28Z | | 
| [263](https://github.com/sudoblockio/icon-tracker-frontend/issues/263) | Pre-populate bonders with existing bonders  | closed | 2023-06-09T10:49:46Z | | 
| [261](https://github.com/sudoblockio/icon-tracker-frontend/issues/261) | Update prep functionalities with button css from contract tab  | closed | 2023-05-24T18:32:37Z | | 
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
| [282](https://github.com/sudoblockio/icon-tracker-frontend/issues/282) | July Sprint | open | 2023-07-01T09:06:19Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | open | 2023-03-08T20:34:13Z | | 
| [83](https://github.com/sudoblockio/icon-tracker-frontend/issues/83) | Show events tab in token detail view  | open | 2022-11-16T18:14:01Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

All backend APIs are developed to support the features lost from Rhizome turning off their tracker. Plan is to integrate them into the frontend this month. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- |--------| --- | --- |
| [17](https://github.com/sudoblockio/icon-governance/pull/17) | chore(main): release 0.4.0 | closed | 2023-06-29T13:47:58Z | | 
| [16](https://github.com/sudoblockio/icon-governance/issues/16) | Add cron to update `grade` of prep | closed | 2023-06-29T12:46:31Z | | 
| [18](https://github.com/sudoblockio/icon-governance/issues/18) | Add ICX per day calculation | closed | 2023-07-01T09:56:08Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [20](https://github.com/sudoblockio/icon-governance/issues/20) | Add alert manifold  | open | 2023-07-01T14:44:11Z | | 
| [19](https://github.com/sudoblockio/icon-governance/issues/19) | Put prep icons in bucket | open | 2023-07-01T13:14:53Z | | 

## Infrastructure Update 

Updates on the status of the migration to be discussed during meeting. Current plans have changed with large savings in operating expenses. Interim migration is underway. 

## Downtime Incidents

No downtime to report. 
> Report generated with [tackle](https://github.com/robcxyz/tackle-box)