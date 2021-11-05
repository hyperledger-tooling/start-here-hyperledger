---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Use WriteByte instead of WriteRune when possible
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
        Created At 2021-11-04 17:42:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    Additional cleanup to support tokens UI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of #218
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 18:55:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Move definitions of datatypes and tokens to their proper namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Messages that use the `ff_system` namespace:

- Org registration
- Node registration
- Namespace definition

Messages that use whatever namespace is specified in the API request path:

- Everything else
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 19:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/311" class=".btn">#311</a>
            </td>
            <td>
                <b>
                    Split the notions of "token balances" and "token accounts"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of #218.

The thing that has up to now been known as an "account" is really just a "balance" - ie given an identity, a pool, and optionally a token index, it tracks a number stating how many of that token are owned. All of this existing functionality has therefore been renamed from "token accounts" to "token balances".

This PR also introduces a _new_ concept of what is a "token account" - currently just a filtered, distinct list of all the identities tracked in "token balances". Eventually this may evolve to include more aggregate details on each identity's holdings, but this is the simplest start without adding another table.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 19:02:29 +0000 UTC
    </div>
</div>

