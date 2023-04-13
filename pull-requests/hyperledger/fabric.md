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
                PR <a href="https://github.com/hyperledger/fabric/pull/4159" class=".btn">#4159</a>
            </td>
            <td>
                <b>
                    Fix failure in 'basic checks'
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

This patch fixes failure during 'basic checks' in the CI. It is possibly caused by the update of Go to v1.20.

#### Additional details

During the "basic checks" job, the command references are compared with the generated ones. Since the Go version is updated to v1.20, the CI job generates slightly different documents from those in the repository, which were generated with the previous versions of Go.

#### Related issues

#4157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 09:47:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4158" class=".btn">#4158</a>
            </td>
            <td>
                <b>
                    Fix typo regarding current LTS release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Fix typo regarding the current LTS release in README
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 09:39:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4157" class=".btn">#4157</a>
            </td>
            <td>
                <b>
                    Add docs for 'ledgerutil verify'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

This is a backport of #4098 to release-2.5, fixing the failed automated backport #4153.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 05:27:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4153" class=".btn">#4153</a>
            </td>
            <td>
                <b>
                    Add docs for 'ledgerutil verify' (backport #4098)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4098 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 19:24:33 +0000 UTC
    </div>
</div>

