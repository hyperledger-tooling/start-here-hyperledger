---
layout: default
title: sawtooth-sabre
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sabre
---

# sawtooth-sabre <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sabre){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/189" class=".btn">#189</a>
            </td>
            <td>
                <b>
                    Remove docs dependency from publish artifacts step
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 00:16:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    Remove docs build from merge GHA workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was inadvertently omitted in PR#119.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 14:12:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/187" class=".btn">#187</a>
            </td>
            <td>
                <b>
                    Replace hyper with reqwest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaces an old version of hyper with the latest version of reqwest. Also adds tests to help ensure the API of affected functions hasn't changed.

Previously, the affected functions used futures but were still blocking; this changes those requests to be explicitly blocking and eliminates the runtime underneath.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 22:35:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    Fix linting from 1.62
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses clippy lints introduced with Rust 1.62.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 22:29:25 +0000 UTC
    </div>
</div>

