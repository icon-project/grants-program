# IBC - May 2024 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-May-2024 to 31-May-2024

## Summary
Integration of xcall to connect ICON and Balanced with prioritized chains.

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
Milestone 10 - xCall on SUI - June 2024 - In Progress <br>
Milestone 11 - xCall on Neon EVM - TBD - On Hold <br>
Milestone 12 - xCall on Stellar - July 2024 - In Progress <br>
Milestone 13 - xCall on Solana - August 2024 - In Progress


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------|
| Stellar - Centralized Relay - Transaction Execution & Message Routing | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/167 |
| add target in Makefile to statically build relayer | Completed | DevOps | https://github.com/icon-project/centralized-relay/issues/181 |
| Add option to run e2e on remote devenet chain | Completed | DevOps | https://github.com/icon-project/IBC-Integration/issues/829 |
| Make gas-limit configurable | Completed | Centralized Relay - Bug Fix | https://github.com/icon-project/centralized-relay/issues/211 |
| Issue with injective chain | Completed | Centralized Relay - Bug Fix | https://github.com/icon-project/centralized-relay/issues/182 |
| Issue with multiple cosmos based chains setup | Completed | Centralized Relay - Bug Fix | https://github.com/icon-project/centralized-relay/issues/217 |
| [Hopchain ICS20Transfer Contract] No caller validation for public external function used for refund | Completed | Hopchain - Audit fix | https://github.com/icon-project/ICON-Projects-Planning/issues/430 |
| Hopchain ICS08 TendermintLC Contract| Completed | Hopchain - Audit fix | https://github.com/icon-project/ICON-Projects-Planning/issues/431 |
| SUI: Contract integration in the relayer | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/204 |
| SUI - Balanced Contract Translation | Completed | Centralized Relay | https://github.com/icon-project/ICON-Projects-Planning/issues/400 |
| Poly network hack study | Completed | Prod Support | https://github.com/icon-project/ICON-Projects-Planning/issues/422 |
| Axelar Amplifier Discovery | Completed | Discovery | https://github.com/icon-project/IBC-Integration/issues/860 |
| SUI - E2E testing framework integration | Completed | E2E Testing | https://github.com/icon-project/ICON-Projects-Planning/issues/398 |
| RLP issue for large message data in SUI | Completed | Bug Fix | https://github.com/icon-project/xcall-multi/issues/315 |
| add stellar test workflow | Completed | DevOps| https://github.com/icon-project/xcall-multi/issues/311 |
| Deploy Centralized relay on mainnet | Completed | Centralized Relay| https://github.com/icon-project/centralized-relay/issues/861 |
| Stress test relayer | Completed | Centralized Relay| https://github.com/icon-project/centralized-relay/issues/183 |
| SUI - xCall Contract Testnet Deployment | Completed | Centralized Relay| https://github.com/icon-project/ICON-Projects-Planning/issues/394 |
| SUI - Devnet Setup | Completed | DevOps | https://github.com/icon-project/ICON-Projects-Planning/issues/434 |
| Stellar - Devnet Setup | Completed | DevOps | https://github.com/icon-project/ICON-Projects-Planning/issues/435 |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| Hopchain | In Progress | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760 . Testing, E2E and Integration of ICS20 on testnet in progress |
| xCall on SUI | In Progress | xCall integration with centralized relay on SUI - https://github.com/icon-project/ibc-planning/issues/334 |
| xCall on Stellar |  In Progress | xCall integration with centralized relay on Stellar - https://github.com/icon-project/ibc-planning/issues/380 |
| xCall on Solana |  In Progress | xCall integration with centralized relay on Solana - https://github.com/icon-project/ibc-planning/issues/392 |

## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
