---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3653" class=".btn">#3653</a>
            </td>
            <td>
                <b>
                    Improves image size for better readability (backport #3646)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3646 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 15:25:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3652" class=".btn">#3652</a>
            </td>
            <td>
                <b>
                    Improves image size for better readability (backport #3646)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3646 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 15:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3651" class=".btn">#3651</a>
            </td>
            <td>
                <b>
                    WIP: Transfer leadership before submitting to raft library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description

If transaction request rotates the current leader cert or removes it then transfer the leadership to another node before proposing the transaction for orderering. It would help to avoid the leadership transfer while committing the block

#### Additional details


#### Related issues
#3629 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 09:51:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3648" class=".btn">#3648</a>
            </td>
            <td>
                <b>
                    GitHub Workflows security hardening
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds explicit [permissions section](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#permissions) to workflows. This is a security best practice because by default workflows run with [extended set of permissions](https://docs.github.com/en/actions/security-guides/automatic-token-authentication#permissions-for-the-github_token) (except from `on: pull_request` [from external forks](https://securitylab.github.com/research/github-actions-preventing-pwn-requests/)). By specifying any permission explicitly all others are set to none. By using the principle of least privilege the damage a compromised workflow can do (because of an [injection](https://securitylab.github.com/research/github-actions-untrusted-input/) or compromised third party tool or action) is restricted.
It is recommended to have [most strict permissions on the top level](https://github.com/ossf/scorecard/blob/main/docs/checks.md#token-permissions) and grant write permissions on [job level](https://docs.github.com/en/actions/using-jobs/assigning-permissions-to-jobs) case by case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 20:06:14 +0000 UTC
    </div>
</div>

