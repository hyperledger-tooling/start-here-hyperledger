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
                PR <a href="https://github.com/hyperledger/fabric/pull/3990" class=".btn">#3990</a>
            </td>
            <td>
                <b>
                    Fix Makefile did't delete docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Because multi-architecture docker image patches removed tags from the docker image, the docker-clean target could not remove the docker image. This patch changes the docker-clean target to remove untagged docker images.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 00:52:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3989" class=".btn">#3989</a>
            </td>
            <td>
                <b>
                    fix(sec): upgrade github.com/opencontainers/runc to 1.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What happened？
There are 1 security vulnerabilities found in github.com/opencontainers/runc v1.0.0-rc8
- [CVE-2022-29162](https://www.oscs1024.com/hd/CVE-2022-29162)


### What did I do？
Upgrade github.com/opencontainers/runc from v1.0.0-rc8 to 1.1.2 for vulnerability fix

### What did you expect to happen？
Ideally, no insecure libs should be used.

### The specification of the pull request
[PR Specification](https://www.oscs1024.com/docs/pr-specification/) from OSCS
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 14:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3988" class=".btn">#3988</a>
            </td>
            <td>
                <b>
                    Fix chaincode interest for private data purge (backport #3986)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3986 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-02 13:12:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3986" class=".btn">#3986</a>
            </td>
            <td>
                <b>
                    Fix chaincode interest for private data purge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Gateway was not calculating chaincode interest correctly for purge private data calls, since writeset metadata was not being added for purge calls.
The collection level endorsement policies will now be honored instead of defaulting to the chaincode level endorsement policy.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 22:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3977" class=".btn">#3977</a>
            </td>
            <td>
                <b>
                    Move purge private data tests to separate runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 10:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3975" class=".btn">#3975</a>
            </td>
            <td>
                <b>
                    Add BFT support to gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extend the gateway Submit() logic to concurrently send transaction to all available orderers if the channel is configured to use BFT ordering service.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 16:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3974" class=".btn">#3974</a>
            </td>
            <td>
                <b>
                    Improve logging for orderer endpoint override (backport #3969)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3969 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-28 16:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3973" class=".btn">#3973</a>
            </td>
            <td>
                <b>
                    Improve logging for orderer endpoint override (backport #3969)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3969 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-28 16:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3972" class=".btn">#3972</a>
            </td>
            <td>
                <b>
                    Remove whitespace character from ORDERER_GENERAL_LISTENPORT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: kartik chauhan <chauhan.kartik25@gmail.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->
env variable `ORDERER_GENERAL_ LISTENPORT` in section `Experimenting with the orderer service` of the page https://github.com/hyperledger/fabric/tree/main/orderer contains a whitespace character. Fixed the issue by removing the whitespace character.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->
https://github.com/hyperledger/fabric/issues/3971

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-28 03:57:57 +0000 UTC
    </div>
</div>

