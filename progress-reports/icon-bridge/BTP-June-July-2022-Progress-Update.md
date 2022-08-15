# BTP - June/July 2022 Progress Update

## Intro
This progress report is for Icon Bridge related development work by iBriz Team. The report is from  1-June-2022 to 31-July-2022

## Summary
Build an usable centralized bridge for BTP Relay System which can deliver digital assets between multiple chains.
For more details please see - https://github.com/icon-project/icon-bridge/blob/main/README.md 

## Amendments to roadmap
Change of focus from Harmony to BSC towards end of June
BSC release date set to 15th August 2022
Simpson leaving the project caused heavy workload changes in Smart Contracts from July
Roadmap Amendments

| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| BSC Release to Testnet | Due date set to August 8th | After the hack on Harmony chain, the focus shifted from Harmony to BSC | None |
| BSC Release to Mainnet | Due date set to August 15th | After testing the release on testnet and verified all the relays are working as expected, to be deployed on Mainnet | BSC Release to Testnet |




## Deliverables Ready


| Name | Development State | Notes | Source / location |
|:----- |:------------------ | :----| :----------------| 
| E2E Test Framework | Released | https://github.com/icon-project/icon-bridge/discussions/141 | https://github.com/icon-project/icon-bridge/issues/44  | Icon side Verification for Relay | Released |
| Adaptable Gas Fees | Released | determine a gas price that ensures a transaction will be included in a block within a user’s required timeline without overpaying | https://github.com/icon-project/icon-bridge/issues/26 | 
| BSC Receiver Optimization | Released | When the relay is restarted and the number of blocks to process is high, the synchronization should complete without any errors. | https://github.com/icon-project/icon-bridge/issues/112 | 
| Updating Contract Deployment Scripts | Released | Deploy contracts on Testnet and output necessary config | https://github.com/icon-project/icon-bridge/issues/180 | 
| BSC Release to Testnet | Released | After the hack on Harmony chain, the focus shifted from Harmony to BSC | Github Repo | 
| BSC Release to Mainnet | Review in Progress | After testing the release on testnet and verified all the relays are working as expected, to be deployed on Mainnet | Github Repo |
| Refine Logging for Relay | Released | Add supplemental logging to help debug. | https://github.com/icon-project/icon-bridge/issues/159 |
| Implement token Limit for BTS Java Contracts | Released | https://docs.google.com/document/d/172B4A6Fo6o5rgO263qCb099Q4IlOV7EJP0D2GtNU4d8/edit | https://github.com/icon-project/icon-bridge/issues/140 |
| Intrachain Blacklisting of addresses | Released | When a blacklist is set on ICON, the addresses are added to the blacklist only after successful response. This will be an issue when a user has to be blacklisted on ICON because BTPAddress of ICON will not be added in links of BMC, and relay for Intrachain transfer will not be maintained | https://github.com/icon-project/icon-bridge/issues/182 |
| BTS Contract Updates | Released | The class BTS Properties in javascore includes 2 fields, sn and feeRatio. Since feeRatio has been implemented for each token, it is not required to implement global feeRatio. Similarly, on removing feeRatio, it's not necessary to make a custom class just for sn. | https://github.com/icon-project/icon-bridge/issues/139 |


## Deliverables Projected for Next Cycle


| Name | Development State | Notes |
|:-----|:------------------|:-----|
| BSC Mainnet Release | Almost complete | This is almost complete and is running through internal reviews. Planned to be released by 15th August |
| Assist with Security Audit | Not Started | The Security Audit will start from the 15th August. Any information needed to be provided or fixes needed based on security audit review will be provided adhoc.|
| Assist with Near release and integration | Not Started | Near integration deployment is being planned for 18th August. Team to assist. |



## Sample of docs
https://github.com/icon-project/icon-bridge/blob/main/README.md 

