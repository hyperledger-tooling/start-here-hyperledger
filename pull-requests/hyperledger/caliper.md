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

