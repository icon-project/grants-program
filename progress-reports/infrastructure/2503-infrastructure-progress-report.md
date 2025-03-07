# Tracker Monthly Report

This is a progress update for 2/2025 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

Several items were done on the backend with nothing major to report with the main focus being on the frontend where this past month we brought on a new frontend dev who did a lot of catching up on issues as you can see from the number of issues that were closed. We also spent time reviewing many alerts from sentry (a frontend observability tool) as we started instrumenting the tracker more with this tool. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [559](https://github.com/sudoblockio/icon-tracker-frontend/pull/559) | fix: payable method added extra value field below data.params field #435 | closed | 2025-02-21T08:49:48Z | | 
| [558](https://github.com/sudoblockio/icon-tracker-frontend/pull/558) | chore(main): release 0.6.7 | closed | 2025-02-20T11:03:34Z | | 
| [557](https://github.com/sudoblockio/icon-tracker-frontend/pull/557) | Apr column | closed | 2025-02-20T11:02:51Z | | 
| [555](https://github.com/sudoblockio/icon-tracker-frontend/pull/555) | chore(main): release 0.6.6 | closed | 2025-02-17T10:27:56Z | | 
| [554](https://github.com/sudoblockio/icon-tracker-frontend/issues/554) | Account for Bonded ICX while voting | closed | 2025-02-17T09:50:42Z | | 
| [553](https://github.com/sudoblockio/icon-tracker-frontend/issues/553) | Address page shows wrong 'Voted' amount | closed | 2025-02-17T08:26:44Z | | 
| [549](https://github.com/sudoblockio/icon-tracker-frontend/pull/549) | chore: updated api docs link #547 | closed | 2025-02-17T06:39:37Z | | 
| [548](https://github.com/sudoblockio/icon-tracker-frontend/issues/548) | Issue with staking % not updating | closed | 2025-02-16T05:14:07Z | | 
| [547](https://github.com/sudoblockio/icon-tracker-frontend/issues/547) | Make redirect to API docs go to the same domain as being served - right now goes to cluster1 | closed | 2025-02-14T07:25:33Z | | 
| [543](https://github.com/sudoblockio/icon-tracker-frontend/pull/543) | chore: empty abi UI glitch #290 | closed | 2025-02-06T11:28:45Z | | 
| [542](https://github.com/sudoblockio/icon-tracker-frontend/pull/542) | Search contract name | closed | 2025-02-05T19:14:26Z | | 
| [540](https://github.com/sudoblockio/icon-tracker-frontend/pull/540) | fix: fixed improper log parsing in contract and transactions #528 | closed | 2025-02-05T13:38:48Z | | 
| [538](https://github.com/sudoblockio/icon-tracker-frontend/issues/538) | Undefined in event log with known ABI | closed | 2025-02-04T20:50:31Z | | 
| [537](https://github.com/sudoblockio/icon-tracker-frontend/pull/537) | fix: sentry optimisation #536 | closed | 2025-02-04T14:44:49Z | | 
| [536](https://github.com/sudoblockio/icon-tracker-frontend/issues/536) | Optimise sentry logging | closed | 2025-02-04T12:36:34Z | | 
| [535](https://github.com/sudoblockio/icon-tracker-frontend/pull/535) | chore: updated all instances of p-reps with validators #446 | closed | 2025-02-04T12:32:19Z | | 
| [534](https://github.com/sudoblockio/icon-tracker-frontend/pull/534) | Prep validator update | closed | 2025-02-04T12:23:55Z | | 
| [533](https://github.com/sudoblockio/icon-tracker-frontend/pull/533) | Add gov info | closed | 2025-02-04T12:06:47Z | | 
| [532](https://github.com/sudoblockio/icon-tracker-frontend/pull/532) | Bugs | closed | 2025-02-04T12:02:06Z | | 
| [531](https://github.com/sudoblockio/icon-tracker-frontend/issues/531) | Update API docs links in tools dropdown | closed | 2025-02-04T12:00:40Z | | 
| [530](https://github.com/sudoblockio/icon-tracker-frontend/pull/530) | fix: added APR column to governance page #513 | closed | 2025-02-03T17:49:46Z | | 
| [529](https://github.com/sudoblockio/icon-tracker-frontend/pull/529) | Apr column | closed | 2025-02-03T17:48:26Z | | 
| [528](https://github.com/sudoblockio/icon-tracker-frontend/issues/528) | Improper event log parsing | closed | 2025-01-21T12:30:06Z | | 
| [527](https://github.com/sudoblockio/icon-tracker-frontend/pull/527) | chore(main): release 0.6.5 | closed | 2025-01-20T14:11:24Z | | 
| [496](https://github.com/sudoblockio/icon-tracker-frontend/issues/496) | Empty event objects in contract event logs | closed | 2024-09-19T09:28:19Z | | 
| [491](https://github.com/sudoblockio/icon-tracker-frontend/issues/491) | Duplicate synchronous REST API calls /governance/preps in governance page | closed | 2024-09-17T15:54:24Z | | 
| [490](https://github.com/sudoblockio/icon-tracker-frontend/issues/490) | contract method with param of type []string fail when trying to call on the the tracker | closed | 2024-09-13T20:36:22Z | | 
| [459](https://github.com/sudoblockio/icon-tracker-frontend/issues/459) | Bond amount not showing in address view | closed | 2024-06-19T12:37:11Z | | 
| [446](https://github.com/sudoblockio/icon-tracker-frontend/issues/446) | Scrub "P-Rep" from tracker and replace with "Validator" | closed | 2024-05-03T18:56:31Z | | 
| [435](https://github.com/sudoblockio/icon-tracker-frontend/issues/435) | Provide icx value input in contract explorer | closed | 2024-03-27T15:10:47Z | | 
| [430](https://github.com/sudoblockio/icon-tracker-frontend/pull/430) | chore: Info popup governance styling | closed | 2024-03-22T18:52:07Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | April Sprint  | closed | 2024-03-10T07:03:17Z | | 
| [408](https://github.com/sudoblockio/icon-tracker-frontend/issues/408) | Add pop-ups to governance page  | closed | 2024-02-21T02:04:25Z | | 
| [352](https://github.com/sudoblockio/icon-tracker-frontend/issues/352) | December Sprint | closed | 2023-11-01T08:00:51Z | | 
| [323](https://github.com/sudoblockio/icon-tracker-frontend/issues/323) | October Sprint | closed | 2023-09-17T09:02:23Z | | 
| [290](https://github.com/sudoblockio/icon-tracker-frontend/issues/290) | Empty abi produces weird output  | closed | 2023-07-24T11:15:35Z | | 
| [282](https://github.com/sudoblockio/icon-tracker-frontend/issues/282) | July Sprint | closed | 2023-07-01T09:06:19Z | | 
| [239](https://github.com/sudoblockio/icon-tracker-frontend/issues/239) | Include delegations and other data for contracts  | closed | 2023-04-21T21:56:31Z | | 
| [232](https://github.com/sudoblockio/icon-tracker-frontend/issues/232) | April Sprint | closed | 2023-04-03T16:20:36Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | closed | 2023-03-08T20:34:13Z | | 
| [165](https://github.com/sudoblockio/icon-tracker-frontend/issues/165) | February Sprint | closed | 2023-02-04T13:16:37Z | | 
| [151](https://github.com/sudoblockio/icon-tracker-frontend/issues/151) | Remove duplicate `/api/v1/contracts/<addr>` calls | closed | 2023-01-24T12:01:33Z | | 
| [103](https://github.com/sudoblockio/icon-tracker-frontend/issues/103) | January Sprint | closed | 2023-01-04T12:52:24Z | | 
| [8](https://github.com/sudoblockio/icon-tracker-frontend/issues/8) | Determine why initial load comes up with different font  | closed | 2022-06-04T22:56:03Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [556](https://github.com/sudoblockio/icon-tracker-frontend/pull/556) | chore: added logging for Sentry ErrorBoundary | open | 2025-02-18T15:08:06Z | | 
| [552](https://github.com/sudoblockio/icon-tracker-frontend/issues/552) | show the current balance while voting in voting page | open | 2025-02-17T07:51:48Z | | 
| [551](https://github.com/sudoblockio/icon-tracker-frontend/issues/551) | add a clear all votes button in voting page | open | 2025-02-17T07:51:30Z | | 
| [550](https://github.com/sudoblockio/icon-tracker-frontend/issues/550) | Voting Page UI/UX | open | 2025-02-17T07:47:26Z | | 
| [546](https://github.com/sudoblockio/icon-tracker-frontend/issues/546) | Merge balanced docs | open | 2025-02-14T07:24:53Z | | 
| [545](https://github.com/sudoblockio/icon-tracker-frontend/issues/545) | Improve bonding experience | open | 2025-02-06T19:02:00Z | | 
| [544](https://github.com/sudoblockio/icon-tracker-frontend/issues/544) | When staking in the tracker you need to leave a small amount for the Tx fee | open | 2025-02-06T18:30:28Z | | 
| [541](https://github.com/sudoblockio/icon-tracker-frontend/issues/541) | Show APR/APY values for validators | open | 2025-02-05T13:57:39Z | | 
| [539](https://github.com/sudoblockio/icon-tracker-frontend/issues/539) | Can't go back when in address view | open | 2025-02-05T07:34:08Z | | 
| [524](https://github.com/sudoblockio/icon-tracker-frontend/issues/524) | Jan Sprint | open | 2025-01-20T12:11:35Z | | 
| [513](https://github.com/sudoblockio/icon-tracker-frontend/issues/513) | Display projected voter APR on tracker | open | 2024-12-09T14:35:28Z | | 
| [502](https://github.com/sudoblockio/icon-tracker-frontend/issues/502) | Prioritized Backlog | open | 2024-10-06T09:40:07Z | | 
| [413](https://github.com/sudoblockio/icon-tracker-frontend/issues/413) | Get contract data showing for berlin   | open | 2024-03-05T17:29:13Z | | 
| [394](https://github.com/sudoblockio/icon-tracker-frontend/issues/394) | after voting on a network proposal, trying to change the vote doesnt work | open | 2024-02-05T00:54:20Z | | 
| [351](https://github.com/sudoblockio/icon-tracker-frontend/issues/351) | Token sending tab in token / address view  | open | 2023-10-31T14:38:50Z | | 
| [322](https://github.com/sudoblockio/icon-tracker-frontend/issues/322) | Running failed tx in Contract tab returns hash seeming success - should be failure  | open | 2023-09-16T18:05:03Z | | 
| [155](https://github.com/sudoblockio/icon-tracker-frontend/issues/155) | Add filters to method column   | open | 2023-01-25T11:04:50Z | | 
| [86](https://github.com/sudoblockio/icon-tracker-frontend/issues/86) | Add search to transaction pages | open | 2022-11-19T20:41:37Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [61](https://github.com/sudoblockio/icon-governance/pull/61) | fix: updated bond_percent formula #60 | closed | 2025-02-01T19:35:31Z | | 
| [56](https://github.com/sudoblockio/icon-governance/pull/56) | chore(main): release 0.10.6 | closed | 2024-11-14T11:27:06Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [62](https://github.com/sudoblockio/icon-governance/pull/62) | chore(main): release 0.10.7 | open | 2025-02-13T08:11:01Z | | 
| [60](https://github.com/sudoblockio/icon-governance/issues/60) | Update bond_percent formula | open | 2025-02-01T19:34:34Z | | 
| [59](https://github.com/sudoblockio/icon-governance/issues/59) | lisbon governance cron failing - int overflow | open | 2025-02-01T06:17:19Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [81](https://github.com/balancednetwork/balanced-backend/issues/81) | Zero address showing up as address in tokens | open | 2025-02-17T13:17:24Z | | 
| [80](https://github.com/balancednetwork/balanced-backend/issues/80) | Looks like issue with sicx:icx chart but pool is actually depleted | open | 2025-02-02T05:03:13Z | | 
| [78](https://github.com/balancednetwork/balanced-backend/pull/78) | chore(main): release 0.8.4 | open | 2024-11-21T09:16:44Z | | 

### [icon-stats](https://github.com/sudoblockio/icon-stats)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [28](https://github.com/sudoblockio/icon-stats/pull/28) | chore(main): release 0.2.9 | closed | 2025-02-20T13:26:26Z | | 
| [27](https://github.com/sudoblockio/icon-stats/pull/27) | fix: openapi schema generator | closed | 2025-02-20T13:25:31Z | | 
| [26](https://github.com/sudoblockio/icon-stats/pull/26) | chore(main): release 0.2.8 | closed | 2025-02-20T10:42:04Z | | 
| [25](https://github.com/sudoblockio/icon-stats/pull/25) | fix: update endpoint for balanced | closed | 2025-02-14T06:58:10Z | | 
| [24](https://github.com/sudoblockio/icon-stats/pull/24) | fix: update openapi merger to handle balanced endpoints | closed | 2025-02-14T05:50:47Z | | 
| [18](https://github.com/sudoblockio/icon-stats/pull/18) | chore(main): release 0.2.7 | closed | 2024-11-30T06:09:52Z | | 


## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| Feb 2 | ~8 hours on Balanced | Operator error - thought an endpoint was instrumented with alerts and did an IP switch that should have triggered the alert but didn't get it so assumed was ok prior sleeping / getting notified by community. | Add correct external alerts. | 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)