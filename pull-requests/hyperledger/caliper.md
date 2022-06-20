---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1376" class=".btn">#1376</a>
            </td>
            <td>
                <b>
                    Port the integration test workflow to GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:

* The integration test workflow which exists in Azure Pipelines is ported over to GitHub Actions.
* A badge is added to the README for the workflow.
* The migration is complete. Optimizations like cache management will be tackled later.
* The `package-lock.json` file which was earlier removed from `.gitignore` is added back.

Closes #1366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 12:45:23 +0000 UTC
    </div>
</div>

