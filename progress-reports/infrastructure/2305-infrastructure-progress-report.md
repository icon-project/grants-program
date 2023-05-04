# Tracker Monthly Report

This is a progress update for 3/2022 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem.

### Summary

This past month had the standard set of tracker maintenance happen with all previous pressing issues dealt with the major work happening on the migration and a new extractor. 

#### Migration 

For running the new infrastructure, we plan on using bare metal instances subdivided into VMs running kubernetes with a solution called harvester. We have installed that and working with setting up VMs but have been caught up with some complicated network issues. Plan is to bond a NIC to a private network running the VMs which requires setting up a DHCP server that can withstand restarts. Normally DHCP is handeled by the provider but in this case we need to handle it ourselves. Happy to provide more details offline but still working through this setup and exploring options around setting up cloud-init scripts to initialize VMs with static IPs which could fix this issue. This is really just the beginning of the migration of everything depends on it. 

##### Extractor

The biggest thing we work on outside of any of the things that have been regularly reported on in these reports is a cross chain extractor. We've been working on it for many months but recently came up with final designs for how we're going to build it. As a core part of the design is building a new RPC client for ICON that will be polyglot (ie supported in each language). As new RPC endpoints are developed, a high level spec will need to be updated and the clients will automatically update as well. One of the exciting features of this new client is that it will also work for generating clients from contract ABIs allowing users to generate clients for their contracts easily. This is just the interface to the chain but behind this, developers will also be able to leverage a common set of tools to index each block with a distributed / fault tolerant execution layer. We have been working on this design for a while which finally solidified and are now looking to scale up development. 

Part of that development is upgrading tackle to allow a couple language features that are blocking this development so that work is also being prioritized for the time being (albeit not conflicting with any of the duties of this contract). 

### [icon-tracker-frontend](https://github.com/sudoblockio/icon-tracker-frontend)

NOTE: No effort has been made to remove the issues associated with the CPS proposal. 

While the CPS proposal is adding specific features, we have been using this budget to work on additional items such as:

- Improvements to mobile responsiveness
- Rebuilt the startup scripts 
  - Much easier to work / better looking readme 
  - Can now run the tracker on testnets / custom networks locally 
- Hooking up unit and e2e tests in CI / release process
  - Before we had poor unit tests that are now being standardized as part of development 

All major improvements are happening in the `dev` branch and will be merged with the main release of the CPS improvements. 

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [251](https://github.com/sudoblockio/icon-tracker-frontend/issues/251) | Setup e2e with coverage in CI  | closed | 2023-04-23T19:26:19Z | | 
| [247](https://github.com/sudoblockio/icon-tracker-frontend/pull/247) | Refactor config to base - rm old config | closed | 2023-04-22T23:16:00Z | | 
| [246](https://github.com/sudoblockio/icon-tracker-frontend/pull/246) | added txEventParser external lib | closed | 2023-04-22T23:05:10Z | | 
| [240](https://github.com/sudoblockio/icon-tracker-frontend/pull/240) | full working version of contract tab in contract page | closed | 2023-04-22T21:26:05Z | | 
| [237](https://github.com/sudoblockio/icon-tracker-frontend/pull/237) | Config refactor | closed | 2023-04-19T19:02:11Z | | 
| [236](https://github.com/sudoblockio/icon-tracker-frontend/pull/236) | progress work on contract tab component | closed | 2023-04-11T14:27:23Z | | 
| [235](https://github.com/sudoblockio/icon-tracker-frontend/pull/235) | update | closed | 2023-04-07T17:40:01Z | | 
| [234](https://github.com/sudoblockio/icon-tracker-frontend/pull/234) | chore: config | closed | 2023-04-07T16:42:25Z | | 
| [233](https://github.com/sudoblockio/icon-tracker-frontend/pull/233) | fix: contract header cache #225 | closed | 2023-04-04T21:15:35Z | | 
| [231](https://github.com/sudoblockio/icon-tracker-frontend/pull/231) | prep details and bonder list modal views | closed | 2023-03-27T15:27:58Z | | 
| [226](https://github.com/sudoblockio/icon-tracker-frontend/issues/226) | Transaction write workflow  | closed | 2023-03-23T21:45:33Z | | 
| [225](https://github.com/sudoblockio/icon-tracker-frontend/issues/225) | Header Data caches and does not refresh when using the magnifier search feature | closed | 2023-03-23T19:35:43Z | | 
| [224](https://github.com/sudoblockio/icon-tracker-frontend/issues/224) | Module to unpack event logs based on ABI  | closed | 2023-03-23T16:41:50Z | | 
| [221](https://github.com/sudoblockio/icon-tracker-frontend/issues/221) | Contract write wireframes  | closed | 2023-03-21T23:29:53Z | | 
| [218](https://github.com/sudoblockio/icon-tracker-frontend/pull/218) | chore(main): release 0.2.17 | closed | 2023-03-19T19:48:50Z | | 
| [216](https://github.com/sudoblockio/icon-tracker-frontend/pull/216) | chore: update dockerfile | closed | 2023-03-18T15:09:10Z | | 
| [214](https://github.com/sudoblockio/icon-tracker-frontend/issues/214) | Disappearing mouse on `Status` field  | closed | 2023-03-18T14:00:37Z | | 
| [212](https://github.com/sudoblockio/icon-tracker-frontend/pull/212) | E2e tests | closed | 2023-03-15T08:59:56Z | | 
| [197](https://github.com/sudoblockio/icon-tracker-frontend/issues/197) | Main page mobile - stack cards so it is 2 x 2  | closed | 2023-03-08T13:24:44Z | | 
| [165](https://github.com/sudoblockio/icon-tracker-frontend/issues/165) | February Sprint | closed | 2023-02-04T13:16:37Z | | 
| [154](https://github.com/sudoblockio/icon-tracker-frontend/issues/154) | Create more obvious link for debug trace  | closed | 2023-01-24T15:50:13Z | | 
| [103](https://github.com/sudoblockio/icon-tracker-frontend/issues/103) | January Sprint | closed | 2023-01-04T12:52:24Z | | 
| [93](https://github.com/sudoblockio/icon-tracker-frontend/issues/93) | December sprint | closed | 2022-12-07T12:12:37Z | | 
| [71](https://github.com/sudoblockio/icon-tracker-frontend/issues/71) | November Sprint | closed | 2022-10-18T04:13:54Z | | 
| [64](https://github.com/sudoblockio/icon-tracker-frontend/issues/64) | Integrate trace into all Txs | closed | 2022-08-11T21:03:22Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [254](https://github.com/sudoblockio/icon-tracker-frontend/issues/254) | Get unit-tests to pass  | open | 2023-04-25T17:47:56Z | | 
| [253](https://github.com/sudoblockio/icon-tracker-frontend/pull/253) | Merge branch 'sudoblockio:dev' into e2e-tests | open | 2023-04-24T10:48:00Z | | 
| [252](https://github.com/sudoblockio/icon-tracker-frontend/issues/252) | Refactor tests into convention  | open | 2023-04-23T19:28:35Z | | 
| [250](https://github.com/sudoblockio/icon-tracker-frontend/issues/250) | Get coverage report from e2e tests  | open | 2023-04-23T15:22:34Z | | 
| [249](https://github.com/sudoblockio/icon-tracker-frontend/issues/249) | Test contract write methods on full page app  | open | 2023-04-23T15:16:04Z | | 
| [248](https://github.com/sudoblockio/icon-tracker-frontend/issues/248) | Be able to test against local network  | open | 2023-04-23T15:14:05Z | | 
| [245](https://github.com/sudoblockio/icon-tracker-frontend/issues/245) | Ledger integration  | open | 2023-04-22T22:31:29Z | | 
| [244](https://github.com/sudoblockio/icon-tracker-frontend/issues/244) | Setting up bonder list page  | open | 2023-04-22T22:29:29Z | | 
| [243](https://github.com/sudoblockio/icon-tracker-frontend/issues/243) | Setting up vote page  | open | 2023-04-22T22:29:14Z | | 
| [242](https://github.com/sudoblockio/icon-tracker-frontend/issues/242) | Setting up proposals full page  | open | 2023-04-22T22:29:01Z | | 
| [241](https://github.com/sudoblockio/icon-tracker-frontend/issues/241) | Setting up full page contract  | open | 2023-04-22T22:28:06Z | | 
| [239](https://github.com/sudoblockio/icon-tracker-frontend/issues/239) | Include delegations and other data for contracts  | open | 2023-04-21T21:56:31Z | | 
| [238](https://github.com/sudoblockio/icon-tracker-frontend/issues/238) | Cleanout all references to configJson | open | 2023-04-21T18:21:23Z | | 
| [232](https://github.com/sudoblockio/icon-tracker-frontend/issues/232) | April Sprint | open | 2023-04-03T16:20:36Z | | 
| [219](https://github.com/sudoblockio/icon-tracker-frontend/issues/219) | Modify `config.js` so that we can run locally on each network  | open | 2023-03-20T16:03:32Z | | 
| [203](https://github.com/sudoblockio/icon-tracker-frontend/issues/203) | March Sprint | open | 2023-03-08T20:34:13Z | | 
| [194](https://github.com/sudoblockio/icon-tracker-frontend/issues/194) | Add new full pages for proposal and contract write  | open | 2023-03-08T12:30:07Z | | 
| [193](https://github.com/sudoblockio/icon-tracker-frontend/issues/193) | EPIC: Contract Write Meta  | open | 2023-03-08T12:19:25Z | | 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [65](https://github.com/sudoblockio/icon-transformer/issues/65) | Missing BTP contracts (internal) in tokens list | closed | 2023-01-20T13:58:47Z | | 

### [icon-go-api](https://github.com/sudoblockio/icon-go-api)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [37](https://github.com/sudoblockio/icon-go-api/pull/37) | chore(main): release 0.4.5 | open | 2023-04-22T03:44:08Z | | 

### [icon-contracts](https://github.com/sudoblockio/icon-contracts)

Solved some lingering issues over here. 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [5](https://github.com/sudoblockio/icon-contracts/pull/5) | chore(main): release 0.2.0 | open | 2023-01-13T09:27:02Z | | 

### [icon-governance](https://github.com/sudoblockio/icon-governance)

Solved the delegation issue where contracts weren't having their delegation accounted for. Now totals match within <.1% of known.

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [11](https://github.com/sudoblockio/icon-governance/issues/11) | Add tool to discover contracts with delegation  | closed | 2023-04-10T07:56:30Z | | 
| [9](https://github.com/sudoblockio/icon-governance/issues/9) | Delegation under counting  | closed | 2023-03-18T09:27:04Z | | 
| [6](https://github.com/sudoblockio/icon-governance/issues/6) | Delegation out of sync with some addresses that have un-delegated  | closed | 2023-03-03T12:29:33Z | | 
| [5](https://github.com/sudoblockio/icon-governance/issues/5) | Add missed blocks to cron  | closed | 2023-02-13T08:01:08Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [15](https://github.com/sudoblockio/icon-governance/issues/15) | Add historical penalties  | open | 2023-05-02T22:17:35Z | | 
| [14](https://github.com/sudoblockio/icon-governance/pull/14) | Add omm delegation #12 | open | 2023-04-26T20:51:30Z | | 
| [13](https://github.com/sudoblockio/icon-governance/pull/13) | chore(main): release 0.3.1 | open | 2023-04-26T11:06:49Z | | 
| [12](https://github.com/sudoblockio/icon-governance/issues/12) | Omm delegations parser  | open | 2023-04-10T10:35:00Z | | 

### [icon-tracker](https://github.com/sudoblockio/icon-tracker)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-tracker/pull/76) | Fix the Governance link | open | 2023-04-29T05:34:14Z | | 

### [tackle-icon-contract](https://github.com/sudoblockio/tackle-icon-contract)

A lot of work was done on this tool which needs a little touching up before publicizing. It is passing integration tests and is able to do the following:

- Generate contracts for each type (contract, irc2, irc3/31)
- Compile the contracts after generating them 
- Create contract generators (a tackle to create tackles)
  - Run the tests which in turn compile the contracts 
- A roadmap has been established showing which features need to be worked on for each contract type to bring this project to parity with openzepplin or create-smart-contract (Alchemy)

#### Closed Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- |
| [3](https://github.com/sudoblockio/tackle-icon-contract/issues/3) | Make contracts compile  | closed | 2023-03-24T12:47:00Z | | 
| [1](https://github.com/sudoblockio/tackle-icon-contract/pull/1) | chore(main): release 0.1.0 | closed | 2022-12-13T14:58:44Z | | 

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [8](https://github.com/sudoblockio/tackle-icon-contract/issues/8) | Feature: `stable`  | open | 2023-04-13T21:28:02Z | | 
| [7](https://github.com/sudoblockio/tackle-icon-contract/issues/7) | Feature: `mintable`  | open | 2023-04-13T21:27:26Z | | 

## Downtime Incidents

| Date | Total Downtime                     | Cause     | Resolution       |
|------|------------------------------------|-----------|------------------|
| 5/2  | 24 hour (lisbon tracker) | See below | Restart the node |

For about 24 hours, the lisbon tracker was not producing new blocks. Cause was a kubernetes worker crashed which managed the alerts for the specific services it was monitoring that went down. Node crashes have happened before and normally A, the pods reschedule on another node with minimal downtime and B, an alert is sent and the node is brought back within a couple minutes. In this one case, both A and B happened at same time which is why the downtime was so long. Reason A is under investigation right now. For reason B, in the future we'll be setting pod scheduling rules to keep the monitoring services apart from the services it is monitoring. 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)