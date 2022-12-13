## Intro

This is ICON: Algorand ICON Bridge project being delivered by Applied Blockchain team. This is a progress report for Cyrus Vorwald for November 2022.

## Summary

In summary we are working on the following 3 components as part of the project:
- Off-chain Message Relayer (Golang)
Responsible for connecting Algorand and Icon, by monitoring new messages from each side, decode them, validate its transactions and forward a service request to the other side.
- BTP Message Center - BMC - (PyTeal)
Smart contract on the Algorand Blockchain, whose function is to exchange messages with the relayer, establishing the Off-Chain - On-Chain communication.
On its receiving end, should validate the messages it gets from the relayer and send them to the BSH smart contract when they contain proper services to be requested.
As a sender, should convert user requests that arrive through the BSH and encode a message to communicate those to the destination blockchain.
- BTP Service Handler - BSH -  (PyTeal)
Smart contract that provides user interaction, by performing asked services on one side and create new service requests on the other.
Will be connected with the front-end and create a new service request, upon user interaction. (e.g. burn tokens to be minted on the other side)
Also executes the services, requested from the other blockchain, that arrived in the BMC message.

## Amendments to roadmap

__Roadmap amendments__

There were no roadmap amendments since October 2022.

## Amendments to budget

There were no budget amendments since August 2022.

| Source | Amount | Time [days] | Notes |
| ------ | ------ | ----------- | ----- |
| Remaining developer days | | 44 | |
| Remaining project support days| | 14.75 | |

## Deliverables

### Accomplished this cycle

| Name | Development State | Notes | Source / location |
| ---- | ----------------- | ----- | ----------------- |
| Relayer: structures of sender module, receiver module, client module (not fully tested yet, no unit test for the sender module) | PR raised | | https://github.com/icon-project/icon-bridge/pull/831 |
| Initial iterations for the BMC and BSH algorand contracts | PR raised | | https://github.com/icon-project/icon-bridge/pull/831 |


### Projected for next cycle

__Deliverables projected for next cycle__

| Name | Development State |
| ---- | ----------------- |
| Integration between Relayer and BMC (exchange messages between both parties, establish an Encoding/Decoding protocol, validate a proper information transaction flow) | due in December |
