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
                PR <a href="https://github.com/hyperledger/caliper/pull/1315" class=".btn">#1315</a>
            </td>
            <td>
                <b>
                    address worker cleanup when an error occurs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This improves the cleanup of a worker if an error occurs which would
cause the worker to terminate the round.

closes #1312

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 17:44:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1314" class=".btn">#1314</a>
            </td>
            <td>
                <b>
                    Change monitor intervals from milliseconds to seconds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For the fabric tests the monitor intervals were set to single
millisecond values such as 3, 4, 5. This adds a massive overhead to the
running of the integration tests and isn't needed, so changing them to
be seconds instead.

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 10:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1311" class=".btn">#1311</a>
            </td>
            <td>
                <b>
                    Fixed colors dependency to 1.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1308 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 08:46:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1310" class=".btn">#1310</a>
            </td>
            <td>
                <b>
                    Peer Gateway: Integration tests for the new Peer Gateway connnector ( + update docker compose to use 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add integration test for peer gateway connector
- updated docker compose to use fabric 2.4


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 10:45:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1306" class=".btn">#1306</a>
            </td>
            <td>
                <b>
                    Fixes for default.yaml in packages/caliper-core/lib/common/config/ and updates for the fabric Channel operations for the v1 fabric connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                edited defaul.yaml (updated comments and deleted sllep after option for fabric) + updated the fabric Chaincode operations for the v1 fabric connector
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 10:27:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1304" class=".btn">#1304</a>
            </td>
            <td>
                <b>
                    [Doc] remove term Observer from monitors page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also renamed the file

closes #1213

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 09:35:59 +0000 UTC
    </div>
</div>

