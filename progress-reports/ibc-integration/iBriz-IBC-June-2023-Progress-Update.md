# IBC - June 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-June-2023 to 30-June-2023

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
| Relay Strategy / Routing | Completed | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/15 |
| Github Workflow Setup to build IBC-relay Project | Completed | DevOps Task | https://github.com/icon-project/ibc-relay/issues/42 |
| Github Workflow Setup to build IBC-integration Project | Completed | DevOps Task | https://github.com/icon-project/IBC-Integration/pull/368 |
| ICON IBC and xCall Testing | In Progress | ICON - Integration Testing | https://github.com/icon-project/ibc-integration/issues/163 |
| merkle path and values generation for verification of memberships and non-memberships | Completed | ICON Module | https://github.com/icon-project/IBC-Integration/pull/399 |
| Relay - Dockerize Configuration | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/407 |
| Update test on ICON after integration | Completed | Integration Optimisation | https://github.com/icon-project/IBC-Integration/issues/415 |
| Update test on Archway after integration | Completed | Integration Optimisation | https://github.com/icon-project/IBC-Integration/issues/414 |
| ICON Configuration setup for E2E | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/414 |
| Archway Configuration setup for E2E testing | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/412 |
| ICON - Gochain Dockerimage File | Completed | E2E Testing | https://github.com/icon-project/IBC-Integration/issues/402 |
| Archway - Relay Integration Testing | Completed | Integration Testing | https://github.com/icon-project/IBC-Integration/issues/411 |
| Relay - Packet Flow from Archway to Relay | Completed | Integration Testing | https://github.com/icon-project/ibc-relay/issues/74 |
| Relay - Archway Connection flow integration | Completed | Integration Testing | https://github.com/icon-project/IBC-Integration/issues/406 |
| Relay - Archway Channel Flow Integration | Completed | Integration Testing | https://github.com/icon-project/ibc-relay/issues/13 |
| Archway - Use empty merkle prefix for ICON | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/442 |
| Remove default merklePrefix "commitment" from javascore | Completed | Code Fix | https://github.com/icon-project/ibc-relay/issues/445 |
| Archway - Changes to ICON Lightclient | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/425 |
| Relay - Test Close Confirm | Completed | Integration Testing | https://github.com/icon-project/IBC-Integration/issues/433 |
| Handle verify packet timeout Request and store request timeout receipt | Completed | Code Fix | https://github.com/icon-project/IBC-Integration/issues/452 |
| Relay - Test Packet Timeout | Completed | Integration Testing | https://github.com/icon-project/IBC-Integration/issues/432 |
| Merge changes from cosmos relayer | Completed | Fork Update | https://github.com/icon-project/ibc-relay/issues/93 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| ICON - Smart Contract Code Review | Not Started | Code Review - https://github.com/icon-project/IBC-Integration/issues/472 |
| Archway - Smart Contract Code Review | Not Started | Code Review - https://github.com/icon-project/IBC-Integration/issues/473 |
| Relay - Code Review | In Progress | Code Review - https://github.com/icon-project/IBC-Integration/issues/474 |
| Relayer - Integration Testing - Edge Cases | In Progress | Integration Test- https://github.com/icon-project/IBC-Integration/issues/467 |
| Relay Robustness Testing | In Progress | Integration Test - https://github.com/icon-project/IBC-Integration/issues/460 |
| Relay - Packet Flow - Height Update | In Progress | Code Fix - https://github.com/icon-project/IBC-Integration/issues/460 |
| Archway - Non adjacent block updates | In Progress | Code Fix - https://github.com/icon-project/IBC-Integration/issues/443 |
| Archway - Decouple IBC Core and Dapp | In Progress | Code Fix - https://github.com/icon-project/IBC-Integration/issues/468 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
