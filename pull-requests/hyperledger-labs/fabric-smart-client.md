---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Notifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces the notifiers that allow us to listen for any row insert/update/delete in the DB.
The new functionality is in the two files notifier.go. The rest is moving files to allow for deduplication of logic between the Postgres and the sqlite implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 08:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    fix bug web service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This PR does the following: It fixes the bug reported in #568 .
The integration tests by default have the web server disabled. Only the `pingpong` test uses it.
The web server can be enabled by setting `WebEnabled` to `true` on the fsc topology.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 15:36:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    remove support for finality listener for all txs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 14:36:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    updated vault's DiscardTx function behaviour
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 04:39:42 +0000 UTC
    </div>
</div>

