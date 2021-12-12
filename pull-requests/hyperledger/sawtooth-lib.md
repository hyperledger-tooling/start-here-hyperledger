---
layout: default
title: sawtooth-lib
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-lib
---

# sawtooth-lib <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-lib){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.7.2
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
        Created At 2021-12-10 22:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-7: Move ConnectionPool to store::pool module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Back-port of #125 to 0-7
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 21:28:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/125" class=".btn">#125</a>
            </td>
            <td>
                <b>
                    Move ConnectionPool to store::pool module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change moves the ConnectionPool enum to a store::pool module. As such, it updates its generics to include the error type. This improves is use with any future stores.

It is guarded by a new feature, "store", which is grandfathered-in as stable and depended on by either "postgres" and "sqlite" features.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 18:11:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Backport 0-7: Implemement exclusive write support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Back-port of #123 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 16:17:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Implement exclusive write support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements exclusive write support in `DieselReceiptStore`.  It extends the existing API such that it is not a breaking change and may be optionally applied.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 21:54:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-7: Fix rust 1.57 lint
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
        Created At 2021-12-07 15:34:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Fix rust 1.57 lint
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
        Created At 2021-12-06 01:06:36 +0000 UTC
    </div>
</div>

