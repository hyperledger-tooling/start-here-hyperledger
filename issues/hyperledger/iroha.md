---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1315" class=".btn">1315</a>
            </td>
            <td>
                <b>
                    Peer responded with QueryResult instead of VersionedQueryResult
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                When client sends request to endpoint /query, it expects as result `VersionedQueryResult`, but the peer returns `QueryResult`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 06:33:19 +0000 UTC
    </div>
</div>

