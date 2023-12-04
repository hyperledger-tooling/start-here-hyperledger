---
layout: default
title: cckit
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/cckit
---

# cckit <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/cckit){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cckit/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    fix delete private key from mockStub
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When deleting private data (with the DelPrivateData function), it returns an error if the key to be deleted is not found in the collection.
But if you perform DelPrivateData of a non-existent key on a real stack, no error is returned
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 10:43:24 +0000 UTC
    </div>
</div>

