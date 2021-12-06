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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3095" class=".btn">#3095</a>
            </td>
            <td>
                <b>
                    Final peer for gateway (backport #3091)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3091 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-02 17:04:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3094" class=".btn">#3094</a>
            </td>
            <td>
                <b>
                    Final network orderers (backport #3090)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3090 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-02 13:13:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3093" class=".btn">#3093</a>
            </td>
            <td>
                <b>
                    Randomize endorsement layouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry pick of https://github.com/hyperledger/fabric/commit/7c736c44b5b9d2ba4d64d148a8fca2be2bb59341 from main branch

For improved load balancing and fairer workload distribution across organizations, then gateway should randomize the endorsement layouts

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 08:43:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3092" class=".btn">#3092</a>
            </td>
            <td>
                <b>
                    Create HashedIndex in Pvtdata Store retroactively
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: manish <manish.sethi@gmail.com>

- Add functions in the pvtdata store package that would be used for creating the HashedIndex in Pvtdata Store retroactively.
- We use this opportunity to upgrade the data format from V11 to V12, so we can simplify the reading code in the future releases.
- Small refactoring is included to simplify the usage of update batch.

#### Type of change
- New feature

#### Related issues
- [RFC](https://github.com/hyperledger/fabric-rfcs/blob/main/text/0000-private_data_purge.md)
- [Issue](https://github.com/hyperledger/fabric/issues/3022) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 20:49:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3091" class=".btn">#3091</a>
            </td>
            <td>
                <b>
                    Final peer for gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peers topic for new gateway service, updates following WebEx with @andrew-coleman 

#### Type of change

- New feature
- Documentation update

#### Description

gateway service running on peers in Fabric v2.4

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 16:43:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3090" class=".btn">#3090</a>
            </td>
            <td>
                <b>
                    Final network orderers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Final doc for Networks and Orderers, following WebEx with @andrew-coleman

#### Type of change

- New feature
- Documentation update

#### Description

Updates for the gateway service now managing Tx proposals and endorsements.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 16:13:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3089" class=".btn">#3089</a>
            </td>
            <td>
                <b>
                    Randomize endorsement layouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For improved load balancing and fairer workload distribution across organizations, then gateway should randomize the endorsement layouts

Resolves https://github.com/hyperledger/fabric-gateway/issues/338

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 11:58:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3088" class=".btn">#3088</a>
            </td>
            <td>
                <b>
                    Corrected container names in commercial paper tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Corrected container names in commercial paper tutorial

#### Type of change

- Documentation update

#### Description
Corrected container names in commercial paper tutorial. The container names for Org1 and Org2 were swapped with each other.

Signed-off-by: Nidhi Singh <nidhi2894@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 11:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3087" class=".btn">#3087</a>
            </td>
            <td>
                <b>
                    Add command reference doc for ledgerutil
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add command reference doc for ledgerutil.
Includes minor edits to the command's user messages.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 17:10:01 +0000 UTC
    </div>
</div>

