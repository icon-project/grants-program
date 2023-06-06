# IBC - May 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-May-2023 to 31-May-2023

## Summary
Integration of IBC to connect ICON with Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay

## Amendments to roadmap

| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| IBC implementation on Polygon to be placed on hold | Polygon IBC implementation for ICON to be placed on hold | Prioritize implementation of Archway and ICON. Another chain to be confirmed and prioritized later. | Archway and ICON IBC Implementation |
| IBC implementation on Neutron to be prioritized after integration of Archway | Neutron IBC implementation for ICON to scoped and reviewed | Prioritize implementation of Archway and ICON. Work to be started on Neutron after Archway implementation | Archway and ICON IBC Implementation |

## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Relay Strategy / Routing | In Review | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/15 |
| Github Workflow Setup to build IBC-relay Project | In Progress | DevOps Task | https://github.com/icon-project/ibc-relay/issues/42 |
| Github Workflow Setup to build IBC-integration Project | In Progress | DevOps Task | https://github.com/icon-project/IBC-Integration/pull/368 |
| Implement merkle proof verification in Java contract | Completed | ICON - Lightclient for Archway | https://github.com/icon-project/ibc-integration/issues/326 |
| Setup and Run E2E Demo for ICON to ICON | Completed | ICON Integration Testing | https://github.com/icon-project/ibc-integration/issues/293 |
| Use Vector commitments in lightclient | Completed | ICON - Lightclient for Archway | https://github.com/icon-project/ibc-integration/issues/218 |
| IBC Core Contract Update | Completed | Archway - Core | https://github.com/icon-project/ibc-integration/issues/340 |
| BTP Mock Client Setup for testing | Completed | Archway - Integration Testing | https://github.com/icon-project/ibc-integration/issues/339 |
| ICON IBC and xCall Testing | In Progress | ICON - Integration Testing | https://github.com/icon-project/ibc-integration/issues/163 |
| Archway Query | Completed | Relay - Archway Module | https://github.com/icon-project/ibc-relay/issues/53 |
| Archway Transactions | Completed | Relay - Archway Module | https://github.com/icon-project/ibc-relay/issues/54 |
| Archway Proofs | Completed | Relay - Archway Module | https://github.com/icon-project/ibc-relay/issues/55 |
| Remote Localnode for Archway | Completed | DevOps Task | https://github.com/icon-project/IBC-Integration/issues/397 |
| ICON Block monitor | Completed | Relay - Archway to ICON | https://github.com/icon-project/ibc-relay/issues/69 |
| IBC Core Contract update | Completed | Archway Module - Contract Update | https://github.com/icon-project/IBC-Integration/issues/340 |
| Lightclient handler check for Archway | Completed | Archway Module - Lightclient Update | https://github.com/icon-project/IBC-Integration/issues/308 |
| merkle path and values generation for verification of memberships and non-memberships | In Review | ICON Module | https://github.com/icon-project/IBC-Integration/pull/399 |
| Integration Testing Fixes | In Progress | Relay to Archway | https://github.com/icon-project/IBC-Integration/issues/74, https://github.com/icon-project/IBC-Integration/pull/395, https://github.com/icon-project/IBC-Integration/pull/394, https://github.com/icon-project/IBC-Integration/pull/391, https://github.com/icon-project/IBC-Integration/pull/389, https://github.com/icon-project/IBC-Integration/pull/388, https://github.com/icon-project/IBC-Integration/pull/387, https://github.com/icon-project/IBC-Integration/pull/385, https://github.com/icon-project/IBC-Integration/pull/384, https://github.com/icon-project/IBC-Integration/pull/383, https://github.com/icon-project/IBC-Integration/pull/383, https://github.com/icon-project/IBC-Integration/pull/382, https://github.com/icon-project/IBC-Integration/pull/378, https://github.com/icon-project/IBC-Integration/pull/377, https://github.com/icon-project/IBC-Integration/pull/376, https://github.com/icon-project/IBC-Integration/pull/375, https://github.com/icon-project/IBC-Integration/pull/369, https://github.com/icon-project/ibc-relay/pull/62, https://github.com/icon-project/ibc-relay/pull/63, https://github.com/icon-project/ibc-relay/pull/65, https://github.com/icon-project/ibc-relay/pull/66, https://github.com/icon-project/ibc-relay/pull/72, https://github.com/icon-project/ibc-relay/pull/73 |




## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Relay - Dockerize Configuration | Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/407 |
| Update test on ICON after integration | Not Started | Integration Optimisation - https://github.com/icon-project/IBC-Integration/issues/415 |
| Update test on Archway after integration | Not Started | Integration Optimisation - https://github.com/icon-project/IBC-Integration/issues/414 |
| ICON Configuration setup for E2E | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/414 |
| Archway Configuration setup for E2E testing | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/412 |
| Relay - God wallet Configuration | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/408 |
| Archway - Build Binary File | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/405 |
| ICON - Gochain Dockerimage File | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/402 |
| Archway - God wallet Configuration | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/404 |
| Archway - Custom Image Update | Not Started | E2E Testing - https://github.com/icon-project/IBC-Integration/issues/403 |
| Archway - Relay Integration Testing | In Progress | Integration Testing - https://github.com/icon-project/IBC-Integration/issues/411 |
| Relay - Packet Flow from Archway to Relay | In Progress | Integration Testing - https://github.com/icon-project/ibc-relay/issues/74 |
| Relay - Archway Connection flow integration | In Progress | Integration Testing - https://github.com/icon-project/IBC-Integration/issues/406 |
| Relay - Archway Channel Flow Integration | In Progress | Integration Testing - https://github.com/icon-project/ibc-relay/issues/13 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
