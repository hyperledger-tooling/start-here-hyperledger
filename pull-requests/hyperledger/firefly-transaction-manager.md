---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Restructure TX input for consistency with ethconnect and idempotence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ... also removes the last vestige of a dependency on FF Core 🪶 

Updates the reply processing to emit all updates - note that FF core will need to process a new `header.type` of `TransactionUpdate` (as well as `TransactionFailure` and `TransactionSuccess`).

I've merged #15 into this branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 22:11:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add support for deploying contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 18:36:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Ensure consistent block state during cycle, to prevent out-of-order delivery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I realized that there was a gap in the ordering logic, in the case that there is a number of pending event waiting confirmation and we go through and do `walkChain()`.

Specifically if new blocks become available during that cycle, we might get a "hit" for a block for a later event, which was a "miss" for that block for an earlier event - simply because the block has just been mined.

So I've added a `blockState` that is created each time we do a cycle, that ensures we don't change answers on ourselves for the duration of that cycle.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 13:07:41 +0000 UTC
    </div>
</div>

