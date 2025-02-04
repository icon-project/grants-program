# Tracker Monthly Report

This is a progress update for 1/2025 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month saw the finalization of the infrastructure migration and getting up to date with the backlog on the frontend. On the infrastructure, we realized we needed to install more ram which requires a server restart. We also used the opportunity to redeploy one of our two active clusters and fix some prior mistakes we had made in configurations. 

On the dev side, we're finally now fully catching up on issues and honestly apologize for letting some issues go unanswered for a couple week period on the tracker frontend. Atif who manages our frontend has joined full time so going forward his notifications should catch issues quicker. As you can see below, lots of issues being cleared many of which we're now able to raise ourselves from better integration with sentry, a front-end observability platform that has been helping a lot lately. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [530](https://github.com/sudoblockio/icon-tracker-frontend/pull/530) | fix: added APR column to governance page #513 | closed | 2025-02-03T17:49:46Z | | 
| [528](https://github.com/sudoblockio/icon-tracker-frontend/issues/528) | Improper event log parsing | closed | 2025-01-21T12:30:06Z | | 
| [526](https://github.com/sudoblockio/icon-tracker-frontend/pull/526) | Bugs | closed | 2025-01-20T14:10:45Z | | 
| [523](https://github.com/sudoblockio/icon-tracker-frontend/pull/523) | fix: sentry environment | closed | 2025-01-17T11:34:02Z | | 
| [522](https://github.com/sudoblockio/icon-tracker-frontend/pull/522) | Bugs | closed | 2025-01-16T07:13:46Z | | 
| [521](https://github.com/sudoblockio/icon-tracker-frontend/issues/521) | Intermittent white screen when logging in | closed | 2025-01-15T02:43:14Z | | 
| [520](https://github.com/sudoblockio/icon-tracker-frontend/issues/520) | Undefined in event field name | closed | 2025-01-15T01:33:05Z | | 
| [519](https://github.com/sudoblockio/icon-tracker-frontend/pull/519) | Bugs | closed | 2025-01-09T12:52:01Z | | 
| [518](https://github.com/sudoblockio/icon-tracker-frontend/pull/518) | chore(main): release 0.6.4 | closed | 2025-01-08T18:48:25Z | | 
| [517](https://github.com/sudoblockio/icon-tracker-frontend/issues/517) | One addresses with token counts above 25, the page jams up and takes a while to load | closed | 2025-01-08T17:54:50Z | | 
| [515](https://github.com/sudoblockio/icon-tracker-frontend/issues/515) | title | closed | 2025-01-07T08:58:23Z | | 
| [514](https://github.com/sudoblockio/icon-tracker-frontend/issues/514) | Speed up governance page load  | closed | 2024-12-09T17:49:55Z | | 
| [507](https://github.com/sudoblockio/icon-tracker-frontend/issues/507) | Modify the the config to accept more backends  | closed | 2024-11-20T06:12:20Z | | 
| [495](https://github.com/sudoblockio/icon-tracker-frontend/issues/495) | Transaction events | closed | 2024-09-19T09:26:52Z | | 
| [478](https://github.com/sudoblockio/icon-tracker-frontend/issues/478) | add support to identify payable methods in an arbitrary contract and add an extra field called "value" to add the amount of ICX to be transferred | closed | 2024-08-16T04:38:27Z | | 
| [477](https://github.com/sudoblockio/icon-tracker-frontend/issues/477) | Signing registerPRep method of chain contract on the tracker fails due to invalid registration fee | closed | 2024-08-16T04:21:52Z | | 
| [469](https://github.com/sudoblockio/icon-tracker-frontend/issues/469) | Using sentry for frontend logs | closed | 2024-07-16T19:14:12Z | | 
| [465](https://github.com/sudoblockio/icon-tracker-frontend/issues/465) | Change login flow + add options drop down  | closed | 2024-07-03T15:17:43Z | | 
| [449](https://github.com/sudoblockio/icon-tracker-frontend/issues/449) | Make site title dynamic according to the page | closed | 2024-05-12T05:25:13Z | | 
| [435](https://github.com/sudoblockio/icon-tracker-frontend/issues/435) | Provide icx value input in contract explorer | closed | 2024-03-27T15:10:47Z | | 
| [432](https://github.com/sudoblockio/icon-tracker-frontend/issues/432) | Create a generic error boundary page  | closed | 2024-03-25T16:41:00Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | April Sprint  | closed | 2024-03-10T07:03:17Z | | 
| [411](https://github.com/sudoblockio/icon-tracker-frontend/issues/411) | Display token balances for contracts | closed | 2024-03-04T07:49:54Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | December Sprint | closed | 2023-11-01T08:00:51Z | | 
| [323](https://github.com/sudoblockio/icon-tracker-frontend/issues/323) | October Sprint | closed | 2023-09-17T09:02:23Z | | 
| [282](https://github.com/sudoblockio/icon-tracker-frontend/issues/282) | July Sprint | closed | 2023-07-01T09:06:19Z | | 
| [239](https://github.com/sudoblockio/icon-tracker-frontend/issues/239) | Include delegations and other data for contracts  | closed | 2023-04-21T21:56:31Z | | 
| [232](https://github.com/sudoblockio/icon-tracker-frontend/issues/232) | April Sprint | closed | 2023-04-03T16:20:36Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | closed | 2023-03-08T20:34:13Z | | 
| [165](https://github.com/sudoblockio/icon-tracker-frontend/issues/165) | February Sprint | closed | 2023-02-04T13:16:37Z | | 
| [151](https://github.com/sudoblockio/icon-tracker-frontend/issues/151) | Remove duplicate `/api/v1/contracts/<addr>` calls | closed | 2023-01-24T12:01:33Z | | 
| [103](https://github.com/sudoblockio/icon-tracker-frontend/issues/103) | January Sprint | closed | 2023-01-04T12:52:24Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [529](https://github.com/sudoblockio/icon-tracker-frontend/pull/529) | Apr column | open | 2025-02-03T17:48:26Z | | 
| [527](https://github.com/sudoblockio/icon-tracker-frontend/pull/527) | chore(main): release 0.6.5 | open | 2025-01-20T14:11:24Z | | 
| [525](https://github.com/sudoblockio/icon-tracker-frontend/issues/525) | Validate that the new global bond rate value is reflected in the governance page | open | 2025-01-20T13:18:08Z | | 
| [524](https://github.com/sudoblockio/icon-tracker-frontend/issues/524) | Jan Sprint | open | 2025-01-20T12:11:35Z | | 
| [516](https://github.com/sudoblockio/icon-tracker-frontend/issues/516) | Transient issue with displaying time to unstaking  | open | 2025-01-08T16:13:53Z | | 
| [502](https://github.com/sudoblockio/icon-tracker-frontend/issues/502) | Prioritized Backlog | open | 2024-10-06T09:40:07Z | | 
| [490](https://github.com/sudoblockio/icon-tracker-frontend/issues/490) | contract method with param of type []string fail when trying to call on the the tracker | open | 2024-09-13T20:36:22Z | | 
| [413](https://github.com/sudoblockio/icon-tracker-frontend/issues/413) | Get contract data showing for berlin   | open | 2024-03-05T17:29:13Z | | 
| [394](https://github.com/sudoblockio/icon-tracker-frontend/issues/394) | after voting on a network proposal, trying to change the vote doesnt work | open | 2024-02-05T00:54:20Z | | 
| [351](https://github.com/sudoblockio/icon-tracker-frontend/issues/351) | Token sending tab in token / address view  | open | 2023-10-31T14:38:50Z | | 
| [322](https://github.com/sudoblockio/icon-tracker-frontend/issues/322) | Running failed tx in Contract tab returns hash seeming success - should be failure  | open | 2023-09-16T18:05:03Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [80](https://github.com/sudoblockio/icon-transformer/issues/80) | restart observed | open | 2025-01-17T11:03:00Z | | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)


#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [56](https://github.com/sudoblockio/icon-go-api/issues/56) | stats not ready causes crash it seems | open | 2025-01-25T01:42:12Z | | 
| [55](https://github.com/sudoblockio/icon-go-api/issues/55) | restarts observed. | open | 2025-01-17T10:49:34Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)


#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [16](https://github.com/sudoblockio/icon-contracts/pull/16) | chore(main): release 0.2.6 | open | 2024-11-20T04:59:00Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [61](https://github.com/sudoblockio/icon-governance/pull/61) | fix: updated bond_percent formula #60 | closed | 2025-02-01T19:35:31Z | | 
| [53](https://github.com/sudoblockio/icon-governance/pull/53) | Bump pydantic | closed | 2024-11-09T06:15:58Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [60](https://github.com/sudoblockio/icon-governance/issues/60) | Update bond_percent formula | open | 2025-02-01T19:34:34Z | | 
| [59](https://github.com/sudoblockio/icon-governance/issues/59) | lisbon governance cron failing - int overflow | open | 2025-02-01T06:17:19Z | | 
| [58](https://github.com/sudoblockio/icon-governance/issues/58) | Type coercion from prior response to scientific notation | open | 2025-01-13T20:45:51Z | | 
| [56](https://github.com/sudoblockio/icon-governance/pull/56) | chore(main): release 0.10.6 | open | 2024-11-14T11:27:06Z | | 
| [52](https://github.com/sudoblockio/icon-governance/issues/52) | Update sqlmodel / pydantic / fastapi / sqlalchemy so that alembic does not create a diff  | open | 2024-11-08T07:07:12Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [80](https://github.com/balancednetwork/balanced-backend/issues/80) | Looks like issue with sicx:icx chart but pool is actually depleted | open | 2025-02-02T05:03:13Z | | 
| [78](https://github.com/balancednetwork/balanced-backend/pull/78) | chore(main): release 0.8.4 | open | 2024-11-21T09:16:44Z | | 

### [icon-stats](https://github.com/sudoblockio/icon-stats)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [19](https://github.com/sudoblockio/icon-stats/pull/19) | Bump pydantic | closed | 2024-11-30T08:53:20Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [23](https://github.com/sudoblockio/icon-stats/issues/23) | Stuck migration | open | 2025-01-14T07:24:43Z | | 
| [18](https://github.com/sudoblockio/icon-stats/pull/18) | chore(main): release 0.2.7 | open | 2024-11-30T06:09:52Z | | 


## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| ~Jan 20th | ~1 week Berlin RPC (more explanation below) | Operator error | Fixed config |

This was somehow missed as we were doing our migrations, the RPC endpoint for berlin seems to have been misconfigured though the tracker stayed working and at head. This is odd and only known through alarm which seems to have been silenced and never addressed. Only RPC was affected and no reports came of any issues so it is possible the alarm was simply not configured properly and this was not a real incident but unlikely. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)