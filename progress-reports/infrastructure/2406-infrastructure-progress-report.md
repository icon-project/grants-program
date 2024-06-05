# Tracker Monthly Report

This is a progress update for 5/2024 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This month saw steady progress on pretty much all fronts. On the frontend we started on a grant that will clean up all the forms around governance along with the core deliverables. Also added a step estimation by default in all Txs now from tracker so hopefully that is never an issue anymore. On the backend I think the bug relating to the backend cron jobs silently failing has been fixed that was a source of some delayed data before. We also brought in a postgres specialist consultant to start to take a deeper look at our DB and indexes. Been fighting a deadlock issue and a couple other things that frankly we're waiting to migrate to worry about too much. The drives we have, despite being nvme, are not enterprise and so operate far below optimal efficiency when they get above 70% capacity and hence our DBs are slower than they could be. That won't be an issue in the future which paired with the consultant should address DB issues for a while. 

Finally, on the dev ops front, hired a new dev ops engineer to help with the migration which got a little delayed due to dev work. Building an SDK that we'll be building the new indexer out of and so worked out some dependency injection patterns that will now be the basis of all our applications into the future. Pretty clean stuff which will later be turned into tackle. We're still likely 3 weeks away anyways from getting pings on our production network because we decided to go BGP which requires a dedicated IP block which must go through tons of hoops. Good for a conversation but we're in the last hurdle to finalize all that. One thing we will mention, networking is a lot more expensive / a pain in the ass than anticipated if you want to operate on an enterprise level with maintaining your own BGP. But now that we are here, we can access wholesale internet and all kinds of other very interesting DDoS measures. Should be a much more reliable connection than what we have now. 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [456](https://github.com/sudoblockio/icon-tracker-frontend/pull/456) | chore: address balance fix #455 | closed | 2024-05-17T14:37:46Z | | 
| [455](https://github.com/sudoblockio/icon-tracker-frontend/issues/455) | Address total balance is wrong | closed | 2024-05-17T14:36:45Z | | 
| [453](https://github.com/sudoblockio/icon-tracker-frontend/pull/453) | chore(main): release 0.5.3 | closed | 2024-05-15T06:15:48Z | | 
| [452](https://github.com/sudoblockio/icon-tracker-frontend/pull/452) | fix: blockheight fix commit #451 | closed | 2024-05-13T17:52:32Z | | 
| [451](https://github.com/sudoblockio/icon-tracker-frontend/pull/451) | chore: target blockheight readded | closed | 2024-05-13T13:34:08Z | | 
| [448](https://github.com/sudoblockio/icon-tracker-frontend/pull/448) | chore: fixed empty contract events #447 | closed | 2024-05-10T10:37:34Z | | 
| [447](https://github.com/sudoblockio/icon-tracker-frontend/issues/447) | Contract Events is always empty | closed | 2024-05-10T10:36:41Z | | 
| [445](https://github.com/sudoblockio/icon-tracker-frontend/pull/445) | chore(main): release 0.5.2 | closed | 2024-04-24T19:01:37Z | | 
| [439](https://github.com/sudoblockio/icon-tracker-frontend/pull/439) | Estimate step limit | closed | 2024-03-30T17:29:11Z | | 
| [409](https://github.com/sudoblockio/icon-tracker-frontend/issues/409) | Estimate step for contract calls on Tracker | closed | 2024-02-26T11:34:39Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [454](https://github.com/sudoblockio/icon-tracker-frontend/issues/454) | Update styling of wallet login  | open | 2024-05-15T07:18:27Z | | 
| [450](https://github.com/sudoblockio/icon-tracker-frontend/issues/450) | Nested contract calls not showing properly  | open | 2024-05-12T17:59:43Z | | 
| [449](https://github.com/sudoblockio/icon-tracker-frontend/issues/449) | Make site title dynamic according to the page | open | 2024-05-12T05:25:13Z | | 
| [446](https://github.com/sudoblockio/icon-tracker-frontend/issues/446) | Scrub "P-Rep" from tracker and replace with "Validator" | open | 2024-05-03T18:56:31Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [77](https://github.com/sudoblockio/icon-transformer/issues/77) | Deadlock on cron  | open | 2024-05-05T02:23:12Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [45](https://github.com/sudoblockio/icon-go-api/issues/45) | Make queries stricter  | closed | 2023-11-10T15:09:33Z | | 

## Downtime Incidents

Nothing affecting production. Fighting an issue we have in dev but very intermittent and likely solved with recent remediation. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)
 