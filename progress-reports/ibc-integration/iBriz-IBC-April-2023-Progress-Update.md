# IBC - April 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-April-2023 to 30-April-2023

## Summary
Integration of IBC to connect ICON with Polygon and Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay

## Amendments to roadmap

| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| IBC implementation on Polygon to be placed on hold | Polygon IBC implementation for ICON to be placed on hold | Prioritize implementation of Archway and ICON. Another chain to be confirmed and prioritized later. | Archway and ICON IBC Implementation |

## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| ICON Connection Method implementation | Completed | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/18 |
| ICON Channel Method implementation | Completed | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/19 |
| ICON xCall Service for IBC | Completed | IBC xCall Service for ICON | https://github.com/icon-project/ibc-integration/issues/97 |
| ICS Vector Commitment Proofs | Completed | ICON Lightclient for Archway Module | https://github.com/icon-project/ibc-integration/issues/96 |
| Add interface for ICS-23 | Completed | ICON Lightclient for Archway Module | https://github.com/icon-project/ibc-integration/issues/150 |
| Protofile Generation from the Relayer for testing | Completed | ICON Lightclient for Archway Module | https://github.com/icon-project/ibc-integration/issues/149 |
| Relay IBC Types | Completed | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/16 |
| Relay Strategy / Routing | In Review | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/15 |
| Relay ICON Integration | Completed | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/14 |
| Relay Message Processor | Completed | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/12 |
| ICON Light Client Development for Archway | Completed | IBC ICON-Archway LightClient Development | https://github.com/icon-project/IBC-Integration/pull/200 |
| Archway Lightclient for ICON Implementation | Completed | IBC Archway Development. https://github.com/icon-project/ibc-integration/issues/189 |
| Adapt RLP encoding and hasing to match with ICON and Solidity Contracts| Completed | IBC Archway Development | https://github.com/icon-project/ibc-integration/issues/189 |
| Message Verfication for ICON Lightclient on Archway | Completed | IBC Archway Development | https://github.com/icon-project/ibc-integration/issues/251 |
| Signature Verfication for ICON Lightclient on Archway | Completed | IBC Archway Development | https://github.com/icon-project/ibc-integration/issues/250 |
| Integrate unit test checks on github workflow for relay | Completed | DevOps Task. https://github.com/icon-project/ibc-relay/issues/43 |
| Codecov Implementation on Relay repo | Completed | DevOps Task | https://github.com/icon-project/ibc-relay/issues/40 |
| Codecov Implementation on Integration repo | Completed | DevOps Task | https://github.com/icon-project/ibc-integration/issues/181 |
| Test Plan Document | In Draft | Create a test plan document in collaboration with Hugobytes | |
| Relay ICON Integration | Completed | ICON Module of Relay to Integrate with Archway Lightclient in ICON | https://github.com/icon-project/ibc-relay/issues/14 |
| ICON Mock Client | Completed | ICON - Archway Module | https://github.com/icon-project/ibc-integration/issues/128 |
| Add Functional and Integration testing for Archway | Completed | Archway - ICON Lightclient | https://github.com/icon-project/ibc-integration/issues/191 |
| Archway Configuration Setup | Completed | Relay - Archway Module | https://github.com/icon-project/ibc-relay/issues/33 |
| Update write acknowledgement method and eventlog to follow IBC Spec | Completed | ICON - Archway Core module | https://github.com/icon-project/ibc-relay/issues/292 |
| Test Vector Commitment for tendermint data | Completed | ICON - Archway Lightclient | https://github.com/icon-project/ibc-integration/issues/292 |
| ICON Module proto implementation | Completed | Relay - ICON Module | https://github.com/icon-project/ibc-relay/issues/48 |
| Signature Verification for ICON Lightclient on Archway | Completed | Archway - ICON Lightclient | https://github.com/icon-project/ibc-integration/issues/250 |
| Archway Chain Processor | Completed | Relay - Archway Module | https://github.com/icon-project/ibc-relay/issues/64 |
| Archway Chain Provider | Completed | Relay - Archway Module | https://github.com/icon-project/ibc-relay/issues/34 |

## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Github Workflow Setup to build IBC-relay Project | In Progress | DevOps Task - https://github.com/icon-project/ibc-relay/issues/42 |
| Github Workflow Setup to build IBC-integration Project | Started | DevOps Task |
| Implement merkle proof verification in Java contract | In Progress | ICON - Lightclient for Archway - https://github.com/icon-project/ibc-integration/issues/326 |
| Setup and Run E2E Demo for ICON to ICON | In Progress | ICON Integration Testing - https://github.com/icon-project/ibc-integration/issues/293 |
| Lightclient handler check for Archway | In Progress | Archway - Lightclient for ICON - https://github.com/icon-project/ibc-integration/issues/208 |
| Use Vector commitments in lightclient | In Progress | ICON - Lightclient for Archway - https://github.com/icon-project/ibc-integration/issues/218 |
| IBC Core Contract Update | In Progress | Archway - Core - https://github.com/icon-project/ibc-integration/issues/340 |
| BTP Mock Client Setup for testing | In Progress | Archway - Integration Testing - https://github.com/icon-project/ibc-integration/issues/339 |
| ICON IBC and xCall Testing | In Progress | ICON - Integration Testing - https://github.com/icon-project/ibc-integration/issues/163 |
| Archway Query | In Progress | Relay - Archway Module - https://github.com/icon-project/ibc-relay/issues/53 |
| Archway Transactions | In Progress | Relay - Archway Module - https://github.com/icon-project/ibc-relay/issues/54 |
| Archway Proofs | In Progress | Relay - Archway Module - https://github.com/icon-project/ibc-relay/issues/55 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
