---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    Fix Solang Logo link for external consumption
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
        Created At 2023-02-16 15:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    docker buildx requires --provenance=false for now
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an issue in docker buildx 0.10:

https://github.com/docker/buildx/issues/1519
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 11:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1181" class=".btn">#1181</a>
            </td>
            <td>
                <b>
                    Split `method_call_pos_args` function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR splits the function `method_call_pos_args` into multiple small functions for better readability and maintenance. I had this idea when thinking about the new API we are going to implement for mappings on Solidity.


I am open to other ideas on how to manage the multiple functions, if you don't like the approach I have taken.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 20:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1179" class=".btn">#1179</a>
            </td>
            <td>
                <b>
                    Use scale encoder in emit for release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed: #1128 introduced a refactor version of the scale encoder in codegen. However, the emit version of the SCALE encoder could not be phased out yet; the dispatcher is written in emit as well, so we need to refactor the decoder (WIP, currently blocked by #1168 ) and then dispatcher into codegen (WIP after the decoder) first, too.

This resulted in the compiler using the new version of the encoder but only fo `abi.encode` and not in the dispatcher.

We don't want to release a version with a half-baked SCALE encoder/decoder implementation. Minor issue is that it "feels wrong" to use different implementations for the same thing, depending on the circumstance. Major issue is that many tests go through the encoding logic in the dispatcher, but the dispatcher still uses the emit version. It is fine for the `main` branch but a no-go to ship that in a release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 18:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1178" class=".btn">#1178</a>
            </td>
            <td>
                <b>
                    Fix wrong selector type in emit SCALE encoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was oversighted in #1128

Signed-off-by: Cyrill Leutwiler <cyrill@parity.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 18:09:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Expand list of code owners, take #2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm hoping I will get it right this time, no way of knowing with github being closed source.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 15:39:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    Expand list of solang code owners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When creating a pull request, the users in this files are used to populate the reviewers. If it lists @hyperledger/solang-committers then we can't see who those users are and as soon as one of the members of @hyperledger/solang-committers leaves a review, then the pull request is marked as approved while we really want *all* the maintainers to approve.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 15:21:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    Account for leading zeros in hex number literals size width
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Matching the behavior of `solc`.

Signed-off-by: xermicus <cyrill@parity.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 23:28:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1172" class=".btn">#1172</a>
            </td>
            <td>
                <b>
                    Update CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 19:32:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1170" class=".btn">#1170</a>
            </td>
            <td>
                <b>
                    Bump solang-parser for crate publish
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
        Created At 2023-02-10 08:52:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    Fix CSE bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @xermicus found a bug in common subexpression elimination while working on the SCALE decoder. This PR fixes the bug, but the fix is only palliative for it might not cover all possible cases.

The problem would be best solved implementing a correct version of partial redundancy elimination, which leverages the available expressions analysis (already available) and an anticipated expression analysis not only to detect common subexpressions, but to know where exactly to evaluate them. This solution, nevertheless, is too time consuming to code and will be easier to implement when we have a new IR with SSA.

More information about partial redundancy elimination can be found in the Chapter 9.5 of the book `Compilers: Principles, Techniques & tools`, second edition, from Monica S. Lam.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 21:07:25 +0000 UTC
    </div>
</div>

