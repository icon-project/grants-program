# BTP - October 2022 Progress Update

## Intro
This progress report is for Icon Bridge related development work by iBriz Team. The report is from  1-October-2022 to 31-October-2022

## Summary
Build an usable centralized bridge for BTP Relay System which can deliver digital assets between multiple chains.
For more details please see - https://github.com/icon-project/icon-bridge/blob/main/README.md 

## Amendments to roadmap
None

## Deliverables Ready


| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Add test for BTS Solidity | In Review | Increase test Coverage for BTS | https://github.com/icon-project/icon-bridge/issues/498 |
| Mainnet BTSCore Upgrade failed with message: ran out of gas | In Review | Mainnet deployment issue analysis and fix | https://github.com/icon-project/icon-bridge/issues/469 |
| Assign nonce manually for parallel transactions | In Review | Handle fix for parallel transfer calls are made to bsc chain with the same source address | https://github.com/icon-project/icon-bridge/issues/539 |
| Verify contracts on BSC mainnet and testnet tracker | Completed | Verify contracts on BSC mainnet and testnet tracker | https://github.com/icon-project/icon-bridge/issues/617 | 
| Research and Planning for xcall service | Completed | Planning and research for xcall service implementation | https://github.com/icon-project/icon-bridge/issues/613 | 
| validator is used few blocks after removal from bsc validator-set | Released | Update so that the BSC Verifier should update validator set at the block as BSC chain | https://github.com/icon-project/icon-bridge/issues/575 | 
| add bsc mock tests | Released |  Increase Test coverage | https://github.com/icon-project/icon-bridge/issues/522 |
| add chain API for SNOW | Released | A SNOW chain API needs to be added to run e2etests. | https://github.com/icon-project/icon-bridge/issues/604 |
| lowercase-keys module requires different node version | Released | Bug fix | https://github.com/icon-project/icon-bridge/issues/592 |
| add bmc and bts upgrade script | Completed | Add ICON upgrade scripts for BMC and BTS | https://github.com/icon-project/icon-bridge/issues/742 |
| Support NEAR integration | In Progress | Support NEAR integration team with integration and support | - |
| SNOW ICON Bridge Rollout | Completed | Support SNOW integration team with integration and support | https://github.com/icon-project/icon-bridge/issues/500 |
| script to change relay owner | Completed | A clear and concise description of the user and their need | https://github.com/icon-project/icon-bridge/issues/744 |
| updated config params for icon-snow testnet deployment | Completed | Deployment script update | https://github.com/icon-project/icon-bridge/issues/624 |
| Security Audit | In Progress | Resolve Issues related raised by Security Auditors | https://github.com/icon-project/icon-bridge-planning/issues/16 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Continue Improvement of code coverage for the code base |In Progress| The codecoverage of the repo is low. Work towards achieving the target of 80% coverage to improve the health of the overall codebase. |
| Assist with Near release and integration | In Progress | Near is currently in Testnet. Mainnet deployment and Nexus integration is being planned. Team to assist. |
| Deploy smart contract and relays to all the chains that have similarity to BSC  | In Discussion | Update script to go through and deploy the contracts and relays to all the chains that have similarity to BSC like Harmony Ethereum, polygon, avalanche on local and testnet - https://github.com/icon-project/icon-bridge/issues/770 |
| Implement the xcall specification for BSC  | Not Started | Development of Arbitrary Call Service Smart Contracts - https://github.com/icon-project/icon-bridge/issues/612 |



## Sample of docs
https://github.com/icon-project/icon-bridge/blob/main/README.md 
