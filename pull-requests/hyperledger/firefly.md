---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/971" class=".btn">#971</a>
            </td>
            <td>
                <b>
                    Fix group race condition, optimize transaction cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Insert local group only after inserting groupinit message.
This ensures no other threads pick up on the group before the
message is sequenced.

Update transaction cache after initial insert.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 17:53:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/970" class=".btn">#970</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/969" class=".btn">#969</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/967" class=".btn">#967</a>
            </td>
            <td>
                <b>
                    Performance improvements for batch lookups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure batch ID queries match the current indexes (to avoid sequential scan), and improve the caching in aggregator when processing a group of pins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 04:15:52 +0000 UTC
    </div>
</div>

