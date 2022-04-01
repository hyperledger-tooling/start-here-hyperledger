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
                PR <a href="https://github.com/hyperledger/caliper/pull/1295" class=".btn">#1295</a>
            </td>
            <td>
                <b>
                    address fabric tutorial not working with newer docker-compose
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                newer docker-compose versions don't work with the specific git checkout
in the tutorial.

I've fixed the bug in fabric-samples but as it hasn't been tagged as a
release yet we need to use another specific git commit but updates to
test-network now means it works with newer docker-compose versions.

closes #1291

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 13:14:49 +0000 UTC
    </div>
</div>

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

