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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Fix CI tests 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CI tests on forks fail, make various parts conditional.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 08:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Implement signatureVerify() correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The actual implementation was different than originally planned.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 14:32:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Ensure output from compiler is deterministic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The codegen for solana dispatch looked for the constructor for a
contract, without checking it was the non-base constructor. So,
the constructor for one of the base contracts may be selected instead.

Since functions are stored in HashMaps at various points, this
as not determinstic.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 11:33:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    Attach libraries to contracts and interfaces with using
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
        Created At 2021-09-06 09:54:28 +0000 UTC
    </div>
</div>

