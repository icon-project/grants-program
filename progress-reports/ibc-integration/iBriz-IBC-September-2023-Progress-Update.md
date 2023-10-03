# IBC - September 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-September-2023 to 30-September-2023

## Summary
Integration of IBC to connect ICON with Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi

## Milestones
Milestone 1 - Testnet Deployment on Archway and ICON - 11th August 2023 - Completed
Milestone 2 - Testnet Deployment - ICON - Libson, Archway and Neutron - 12th September 2023 - Completed
Milestone 3 - Mainnet Deployment - ICON and Archway - 6th October

## Amendments to roadmap

| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| IBC implementation on Polygon to be placed on hold | Polygon IBC implementation for ICON to be placed on hold | Prioritize implementation of Archway and ICON. Another chain to be confirmed and prioritized later. | Archway and ICON IBC Implementation |
| IBC implementation on Neutron to be prioritized after integration of Archway | Neutron IBC implementation for ICON to be implemented along with Archway | As Neutron and Archway deployments are similar, Deployments on both Archway and Neutron to be run Parellelly. | Testnet deployment for Neutron, Archway and ICON |


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Internal Security Review | Completed | Security Review | https://github.com/icon-project/ibc-planning/issues/166 |
| Testnet Release | Completed| Libson Testnet Release after security audit fixes | https://github.com/icon-project/IBC-Integration/wiki/%5BLisbon%5D-IBC%E2%80%90Integration%E2%80%90Contract%E2%80%90Addresses |
| [IBC Cosmwasm] query method getConsensusStatebyHeight should return any type consensus state | Completed| Fixes | https://github.com/icon-project/IBC-Integration/issues/726 |
| BSC - xCall Multi - Deployment | Completed| xCall deployment on Testnet | https://github.com/icon-project/xcall-multi/issues/95 |
| xCall - Solidity Translation | Completed | xCall Translation | https://github.com/icon-project/xcall-multi/issues/36 |
| Havah- xCall Multi - Contract Deployment | Completed | xCall deployment on Testnet |  |
| Signature Parse from proof shouldn't be unwrapped | Completed| Fixes | https://github.com/icon-project/IBC-Integration/issues/716 |
| Implement automatic version bump | Completed| DevOps | https://github.com/icon-project/xcall-multi/issues/37 |
| Add tests sending multiple packets on same height | Completed| Integration Test | https://github.com/icon-project/IBC-Integration/issues/724 |
| publish xCall library to maven repository | Completed| DevOps | https://github.com/icon-project/xcall-multi/issues/30 |
| [IBC-Javascore] Save WriteAck Heights when emitting writeAck event log | Completed| Fixes | https://github.com/icon-project/IBC-Integration/issues/706 |
| Mainnet Release | In Progress | Mainnet release after testnet release and testing. | https://github.com/icon-project/IBC-Integration/wiki/%5BMainnet%5D-IBC-Integration-Mainnet-Contract-Addresses |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Mainnet Release | In Progress | Mainnet release after testnet release and testing. |
| Hopchain | Started | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760 |
| Centralized Relay | Started | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/1 |
| xCall Smart Contract - Rapid Deployment | In Planning | Centralised relay and xcall integration - https://github.com/icon-project/xcall-multi/issues/120 |
| Wormhole Adapter | In Planning | https://github.com/icon-project/xcall-multi/issues/105 |
| LayerZero Adapter  | In Planning | https://github.com/icon-project/xcall-multi/issues/111 |




## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
