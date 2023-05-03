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
                PR <a href="https://github.com/hyperledger/firefly/pull/1295" class=".btn">#1295</a>
            </td>
            <td>
                <b>
                    Handle duplicate pool locators properly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since there is a unique index on pool locators, it must be checked during token pool upsert.

This behavior will be changing again in #1261, but this is a more immediate fix without pulling in all of that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 21:45:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1293" class=".btn">#1293</a>
            </td>
            <td>
                <b>
                    Remove duplicates prior to adding unique index on contract API ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also ensure ID is always unset when creating a new API.

Follow-up to #1292, #1275
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 19:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1292" class=".btn">#1292</a>
            </td>
            <td>
                <b>
                    Add proper WHERE clause to contract API updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that insert and update are executed correctly, and add a unique index on ID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 15:08:23 +0000 UTC
    </div>
</div>

