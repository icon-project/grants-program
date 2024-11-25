# IBC - June 2024 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-June-2024 to 30-June-2024

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
Milestone 10 - xCall on SUI - July 2024 - In Progress <br>
Milestone 11 - xCall on Neon EVM - TBD - On Hold <br>
Milestone 12 - xCall on Stellar - July 2024 - In Progress <br>
Milestone 13 - xCall on Solana - August 2024 - In Progress


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| SUI - xCall Contract Translation | Completed | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/281 |
| SUI - xCall Contract Testnet Deployment | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/394 |
| SUI - Auto executor | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/213 |
| refactor: Sui Listener and add last processed tx info to track the relayed messages of the source chain | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/258 |
| SUI - Devnet Setup | Completed | Centralized Relay | https://github.com/icon-project/ICON-Projects-Planning/issues/434 |
| Internal Audit - SUI - Balanced and xCall | Completed | Centralized Relay | https://github.com/icon-project/ICON-Projects-Planning/issues/444 |
| SUI - Documentation | Completed | Documentation | https://github.com/icon-project/ICON-Projects-Planning/issues/347 |
| Solana - Centralized Relay - Listeners | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/189 |
| Solana - Centralized Relay - Transaction Execution & Message Routing | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/188 |
| Solana - Centralized Relay - KMS | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/187 |
| Solana - Centralized Relay - Config and Interfaces | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/186 |
| Solana - Devnet Setup | Completed | Centralized Relay | https://github.com/icon-project/ICON-Projects-Planning/issues/441 |
| Deployment script consolidation | Completed | DevOps | https://github.com/icon-project/IBC-integration/issues/864 , https://github.com/icon-project/IBC-integration/issues/863 |
| Centralized Relay Production Fixes | Completed | Prod Support | https://github.com/icon-project/centralized-relay/issues/260 , https://github.com/icon-project/centralized-relay/issues/241 , https://github.com/icon-project/centralized-relay/issues/247 , https://github.com/icon-project/centralized-relay/issues/262 , https://github.com/icon-project/centralized-relay/issues/248 , https://github.com/icon-project/centralized-relay/issues/250 , https://github.com/icon-project/centralized-relay/issues/251 |
| [Discorvery] - Babylon Cosmos Chain | Completed | Discovery | https://github.com/icon-project/ICON-Project-Planning/issues/438 |
| [Discovery] Migrating contract ownership to multisig address in evm and cosmos | Completed | Discovery | https://github.com/icon-project/ICON-Project-Planning/issues/439 |
| [Discover] Administration tools for relayer. | Completed | Discovery | https://github.com/icon-project/centralized-relay/issues/192 |
| gnosis safe for EVM and Cosmwasm contracts | In Testing | Security | https://github.com/icon-project/ICON-Project-Planning/issues/437 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| Hopchain | On Hold | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760 . Paused due to upgrades in the relay for centauri presented alot of compatibility issues. Further testing and development required. |
| xCall on SUI | In Review | xCall integration with centralized relay on SUI - https://github.com/icon-project/ibc-planning/issues/334. In External Audit |
| xCall on Stellar |  In Progress | xCall integration with centralized relay on Stellar - https://github.com/icon-project/ibc-planning/issues/380 |
| xCall on Solana |  In Progress | xCall integration with centralized relay on Solana - https://github.com/icon-project/ibc-planning/issues/392 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
