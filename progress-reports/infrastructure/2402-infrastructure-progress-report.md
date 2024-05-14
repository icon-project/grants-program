# Tracker Monthly Report

This is a progress update for 1/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary


This past month saw a number of issues related to upgrading the tracker and backend for IISS v4, infrastructure migration activities, steady work on the new stats service, and progress on a new client for the new backend being slowly worked on. Issues related to IISS v4 are all in place with fixes to smooth the transition to having access to all the data such as jail and commission. On the infrastructure migration, VM and kubernetes setup code has been created and tested. Working on clearing out some dev backlog before getting them installed in the coming weeks with the servers coming online a few weeks after that. Stats service has been seeing a lot of attention as we broadly are working out a pattern for rebuilding all of our http clients. New clients will be async, have pluggable middleware, and a pydantic validated output. This will then allow for a local cache of ABIs and a decoder for events / client generator for ABIs. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [393](https://github.com/sudoblockio/icon-tracker-frontend/pull/393) | chore(main): release 0.4.2 | closed | 2024-02-02T20:45:20Z | | 
| [392](https://github.com/sudoblockio/icon-tracker-frontend/pull/392) | fix: fixed breaking css styles in governance page | closed | 2024-02-01T23:44:49Z | | 
| [391](https://github.com/sudoblockio/icon-tracker-frontend/pull/391) | changed default values for initCommissionRate and setCommissionRate  | closed | 2024-02-01T21:56:58Z | | 
| [390](https://github.com/sudoblockio/icon-tracker-frontend/pull/390) | chore(main): release 0.4.1 | closed | 2024-02-01T17:30:18Z | | 
| [388](https://github.com/sudoblockio/icon-tracker-frontend/pull/388) | #chore: for #364 fixed the spacing | closed | 2024-01-23T08:29:43Z | | 
| [387](https://github.com/sudoblockio/icon-tracker-frontend/pull/387) | chore: updated #362 and #364 | closed | 2024-01-23T06:18:04Z | | 
| [386](https://github.com/sudoblockio/icon-tracker-frontend/pull/386) | chore: adding dependecy files for Linting | closed | 2024-01-23T05:18:28Z | | 
| [385](https://github.com/sudoblockio/icon-tracker-frontend/pull/385) | Add jail badges to address page | closed | 2024-01-22T06:19:41Z | | 
| [384](https://github.com/sudoblockio/icon-tracker-frontend/pull/384) | Add jail badges to governance table | closed | 2024-01-22T06:19:28Z | | 
| [383](https://github.com/sudoblockio/icon-tracker-frontend/pull/383) | fix: conditional around showing the unjail button | closed | 2024-01-22T03:57:53Z | | 
| [382](https://github.com/sudoblockio/icon-tracker-frontend/issues/382) | Update logic for governance page node status and state  | closed | 2024-01-21T17:58:32Z | | 
| [381](https://github.com/sudoblockio/icon-tracker-frontend/pull/381) | Iiss4 update. Merge fix | closed | 2024-01-20T01:43:36Z | | 
| [380](https://github.com/sudoblockio/icon-tracker-frontend/pull/380) | IISS v2 | closed | 2024-01-19T02:53:03Z | | 
| [379](https://github.com/sudoblockio/icon-tracker-frontend/pull/379) | fixing merge issues | closed | 2024-01-18T19:52:40Z | | 
| [378](https://github.com/sudoblockio/icon-tracker-frontend/pull/378) | chore: updated #366 #368 #370 and #369 | closed | 2024-01-18T17:46:24Z | | 
| [377](https://github.com/sudoblockio/icon-tracker-frontend/pull/377) | IISS 4 Updates  | closed | 2024-01-18T05:54:46Z | | 
| [376](https://github.com/sudoblockio/icon-tracker-frontend/pull/376) | chore(main): release 0.4.0 | closed | 2024-01-18T03:00:04Z | | 
| [375](https://github.com/sudoblockio/icon-tracker-frontend/pull/375) | Add request unjail feature | closed | 2024-01-11T22:57:56Z | | 
| [374](https://github.com/sudoblockio/icon-tracker-frontend/pull/374) | chore(main): release 0.3.5 | closed | 2024-01-10T19:30:15Z | | 
| [372](https://github.com/sudoblockio/icon-tracker-frontend/issues/372) | signing contract method of type []Address adds invalid characters  | closed | 2024-01-10T12:37:20Z | | 
| [371](https://github.com/sudoblockio/icon-tracker-frontend/issues/371) | Change order of wallets in login - Hana | ICONex | closed | 2024-01-08T18:36:44Z | | 
| [370](https://github.com/sudoblockio/icon-tracker-frontend/issues/370) | Add discord logo to footer | closed | 2024-01-08T18:32:35Z | | 
| [369](https://github.com/sudoblockio/icon-tracker-frontend/issues/369) | Change "Contact Us" to "Get Support" on footer | closed | 2024-01-08T18:31:42Z | | 
| [368](https://github.com/sudoblockio/icon-tracker-frontend/issues/368) | Remove "Support & request to add the token homepage URL" from footer | closed | 2024-01-08T18:30:35Z | | 
| [367](https://github.com/sudoblockio/icon-tracker-frontend/pull/367) | chore: added feature for #363 | closed | 2024-01-08T01:34:26Z | | 
| [366](https://github.com/sudoblockio/icon-tracker-frontend/issues/366) | Copyright year should update based on date | closed | 2024-01-07T18:25:10Z | | 
| [365](https://github.com/sudoblockio/icon-tracker-frontend/issues/365) | Voter reward rate broken on Berlin | closed | 2024-01-04T04:06:59Z | | 
| [364](https://github.com/sudoblockio/icon-tracker-frontend/issues/364) | New row in governance table  | closed | 2024-01-04T04:05:06Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [394](https://github.com/sudoblockio/icon-tracker-frontend/issues/394) | after voting on a network proposal, trying to change the vote doesnt work | open | 2024-02-05T00:54:20Z | | 
| [389](https://github.com/sudoblockio/icon-tracker-frontend/pull/389) | feat: add initial tools drop down #373 | open | 2024-01-29T05:59:56Z | | 
| [373](https://github.com/sudoblockio/icon-tracker-frontend/issues/373) | Tools drop down  | open | 2024-01-10T19:01:52Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [39](https://github.com/sudoblockio/icon-governance/pull/39) | chore(main): release 0.7.5 | closed | 2024-02-04T08:01:27Z | | 
| [38](https://github.com/sudoblockio/icon-governance/pull/38) | chore(main): release 0.7.4 | closed | 2024-02-02T20:55:54Z | | 
| [37](https://github.com/sudoblockio/icon-governance/pull/37) | chore(main): release 0.7.3 | closed | 2024-02-02T09:39:30Z | | 
| [36](https://github.com/sudoblockio/icon-governance/pull/36) | chore(main): release 0.7.2 | closed | 2024-02-01T17:40:43Z | | 
| [35](https://github.com/sudoblockio/icon-governance/pull/35) | chore(main): release 0.7.1 | closed | 2024-01-09T23:02:12Z | | 
| [33](https://github.com/sudoblockio/icon-governance/pull/33) | chore(main): release 0.7.0 | closed | 2023-12-27T23:05:15Z | | 
| [32](https://github.com/sudoblockio/icon-governance/issues/32) | Update `preps` table with new IISS attributes  | closed | 2023-12-27T23:02:10Z | | 
| [31](https://github.com/sudoblockio/icon-governance/issues/31) | apy time crashing in testnets  | closed | 2023-12-08T13:00:48Z | | 
| [30](https://github.com/sudoblockio/icon-governance/issues/30) | Update CPS rpc calls  | closed | 2023-11-15T16:54:30Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [34](https://github.com/sudoblockio/icon-governance/issues/34) | Fix the status and IP discovery on testnets to test iiss 4  | open | 2024-01-09T22:53:34Z | | 


## Downtime Incidents

None 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)