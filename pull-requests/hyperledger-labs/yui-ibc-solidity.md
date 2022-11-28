---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    Split contracts into corresponding ics directories
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * rename IClient to ILightClient
* ILightClient: fix to createClient returns one ConsensusUpdate
* update generated code
* IBCConnection: rename to setSupportedVersions
* rename IModuleCallbacks to IIBCModule
* add OwnableIBCHandler
* tests: remove clients for IBFT2Client and MockClient
* add code comments

Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 08:30:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Refactor architecture
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Core changes

- All states are defined in IBCStore contract.
- IBCHandler inherits IBCStore and is the only contract that has storage.
- IBCChannel, IBCConnection, and IBCClient also inherit IBCStore.
- IBCHandler calls the above contracts with delegatecall.

## Light Client changes

- The `createClient` and `updateClient` functions of LC contract return only the commitment of updated state and the updated height as return value. Note: serialized state is not returned.
- LC contract keeps client and consensus states in its own storage.

## Gas cost efficiency

Note: increased size of the handler is mainly due to the merging of the handler and host into a single contract.

### Before

https://github.com/hyperledger-labs/yui-ibc-solidity/actions/runs/3564254808/jobs/5987996346#step:7:168

| contracts/core/IBCHandler.sol:IBCHandler contract |                 |        |        |        |         |
|---------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                   | Deployment Size |        |        |        |         |
| 2996313                                           | 14945           |        |        |        |         |
| Function Name                                     | min             | avg    | median | max    | # calls |
| bindPort                                          | 49944           | 49944  | 49944  | 49944  | 4       |
| createClient                                      | 302130          | 302130 | 302130 | 302130 | 4       |
| recvPacket                                        | 280969          | 280969 | 280969 | 280969 | 1       |
| registerClient                                    | 29833           | 29833  | 29833  | 29833  | 4       |
| sendPacket                                        | 219600          | 219600 | 219600 | 219600 | 1       |
| updateClient                                      | 245033          | 245033 | 245033 | 245033 | 1       |

### After

https://github.com/hyperledger-labs/yui-ibc-solidity/actions/runs/3563307889/jobs/5985944182#step:7:186

| tests/foundry/src/TestableIBCHandler.t.sol:TestableIBCHandler contract |                 |        |        |        |         |
|------------------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                                        | Deployment Size |        |        |        |         |
| 5534183                                                                | 28063           |        |        |        |         |
| Function Name                                                          | min             | avg    | median | max    | # calls |
| bindPort                                                               | 46515           | 46515  | 46515  | 46515  | 5       |
| channelCapabilityPath                                                  | 2188            | 2188   | 2188   | 2188   | 10      |
| claimCapabilityDirectly                                                | 24514           | 35005  | 35005  | 45496  | 10      |
| connectionOpenInit                                                     | 286684          | 286684 | 286684 | 286684 | 1       |
| createClient                                                           | 195989          | 201629 | 202758 | 202758 | 6       |
| recvPacket                                                             | 145496          | 145496 | 145496 | 145496 | 1       |
| registerClient                                                         | 25221           | 25221  | 25221  | 25221  | 5       |
| sendPacket                                                             | 97100           | 97100  | 97100  | 97100  | 1       |
| setChannel                                                             | 178780          | 178780 | 178780 | 178780 | 5       |
| setConnection                                                          | 288162          | 288162 | 288162 | 288162 | 5       |
| setNextChannelSequence                                                 | 662             | 662    | 662    | 662    | 5       |
| setNextConnectionSequence                                              | 681             | 681    | 681    | 681    | 5       |
| setNextSequenceAck                                                     | 23400           | 23400  | 23400  | 23400  | 5       |
| setNextSequenceRecv                                                    | 48821           | 48821  | 48821  | 48821  | 5       |
| setNextSequenceSend                                                    | 23376           | 23376  | 23376  | 23376  | 5       |
| updateClient                                                           | 116088          | 116088 | 116088 | 116088 | 1       |


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 22:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    CI:  Gas report output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 02:45:53 +0000 UTC
    </div>
</div>

