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
                PR <a href="https://github.com/hyperledger/bevel/pull/2340" class=".btn">#2340</a>
            </td>
            <td>
                <b>
                    [ci-skip] fix default values in values.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs(corda): fix default values in values.yaml

fix default values in values.yaml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 04:57:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2339" class=".btn">#2339</a>
            </td>
            <td>
                <b>
                    [ci-skip] move hashicorp vault functions to a single script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(quorum): move hashicorp vault functions to a single script**

```
This commit decouples the vault related functionality from individual helm charts by utilizing the bevel-vault.sh script.

Changes Made:

 • Removed vault-related code from individual Quorum Helm charts.
 • Updated all Helm charts to utilize the shared bevel-vault.sh script.
 • Improved code quality by fixing if-conditions defined in the shared bevel-vault.sh script.
 • Deleted the node_quorum Helm chart and its quorum.tpl template file because they are not being used. Instead, we always use the node_quorum_member Helm chart for the same purpose.

These changes will improve code maintainability and efficiency by reducing code duplication and making it easier to maintain consistency.
```

fixes #2323
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 13:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2338" class=".btn">#2338</a>
            </td>
            <td>
                <b>
                    [docs] Fix Sphinx version to solve build error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix Sphinx build errors on readthedocs

#2337
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 10:42:31 +0000 UTC
    </div>
</div>

