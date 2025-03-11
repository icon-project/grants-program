# IBC - April 2024 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-April-2024 to 30-April-2024

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
Milestone 10 - xCall on SUI - June 2024 - In Progress <br>
Milestone 11 - xCall on Neon EVM - TBD - On Hold <br>
Milestone 12 - xCall on Stellar - July 2024 - In Progress <br>
Milestone 13 - xCall on Solana - August 2024 - In Progress


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| SUI - Centralized Relay - Config and Interfaces | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/151 |
| SUI - Centralized Relay - KMS Integration | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/152 |
| SUI - Centralized Relay - Transaction Execution & Message Routing | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/141 |
| SUI - Centralized Relay - Listeners | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/142 |
| SUI - RLP Encoding | Completed | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/284 |
| SUI - Adapter | Completed | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/282 |
| SUI - xcall contract Translation | In Review | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/281 |
| Stellar - Centralized Relay - Config and Interfaces | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/169 |
| Stellar - Centralized Relay - KMS Integration | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/168 |
| Stellar - Centralized Relay - Transaction Execution & Message Routing | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/167 |
| Stellar - Centralized Relay - Listeners | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/166 |
| Stellar - RLP Encoding | Completed | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/284 |
| Stellar - Adapter | Completed | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/292 |
| Stellar - xcall contract Translation | In Review | Centralized Relay | https://github.com/icon-project/xcall-multi/issues/295 |
| xCall 2.1 - Mainnet Deployment | Completed | xcall enhancement | https://github.com/icon-project/xcall-multi/issues/286 |
| Discovery - Centralized Relay, xcall and Balanced on Solana | Completed | Discovery | https://github.com/icon-project/ICON-Project-Planning/issues/423 |
| xcall 2.1 - Code Coverage - Solidity | Completed | xcall enhancement | https://github.com/icon-project/xcall-multi/issues/282 |
| Bug when generating message with manual relay cmd | Completed | Centralized Relay - Bug fix | https://github.com/icon-project/centralized-relay/issues/164 |
| Auto clean expired messages | Completed | Centralized Relay - Bug fix | https://github.com/icon-project/centralized-relay/issues/170 |
| Add event subscription instead of polling | Completed | Centralized Relay - Bug fix | https://github.com/icon-project/centralized-relay/issues/158 |
| Try CallMessage event only twice | Completed | Centralized Relay - Bug fix | https://github.com/icon-project/centralized-relay/issues/162 |
| Start height priority from config instead of db for icon | Completed | Centralized Relay - Bug fix | https://github.com/icon-project/centralized-relay/issues/163 |
| Local KMS Support | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/165 |
| Differences in xcall empty reply encoding | Completed | Centralized Relay - Bug fix | https://github.com/icon-project/xcall-multi/issues/291 |
| Centralized Relay - Enhancement Exploration | Completed | Centralized Relay - Enhancements | https://github.com/icon-project/ICON-Project-Planning/issues/420 |
| Utilize go workspace rather the single `go.mod` to separate dependencies between main module and e2e modulet | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/184 |
| Internal Audit - Hopchain - Java Contracts | Completed | Hopchain | https://github.com/icon-project/ICON-Projects-Planning/issues/428 |
| Internal Audit - Hopchain - wasm contract changes | Completed | Hopchain | https://github.com/icon-project/ICON-Projects-Planning/issues/429 |
| Stress test relayer | Completed | Centralized Relay | https://github.com/icon-project/centralized-relay/issues/183 |

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
