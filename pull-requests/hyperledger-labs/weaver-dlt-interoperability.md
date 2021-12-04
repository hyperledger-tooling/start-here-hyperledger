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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    Using protos for Asset Transfer in fabric.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Using protos for Asset Transfer in fabric.
2. Clean up `simpleassettransfer` and `simpleasset` chaincode.
3. Added new local query function to `simpleassettransfer` named `GetAssetPledgeDetails` to fetch asset pledge details locally (not for remote query).
4. Updated fabric-cli, added native fabric-cli commands for `claim` and `reclaim` instead of scripts.
5. Moved common code for interop call to helpers, and some fabric-cli bug fixes.
6. Updated docs as per new changes.

Edit:
1. Added workflow to automate deployment of docs as soon as `docs` folder is updated on PR merge.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 17:36:34 +0000 UTC
    </div>
</div>

