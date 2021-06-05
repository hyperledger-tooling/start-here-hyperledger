---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2381" class=".btn">#2381</a>
            </td>
            <td>
                <b>
                    Replace try!() with ?
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                try!() is very old and this avoids a compiler warning.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 21:13:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2380" class=".btn">#2380</a>
            </td>
            <td>
                <b>
                    Fix panic w/non-static String compiler warning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The solution here is to reduce it a simple string, which isn't ideal
since it will no longer print the missing transaciton type. However,
this code is unrefined anyway since it panics at all, and the solution
of rewriting it with proper error handling can happen in a future change
aimed at removing the panics.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 21:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2379" class=".btn">#2379</a>
            </td>
            <td>
                <b>
                    Update protobuf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updated the usage of protobuf so it no longer causes compiler warnings and specify the minimum version of protobuf to be 2.23.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 20:04:30 +0000 UTC
    </div>
</div>

