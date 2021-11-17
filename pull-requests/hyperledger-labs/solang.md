---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    Vector to slice pass creates invalid phi nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the vector to slice pass updates once incoming value for a phi node,
but not another we end up with a phi node that is invalid; one entry
is a vector and the other a slice.

This fix does the following.

1. First collect all the set instructions we are going to update.
2. For all phi nodes, check if there are any reaching definitions we
   are not updating.
3. If any reaching definition for the phi node is not updated, then do
   not update any of them.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 17:52:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    Do not link against libffi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                libffi is not needed and we shouldn't depend on it.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 14:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    Divide optimizer into sections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, the 'Unused Variable Elimination' and 'Common Subexpression Eimination' are sub sections under 'Vector to Slice Pass' in [Solang docs](https://solang.readthedocs.io/en/latest/optimizer.html). They should be a new section under Optimization Passes, instead of a subsection. This PR fix this issue.

![Screen Shot 2021-11-14 at 09 53 10](https://user-images.githubusercontent.com/38472950/141681928-b414c934-61bc-4434-a78c-402b60933ba0.png)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-14 12:55:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/564" class=".btn">#564</a>
            </td>
            <td>
                <b>
                    Minor fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #561 and other issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 23:03:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/563" class=".btn">#563</a>
            </td>
            <td>
                <b>
                    Disable eliminating unused variables when optimization level is None (-O none)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi,

I created this new PR to fix all problems mentioned in the previous PR https://github.com/hyperledger-labs/solang/pull/560

I also fixed the problems mentioned by @LucasSte in https://github.com/hyperledger-labs/solang/pull/560#issuecomment-967294935

Can you help to review it?

Thanks!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 04:48:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/562" class=".btn">#562</a>
            </td>
            <td>
                <b>
                    Minor fixes
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
        Created At 2021-11-12 15:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Fix recursive structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Iwan Waitusenok <sleepplease@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 12:56:31 +0000 UTC
    </div>
</div>

