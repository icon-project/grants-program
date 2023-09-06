# IBC - August 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-August-2023 to 30-August-2023

## Summary
Integration of IBC to connect ICON with Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay

## Milestones
Milestone 1 - Testnet Deployment on Archway and ICON - 11th August 2023
Milestone 2 - Testnet Deployment - ICON - Libson, Archway and Neutron - 12th September 2023

## Amendments to roadmap

| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| IBC implementation on Polygon to be placed on hold | Polygon IBC implementation for ICON to be placed on hold | Prioritize implementation of Archway and ICON. Another chain to be confirmed and prioritized later. | Archway and ICON IBC Implementation |
| IBC implementation on Neutron to be prioritized after integration of Archway | Neutron IBC implementation for ICON to be implemented along with Archway | As Neutron and Archway deployments are similar, Deployments on both Archway and Neutron to be run Parellelly. | Testnet deployment for Neutron, Archway and ICON |


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Relayer - Integration Testing - Edge Cases | Completed | Integration Test | https://github.com/icon-project/IBC-Integration/issues/467 |
| Relay Robustness Testing | Completed | Integration Test | https://github.com/icon-project/IBC-Integration/issues/460 |
| Internal Code Reviews | Completed | Code Reviews | https://github.com/icon-project/IBC-Integration/issues/471 |
| Documentation | Completed | Documentation | https://github.com/icon-project/IBC-Integration/issues/113 |
| Testnet Release | Completed | Testnet Release. Milestone 1. | https://github.com/icon-project/IBC-Integration/issues/76 |
| E2E Testing | Completed | E2E Testing Framework and Demo | https://github.com/icon-project/IBC-Integration/issues/75 |
| CI Workflow Update - IBC relay repo | Completed | DevOps Task | https://github.com/icon-project/ibc-relay/issues/136 |
| Key store management on Icon | Completed | Relay Code Fix | https://github.com/icon-project/ibc-relay/issues/138 |
| Improve Log messages | Completed | Relay Code Fix | https://github.com/icon-project/ibc-relay/issues/133 |
| Internal Security Review | In Progress | Security Review | https://github.com/icon-project/ibc-planning/issues/166 |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Testnet Release | In Progress | Libson Testnet Release after security audit fixes|
| Internal Security Review | In Progress | Security Review - https://github.com/icon-project/ibc-planning/issues/166 |
| Mainnet Release | Not Started | Mainnet release after testnet release and testing. |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
