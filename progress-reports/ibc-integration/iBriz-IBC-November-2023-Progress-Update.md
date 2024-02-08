# IBC - November 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of other chains to the bridging ecosystem. The report is from  1-November-2023 to 30-November-2023

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
Milestone 3 - Mainnet Deployment - ICON and Archway - 6th October - Completed <br>
Milestone 4 - Mainnet Deployment - Neutron - 31st October - Completed <br>
Milestone 5 - Mainnet Deployment - Injective - TBD - In Progress <br>
Milestone 6 - Centralised Relay for Avalanche and ICON - 15th December <br>


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Avalanche - Listeners | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/8 |
| Avalanche - Providers | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/9 |
| ICON - Providers | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/6 |
| ICON - Listeners | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/5 |
| Flush Logic | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/32 |
| Verifier RPC Client | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/27 |
| ICON & Avalanche - Module Interaction testing | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/15 |
| EVM Gas Estimation | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/28 |
| Core Adapter Development for xcall over Layerzero | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/147 |
| Core Adapter Development for xcall over Wormhole | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/147 |
| Base - Wormhole Module | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/109 |
| Avalanche - LayerZero Module | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/115 |
| BSC - LayerZero Module | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/114 |
| Add Airdrop Functionality to Wormhole | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/169 |
| Add Airdrop Functionality to LayerZero | Completed | Adapters | https://github.com/icon-project/xcall-multi/issues/170 |
| Injective Testnet Integration to IBC | Completed | IBC | https://github.com/icon-project/ibc-integration/issues/777 |
| Update relay build to support Injective | Completed | IBC | https://github.com/icon-project/ibc-integration/issues/782 |
| [BUG] IBC Relay - Recovery from older height not capturing all the transaction | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/196 |
| [BUG] IBC Relay - Multiple messages per update | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/189 |
| [BUG] IBC Relay - Memory Leakage Issue | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/297 |
| Injective relay error | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/188 |
| [BUG] IBC Relay - UpdateClient should only go to relevant chains | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/188 |
| [BUG] IBC Relay - Multiple retry of Transactions with UpdateClient | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/188 |
| Fix missing version name in cosmwasm artifact file | Completed | IBC | https://github.com/icon-project/ibc-relay/issues/198 |
| Rust: Implement new message flow | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/183 |
| create demo for JVM-Cosmwasm | Completed | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/200 |
| xCall multi - Upgrade solidity contract using library | In Review | xCall Enhancements | https://github.com/icon-project/xcall-multi/issues/206 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:------|
| Testnet and Mainnet Release over IBC for Injective | In Progress | Deployed and Testing in Progress in Berlin. To be deployed on Libson and Mainnet |
| Hopchain | In Progress | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760. Current blocker due to Protobuf file changes on ICON. Investigation ongoing |
| Centralized Relay core integration of ICON and Avalanche | In Progress | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/1 |




## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
