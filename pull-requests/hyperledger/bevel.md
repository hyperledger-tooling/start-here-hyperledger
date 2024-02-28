---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2517" class=".btn">#2517</a>
            </td>
            <td>
                <b>
                    feat(besu): implement proposevalidatorvote  method to add or rem…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ove a node

Changes:

Introduced new helm chart named besu-propose-validator at path platforms/hyperledger-besu/charts/. This chart utilizes the qbft_proposeValidatorVote  method to facilitate the addition or removal of nodes from the validator set based on majority votes. fixes #2508
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 15:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2516" class=".btn">#2516</a>
            </td>
            <td>
                <b>
                    [quorum] implement istanbul_propose method to add or remove a node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(quorum): implement istanbul_propose method to add or remove a node**

**Changes:**
- Introduced new helm chart named `quorum-propose-validator` at path `platforms/quorum/charts/`.
- This chart utilizes the `istanbul_propose` method to facilitate the addition or removal of nodes from the validator set based on majority votes.

fixes #2508
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 12:32:49 +0000 UTC
    </div>
</div>

