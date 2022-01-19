---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Add config options whether to enable some APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds the following options whether to enable APIs:
- API_CH_PROPOSAL_ENABLED: Whether to enable the Channel Update Proposal APIs
- API_UTIL_ENABLED: Whether to enable the Utility APIs

NOTE: This option only controls at the API server layer. Note that direct execution of the chaincode is still allowed.

This also includes some minor fixes for the default values of some config options.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 03:05:13 +0000 UTC
    </div>
</div>

