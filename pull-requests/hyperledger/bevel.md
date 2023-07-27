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
                PR <a href="https://github.com/hyperledger/bevel/pull/2322" class=".btn">#2322</a>
            </td>
            <td>
                <b>
                    [ci-skip]Fix operations console and remove legacy code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following fixes:
- Update for fabric-operations-console
- vault-auth and vault-reviewer creation removed from fabric (only shared role to be used)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 11:40:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2321" class=".btn">#2321</a>
            </td>
            <td>
                <b>
                    [ci-skip] add README.md files for each Helm chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**docs(fabric): add README.md files for each Fabric Helm chart**

```
This commit adds the README.md file for each Fabric Helm chart. The README.md files provide essential information and instructions about the respective Helm charts, enabling users and developers to deploy each chart individually.

Additionally, the following changes have been made:

 • Updated values.yaml of each Helm chart with default values to provide a clear configuration reference.
 • Added helpers.tpl template file only to Helm charts where it was missing, ensuring consistency across the charts.
 • Updated the description and version fields of each Fabric Helm chart.

These changes enhance the usability and documentation of the Fabric Helm charts, making it easier for users and developers to understand and work with the charts.
```

fixes #2283
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 10:03:00 +0000 UTC
    </div>
</div>

