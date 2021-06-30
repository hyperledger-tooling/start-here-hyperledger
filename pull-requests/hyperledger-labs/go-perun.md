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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Add functions to register new assets in ethereum funder implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - As these methods provide convenience for the user (to register assets after funder is initialized) and are not required by the framework itself for the process of funding, they are not added to the `Funder` interface.

- Use the `RegisterAsset` method in place of `WithDepositor`, as the newly added method provides the same functionality without making a copy of the funder.

- Also, fixed a bug in `funder_test.go`. See the last before commit for details. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 15:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Core82 open and close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split some more commits from #83 .

In particular, this PR includes the following:

- Open virtual channels
- Close virtual channels
- Test virtual channels happy case
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 14:16:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    Fix testHashState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test the HashState function instead of CalcID, which is already being tested in testCalcID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 11:22:41 +0000 UTC
    </div>
</div>

