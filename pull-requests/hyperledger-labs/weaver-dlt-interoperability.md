---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    Provision for dynamic arguments in the query for data-sharing push via events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The data-sharing query specified at the time of even-subscription currently is static nature. However, under certain scenarions, it may be required it to be constructed dynamically (e.g., in the view address `"view_address": "localhost:9083/network2/mychannel:simplestate:Read:a"` the key `a` to be read might be available only at run time). The changes in this PR replace such dynamic query arguments (e.g., in the view address `"view_address": "localhost:9083/network2/mychannel:simplestate:Read:?"` the `?` will be replaced with the corresponding argument values dynamically by the interop-CC before querying the app-CC)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 02:35:28 +0000 UTC
    </div>
</div>

