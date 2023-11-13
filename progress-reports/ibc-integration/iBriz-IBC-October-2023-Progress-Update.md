# IBC - October 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by iBriz Team. 
The next phase of the project will include Centralised Relay development, Hopchain integration, Wormhole and Layerzero adapter integration as well as integration of priority chains to the bridging ecosystem. The report is from  1-October-2023 to 31-October-2023

## Summary
Integration of IBC to connect ICON with Archway
For more details please see : <br>
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay

## Milestones
Milestone 1 - Testnet Deployment on Archway and ICON - 11th August 2023 - Completed
Milestone 2 - Testnet Deployment - ICON - Libson, Archway and Neutron - 12th September 2023 - Completed
Milestone 3 - Mainnet Deployment - ICON and Archway - 6th October - Completed
Milestone 4 - Mainnet Deployment - Neutron - 31st October - Completed


## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| Mainnet Release | Completed | Mainnet release on Archway and Neutron. | https://github.com/icon-project/IBC-Integration/wiki/%5BMainnet%5D-IBC-Integration-Mainnet-Contract-Addresses |
| Mock dapp for Solidity | Completed | Translate mock dapp for evm chains | https://github.com/icon-project/xcall-multi/issues/133 |
| Develop Centralized Relay Core Logic | Completed | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/2 |
| Avalanche - Listeners | In Review | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/8 |
| Avalanche - Providers | In Review | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/9 |
| ICON - Providers | In Review | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/6 |
| ICON - Listeners | In Review | Centralised Relay | https://github.com/icon-project/centralised-relay/issues/5 |
| Core Adapter Development for xcall over Layerzero | In Review | Adapters | https://github.com/icon-project/xcall-multi/issues/147 |
| Core Adapter Development for xcall over Wormhole | In Review | Adapters | https://github.com/icon-project/xcall-multi/issues/147 |
| Base - Wormhole Module | In Review | Adapters | https://github.com/icon-project/xcall-multi/issues/109 |
| Avalanche - LayerZero Module | In Review | Adapters | https://github.com/icon-project/xcall-multi/issues/115 |
| BSC - LayerZero Module | In Review | Adapters | https://github.com/icon-project/xcall-multi/issues/114 |



## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| Testnet and Mainnet Release over IBC for Injective | Started | Testnet and Mainnet release of IBC on Injective |
| Hopchain | In Progress | Cosmos SDK chains integration with centauri - https://github.com/icon-project/IBC-Integration/issues/760. Translation of Lightclient is complete but facing issues with compatibility of the current relayer and the version of wasm client on centauri chain. Further investigation in progress to mitigate blockers in progress. |
| Centralized Relay core integration of ICON and Avalanche | In Progress | Centralised relay and xcall integration - https://github.com/icon-project/centralised-relay/issues/1 |
| Wormhole Adapter | In Progress | Testing of wormhole adapters on EVM chains - https://github.com/icon-project/xcall-multi/issues/105 |
| LayerZero Adapter  | In Progress | Testing of layerzero adapters on EVM chains - https://github.com/icon-project/xcall-multi/issues/111 |




## Sample of docs
https://github.com/icon-project/IBC-Integration <br>
https://github.com/icon-project/ibc-relay <br>
https://github.com/icon-project/xcall-multi <br>
https://github.com/icon-project/centralised-relay
