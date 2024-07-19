# Tracker Monthly Report

This is a progress update for 6/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month has seen a lot of activity practically everywhere. 

##### Frontend 

We missed submitting progress report (12 hours late) for the CPS grant but development of milestone 1 + 2 is nearing a close. We brought in an designer who polished things up and can say the new voting interface looks better than ICONex (in our humble opinion). Will be deployed soon. 

##### Backend 

Can check issues per the individual repos but some of the stuff that isn't covered is specifically for the tracker include working out some issues with migrations that caused persistent issues with one of our regions. Way outside of scope to explain - looped in contractor and everything to work it out, but suffice to say one of the main issues affecting our dev environment and is now at least not sending alarms. 

Some of the other updates have to do with preparing for a CPS proposal that we'll be updating Cyrus directly on and others have to do with the tracker backend rebuild which again we'll be updating Cyrus on directly. 

##### Infrastructure 

Moving to bare metal has been a challenge. Sparing technical details, we are now moving to our third different OS install / VM orchestration solution. Main issue has been networking where each time we get up to the point of installing kubernetes we find deficiencies in the process pushing us into more and more complex solutions. We're now moving to Openstack which is no joke complex but solves critical issues we had with proxmox and custom libvirt implementations we had worked with before. Benefits are we'll have our own private cloud using the most capable open source cloud orchestration platform. It's basically like a private AWS. The right consultants have been engaged and hoping to have initial deployment done in a week and serving public traffic soon there after. Don't want to commit to any other timelines until we get through the initial install.

Lastly it is worth mentioning we brought on a new dev ops engineer who has been great. Next deployments will massively benefit from new additions to help with observabilty and monitoring where we're bringing in a suite of 5 additional tools. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

Not mentioned is working with HANA to sort out some issues with their wallet which allowed us to debug some issues. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [443](https://github.com/sudoblockio/icon-tracker-frontend/issues/443) | Estimated blockheight not shown in tracker while unstaking | closed | 2024-04-13T13:17:57Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [469](https://github.com/sudoblockio/icon-tracker-frontend/issues/469) | Using sentry for frontend logs | open | 2024-07-16T19:14:12Z | | 
| [468](https://github.com/sudoblockio/icon-tracker-frontend/issues/468) | Redesign Code tab in contracts view | open | 2024-07-03T15:29:16Z | | 
| [467](https://github.com/sudoblockio/icon-tracker-frontend/issues/467) | Updated json viewer for code section  | open | 2024-07-03T15:27:57Z | | 
| [466](https://github.com/sudoblockio/icon-tracker-frontend/issues/466) | Sectioned ABI view  | open | 2024-07-03T15:25:34Z | | 
| [465](https://github.com/sudoblockio/icon-tracker-frontend/issues/465) | Change login flow + add options drop down  | open | 2024-07-03T15:17:43Z | | 
| [464](https://github.com/sudoblockio/icon-tracker-frontend/issues/464) | Clean up old testing cruft + make tests run  | open | 2024-07-03T14:55:29Z | | 
| [463](https://github.com/sudoblockio/icon-tracker-frontend/issues/463) | Review M2  | open | 2024-07-03T14:44:11Z | | 
| [462](https://github.com/sudoblockio/icon-tracker-frontend/issues/462) | Last page doesn't work in contract view | open | 2024-07-03T14:42:51Z | | 
| [461](https://github.com/sudoblockio/icon-tracker-frontend/issues/461) | Pick base libraries for openapi docs  | open | 2024-07-03T14:24:16Z | | 
| [460](https://github.com/sudoblockio/icon-tracker-frontend/issues/460) | Network revision ran into issue  | open | 2024-06-28T21:51:22Z | | 
| [459](https://github.com/sudoblockio/icon-tracker-frontend/issues/459) | Bond amount not showing in address view | open | 2024-06-19T12:37:11Z | | 
| [458](https://github.com/sudoblockio/icon-tracker-frontend/issues/458) | Staking feedback turn #1  | open | 2024-06-12T15:21:39Z | | 
| [457](https://github.com/sudoblockio/icon-tracker-frontend/issues/457) | Ability logout with wallet  | open | 2024-06-12T15:12:38Z | | 
| [418](https://github.com/sudoblockio/icon-tracker-frontend/issues/418) | April Sprint  | open | 2024-03-10T07:03:17Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [78](https://github.com/sudoblockio/icon-transformer/pull/78) | fix: update protoc gorm | closed | 2024-06-28T03:45:05Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [79](https://github.com/sudoblockio/icon-transformer/pull/79) | Update Protoc Gorm Generation | open | 2024-07-15T05:22:06Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [48](https://github.com/sudoblockio/icon-go-api/pull/48) | chore(main): release 0.5.4 | closed | 2024-06-27T03:02:35Z | | 

### [balanced-backend](https://github.com/balancednetwork/balanced-backend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [59](https://github.com/balancednetwork/balanced-backend/pull/59) | chore(main): release 0.6.2 | closed | 2024-07-04T00:35:41Z | | 
| [57](https://github.com/balancednetwork/balanced-backend/issues/57) | Sync the name of renamed USDC token contract | closed | 2024-07-01T09:55:04Z | | 
| [56](https://github.com/balancednetwork/balanced-backend/pull/56) | chore(main): release 0.6.1 | closed | 2024-06-28T21:39:28Z | | 
| [52](https://github.com/balancednetwork/balanced-backend/pull/52) | chore(main): release 0.6.0 | closed | 2024-06-05T21:04:51Z | | 
| [51](https://github.com/balancednetwork/balanced-backend/pull/51) | chore(main): release 0.5.5 | closed | 2024-06-05T16:07:05Z | | 
| [50](https://github.com/balancednetwork/balanced-backend/pull/50) | chore(main): release 0.5.4 | closed | 2024-06-05T05:53:52Z | | 
| [39](https://github.com/balancednetwork/balanced-backend/issues/39) | Fix pools endpoint | closed | 2024-05-16T06:51:50Z | | 
| [28](https://github.com/balancednetwork/balanced-backend/issues/28) | Create new pool series endpoint similar to /tokens/prices and interpolate prices for missing pools | closed | 2023-06-18T13:06:46Z | | 
| [27](https://github.com/balancednetwork/balanced-backend/issues/27) | Build in cutoff for listing on both the cmc and gecko endpoints  | closed | 2023-06-02T14:17:23Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [60](https://github.com/balancednetwork/balanced-backend/pull/60) | chore(main): release 0.6.3 | open | 2024-07-19T00:16:52Z | | 
| [58](https://github.com/balancednetwork/balanced-backend/issues/58) | Confirm pool changes  | open | 2024-07-04T00:33:31Z | | 
| [55](https://github.com/balancednetwork/balanced-backend/issues/55) | Formalize the definitions of all the prices  | open | 2024-06-25T20:15:54Z | | 
| [54](https://github.com/balancednetwork/balanced-backend/issues/54) | Include volumes and fees in implied charts  | open | 2024-06-25T19:32:42Z | | 
| [53](https://github.com/balancednetwork/balanced-backend/issues/53) | Calculate volume and fees for every token in series / static  | open | 2024-06-25T19:32:23Z | | 
| [49](https://github.com/balancednetwork/balanced-backend/issues/49) | additional collateral and laon charts | open | 2024-05-29T13:33:30Z | | 
| [48](https://github.com/balancednetwork/balanced-backend/issues/48) | Implied charts  | open | 2024-05-28T17:41:25Z | | 
| [46](https://github.com/balancednetwork/balanced-backend/issues/46) | performance details backend | open | 2024-05-28T17:31:51Z | | 
| [45](https://github.com/balancednetwork/balanced-backend/issues/45) | savings rate deposit chart  | open | 2024-05-28T17:31:00Z | | 
| [44](https://github.com/balancednetwork/balanced-backend/issues/44) | ICX Burned chart | open | 2024-05-28T17:27:30Z | | 
| [43](https://github.com/balancednetwork/balanced-backend/issues/43) | Oracle time series / scrape all the data  | open | 2024-05-28T17:27:05Z | | 
| [33](https://github.com/balancednetwork/balanced-backend/issues/33) | Historical claim values per address | open | 2024-02-26T13:33:45Z | | 
| [26](https://github.com/balancednetwork/balanced-backend/issues/26) | Validate gecko data  | open | 2023-05-29T10:11:34Z | | 
| [12](https://github.com/balancednetwork/balanced-backend/issues/12) | Endpoint for redemptions | open | 2023-03-03T10:43:01Z | | 

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 7/16/2024 | 3 min delay in block indexing | Cloud provider restarting servers | Nothing, they are terrible and we're moving away. This also glitched balanced and another fix to the connection issue is being tried out. |

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)