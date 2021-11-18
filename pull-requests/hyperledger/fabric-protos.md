---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Remove EndorseResponse.result field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This duplicates information already present in the EndorseResponse.prepared_transaction field and, if the content is large, can cause failures due to gRPC message size limits. The Fabric Gateway client and server implementations no longer use this field.

Contributes to hyperledger/fabric-gateway#316
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 18:30:00 +0000 UTC
    </div>
</div>

