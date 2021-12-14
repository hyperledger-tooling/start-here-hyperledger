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
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add voting config option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds a voting configuration option for chaincode_ops.
This allows OpsSC users to configure the maximum number of malicious organizations (`f`) in the voting process.

- If the option is set, 2f + 1 is required to judge a proposal get `Approved`.
- If the option is not set, a majority of all participating organizations is required to judge a proposal get `Approved`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 11:23:01 +0000 UTC
    </div>
</div>

