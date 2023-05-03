# IBC - March 2023 Progress Update

## Intro
This progress report is for IBC Integration related development work by HugoByte Team. The report is from  1-March-2023 to 31-March-2023

## Summary

Integration of IBC to connect ICON with Archway

## Amendments to roadmap
| Name  | Change | Explanation | Dependants |
| :-----| :-------| :----------| :----------|
| Implement IBC Core | Prioritize implementation of IBC Core | Prioritize implementation of IBC Core to speed up the development and iBriz team will implement the Light Client |  |

## Deliverables

### Accomplished this cycle

__Deliverables ready__
| Module| Name | Development State | Notes | Source / location |
| ---- | --------- | ----------------- | ----- | ----------------- |
| xCall | Protocol Fee Handler | Beta | | https://github.com/icon-project/IBC-Integration/pull/43 |
|  | Protocol Fee | Beta | | https://github.com/icon-project/IBC-Integration/pull/43 |
|  | CallService Implementation | Release | | https://github.com/icon-project/IBC-Integration/pull/53 |
| Test Framework | Configuration | Release | | https://github.com/icon-project/IBC-Integration/pull/45 |
|  | Integrate with CI/CD | Release | | https://github.com/icon-project/IBC-Integration/pull/194|
| IBC Core | Client - Storage implementation | Beta | | https://github.com/icon-project/IBC-Integration/pull/83 <br/> https://github.com/icon-project/IBC-Integration/pull/93 |
|  | Client - Events/Messages | Beta | | https://github.com/icon-project/IBC-Integration/pull/119 <br/> https://github.com/icon-project/IBC-Integration/pull/126 <br/> https://github.com/icon-project/IBC-Integration/pull/123 <br/> https://github.com/icon-project/IBC-Integration/pull/139 <br/> https://github.com/icon-project/IBC-Integration/pull/148 <br/> https://github.com/icon-project/IBC-Integration/pull/156 |
|  | Client - Handlers | Beta | | https://github.com/icon-project/IBC-Integration/pull/165 <br/> https://github.com/icon-project/IBC-Integration/pull/201 <br/> https://github.com/icon-project/IBC-Integration/pull/177 <br/> https://github.com/icon-project/IBC-Integration/pull/216 |
|  | Connection - Storage implementation | Beta | | https://github.com/icon-project/IBC-Integration/pull/81 <br/> https://github.com/icon-project/IBC-Integration/pull/85 <br/> https://github.com/icon-project/IBC-Integration/pull/143 |
|  | Connection - Events/Messages | Beta | | https://github.com/icon-project/IBC-Integration/pull/119 <br/> https://github.com/icon-project/IBC-Integration/pull/123 <br/> https://github.com/icon-project/IBC-Integration/pull/126 <br/> https://github.com/icon-project/IBC-Integration/pull/139 <br/> https://github.com/icon-project/IBC-Integration/pull/148 <br/> https://github.com/icon-project/IBC-Integration/pull/156 |
|  | Connection - Handlers | Beta | | https://github.com/icon-project/IBC-Integration/pull/177 <br/> https://github.com/icon-project/IBC-Integration/pull/165 <br/> https://github.com/icon-project/IBC-Integration/pull/201 <br/> https://github.com/icon-project/IBC-Integration/pull/216 |
|  | Connection - Query Handler | Beta | | https://github.com/icon-project/IBC-Integration/pull/253 <br/> https://github.com/icon-project/IBC-Integration/pull/221 |
|  | Connection Helpers | Beta | | https://github.com/icon-project/IBC-Integration/pull/222 |
|  | Channel - Storage implementation | Beta | | https://github.com/icon-project/IBC-Integration/pull/81 <br/> https://github.com/icon-project/IBC-Integration/pull/85 <br/> https://github.com/icon-project/IBC-Integration/pull/143 |
|  | Channel - Events/Messages | Beta | | https://github.com/icon-project/IBC-Integration/pull/117 <br/> https://github.com/icon-project/IBC-Integration/pull/130 <br/> https://github.com/icon-project/IBC-Integration/pull/129 <br/> https://github.com/icon-project/IBC-Integration/pull/131 <br/> https://github.com/icon-project/IBC-Integration/pull/136 <br/> https://github.com/icon-project/IBC-Integration/pull/140 <br/> https://github.com/icon-project/IBC-Integration/pull/147 |
|  | Channel - Handlers | Beta | | https://github.com/icon-project/IBC-Integration/pull/164 <br/> https://github.com/icon-project/IBC-Integration/pull/196 <br/> https://github.com/icon-project/IBC-Integration/pull/203 <br/> https://github.com/icon-project/IBC-Integration/pull/172 <br/> https://github.com/icon-project/IBC-Integration/pull/214 <br/> https://github.com/icon-project/IBC-Integration/pull/208 |


### Projected for next cycle

__Deliverables projected for next cycle__

| Module| Name | Development State | Notes |
| ---- | ---- | ----------------- | ----- |
| IBC Core | Client Context | In Progress | |
|  | Client Type Definition | Not Started | |
|  | Client - Query Handler | Not Started | |
|  | Channel - Packet and Acknowledge Module | In Progress | |
|  | Channel - Query Handler | Not Started | |
|  | Port Reader | In Progress | |
|  | Port - Module Manager | Not Started | |
|  | Port - Error Handling | Not Started  | |
|  | Host - Storage Implementation | Not Started | |
|  | Host - Path and Identifier Implementation | Not Started | |
|  | Host - Validators | Not Started | |
|  | Host - Storage Implementation/Path and Identifier Implementation/Validators | Not Started | |


