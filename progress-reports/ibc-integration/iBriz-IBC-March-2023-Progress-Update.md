# IBC - March 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. The report is from  1-March-2023 to 31-March-2023

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
| ICON IBC Handler Development | Complete | IBC Handler Development for ICON | https://github.com/icon-project/IBC-Integration/pull/49 |
| ICON IBC Host Development | Completed | IBC Host Development for ICON | https://github.com/icon-project/IBC-Integration/pull/37 |
| ICON Relay Configuration Setup | Complete | IBC Relay Development - ICON Module| https://github.com/icon-project/ibc-relay/issues/24 |
| ICON Client Setup | Complete | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/23 |
| ICON Event Parser | Complete | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/22 |
| ICON Message Handlers | Complete | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/20 |
| ICON Chain Processor | Complete | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/21 |
| ICON Chain Provider | Complete | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/25 |
| ICON Connection Method implementation | In Review | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/18 |
| ICON Channel Method implementation | In Review | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/19 |
| ICON xCall Service for IBC | In Review | IBC xCall Service for ICON | https://github.com/icon-project/ibc-integration/issues/97 |
| ICS Vector Commitment Proofs | In Review | ICON Lightclient for Archway Module | https://github.com/icon-project/ibc-integration/issues/96 |
| Add interface for ICS-23 | In Review | ICON Lightclient for Archway Module | https://github.com/icon-project/ibc-integration/issues/150 |
| Protofile Generation from the Relayer for testing | In Review | ICON Lightclient for Archway Module | https://github.com/icon-project/ibc-integration/issues/149 |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| ICON xCall Service for IBC | In Review | https://github.com/icon-project/ibc-integration/issues/97 |
| Relay IBC Types | Started | IBC Relay Development - ICON Module | https://github.com/icon-project/ibc-relay/issues/16 |
| Relay Strategy / Routing | Started | IBC Relay Development - ICON Module. https://github.com/icon-project/ibc-relay/issues/15 |
| Relay ICON Integration | Started | IBC Relay Development - ICON Module. https://github.com/icon-project/ibc-relay/issues/14 |
| Relay Message Processor | Started | IBC Relay Development - ICON Module. https://github.com/icon-project/ibc-relay/issues/12 |
| ICON Light Client Development for Archway | In Review | IBC ICON-Archway LightClient Development. Development complete but some changes required for Vector proofs and Relay integration Testing. https://github.com/icon-project/ibc-relay/issues/12|
| Relay Message Processor | Started | IBC Relay Development - ICON Module. https://github.com/icon-project/ibc-relay/issues/12 |
| Archway Lightclient for ICON Implementation | In Progress | IBC Archway Development. https://github.com/icon-project/ibc-integration/issues/189 |
| Adapt RLP encoding and hasing to match with ICON and Solidity Contracts| Started | IBC Archway Development. https://github.com/icon-project/ibc-integration/issues/189 |
| Message Verfication for ICON Lightclient on Archway | Not Started | IBC Archway Development. https://github.com/icon-project/ibc-integration/issues/251 |
| Signature Verfication for ICON Lightclient on Archway | Not Started | IBC Archway Development. https://github.com/icon-project/ibc-integration/issues/250 |
| Github Workflow Setup to build IBC-relay Project | Not Started | DevOps Task. https://github.com/icon-project/ibc-relay/issues/42 |
| Integrate unit test checks on github workflow for relay | Not Started | DevOps Task. https://github.com/icon-project/ibc-relay/issues/43 |
| Codecov Implementation on Relay repo | Not Started | DevOps Task. https://github.com/icon-project/ibc-relay/issues/40 |
| Codecov Implementation on Integration repo | Not Started | DevOps Task. https://github.com/icon-project/ibc-integration/issues/181 |
| Test Plan Document | Not Started | Create a test plan document in collaboration with Hugobytes |
| Relay ICON Integration | Started | ICON Module of Relay to Integrate with Archway Lightclient in ICON. https://github.com/icon-project/ibc-relay/issues/14 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay
