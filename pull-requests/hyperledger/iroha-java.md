---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Iroha-121: implement queries in QueryBuilder
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
        Created At 2021-10-04 14:24:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Iroha-121: implement queries in QueryBuilder
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
        Created At 2021-10-04 08:11:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Altered queries builder to avoid passing result extractor by sdk client, now it can be defined based on query type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [Task](https://app.zenhub.com/workspaces/iroha-v2-60ddb820813b9100181fc060/issues/hyperledger/iroha-java/115)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-03 10:37:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    Fixed incorrect closing of websocket connection if peer responds with `Validating` event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peer can responds with 3 events signaling tx status: Committed, Rejected and Validating. Committed and Rejected are final statuses, so after receiving them client need to close socket connection, but after Validating status nothing need to do.

Signed-off-by: rkharisov <rinat@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 10:48:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    Restrict execution race during subscribing/sending transaction#147
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [Task](https://app.zenhub.com/workspaces/iroha-v2-60ddb820813b9100181fc060/issues/hyperledger/iroha-java/147)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 06:39:03 +0000 UTC
    </div>
</div>

