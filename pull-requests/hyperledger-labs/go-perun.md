---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    Fix tx nonce mismatch error: approach 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix is attempted using approach 1 suggested in #62. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 13:14:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    :bug: [client] Defer release version 1 cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #128 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 07:39:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    Draft channel redesign
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR explores possibilities to streamline channel operation. Usage of the channel became more complicated since sub-channels and app channels were introduced.

One complication was caused by the fact that the register call was exposed and needed to be called manually before enforcing on-chain state progression.

This PR proposes to simplify the process of on-chain progression:

- Rename Channel.Progress to Channel.ForceUpdate: This conveys more clearly that the functionality is related to "Channel.Update".
- Implicitly register state on `ForceUpdate`: This simplifies the usage because the user does need to take care of manually registering before calling `ForceUpdate`.

The PR also includes parameter consolidation for `Adjudicator.Register` and `Withdraw`, similar to `Adjudicator.Progress`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 18:45:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    :bug: [client] Fix update error propagation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a bug where `updateGeneric` discarded a `PeerRejectedError` and replaced it with a different error.

Signed-off-by: Matthias Geihs <matthias@perun.network>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 18:26:26 +0000 UTC
    </div>
</div>

