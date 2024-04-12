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
                PR <a href="https://github.com/hyperledger/solang/pull/1639" class=".btn">#1639</a>
            </td>
            <td>
                <b>
                    Release 0.3.4 Athens
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
        Created At 2024-04-12 11:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1638" class=".btn">#1638</a>
            </td>
            <td>
                <b>
                    Fix CI: SPDX headers in shell scripts
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
        Created At 2024-04-11 12:22:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1637" class=".btn">#1637</a>
            </td>
            <td>
                <b>
                    Polkadot: Bugfix codegen for empty events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an oversight from #1632: The ABI encoder panics when trying to encoding no arguments. Previously, events always contained at least a single byte of data (empty events would have the discriminant/index of the event enum). However now, the data field for empty events is actually empty. So in codegen we check if we have to encode data first and pass a pointer to an empty buffer if not.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 12:16:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1636" class=".btn">#1636</a>
            </td>
            <td>
                <b>
                    Add salaheldin to MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A proud moment.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 14:46:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1635" class=".btn">#1635</a>
            </td>
            <td>
                <b>
                    Polkadot: Update rust cross contract call example to ink! v5.0
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
        Created At 2024-04-08 13:01:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1634" class=".btn">#1634</a>
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
                - Upgrade dependencies
- Add SPDX header to TS sources as the GH action now requires it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 10:44:20 +0000 UTC
    </div>
</div>

