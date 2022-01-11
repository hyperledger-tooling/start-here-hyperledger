---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Committed by Hanan on Dec 28 2021 11:40 (2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Hanan Singer <hanan@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 14:25:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    Limit access to cluster config to admins
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
        Created At 2022-01-06 14:57:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Rename httputils package to utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename `httputils` package to `utils`
Rename file `utils.go` to `http.go`

No functional change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 12:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    Refactor SharedConfiguration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change the **SharedConfiguration** field Nodes
from

- Nodes []NodeConf

to

- Nodes []*NodeConf

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 11:05:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Prevent proposals inflight config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                We are preventing all proposals when a config is in flight, by using the same mechanism that prevents proposals when there are too many regular blocks in flight. This is not strictly necessary (what we strictly need is to prevent proposing a config when another config is in-flight), but is easier to implement. The implications on steady state performance are negligible, as config transactions are rare.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 13:20:05 +0000 UTC
    </div>
</div>

