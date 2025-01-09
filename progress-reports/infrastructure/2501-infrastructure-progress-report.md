# Tracker Monthly Report

This is a progress update for 12/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month was off to a busy start but ended up slowing down at the end due to the holidays / vacations / one of our devs having a baby. Regardless, there are updates on the infrastructure and development side of things.

On the infrastructure side, we have been able to turn off one of the cloud clusters and the timing could not have come sooner as the cluster has began to fill up to the point that it would need its own migration to stay with the same level of service. Currently running testnet trackers and the main RPC nodes off the bare metal clusters since the beginning of the month. So far all has been smooth as the nodes are extremely powerful. Still one cloud cluster is on which was the plan as we wanted to make sure everything was operating smoothly / give ourselves some headroom as we do a redeploy on our second bare metal cluster. Plan is to have that happen over the next week or so ensuring that we have a backup at all times. 

On the development side of things, we worked on PRs for doing some updates to core packages that we had to do in balanced in all our other python services. This seemingly small thing diffed practically everything and required expanding test coverage based on experience rolling out this update last time with Balanced where endpoints went down for a short period with a high failure rate. A We also did some small updates with the go services but in general starting to have bandwidth to look more of the crashes intermittent crashes and slow queries in our new cluster. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [512](https://github.com/sudoblockio/icon-tracker-frontend/pull/512) | chore: unregistered prep in voting | closed | 2024-12-03T11:52:49Z | | 
| [511](https://github.com/sudoblockio/icon-tracker-frontend/issues/511) | Allow unstaking from preps that have left the network - ie Rhizome | closed | 2024-12-03T11:15:13Z | | 
| [510](https://github.com/sudoblockio/icon-tracker-frontend/pull/510) | chore: WIP, added value field if payable | closed | 2024-12-03T07:12:56Z | | 
| [509](https://github.com/sudoblockio/icon-tracker-frontend/pull/509) | chore: udpate btp2 links and contract write []string bug fix #508 && … | closed | 2024-11-27T15:29:17Z | | 
| [508](https://github.com/sudoblockio/icon-tracker-frontend/issues/508) | update btp2 monitors links | closed | 2024-11-27T15:26:37Z | | 
| [506](https://github.com/sudoblockio/icon-tracker-frontend/pull/506) | chore(main): release 0.6.3 | closed | 2024-11-07T06:27:56Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [514](https://github.com/sudoblockio/icon-tracker-frontend/issues/514) | Speed up governance page load  | open | 2024-12-09T17:49:55Z | | 
| [513](https://github.com/sudoblockio/icon-tracker-frontend/issues/513) | Display projected voter APR on tracker | open | 2024-12-09T14:35:28Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [15](https://github.com/sudoblockio/icon-contracts/pull/15) | bump sqlmodel / pydantic / fastapi | closed | 2024-11-10T12:26:09Z | | 
| [8](https://github.com/sudoblockio/icon-contracts/issues/8) | Contract code is not updated in community tracker | closed | 2023-07-15T18:45:31Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [44](https://github.com/sudoblockio/icon-governance/issues/44) | Add sort to preps endpoint | closed | 2024-07-31T15:07:32Z | | 
| [42](https://github.com/sudoblockio/icon-governance/issues/42) | Update DB connection to fail | closed | 2024-03-24T15:04:32Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [26](https://github.com/sudoblockio/icon-governance/issues/26) | Add current APY Endpoint? | open | 2023-11-06T08:18:59Z | | 
| [20](https://github.com/sudoblockio/icon-governance/issues/20) | Add alert manifold  | open | 2023-07-01T14:44:11Z | | 
| [19](https://github.com/sudoblockio/icon-governance/issues/19) | Put prep icons in bucket | open | 2023-07-01T13:14:53Z | | 
| [15](https://github.com/sudoblockio/icon-governance/issues/15) | Add historical penalties  | open | 2023-05-02T22:17:35Z | | 
| [12](https://github.com/sudoblockio/icon-governance/issues/12) | Omm delegations parser  | open | 2023-04-10T10:35:00Z | | 
| [1](https://github.com/sudoblockio/icon-governance/issues/1) | governance/proposals route is not consistence in its returns. | open | 2022-06-29T18:53:29Z | | 


### [icon-stats](https://github.com/sudoblockio/icon-stats)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [21](https://github.com/sudoblockio/icon-stats/pull/21) | updated sa_coloumn to only coloumn fixing failing api tests | closed | 2024-12-01T17:12:20Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [22](https://github.com/sudoblockio/icon-stats/issues/22) | sqla update - cancelling with conflict of recovery  | open | 2024-12-06T05:21:24Z | | 
| [20](https://github.com/sudoblockio/icon-stats/issues/20) | sqla update - Passing primary_key is not supported when also passing a sa_column | open | 2024-12-01T07:32:46Z | | 
| [19](https://github.com/sudoblockio/icon-stats/pull/19) | Bump pydantic | open | 2024-11-30T08:53:20Z | | 


## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| ~December 25th | None - Date when a user started to report 404 on main endpoints | Not sure yet but working to get the xyz endpoint reprovisioned on new cluster | Ongoing |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)