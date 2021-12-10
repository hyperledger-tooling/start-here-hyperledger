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
                PR <a href="https://github.com/hyperledger/fabric/pull/3111" class=".btn">#3111</a>
            </td>
            <td>
                <b>
                    Update the Makefile target for release/
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updating the release/xxx target to include the cc builders in the tgz
The dist/xxx target was originally updated, but the actual publishing from the fabric-interop test doesn't use this target.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 09:55:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3110" class=".btn">#3110</a>
            </td>
            <td>
                <b>
                    Update 'Running a Fabric Application' tutorial for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also fixed a few build warnings in other documents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 22:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3109" class=".btn">#3109</a>
            </td>
            <td>
                <b>
                    Update config transaction validation logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix misleading debug message.
Log info when channel config is applied.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 21:59:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3108" class=".btn">#3108</a>
            </td>
            <td>
                <b>
                    Adding chaincode-as-a-service external builder to peer's docker image (backport #2990)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2990 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-09 14:50:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3107" class=".btn">#3107</a>
            </td>
            <td>
                <b>
                    Fix channel config callback in gateway (backport #3102)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3102 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-08 20:36:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3104" class=".btn">#3104</a>
            </td>
            <td>
                <b>
                    Gateway to use simplified createTx function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway has been reusing the protoutil.CreateTx function to build the transaction envelope from the set of endorsements.  This function changed recently to add extra information into the error message if the proposal responses don’t all match.  This change was identified as causing a problem for the gateway (https://github.com/hyperledger/fabric-gateway/issues/332).
This commit adds a simplified createTx function in the gateway package that removes this amendment and also removes some other checks that aren’t relevant to its usage in the gateway.

Resolves https://github.com/hyperledger/fabric-gateway/issues/332

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 15:52:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3102" class=".btn">#3102</a>
            </td>
            <td>
                <b>
                    Fix channel config callback in gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, the config update callback triggers a discovery call to get the updated channel orderers.
However, this relies on the discovery service having processed the config message before the gateway.  If it hasn’t, the gateway just gets the stale orderer config.
This commit changes the logic so the gateway extracts the orderer endpoints directly from the config bundle.

Resolves https://github.com/hyperledger/fabric-gateway/issues/318

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 09:59:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3099" class=".btn">#3099</a>
            </td>
            <td>
                <b>
                    updating peer-chaincode-devmode.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding new instructions to create /var/hyperledger folder required by Hyperledger

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

This PR updates the documentation by adding instructions for creating `/var/hyperledger` directory. If such directory doesn't exist the orderer will not be able to run after executing 
`ORDERER_GENERAL_GENESISPROFILE=SampleDevModeSolo orderer`


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
        Created At 2021-12-04 21:55:34 +0000 UTC
    </div>
</div>

