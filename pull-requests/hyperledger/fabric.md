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
                PR <a href="https://github.com/hyperledger/fabric/pull/3891" class=".btn">#3891</a>
            </td>
            <td>
                <b>
                    Trim the (optional) semrev leading 'v' when resolving the ccenv image URL (backport #3879)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3879 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-03 14:26:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3890" class=".btn">#3890</a>
            </td>
            <td>
                <b>
                    Endorsement policies doc edited
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - to avoid confusion for any user reading the document.
- to enable direct copying and pasting of the commands

Signed-off-by: Rajat Sharma <Rajat16.Sharma@ril.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->
- Documentation update

#### Description

The default documentation mentioned for [endorsement-policies](https://hyperledger-fabric.readthedocs.io/en/latest/endorsement-policies.html), does not work.

As the samples only use `Org1MSP` or `Org2MSP`, all the examples state `"AND('Org1.peer', 'Org2.peer')"`. These don't work on the test network.

#### Additional details

This is a documentation change that will help a user to use custom endorsements effectively.

#### Related issues
#3884 
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
        Created At 2023-01-03 14:07:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3889" class=".btn">#3889</a>
            </td>
            <td>
                <b>
                    Update jq command in channel config docs (backport #3888)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3888 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-03 11:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3888" class=".btn">#3888</a>
            </td>
            <td>
                <b>
                    Update jq command in channel config docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've found that quotes are needed around the jq target path.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 02:23:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3885" class=".btn">#3885</a>
            </td>
            <td>
                <b>
                    Fix: Ethereum has POS-based consensus mechanism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We are in the post _The MERGE_ era.

Signed-off-by: AMIT KUMAR MISHRA <71893015+Amit0617@users.noreply.github.com>

#### Type of change
- Documentation update

#### Description

Ethereum is now POS based

#### Additional details

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-29 08:12:08 +0000 UTC
    </div>
</div>

