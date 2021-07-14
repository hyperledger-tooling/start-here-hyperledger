---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Fix catchup for restored subscriptions, and add log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #130 missed the configuration of block catchup for restored subscriptions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 02:59:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Catchup mode: read pages of blocks, when we're a long way behind
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The ethereum log streaming interface, doesn't have any ability to limit/paginate calls to `eth_getFilterLogs` / `eth_getFilterChanges`, per https://github.com/ethereum/go-ethereum/issues/17487

This is problematic on chains with large numbers of blocks & transactions, when trying to reply events from a long way behind the current block.

Currently the code performs an `eth_getFilterLogs` from the latest checkpoint -> `latest`, which could be millions of blocks in the case of a new node joining the network.

So this PR proposes adding an automatically enabled "catchup" mode, in the case that a stream is restarting and finds itself a long way behind in the latest block on the node it's on. 
In this mode we repeat the following to read pages of blocks:
1. `eth_blockNumber`
2. `eth_getLogs` - checkpoint (or last page end), to end of page
... that happens until we find we're get within that window of the head again.

Default is to enable it when we are restarting `250` blocks or more behind the head, and read `250` blocks at a time.

There are some unrelated lint fixes in this PR too that were picked up by my compiler.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 17:07:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    Add git action for build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 14:38:19 +0000 UTC
    </div>
</div>

