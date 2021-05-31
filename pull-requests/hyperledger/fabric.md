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
                PR <a href="https://github.com/hyperledger/fabric/pull/2626" class=".btn">#2626</a>
            </td>
            <td>
                <b>
                    [FAB-18479] Log error if orderer can't forward SubmitRequest (backport #2624)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2624 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-31 11:51:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2625" class=".btn">#2625</a>
            </td>
            <td>
                <b>
                    [FAB-18479] Log error if orderer can't forward SubmitRequest (backport #2624)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2624 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-31 11:51:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2624" class=".btn">#2624</a>
            </td>
            <td>
                <b>
                    [FAB-18479] Log error if orderer can't forward SubmitRequest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [FAB-18479] Log error if orderer can't forward SubmitRequest to Raft leader

If order cannot forward client transaction SubmitRequest to Raft leader,
it only logged it in a debug message. And since the error does
not get returned to the client either, it is difficult to identify
and troubleshoot.

This commit changes the message to an error in the orderer log.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-30 19:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2621" class=".btn">#2621</a>
            </td>
            <td>
                <b>
                    fix duplicate entry in code snippet (backport #2616)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2616 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-29 02:37:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2618" class=".btn">#2618</a>
            </td>
            <td>
                <b>
                    fix duplicate entry in code snippet (backport #2616)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2616 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-29 02:35:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2616" class=".btn">#2616</a>
            </td>
            <td>
                <b>
                    fix duplicate entry in code snippet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

Code snippet had duplicate export.

#### Type of change

- Documentation update

#### Description

Fix duplicate export entry in code snippet.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 22:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2615" class=".btn">#2615</a>
            </td>
            <td>
                <b>
                    Update Building docs to reflect UI changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the Building on GitHub instructions
to reflect UI changes in readthedocs.org

Signed-off-by: Asher T. Scott <ashertlalka@gmail.com>
Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 21:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2614" class=".btn">#2614</a>
            </td>
            <td>
                <b>
                    Add block-number along with validation code for a given TXID
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
This allows gateway to pass on additional relevant info to client and for using it for logging that could be helpful in debugging
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 17:26:13 +0000 UTC
    </div>
</div>

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
                    FABGW-21: Realtime implementation of ChaincodeEvents service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial implementation of Fabric Gateway's ChaincodeEvents service, allowing only listening for realtime chaincode events.
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

