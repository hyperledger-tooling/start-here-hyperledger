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
                PR <a href="https://github.com/hyperledger/firefly/pull/1218" class=".btn">#1218</a>
            </td>
            <td>
                <b>
                    Correction of typos
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
        Created At 2023-03-13 18:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1216" class=".btn">#1216</a>
            </td>
            <td>
                <b>
                    Ensure cached transaction gets updated with new blockchain IDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are multiple paths that record the blockchainID for a transaction. Along this path, we were updating the column in the database but not the cache - resulting in this field being intermittently out of sync.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 05:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1215" class=".btn">#1215</a>
            </td>
            <td>
                <b>
                    Fix logging of blockchain event inserts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is causing blockchain event inserts to incorrectly be logged as message inserts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 19:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1214" class=".btn">#1214</a>
            </td>
            <td>
                <b>
                    [resolver] Unit Test for URL Encoding Key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Confirms we can use Go template's builtin `urlquery` to URL encode key IDs which may require it, such as URIs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 03:35:07 +0000 UTC
    </div>
</div>

