---
layout: default
title: indy-test-automation
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-test-automation
---

# indy-test-automation <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-test-automation){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-test-automation/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Refactor installation of package under test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor get dependency script to work recursively and traverse to the required depth.
  - The node specific version of this script is no longer needed.
  - Update (simplify) related scripts and workflows.
  - After deleting an erroneous package (python3-semver > 2.13.0) from the `dev` channel traversing the top dependencies for an indy-node based deb is enough.
- Remove unused files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 17:16:12 +0000 UTC
    </div>
</div>

