# IBC - July 2024 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-July-2024 to 31-July-2024

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
Milestone 8 - Centralised Relay integration for Archway - 29th March - Completed <br>
Milestone 9 - Hopchain and ICS20 Integration to IBC - TBD - In Progress <br>
Milestone 10 - xCall on SUI - August 2024 - In Progress <br>
Milestone 11 - xCall on Neon EVM - TBD - On Hold <br>
Milestone 12 - xCall on Stellar - September 2024 - In Progress <br>
Milestone 13 - xCall on Solana - September 2024 - In Progress


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Stellar - Internal Review - xcall Contracts | Completed | Centralized Relay - Internal Security review and fixes | https://github.com/icon-project/ICON-Project-Planning/issues/409 |
| SUI - Audit Support | In Progress | Centralized Relay | - |
| gnosis safe for EVM and Cosmwasm contracts | Completed | Security | https://github.com/icon-project/ICON-Project-Planning/issues/437 |
| Cleanup and fix failing test cases | Completed | Devops | https://github.com/icon-project/centralized-relay/issues/280 |
| [BUG]: wasm keyring gets cleared randomly. | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/288 |
| Listen for XCALL rollback event | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/193 |
| Cleanup e2e test cases removing unwanted/unused functions | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/287 |
| Make consistency of toolchain version in ci files | Completed | Devops | https://github.com/icon-project/xcall-multi/issues/340 |
| while saving message in db for sui callMessage event, dappModuleCapId also needs to saved. Because when we retry we need that field to determine the module on which ExecuteCall has to be executed | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/271 |
| Ability to disable batch queries | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/301 |
| Wait for certain interval when syncing | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/305 |
| Last saved block returns 0 on empty database | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/304 |
| High CPU usage when using cosmos chains | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/321 |
| SDK lock prevents key storation | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/325 |
| Update rust version from 1.69.0 to 1.78.0 | Completed | IBC | https://github.com/icon-project/IBC-Integration/issues/873 |
| Polygon - xcall Deployment on testnet and mainnet | Completed | Centralized Relay | https://github.com/icon-project/ICON-Projects-Planning/issues/473 |
| refactor: Sui Listener and add last processed tx info to track the relayed messages of the source chain | Completed | Centralized Relay | https://github.com/icon-project/ICON-Projects-Planning/issues/258 |
| Update e2e for auto rollback feature in icon/evm/wasm chains | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/282 |
| Use batch block polling strategy | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/248 |
| Docker image of rly not being built | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/213 |
| Improve message recovery | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/249 |
| Gas optimization for evm | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/245 |
| Optimize resource usage | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/246 |
| Optimize nonce tracker for evm and cosmwasm | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/247 |
| Early exit strategy for network failures | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/251 |
| Solana - xCall Contract Translation | In Review | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/300 |
| Solana - RLP Encoding | In Review | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/301 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| Hopchain | On Hold | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760 . Paused due to upgrades in the relay for centauri presented alot of compatibility issues. Further testing and development required. |
| xCall on SUI | Audit | xCall integration with centralized relay on SUI - https://github.com/icon-project/ibc-planning/issues/334. In External Audit |
| xCall on Stellar |  Internal Review | xCall integration with centralized relay on Stellar - https://github.com/icon-project/ibc-planning/issues/380 |
| xCall on Solana |  Integration Testing | xCall integration with centralized relay on Solana - https://github.com/icon-project/ibc-planning/issues/392 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
