# Progress Report

**Project:**  ICON Bridge - Near Integration  
**Proposal:** Private  
**Team:** HugoByte  
**Reporting Period:** 01 Sept 2022 - 30 Sept 2022

## Summary
Merged to main branch. Improved BMR Performance significantly, upto 50X improvement in Block Monitoring. Added Blacklisting and Transfer Restriction in BTS Contracts. Integration with Nexus has started.

## Deliverables

### Accomplished this cycle

__Deliverables ready__


| Module| Name | Development State | Notes | Source / location |
| ---- | --------- | ----------------- | ----- | ----------------- |
| E2E Testing | [E2E Test framework](https://github.com/icon-project/icon-bridge-planning/issues/47) | Alpha | Need to add test scripts  | [Github repo](https://github.com/icon-project/icon-bridge/tree/feat/402-create-chain-api-rpc-client-for-e2e-test/cmd/e2etest/chain/near) |
| BMR | [Improvement in Block Monitoring](https://github.com/icon-project/icon-bridge/issues/387) | Release |  | [Pull Request](https://github.com/icon-project/icon-bridge/pull/401) |
| BTS | [Implement Transfer Restriction](https://github.com/icon-project/icon-bridge/issues/152) | Release |  | [Pull Request](https://github.com/icon-project/icon-bridge/pull/549) |
|  | [Implement Blacklist](https://github.com/icon-project/icon-bridge/issues/188) | Release |  | [Pull Request](https://github.com/icon-project/icon-bridge/pull/408) |
|  | [Update coin id to u8[32] for performance ](https://github.com/icon-project/icon-bridge/issues/153) | Beta |  | [Pull Request](https://github.com/icon-project/icon-bridge/pull/554) |

### Projected for next cycle

__Deliverables projected for next cycle__
| Name | Development State | Notes |
| ---- | ----------------- | ----- |
| Complete Integration with Nexus Portal | In Progress | |
| Fix Reconnection Issue for BMR | Not Started | |
| Add Documentation for API Reference, Build, Deployment, Tests | In Progress | |
| Update NEAR SDK | Not Started | |
| Optimize smart contract storage | Not Started | |
| Add Code coverage | Alpha | |
| Add verifier for NEAR BMR | Not Started | |
| Fix Identified u128 serialization error | Not Started | |


