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
                PR <a href="https://github.com/hyperledger/solang/pull/1273" class=".btn">#1273</a>
            </td>
            <td>
                <b>
                    modifiers are allowed in libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solang did not permit this, but solc does.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-15 12:25:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1272" class=".btn">#1272</a>
            </td>
            <td>
                <b>
                    Encode addreses in base58 for print
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses on Solana and Substrate are often shown in base58 encoding, so we should print them like so.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 21:27:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    Enable the `accounts` call argument for constructors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling the constructor of a contract, we should be able to specify the account metas for the transaction. We need this feature, so we can automatically pass the accounts for the contract construction.

This PR is the second task in https://github.com/hyperledger/solang/issues/1251
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 19:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1270" class=".btn">#1270</a>
            </td>
            <td>
                <b>
                    Use rationals rather than float for calculating flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Flow calculation involves division followed by addition, e.g. 10/3 + 10/3 + 10/3 is not exactly 10 when using floats. So, use rationals instead.

I *think* `Rational<usize>` will suffice but I chicked out and used BigRational instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 10:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1269" class=".btn">#1269</a>
            </td>
            <td>
                <b>
                    Rename more unchecked to overflowing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recently unchecked was renamed overflowing in CFG. A few renames were missed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 15:04:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1268" class=".btn">#1268</a>
            </td>
            <td>
                <b>
                    Disallow dynamic arrays for account metas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Account metas do not support dynamic arrays and we do not inform that to the user.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 21:57:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Test large github runners
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
        Created At 2023-04-12 15:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    Remove redundancies in `is_next_reachable()`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After merging #1260 , I noticed the checks in my code were redundant.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 15:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1260" class=".btn">#1260</a>
            </td>
            <td>
                <b>
                    Ensure that the last instruction of a block is reachable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR supersedes #1257.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 17:28:12 +0000 UTC
    </div>
</div>

