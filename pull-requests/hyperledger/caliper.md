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
                PR <a href="https://github.com/hyperledger/caliper/pull/1364" class=".btn">#1364</a>
            </td>
            <td>
                <b>
                    Port the unit test workflow to GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The unit test workflow which exists in Azure Pipelines is ported over to GitHub Actions
* A badge is added to the README for the workflow

Closes #1359 

#### Some additional notes:

* Package lock is added to help keep track of the dependency cache (It is also recommended to commit the lock file to source control in the official NodeJS guide https://nodejs.dev/learn/the-package-lock-json-file)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 12:12:07 +0000 UTC
    </div>
</div>

