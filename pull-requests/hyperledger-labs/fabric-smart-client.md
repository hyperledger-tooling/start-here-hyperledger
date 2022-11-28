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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    key validation removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Currently, FSC Vault is more restrictive when parsing RW sets imposing rules that Fabric does not actually impose.
This results in panic when transactions with a RW sets containing keys that do not pass the FSC check are committed to Fabric.

This PR fixes this issue by removing the extra checks.

Signed-off-by: Norhan Ali Araba <Norhan.Ali.Araba-CICNetherlands@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 11:05:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    extensions
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
        Created At 2022-11-22 10:03:29 +0000 UTC
    </div>
</div>

