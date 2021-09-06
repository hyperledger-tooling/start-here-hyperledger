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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    Get the function selector via contract.function.selector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                contract does not have to be a base class, it can be an interface as
well.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 16:40:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    Use new solana mechanism for return data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requires:
 - https://github.com/solana-labs/solana/pull/19548
 - https://github.com/solana-labs/solana/pull/19318

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 17:15:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    Solang language server should announce version
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
        Created At 2021-08-31 17:03:05 +0000 UTC
    </div>
</div>

