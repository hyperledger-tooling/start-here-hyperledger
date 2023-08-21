---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.7.1
                </span>
            </td>
            <td>
                ## 23.7.1

This is a recommended update for Proof of Stake users on public networks. This update removes some compatibility with GoQuorum permissioning, so please read these notes carefully if you are using these features. 

This release is focused primarily on performance and stability improvements, updating dependencies, and extending functionality of the EVM tool and the RPC trace modules. It also fixes some bugs with the new [layered transaction pool](https://github.com/hyperledger/besu/pull/5290), peering, and memory usage. 

### Breaking Changes
- Removed deprecated GoQuorum permissioning interop [#5607](https://github.com/hyperledger/besu/pull/5607)
- Removed support for version 0 of the database as it is no longer used by any active node. [#5698](https://github.com/hyperledger/besu/pull/5698)

### Additions and Improvements
- `evmtool` launcher binaries now ship as part of the standard distribution. [#5701](https://github.com/hyperledger/besu/pull/5701) 
- EvmTool now executes the `execution-spec-tests` via the `t8n` and `b11r`. See the [README](ethereum/evmtool/README.md) in EvmTool for more instructions.
- Improve lifecycle management of the transaction pool [#5634](https://github.com/hyperledger/besu/pull/5634)
- Add extension points in AbstractCreateOperation for EVM libraries to react to contract creations [#5656](https://github.com/hyperledger/besu/pull/5656)
- Update to Tuweni 2.4.2. [#5684](https://github.com/hyperledger/besu/pull/5684)
- Decouple data field from Enum JsonRpcError by creating new enum holder RpcErrorType[#5629](https://github.com/hyperledger/besu/pull/5629)
- Update to bouncycastle 1.75 [#5675](https://github.com/hyperledger/besu/pull/5675) 
- Extend OperationTracer with new methods [#5662](https://github.com/hyperledger/besu/pull/5662)
- Eip 6780 selfdestruct [#5430](https://github.com/hyperledger/besu/pull/5430)
- Add new debug_getRawTransaction to the DEBUG engine [#5635](https://github.com/hyperledger/besu/pull/5635)

### Bug Fixes
- Use the node's configuration to determine if DNS enode URLs are allowed in calls to `admin_addPeer` and `admin_removePeer` [#5584](https://github.com/hyperledger/besu/pull/5584)
- Align the implementation of Eth/68 `NewPooledTransactionHashes` to other clients, using unsigned int for encoding size. [#5640](https://github.com/hyperledger/besu/pull/5640)
- Failure at startup when enabling layered txpool before initial sync done [#5636](https://github.com/hyperledger/besu/issues/5636)
- Remove miner-related option warnings if the change isn't using Ethash consensus algorithm [#5669](https://github.com/hyperledger/besu/pull/5669)
- Fix for pending transactions reference leak [#5693](https://github.com/hyperledger/besu/pull/5693) 
- Address a performance regression observed in import testing [#5734](https://github.com/hyperledger/besu/pull/5734)
- Update native libraries that have JPMS friendly module names [#5749](https://github.com/hyperledger/besu/pull/5749)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.7.1/besu-23.7.1.tar.gz / sha256: 85dce66c2dbd21b4e5d3310770434dd373018a046b78d5037f6d4955256793cd
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.7.1/besu-23.7.1.zip / sha256: dfac11b2d6d9e8076ab2f86324d48d563badf76fd2a4aadc4469a97aef374ef5

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.7.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-21 14:12:16 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.7.0
                </span>
            </td>
            <td>
                ## 23.7.0 

- Was not released (failed burn-in test)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.7.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-07-25 00:11:10 +0000 UTC
    </span>
</div>

