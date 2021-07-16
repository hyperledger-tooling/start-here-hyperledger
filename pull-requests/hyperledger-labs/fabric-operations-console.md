---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Use the --production flag on 'npm audit'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                npm audit was broken as the 'default' working-directory and the run steps working-directory were in conflict. The existing 'npm audit' didn't actually run but was hidden by the 'continue-on-error' property. This change fixes the working directory and replaces the use of modifying the package.json file with the npm audit '--production' flag to prevent scanning the devDependencies.

Signed-off-by: Brett Logan <lindluni@github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 05:04:25 +0000 UTC
    </div>
</div>

