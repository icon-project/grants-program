# IBC - July 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-July-2023 to 31-July-2023

## Summary
Integration of IBC to connect ICON with Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay

## Milestones
Milestone 1 - Testnet Deployment on Archway and ICON - 11th August 2023

## Amendments to roadmap

| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| IBC implementation on Polygon to be placed on hold | Polygon IBC implementation for ICON to be placed on hold | Prioritize implementation of Archway and ICON. Another chain to be confirmed and prioritized later. | Archway and ICON IBC Implementation |
| IBC implementation on Neutron to be prioritized after integration of Archway | Neutron IBC implementation for ICON to scoped and reviewed | Prioritize implementation of Archway and ICON. Work to be started on Neutron after Archway implementation | Archway and ICON IBC Implementation |


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| ICON IBC and xCall Testing | Completed | ICON - Integration Testing | https://github.com/icon-project/ibc-integration/issues/163 |
| ICON - Smart Contract Code Review | In Progress | Code Review | https://github.com/icon-project/IBC-Integration/issues/472 |
| Archway - Smart Contract Code Review | In Progress | Code Review | https://github.com/icon-project/IBC-Integration/issues/473 |
| Relay - Code Review | Completed | Code Review | https://github.com/icon-project/IBC-Integration/issues/474 |
| Relayer - Integration Testing - Edge Cases | In Progress | Integration Test | https://github.com/icon-project/IBC-Integration/issues/467 |
| Relay Robustness Testing | In Progress | Integration Test | https://github.com/icon-project/IBC-Integration/issues/460 |
| Relay - Packet Flow - Height Update | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/461 |
| Archway - Non adjacent block updates | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/443 |
| Archway - Decouple IBC Core and Dapp | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/468 |
| Neutron - Relay Updates | Completed | Neutron Implementation | https://github.com/icon-project/IBC-Integration/issues/537 |
| Neutron - Testnet Deployment | Completed | Neutron Implementation | https://github.com/icon-project/IBC-Integration/issues/535 |
| Archway - Reduce callbacks | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/524 |
| Add fee query in xcall | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/43 |
| Remove lightclient callbacks | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/531 |
| Fix config after relay config update | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/552 |
| Archway - Build Binary File | Completed | DevOps | https://github.com/icon-project/IBC-Integration/issues/405 |
| Neutron - E2E Integration | Completed | Neutron Integration | https://github.com/icon-project/IBC-Integration/issues/536 |
| xCall Repo - Codecov and CI setup | Completed | xCall | https://github.com/icon-project/IBC-Integration/issues/540 |
| Happy path - Icon to Archway | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/484 |
| Happy path - Archway to ICON | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/486 |
| E2E testing - non-adjacent changes update to E2E framework | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/528 |
| Deploy contracts on Archway Testnet | Completed | Testnet Deployment | https://github.com/icon-project/IBC-Integration/issues/464 |
| Implement changes for non-adjacent icon client on relay | Completed | Relay code fix | https://github.com/icon-project/IBC-Integration/issues/520 |
| Initiate BTP node for Archway on ICON testnet | Completed | Testnet Deployment | https://github.com/icon-project/IBC-Integration/issues/516 |
| Archway - Rust Contract commitment storage | Completed | Archway - code fix | https://github.com/icon-project/IBC-Integration/issues/440 |
| cosmwasm - storage issue | Completed | Archway - code fix | https://github.com/icon-project/IBC-Integration/issues/529 |
| Archway - non adjacent block updates | Completed | Archway - code fix | https://github.com/icon-project/IBC-Integration/issues/443 |
| Deploy relayer for Tesnet | Completed | Testnet Deployment | https://github.com/icon-project/IBC-Integration/issues/465 |
| Add btp block verifier to icon chain | Completed | Relay - Code Update | https://github.com/icon-project/IBC-relay/issues/104 |
| Implement Verifier for Archway module | Completed | Relay - Code Update | https://github.com/icon-project/IBC-integration/issues/518 |
| xCall Migration | Completed | Relay - Code Update | https://github.com/icon-project/IBC-integration/issues/527 |
| Relay - multiprotocol xcall testing | Completed | Relay - Code Update | https://github.com/icon-project/IBC-relay/issues/101 |
| Deploy contracts on ICON testnet | Completed | Testnet Deployment | https://github.com/icon-project/IBC-integration/issues/463 |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Internal Code Reviews | In Progress | Code Reviews - https://github.com/icon-project/IBC-Integration/issues/471 |
| Documentation | In Progress | Documentation - https://github.com/icon-project/IBC-Integration/issues/113 |
| Internal Security Review | In Progress | Security Review - https://github.com/icon-project/ibc-planning/issues/166 |
| Testnet Release | In Progress | Code Fix - https://github.com/icon-project/IBC-Integration/issues/76 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
