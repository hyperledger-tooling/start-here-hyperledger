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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Remove "stores" and associated implementations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes all of the "stores" feature.  This experimental feature was developed using an earlier pattern that has been superseded by the pattern seen in `sawtooth::receipt::store` (under the `"transaction-receipt-feature"`).  It removes all implementations of these stores.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 13:55:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Remove "receipt-store" feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This has been replaced with the stabilized "transaction-receipt-store" feature.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 20:24:46 +0000 UTC
    </div>
</div>

