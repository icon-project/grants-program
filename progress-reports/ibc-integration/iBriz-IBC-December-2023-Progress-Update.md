# IBC - December 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-December-2023 to 31-December-2023

## Summary
Integration of IBC to connect ICON with Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay

## Milestones
Milestone 1 - Testnet Deployment on Archway and ICON - 11th August 2023 - Completed <br>
Milestone 2 - Testnet Deployment - ICON - Libson, Archway and Neutron - 12th September 2023 - Completed <br>
Milestone 3 - Mainnet Deployment - ICON and Archway - 6th October 2023- Completed <br>
Milestone 4 - Mainnet Deployment - IBC Neutron - 31st October 2023- Completed <br>
Milestone 5 - Mainnet Deployment - IBC Injective - 5th January 2024 - Completed <br>
Milestone 6 - Centralised Relay for Avalanche and ICON - TBD <br>


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Testnet and Mainnet Release over IBC for Injective | Completed | Mainnet Deployment | https://github.com/icon-project/IBC-Integration/issues/803 |
| Centralized Relay core integration of ICON and Avalanche | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/1 |
| Update documentation for Centralised Relay | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/13 |
| Solidity: Implement new message flow | Completed | xCall Enhancements - https://github.com/icon-project/xcall-multi/issues/177 |
| Solidity: Implement Persistent message | Completed | xCall Enhancements - https://github.com/icon-project/xcall-multi/issues/186 |
| Rust: Implement Persistent message | Completed | xCall Enhancements - https://github.com/icon-project/xcall-multi/issues/187 |
| xCall multi - Upgrade using the library | Completed | xCall Enhancements - https://github.com/icon-project/xcall-multi/issues/206 |
| Improvements for the e2e-integration-test-setup tutorial | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/13 |
| E2E testing setup | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/42 |
| Module Integration - ICON & Avalance | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/61 |
| Chains Mapping with NID | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/43 |
| Missing src chain from event parse | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/48 |
| Using criterion for identifying duplicate message | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/51 |
| EVM chain - block Finality | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/41 |
| Flush message test | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/59 |
| Retry logic for chains network | Completed | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/37 |
| Fix sequence mismatch on estimate txn | Completed | Centralised relay and xcall integration - https://github.com/icon-project/ibc-relay/issues/197 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| Hopchain | In Progress | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760. Testing and Integration of ICS20. |
| xCall Execution | In Progress | Centralised Relay - https://github.com/icon-project/centralised-relay/issues/73 |
| Archway Module - Centralised Relay | In Progress | Centralised Relay - https://github.com/icon-project/centralised-relay/issues/10 |
| KMS Integration | In Progress | Centralised Relay - https://github.com/icon-project/centralised-relay/issues/72 |
| E2E for wormhole | In Progress | Adapters - https://github.com/icon-project/xcall-multi/issues/227 |
| ICON Devnet Setup | In Progress | Testing - https://github.com/icon-project/xcall-multi/issues/304 |
| Rust contracts for xCall update for Future proof messaging | In Progress | xCall Enhancements - https://github.com/icon-project/xcall-multi/issues/137 |



## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
