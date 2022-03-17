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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/701" class=".btn">#701</a>
            </td>
            <td>
                <b>
                    Bump dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 17:31:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    feat(parser): support revert statement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #696

Followed these instructions https://github.com/hyperledger-labs/solang/issues/696#issuecomment-1066666159

revert statement remains `unimplemented!` in `sema`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 21:03:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/695" class=".btn">#695</a>
            </td>
            <td>
                <b>
                    Fix issue with dead storage eliminating the wrong storage load
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the same variable loaded from storage twice in a loop, then first
may be eliminated rather than the second. The issue is that the reaching
definition for the second load reaches the first; the possible
undefined value from the entry point of the function is not reaching.

To fix this, for block 0, populate the variable table all undefined
values.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 11:53:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/694" class=".btn">#694</a>
            </td>
            <td>
                <b>
                    Include trait for loc() functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds traits for `fn loc(&self) -> Loc` and `fn loc(&self) -> Option<Loc>`, so that we can maintain more uniformity throughout the code, while creating the loc() functions for many structs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 12:56:59 +0000 UTC
    </div>
</div>

