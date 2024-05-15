---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/713" class=".btn">#713</a>
            </td>
            <td>
                <b>
                    Remove unnecessary GitHub Actions permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Explicit default permissions in workflows are not required with read-only permissions set at the repository level.

Also use a concurrency group for GitHub Pages deployment.

Closes #712
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 17:43:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    Use workflow to publish directly to GitHub Pages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than pushing a commit to the gh-pages branch and having the built-in GitHub pages workflow deploy the contents of that branch, deploy the site content directly using a custom workflow. This avoids complexity and access requirements of pushing to another branch within a workflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 18:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    Use latest stable Go and Node releases in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For GitHub Actions jobs that are not sensitive to the version of Go or Node used, use "stable" or "lts/*" as the version for Go and Node respectively.

Previously the version number was specified explicitly, which requires more ongoing maintenance and conveys less clarity of the intent that the latest stable version should be used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-12 13:49:25 +0000 UTC
    </div>
</div>

