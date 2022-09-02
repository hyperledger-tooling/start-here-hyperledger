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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    Added automated publishing of go modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added workflow to publish go modules automatically. (Don't update module and its dependency in same PR, else if want to do both, make sure `go.mod` and `go.sum` reflect correct version (new) and correct hash of go module)
2. Added `VERSION` files in all go modules, to indicate version of the go module.
3. Added empty `README.md` file (made the filename consistent across all go modules). Need to fill these readmes later.
4. Version bump for utils, assetexchange, and asset-mgmt.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 11:08:27 +0000 UTC
    </div>
</div>

