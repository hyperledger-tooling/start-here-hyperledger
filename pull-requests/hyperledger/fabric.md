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
                PR <a href="https://github.com/hyperledger/fabric/pull/3463" class=".btn">#3463</a>
            </td>
            <td>
                <b>
                    Document GetStateByRangeWithPagination behavior
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document GetStateByRangeWithPagination behavior including
the difference between leveldb and couchdb that was identified in #3229.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 23:04:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3462" class=".btn">#3462</a>
            </td>
            <td>
                <b>
                    Fixed Found Typos (Backport #2939)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of PR #2939
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-05 17:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3461" class=".btn">#3461</a>
            </td>
            <td>
                <b>
                    Gateway support for chaincode event checkpointing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of c55b7eed46da67098f9393dbb23df4167a53ebff and 2f2e5aa3f9858928003969282a0b56b271e3ec9c from main branch.

Gateway service will use an `AfterTransactionId` field in a ChaincodeEventsRequest message to locate the exact chaincode event from which eventing should be resumed. Provides server-side support for client checkpointing of chaincode events in Fabric Gateway client API v1.1.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 17:35:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3460" class=".btn">#3460</a>
            </td>
            <td>
                <b>
                    Small typo fix in Ordering Service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Saniyat Al Ahmed <32844821+saniyat013@users.noreply.github.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

There was a small typo in the Ordering Service page of the documentation, in the Raft vs Kafka differences section.
The word "Raft" was used, while it will be "Kafka"

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
        Created At 2022-06-01 08:08:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3459" class=".btn">#3459</a>
            </td>
            <td>
                <b>
                    Add -buildvcs=false for building binaries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go 1.18 tries to pull git version control information into the binaries that it builds,
based on the presence of .git directory. 'git' is not available when building
the Fabric docker images however, and therefore the build fails.

This change adds -buildvcs=false to the builds to suppress the Go 1.18 behavior change.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 04:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3457" class=".btn">#3457</a>
            </td>
            <td>
                <b>
                    Add -buildvcs=false for building binaries (backport #3450)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3450 done by [Mergify](https://mergify.com).


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
        Created At 2022-06-01 04:12:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3456" class=".btn">#3456</a>
            </td>
            <td>
                <b>
                    Fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Waleed Mortaja <waleedmortaja@protonmail.com>

#### Type of change
- Documentation update

#### Description

Duplicated symbols

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 03:45:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3455" class=".btn">#3455</a>
            </td>
            <td>
                <b>
                    Update 'Using Private Data in Fabric' tutorial (Backport #1875)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #1875.
The rst file has already been backported in pull request #1983 but the image and the presentation files have not been backported.
This backport is for the image and the presentation files.
(cherry picked from commit 17858a570ebd0c783e1cb25a4f5ffe2e7889653f)

Signed-off-by: Waleed Mortaja <waleedmortaja@protonmail.com>

Update 'Using Private Data in Fabric' tutorial

Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

fix invoke command on first ReadAsset

Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

minor grammatical fixes

Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

resolve comments

Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

Add Asset Transfer section header and delete pipfile

Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

address comments and add use case section

Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

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
        Created At 2022-06-01 00:13:19 +0000 UTC
    </div>
</div>

