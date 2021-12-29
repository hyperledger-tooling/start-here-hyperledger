---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    chore(chaincode): Remove old chaincode and rearrange files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR closes #51. It makes the following changes:
* Deletes the `chaincode/go`, `chaincode/node` and `emissions_calc_test` directories
* Moves the `typescript`, `packaging` and `deploy` directories into a new `emissionscontract` directory
* Modifies Ansible script to use new file path
* Modifies CI workflow to use new file paths
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 18:43:28 +0000 UTC
    </div>
</div>

