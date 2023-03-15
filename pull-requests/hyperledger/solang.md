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
                PR <a href="https://github.com/hyperledger/solang/pull/1222" class=".btn">#1222</a>
            </td>
            <td>
                <b>
                    fix compilation failure with -g flag in substrate integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes compilation error when inserting the `-g` flag in Substrate integration tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 19:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1221" class=".btn">#1221</a>
            </td>
            <td>
                <b>
                    Implement rational eval of compare, or, and, and conditional operator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are all accepted by solc so solang should do the same.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 16:45:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1220" class=".btn">#1220</a>
            </td>
            <td>
                <b>
                    Remove non-idiomatic use of LinkedList
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See the note here:

https://doc.rust-lang.org/std/collections/struct.LinkedList.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 09:23:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1218" class=".btn">#1218</a>
            </td>
            <td>
                <b>
                    improve resolve pragma
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
        Created At 2023-03-10 08:20:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1217" class=".btn">#1217</a>
            </td>
            <td>
                <b>
                    Collect the accounts a contract needs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR, we collect all accounts we can from a Solidity contract and insert them into the accounts vector for an instruction, so developers do not have to input them manually.

Closes #1191.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 18:38:41 +0000 UTC
    </div>
</div>

