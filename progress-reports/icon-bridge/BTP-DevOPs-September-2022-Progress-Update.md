# BTP DevOps - September 2022 Progress Update



## Intro
This is Icon Bridge by iBriz DevOps Team. This is progress report 3 from 1-September-2022 to 30-September-2022.

## Summary
Set up environment for the production release of ICON-BSC integration, created github workflow for testnet deployment and implementation of code coverage reporting using codecov.

## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:-----|:------------------|:------|:------------------|
| Separate solidity integration test to separate jobs in Github Actions | Completed | Update the actions to allow running them in parallel to reduce test time | https://github.com/icon-project/icon-bridge/issues/411 |
| Add CodeQL static analysis workflow | Completed | Add CodeQL to scan the Java and Go code bases for vulnerabilities | https://github.com/icon-project/icon-bridge/issues/355 |
| Pipeline for Solidity BTS deployment on BSC Testnet | Completed | Deployment pipeline to deploy Solidity BTS on BSC Testnet | https://github.com/icon-project/icon-bridge/issues/345|
| Pipeline for Solidity BMC deployment on BSC Testnet | Completed | Github actions pipeline for Solidity BMC deployment on BSC Testnet | https://github.com/icon-project/icon-bridge/issues/344 |
| Action to build and generate artifacts | Completed | Deployment flow to build and generate artifacts to respective servers after release using Github Actions | https://github.com/icon-project/icon-bridge/issues/202 |
| Script to configure and register token for BSC & Icon | Completed | Generating BMR config at deployment time | https://github.com/icon-project/icon-bridge/issues/442 |
| Create Github Actions pipeline for BSC<>Icon link | Completed | Before deploying BMR, we need to create link between the two chains | https://github.com/icon-project/icon-bridge/issues/424 |
| Action to manually deploy contracts in Testnet | Completed | Manual actions that can be triggered from the Actions tab for deploying the contracts on Testnet | https://github.com/icon-project/icon-bridge/issues/236 |
| Build a pipeline to generate BMR config and deploy BMR docker image | Completed | Pipeline to generate config and deploy BMR docker image | https://github.com/icon-project/icon-bridge/issues/425 |
| BMR Deployment setup with Github Actions | Completed | Deploy BMR artifact by choosing the github tag | https://github.com/icon-project/icon-bridge/issues/218 |
| Github Actions to deploy and configure contracts to generate .env file | Completed | Manual actions that can be triggered from the Actions tab for deploying the contracts | https://github.com/icon-project/icon-bridge/issues/219 |
| Fix BMC integration test failure | Completed | Fix issues with integration test failing | https://github.com/icon-project/icon-bridge/issues/414 |
| Fix: Unexpected Coverage Change False Alarm | Completed | Fix issues with unexpected codecov pipeline failure | https://github.com/icon-project/icon-bridge/issues/462 |
| Documentation for Repository Managemen | Completed 1st Draft | Documentations | https://github.com/icon-project/icon-bridge-planning/issues/33 |


## Deliverables Projected for Next Cycle

None


## Sample of docs
https://github.com/icon-project/icon-bridge/blob/main/README.md 
