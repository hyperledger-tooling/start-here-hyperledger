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
                PR <a href="https://github.com/hyperledger/firefly/pull/1050" class=".btn">#1050</a>
            </td>
            <td>
                <b>
                    Handle FFTM new style acks with batchNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-transaction-manager/pull/36

> Leaving in draft mode until we have an FFTM+EVMConnect release, to include in the manifest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 02:57:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1048" class=".btn">#1048</a>
            </td>
            <td>
                <b>
                    Consistently fall back to ff_system for legacy identity lookups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts #1035 
Fixes #1032
Fixes #1045 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 18:07:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1047" class=".btn">#1047</a>
            </td>
            <td>
                <b>
                    Properly enforce uniqueness of BatchPin blockchain events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Because listener_id is NULL for these events, we need separate indexes for when it is NULL and not NULL.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 14:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1046" class=".btn">#1046</a>
            </td>
            <td>
                <b>
                    update public chain docs
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
        Created At 2022-09-07 14:07:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1044" class=".btn">#1044</a>
            </td>
            <td>
                <b>
                    adding test cases for cache init errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix coverage decrement introduced by central cache PR.

Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 21:28:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1043" class=".btn">#1043</a>
            </td>
            <td>
                <b>
                    Fix sequence query in auditevents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need to keep requesting new chunks of events even if the previous chunk
contained no matches.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 19:45:42 +0000 UTC
    </div>
</div>

