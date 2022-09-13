# BTP DevOps - August 2022 Progress Update



## Intro
This is Icon Bridge by iBriz DevOps Team. This is progress report 2 from 1-August-2022 to 31-August-2022.

## Summary
Set up environment for the production release of ICON-BSC integration, created github workflow for testnet deployment and implementation of code coverage reporting using codecov.

## Deliverables Ready

| Name | Development State | Notes | Source / location |
|:-----|:------------------|:------|:------------------|
| Github code coverage tracking and reporting | Completed | Researched code coverage solutions such as coveralls.io and codecov and went ahead with an implementation using codecov | https://github.com/icon-project/icon-bridge/issues/145 |
| Setup production environment and monitoring for ICON-BSC Beta release | Completed | Configured EC2 instances and setup monitoring and reporting environment to keep track of the BMR service | https://github.com/icon-project/icon-bridge/issues/31 |
| Javascore contracts BMC/BTS deployment to Testnet via Github actions | Completed | Implemented a workflow to manually trigger a deployment of javascore smart contracts such as BMC and BTS on Testnet (ICON) | https://github.com/icon-project/icon-bridge/issues/331, https://github.com/icon-project/icon-bridge/issues/342 |
| Solidity contracts BMC/BTS deployment to testnet with github actions | Completed | Implemented a workflow to manually trigger a deployment of solidity smart contracts such as BMC and BTS on Testnet (BSC) | https://github.com/icon-project/icon-bridge/issues/344 |
| Dockerize BMR and unified base image for build to be used with Github actions | Completed | Created a docker image that includes all the dependencies required to build each components of the BTP repo. This image is used by all github actions responsible for building such components. | https://github.com/icon-project/icon-bridge/pull/334


## Deliverables Projected for Next Cycle

| Name | Development State | Notes |
|:-----|:------------------|:------|
| Support production deployment of NEAR integration | Planning | |
| Improve stateful auto-deployment on testnet for NEAR integration | Planning | |
| Create a release flow | In Progress | https://github.com/google-github-actions/release-please-action |


## Sample of docs
https://github.com/icon-project/icon-bridge/blob/main/README.md 

