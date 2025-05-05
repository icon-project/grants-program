# Tracker Monthly Report

This is a progress update for 3/2025 on infrastructure provided by sudoblock including development of the tracker, indexer, and operation of RPC endpoints being used to support the ICON ecosystem. 

### Summary

For the frontend this month was a light month after clearing out a lot of the backlogs for the frontend. Most work has been on the backend was we're in the middle of a final migration after realizing some bad designs the current DB is running on. This month was mostly working through some of the nuances of the migration of these production workloads. 

### [icon-transformer](https://github.com/sudoblockio/icon-transformer)

#### Open Issues

| Number | Name | Status | Created | Notes |
| --- | --- | --- | --- | --- | 
| [76](https://github.com/sudoblockio/icon-transformer/pull/76) | chore(main): release 0.3.5 | open | 2023-05-29T19:14:58Z | | 

### Infrastructure 

- Ran numerous benchmarks to figure out optimal server configuration parameters 
  - Able to double performance of the nodes for DB / blockchain applications 
  - Figured out real bottlenecks and working towards new deployment strategy 
- Added new active alarms as just scripts 
  - Before was just probes to see if endpoint was active. Now we send RPC payloads and do other custom logic on http probes which make up our status pages and alarms 

## Downtime Incidents

| Date | Total Downtime | Cause | Resolution |
| --- | --- | --- | --- |

> None to be reported 

> Report generated with [tackle](https://github.com/robcxyz/tackle-box)