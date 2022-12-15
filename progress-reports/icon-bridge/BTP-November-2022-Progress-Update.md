# BTP - November 2022 Progress Update

## Intro
This progress report is for Icon Bridge related development work by iBriz Team. The report is from  1-November-2022 to 30-November-2022

## Summary
Build an usable centralized bridge for BTP Relay System which can deliver digital assets between multiple chains.
For more details please see - https://github.com/icon-project/icon-bridge/blob/main/README.md 

## Amendments to roadmap
| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| IBC Research | Explore implmentation of IBC before implementation of Arbituary Call Service Implementation | Research Inter-Blockchain Communication Protocol (IBC) services like Cosmos | None |

## Deliverables Ready


| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Add test for BTS Solidity | In Review | Increase test Coverage for BTS | https://github.com/icon-project/icon-bridge/issues/498 |
| Mainnet BTSCore Upgrade failed with message: ran out of gas | In Review | Mainnet deployment issue analysis and fix | https://github.com/icon-project/icon-bridge/issues/469 |
| Assign nonce manually for parallel transactions | In Review | Handle fix for parallel transfer calls are made to bsc chain with the same source address | https://github.com/icon-project/icon-bridge/issues/539 |
| SNOW mainnet release | Completed | Support SNOW mainnet release | - |
| Security Audit Fixes | Completed| Resolve Issues related raised by Security Auditors | https://github.com/icon-project/icon-bridge-planning/issues/16 |
| Security Audit Fixes Mainnet Release | In Progress | Deploy security audit fixes to mainnet | - |
| Research on IBC | In Progress | Inter-Blockchain Communication research and plan for ICON | - |
| Redeployment on Artic | In Progress | Artic testnet got reset requiring everything to be redeployed | - |
| Planning for deployment scripts  | In Progress | Assist with planning and discuss plans for deployment scripts | - |
| Review BTP Message verifier for BTP 2.0  | In Progress | Review BTP Message verifier code for 2.0 | - |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Continue Research on IBC Implementation |In Progress| Continue research and development on IBC Protocol service implementation for ICON |
| Plan implementation the xcall specification for BSC  | Not Started | Development of Arbitrary Call Service Smart Contracts - https://github.com/icon-project/icon-bridge/issues/612 |
| Deployment for SNOW | In Progress | Artic testnet got reset requiring everything to be redeployed | - |
| Security Audit Fixes Mainnet Release | In Progress | Deploy security audit fixes to mainnet | - |



## Sample of docs
https://github.com/icon-project/icon-bridge/blob/main/README.md 
	
