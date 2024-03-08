# Tracker Monthly Report

This is a progress update for 2/2023 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month has been a lot of work behind the scenes working on proving out some concepts that will be presented at a later date along with further infrastructure migrations. To be honest, this was a light month but some new people have joined with one, a very good frontend engineer, taking over work on the tracker and clearing out the backlog. Touched base with the designer and others and going to make a push over the next months to clear out the whole backlog and get into some CSS improvements. Aside from that, stats service for summarizing info across the ecosysem is up and can check it out here. 

https://tracker.icon.community/api/v1/statistics/docs
https://github.com/sudoblockio/icon-stats
https://github.com/sudoblockio/icon-stats/blob/main/icon_stats/crons/ecosystem_stats.py

Service is able to run queries across all the databases and summarize any data. Adding queries / stats is [trivial](https://github.com/sudoblockio/icon-stats/blob/main/icon_stats/crons/ecosystem_stats.py) now. Tono who did the current stats work was contacted and potentially will be merging his work into this service.

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [410](https://github.com/sudoblockio/icon-tracker-frontend/pull/410) | chore(main): release 0.4.8 | closed | 2024-03-03T05:57:34Z | | 
| [406](https://github.com/sudoblockio/icon-tracker-frontend/pull/406) | chore(main): release 0.4.7 | closed | 2024-02-21T01:59:25Z | | 
| [401](https://github.com/sudoblockio/icon-tracker-frontend/pull/401) | chore(main): release 0.4.6 | closed | 2024-02-14T08:18:07Z | | 
| [400](https://github.com/sudoblockio/icon-tracker-frontend/pull/400) | chore(main): release 0.4.5 | closed | 2024-02-14T08:06:59Z | | 
| [399](https://github.com/sudoblockio/icon-tracker-frontend/issues/399) | error showcasing max rate and max change rate on validator address page | closed | 2024-02-14T01:34:26Z | | 
| [398](https://github.com/sudoblockio/icon-tracker-frontend/pull/398) | chore(main): release 0.4.4 | closed | 2024-02-07T05:04:11Z | | 
| [397](https://github.com/sudoblockio/icon-tracker-frontend/pull/397) | chore(main): release 0.4.3 | closed | 2024-02-07T04:24:10Z | | 
| [396](https://github.com/sudoblockio/icon-tracker-frontend/pull/396) | fix: changed default values for commission rate in the form | closed | 2024-02-07T04:13:43Z | | 
| [395](https://github.com/sudoblockio/icon-tracker-frontend/issues/395) | Update tracker logo | closed | 2024-02-06T21:07:16Z | | 
| [393](https://github.com/sudoblockio/icon-tracker-frontend/pull/393) | chore(main): release 0.4.2 | closed | 2024-02-02T20:45:20Z | | 
| [392](https://github.com/sudoblockio/icon-tracker-frontend/pull/392) | fix: fixed breaking css styles in governance page | closed | 2024-02-01T23:44:49Z | | 
| [391](https://github.com/sudoblockio/icon-tracker-frontend/pull/391) | changed default values for initCommissionRate and setCommissionRate  | closed | 2024-02-01T21:56:58Z | | 
| [390](https://github.com/sudoblockio/icon-tracker-frontend/pull/390) | chore(main): release 0.4.1 | closed | 2024-02-01T17:30:18Z | | 
| [205](https://github.com/sudoblockio/icon-tracker-frontend/issues/205) | In `/token/<>` there is no transactions tab  | closed | 2023-03-09T10:36:32Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | closed | 2023-03-08T20:34:13Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [415](https://github.com/sudoblockio/icon-tracker-frontend/pull/415) | Fix: #402 when unstaking, the target block height label is missplaced | open | 2024-03-07T00:38:39Z | | 
| [414](https://github.com/sudoblockio/icon-tracker-frontend/issues/414) | Cache issue in lisbon | open | 2024-03-05T17:29:41Z | | 
| [413](https://github.com/sudoblockio/icon-tracker-frontend/issues/413) | Get contract data showing for berlin   | open | 2024-03-05T17:29:13Z | | 
| [412](https://github.com/sudoblockio/icon-tracker-frontend/issues/412) | Paging broken on token transfers  | open | 2024-03-04T17:57:56Z | | 
| [411](https://github.com/sudoblockio/icon-tracker-frontend/issues/411) | Display token balances for contracts | open | 2024-03-04T07:49:54Z | | 
| [409](https://github.com/sudoblockio/icon-tracker-frontend/issues/409) | Estimate step for contract calls on Tracker | open | 2024-02-26T11:34:39Z | | 
| [408](https://github.com/sudoblockio/icon-tracker-frontend/issues/408) | Add pop-ups to governance page  | open | 2024-02-21T02:04:25Z | | 
| [407](https://github.com/sudoblockio/icon-tracker-frontend/pull/407) | Add info popups to gov | open | 2024-02-21T02:01:36Z | | 
| [405](https://github.com/sudoblockio/icon-tracker-frontend/issues/405) | Add `auto-vote` feature | open | 2024-02-18T23:04:53Z | | 
| [404](https://github.com/sudoblockio/icon-tracker-frontend/issues/404) | Add `voting` feature  | open | 2024-02-18T23:03:42Z | | 
| [403](https://github.com/sudoblockio/icon-tracker-frontend/issues/403) | Add `staking` feature   | open | 2024-02-18T22:51:08Z | | 
| [402](https://github.com/sudoblockio/icon-tracker-frontend/issues/402) | fix position of unstaking information in the address page | open | 2024-02-16T22:19:10Z | | 
| [394](https://github.com/sudoblockio/icon-tracker-frontend/issues/394) | after voting on a network proposal, trying to change the vote doesnt work | open | 2024-02-05T00:54:20Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

More issues were actually opened / closed but missed filter. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [39](https://github.com/sudoblockio/icon-governance/pull/39) | chore(main): release 0.7.5 | closed | 2024-02-04T08:01:27Z | | 
| [38](https://github.com/sudoblockio/icon-governance/pull/38) | chore(main): release 0.7.4 | closed | 2024-02-02T20:55:54Z | | 
| [37](https://github.com/sudoblockio/icon-governance/pull/37) | chore(main): release 0.7.3 | closed | 2024-02-02T09:39:30Z | | 
| [36](https://github.com/sudoblockio/icon-governance/pull/36) | chore(main): release 0.7.2 | closed | 2024-02-01T17:40:43Z | | 
| [34](https://github.com/sudoblockio/icon-governance/issues/34) | Fix the status and IP discovery on testnets to test iiss 4  | closed | 2024-01-09T22:53:34Z | | 

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |
| 4/3 | 1 min | Not sure but but the DB disconnected for a second which produced a bug that is shocking we have not found before. Regardless, clusters are getting synced right now because we missed a few records. Also lost a cache on a testnet but that was brought back | Fix the things... |
| 4/5 | 2 min | Not sure but both clusters had issues which means it was not me | Burp the internet... |


> Report generated with [tackle](https://github.com/robcxyz/tackle-box)