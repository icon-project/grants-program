# IBC - January 2024 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-January-2024 to 31-January-2024

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
Milestone 6 - Centralised Relay for Avalanche and ICON - 19th January 2024 - Completed <br>
Milestone 7 - xCall deployments for Wormhole and LayerZero - 5th February - Completed <br>
Milestone 8 - Centralised Relay integration for Archway - TBD - In Progress <br>
Milestone 9 - Hopchain and ICS20 Integration to IBC - TBD - In Progress <br>


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| KMS Integration | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/72 |
| ICON Devnet Setup | Completed | Testing | https://github.com/icon-project/xcall-multi/issues/304 |
| E2E for wormhole & LayerZero | Completed | Adapters - Issues with running local setup. Testing completed on testnet | https://github.com/icon-project/xcall-multi/issues/227 |
| Rust contracts for xCall update for Future proof messaging | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/137 |
| Rust contracts for xCall update for Future proof messaging | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/137 |
| LayerZero and Wormhole testing on Testnet | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/249 |
| Solidity Artefact Release | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/254 |
| xCall EVM Scripts | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/259 |
| Improvements for the e2e integration test setup tutorial | Completed | xCall Enhancements | https://github.com/icon-project/ibc-integration/issues/775 |
| ICON Bridge Issue | Completed | Prod Support | https://github.com/icon-project/ibc-planning/issues/312 |
| [Discovery] Exploration of other products involving multiple chains | Completed | Prod Support | https://github.com/icon-project/ibc-planning/issues/284 |
| Implement new message type in dapp: Solidity | Completed | xcall Enhancements | https://github.com/icon-project/xcall-multi/issues/237 |
| Implement new message type in dapp: Javascore | Completed | xcall Enhancements | https://github.com/icon-project/xcall-multi/issues/235 |
| CLI command to manually call update client | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/207 |
| CLI command to claim fees | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/205 |
| Transfer Admin and fee Handler rights on Avalanche mainnet deployment | Completed | Centralized Relay | https://github.com/icon-project/ibc-planning/issues/315 |
| Create keystore Command | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/70 |
| DB Reuse - Bug Fixes - Pagniation Issue | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/69 |
| Fix Nonce | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/88 |
| Integration Tets for Response Message Type | Completed | IBC | https://github.com/icon-project/ibc-integration/issues/796 |
| Avalanche Mainnet Deployment | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/230 |
| Implement getTimestap() function in the consensus_state_extended.go for tendermint | Completed | Centralized Relay | https://github.com/icon-project/ibc-integration/issues/823 |

## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| Hopchain | In Progress | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760. Testing and Integration of ICS20. |
| xCall Execution | In Progress | Centralised Relay - https://github.com/icon-project/centralised-relay/issues/73 |
| Archway Module - Centralised Relay | In Review | Centralised Relay - https://github.com/icon-project/centralised-relay/issues/10 |




## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
