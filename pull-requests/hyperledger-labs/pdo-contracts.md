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
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Jupyter Notebooks to illustrate the inference-contract family.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Notebooks' structure, installation, execution patterns are same as those used by the Noteboks provided for the Exchange contract family. Please note that the inference guardian service must be started prior to executing the notebooks. Please see inference-contract/README.md for instructions.

Some of the additional features offered by this PR taking advantage of recent commits to the contracts repo:

1. It is possible to use the inference contract jupyter notebook via docker (using features from PR 23)
2. When using docker, the inference guardian will run in a separate container (using features from PR 27)
3. The notebooks are constructed using jupytext python modules (using features from PR 29)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-19 23:08:00 +0000 UTC
    </div>
</div>

