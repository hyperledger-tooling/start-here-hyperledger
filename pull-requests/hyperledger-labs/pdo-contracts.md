---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Fix numpy version to 1.24.4 for use within Inference contract guardian.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before this PR, numpy was autoinstalled as part of opencv installation. At the time of this PR, opencv attempts to install numpy 2.0.0, and this is not consistent with the rest of the guardian code. This change fixes the recent guardian failures that were being seen due to the numpy dependency issue.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 22:57:19 +0000 UTC
    </div>
</div>

