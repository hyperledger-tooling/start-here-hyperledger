---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1292" class=".btn">#1292</a>
            </td>
            <td>
                <b>
                    fix RecordRate rate controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses the record rate controller as it doesn't work and causes a
node stack overflow

closes #1131

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:59:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    remove latency values if no successful txns in final report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1065

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 11:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Caliper terminates if prometheus is not available
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is due to the error event not being correctly captured when a
request is made to prometheus

Also added some extra code to output a warning and stop trying to do any
more queries for the round.

It won't stop it for all rounds but checks on every round.

closes #1267

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 14:30:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    change web3js-eea to web3js-quorum
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
        Created At 2022-03-24 09:17:25 +0000 UTC
    </div>
</div>

