---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Introduce staticchecks and spellchecking for go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                **What this PR does / why we need it**:

This PR introduces more tools to enhance code quality to our build pipeline.
In particular, we add [staticcheck](https://staticcheck.io/) and spellchecking to our golinter script and fix all detected issues, including dead code, removing dependencies of deprecated code, unchecked vars, and spelling issues.

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Closes #403 

**Special notes for your reviewer**:

Note that there exists a commit for adding the new tool and another commit that fixes the detected issues. I suggest review commit by commit.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 12:21:45 +0000 UTC
    </div>
</div>

