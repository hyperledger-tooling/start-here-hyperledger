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
                PR <a href="https://github.com/hyperledger/solang/pull/1127" class=".btn">#1127</a>
            </td>
            <td>
                <b>
                    Update Rust version from workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The test workflows are failing because clap does not support Rust 1.63 anymore, so I updated it to 1.64.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 18:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1126" class=".btn">#1126</a>
            </td>
            <td>
                <b>
                    Differentiate between caller contract and the constructor contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When invoking `call_constructor` we were passing the same contract number for both the caller contract and the contract being called.

This fixes https://github.com/xermicus/fuzzy-sol/issues/118
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 17:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1125" class=".btn">#1125</a>
            </td>
            <td>
                <b>
                    Use anchor npm library rather than @solana/solidity
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
        Created At 2023-01-11 15:31:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1124" class=".btn">#1124</a>
            </td>
            <td>
                <b>
                    Use match statements for comparison chains
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lucas Steuernagel <lucas.tnagel@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 17:13:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1123" class=".btn">#1123</a>
            </td>
            <td>
                <b>
                    Fix storage deref bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Alternate implementation to #1112 

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-07 10:46:10 +0000 UTC
    </div>
</div>

