# BTP - August 2022 Progress Update

## Intro
This progress report is for Icon Bridge related development work by iBriz Team. The report is from  1-August-2022 to 31-August-2022

## Summary
Build an usable centralized bridge for BTP Relay System which can deliver digital assets between multiple chains.
For more details please see - https://github.com/icon-project/icon-bridge/blob/main/README.md 

## Amendments to roadmap
BSC Mainnet launched on 17th August instead of 15th August

## Deliverables Ready


| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| BSC Testnet Release | Released | BSC Tesnet Release| https://github.com/icon-project/icon-bridge/releases/tag/v0.0.9-rc.1 |
| BSC Mainnet Release | Released | BSC Mainnet Beta Release | https://github.com/icon-project/icon-bridge/releases/tag/v0.0.9-rc.2 |
| Javascore & Solidity Smart Contract Internal Audit| Released | There has been significant changes in BTS (Token Service) contract in recent days, and BSR (restrictions/blacklist) contract has been implemented recently. So it makes sense to do a thorough review of these contract, identify issues and areas to improve test coverage. | https://github.com/icon-project/icon-bridge/issues/25| 
| Unittests fix/update for BTS/BMC on solidity | Released | Support for Github actions (CI/CD), tests for the BTS and BMC on solidity | https://github.com/icon-project/icon-bridge/issues/146 | 
| Update contract deploy script | Released | Deploy contracts on Testnet and output necessary config | https://github.com/icon-project/icon-bridge/issues/180 | 
| Unit Tests for relay | Released | Unit tests for the relay code. | https://github.com/icon-project/icon-bridge/issues/143 |
| Blacklist restriction issue in current implementations | Released | Blacklist message transferred to relayer so the BTS contract can send message to BMC contract | https://github.com/icon-project/icon-bridge/issues/45 |
| update solc version used by ERC20TKN and HRC20 contracts | Released | Update Solc version as ERC20TKN and HRC20 contracts still use solidity versions less than v0.8.0 while other contracts use version greater than it. | https://github.com/icon-project/icon-bridge/issues/174 |
| Update bsc relay config parameters | Released | Hard-coded config params to be reflected in the deployment environment | https://github.com/icon-project/icon-bridge/issues/161 |
| Add useful logging to relay | Released | Add logging data necessary to debug issues on the relay | https://github.com/icon-project/icon-bridge/issues/159 |
| Get receipts from blocks| Released | Reduce the number of RPC calls | https://github.com/icon-project/icon-bridge/issues/240 |
| BSC header verification | Released | improve security and conform to the definition of having chained blocks | https://github.com/icon-project/icon-bridge/issues/243 |
| Improve slack message formatting | Released | Improve readability of slack log messages | https://github.com/icon-project/icon-bridge/issues/214 |
| Sanitize E2E framework code | Released | Remove mention of keys, including test units, and hard-coded values | https://github.com/icon-project/icon-bridge/issues/204 |
| Include uint256 as maximum value for transactions | Released |  Smart contracts must conform to common integer bound | https://github.com/icon-project/icon-bridge/issues/195 |
| Use filter query to check if BTP message exists in chain | Released |  Enhancement to reduce the number of RPC calls | https://github.com/icon-project/icon-bridge/issues/305 |
| TransferBatch check if input request empty | Released |  Avoid wasteful transactions especially on the side of BMR | https://github.com/icon-project/icon-bridge/issues/251 |
| Duplication of Serial Number  | Released |  Serial numbers should be unique even after contract upgrade | https://github.com/icon-project/icon-bridge/issues/324 |
| Update block confirmation interval | Released |  Issue fix regarding block verifier failing and gets stuck in a loop causing the relay to become stuck | https://github.com/icon-project/icon-bridge/issues/322|



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Documentation for the Icon Bridge Repo | Almost complete | This is almost complete and is running through internal reviews. This will be an ongoing task to ensure new users of the repo can understand the codebase more easily |
| Improve code coverage of the code base | Not Started | The codecoverage of the repo is low. Work towards achieving the target of 80% coverage to improve the health of the overall codebase. |
| Assist with Security Audit | In Progress | The Security Audit has started. Any information needed to be provided or fixes needed based on security audit review will be provided adhoc.|
| Assist with Near release and integration | In Progress | Near integration deployment is being planned September Release. Team to assist. |



## Sample of docs
https://github.com/icon-project/icon-bridge/blob/main/README.md 
