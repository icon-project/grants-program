# IBC - September 2024 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-September-2024 to 30-September-2024

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
Milestone 10 - xCall on SUI - August 2024 - Completed <br>
Milestone 11 - xCall on Neon EVM - TBD - On Hold <br>
Milestone 12 - xCall on Stellar - September 2024 - Completed <br>
Milestone 13 - xCall on Solana - September 2024 - Completed


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Monitoring tool for Relayer status | In Review | Centralized Relay | https://github.com/icon-project/centralized-relay/673 |
| Optimize the efficiency of blocks and transactions fetching in wasm chains | In Review | Centralized Relay | https://github.com/icon-project/centralized-relay/223 |
| xCall on Solana | Completed | xCall integration with centralized relay on Solana | https://github.com/icon-project/ibc-planning/issues/392 |
| [Fixes] EVM - xcall 2.1 Upgrades | Completed | Hot Fix | https://github.com/icon-project/xcall-multi/364 |
| Internal Audit - Cross Chain Token | Completed | Audit | https://github.com/icon-project/icon-projects-planning/478 |
| Stellar - xcall contracts - Mainnet Deployment | Completed | xCall integration with centralized relay on Stellar | https://github.com/icon-project/icon-projects-planning/412 |
| Implement SAST (Static Application Security Testing) | Completed | DevOps | https://github.com/icon-project/ibc-integration/886 |
| Run centralized relay in docker container | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/356 |
| Implement event listener and parsing for the transmit ready event | Completed | Relay Security Upgrade | https://github.com/icon-project/centralized-relay/376 |
| Implement different processMessages function for different modes | Completed | Relay Security Upgrade | https://github.com/icon-project/centralized-relay/378 |
| Add mechanisms to sign packet and act on the initial event including contract interaction | Completed | Relay Security Upgrade | https://github.com/icon-project/centralized-relay/375 |
| Implement event listener and parsing for the initial event | Completed | Relay Security Upgrade | https://github.com/icon-project/centralized-relay/374 |
| Expose configuration to specify cluster mode in the relayer | Completed | Relay Security Upgrade | https://github.com/icon-project/centralized-relay/373 |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| xCall on Stellar |  Audit | xCall integration with centralized relay on Stellar - https://github.com/icon-project/ibc-planning/issues/380 |
| Swap Intent |  In Progress | Swap Intent Development - https://github.com/icon-project/ibc-planning/issues/494 |
| Relayer Security Upgrades |  In Progress | Relay Cluster Development - https://github.com/icon-project/ibc-planning/issues/495 |


## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
