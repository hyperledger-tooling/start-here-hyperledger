---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.2
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Execution layer (The Merge):
  - Execution specific RPC endpoint [#3378](https://github.com/hyperledger/besu/issues/3378)
  - Adds JWT authentication to Engine APIs
  - Supports kiln V2.1 spec
- Tracing APIs 
  - new API methods: trace_rawTransaction, trace_get, trace_callMany
  - added revertReason to trace APIs including: trace_transaction, trace_get, trace_call, trace_callMany, and trace_rawTransaction
- Allow mining beneficiary to transition at specific blocks for ibft2 and qbft consensus mechanisms.  [#3115](https://github.com/hyperledger/besu/issues/3115)
- Return richer information from the PrecompiledContract interface. [\#3546](https://github.com/hyperledger/besu/pull/3546)

### Bug Fixes
- Reject locally-sourced transactions below the minimum gas price when not mining. [#3397](https://github.com/hyperledger/besu/pull/3397)
- Fixed bug with contract address supplied to `debug_accountAt` [#3518](https://github.com/hyperledger/besu/pull/3518)

## Download Links
 - https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.2/besu-22.1.2.zip /  SHA256 
 1b26e3f8982c3a9dbabc72171f83f1cfe89eef84ead45b184ee9101f411c1251
 - https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.2/besu-22.1.2.tar.gz / SHA256 
1eca9abddf351eaaf4e6eaa1b9536b8b4fd7d30a81d39f9d44ffeb198627ee7a
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.1.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-16 04:53:57 +0000 UTC
    </span>
</div>

