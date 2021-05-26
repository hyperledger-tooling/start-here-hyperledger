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
                PR <a href="https://github.com/hyperledger/fabric/pull/2610" class=".btn">#2610</a>
            </td>
            <td>
                <b>
                    Optionally disable gossip block forwarding (backport #2606)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2606 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 03:15:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2609" class=".btn">#2609</a>
            </td>
            <td>
                <b>
                    Optionally disable gossip block forwarding (backport #2606)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2606 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 03:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2608" class=".btn">#2608</a>
            </td>
            <td>
                <b>
                    Update deploy_chaincode.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix some typos.

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 02:36:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2607" class=".btn">#2607</a>
            </td>
            <td>
                <b>
                    Updated setting up environment documentation to reflect "brew cask" no longer being a valid command
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

Replaced "brew cask install --appdir=“/Applications” docker" with "brew install --cask docker"

Cask is no longer a brew command. When you want to install a Cask, you just do brew install or brew install --cask instead of brew cask install.

#### Additional details

N/A

#### Related issues

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2606" class=".btn">#2606</a>
            </td>
            <td>
                <b>
                    Optionally disable gossip block forwarding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds a new configuration option to the peer which makes peers
not forward blocks that they pull from the ordering service.

If all peers in an organization explictly set "peer.deliveryclient.blockGossipEnabled" to false, 
no peer in the organization gossips blocks to any other peer in that organization.

Change-Id: I5d9b278ae72f239129827c044fa78179f6ba87ab
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:11:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2604" class=".btn">#2604</a>
            </td>
            <td>
                <b>
                    FABGW-21: Return block number in CommitStatusResponse
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor Gateway's CommitStatus service in line with updated protobufs, so the returned CommitStatusResponse message includes the block number in which the transaction committed.

First step towards implementing chaincode event listening. A dummy implementation of that service that returns an error is included.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 17:42:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    Fixed JIRA issue FLY2- 64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have updated chain.go  Submit and ordered method..

#Fixed FLY2-64
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 09:36:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2601" class=".btn">#2601</a>
            </td>
            <td>
                <b>
                    Maintain order of transactions in the commit notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Maintain order of transactions in the commit notification so the gateway can deliver the clients the chaincode events in the same and consistent order.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 18:21:07 +0000 UTC
    </div>
</div>

