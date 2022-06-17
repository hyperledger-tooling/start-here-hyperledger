---
layout: default
title: aries-framework-go-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go-ext
---

# aries-framework-go-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    feat: MongoDB BulkWrite, multiple index creation, and doc helper func
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Added a BulkWrite method that allows a caller to directly call the MongoDB BulkWrite function with their own custom models
* Updated the CreateCustomIndex function to accept multiple index models at once (and updated the name to CreateCustomIndexes)
* Exposed the PrepareDataForBSONStorage helper function

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:22:09 +0000 UTC
    </div>
</div>

