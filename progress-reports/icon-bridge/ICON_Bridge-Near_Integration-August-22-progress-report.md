# Progress Report

**Project:**  ICON Bridge - Near Integration  
**Proposal:** Private  
**Team:** HugoByte  
**Reporting Period:** July 2022 - Aug 2022

## Summary
Development of Relay, JAVA Score and NEAR Smart Contracts has been completed and Deployed to Testnet. Couple of bugs has been identified upon testing and is being fixed. Bazel rules has been added for build which helps in hermetic builds.

## Deliverables

### Accomplished this cycle

__Deliverables ready__


| Module| Name | Development State | Notes | Source / location |
| ---- | --------- | ----------------- | ----- | ----------------- |
| BMR | [Block Monitoring Interface](https://github.com/icon-project/icon-bridge/issues/53) | Alpha | Need to be improve Block Monitoring Frequency from NEAR  | [Github repo](https://github.com/icon-project/icon-bridge/tree/hugobyte/development/cmd/iconbridge/chain/near) |
|  | [Add bazel rules for BMR](https://github.com/icon-project/icon-bridge/issues/111) | Beta | Need to be merged after finalizing build | [Github repo](https://github.com/icon-project/icon-bridge/tree/hugobyte/feature/bazel/cmd/iconbridge) |
| BMC | [Handle BTP Messages](https://github.com/icon-project/icon-bridge/issues/154) | Testing | Need to do E2E Testing | [Github repo](https://github.com/icon-project/icon-bridge/tree/hugobyte/development/rust/near/bmc/src) |
| BTS | [Coin and Token Management for NEAR BTS](https://github.com/icon-project/icon-bridge/issues/152) | Beta |  | [Github repo](https://github.com/icon-project/icon-bridge/tree/hugobyte/development/rust/near/bsh/bts/src) |
|  | [Bazel rules and provisioning - BTS](https://github.com/icon-project/icon-bridge/issues/188) | Beta |  | [Github repo](https://github.com/icon-project/icon-bridge/tree/hugobyte/feature/bazel/rust/near/bsh/bts) |
|  | [Fee Management for NEAR BTS](https://github.com/icon-project/icon-bridge/issues/153) | Beta |  | [Github repo](https://github.com/icon-project/icon-bridge/tree/hugobyte/development/rust/near/bsh/bts/src) |

### Projected for next cycle

__Deliverables projected for next cycle__
| Name | Development State | Notes |
| ---- | ----------------- | ----- |
| Functional NEAR Integration in Testnet | Testing | Bug Identified are being fixed |
| Implement E2E Testing | Not started |  |
| Improve Block Monitoring Performace | Alpha | Block Monitoring need to be improved using parellel processing of blocks |
| Configurable Coin / Token Transfer and Registration | Not Started |  |
| Improve Build and Provisioning workflow to be compatible with CI/CD | Not Started |  |
| Support Integration with Nexus Portal | Not Started | |
| Coin/Token Transfer Restriction | Not Started | |
| Implement Account Blacklisting | Not Started | |
| Fix Reconnection Issue for BMR | Not Started | |
| Add Documentation for API Reference, Build, Deployment, Tests | Not Started | |

