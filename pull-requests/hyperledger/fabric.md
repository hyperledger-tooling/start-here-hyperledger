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
                PR <a href="https://github.com/hyperledger/fabric/pull/2732" class=".btn">#2732</a>
            </td>
            <td>
                <b>
                    [FAB-11334] Adds a new 'peer node unjoin' feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The UnjoinChannel routine will mark a ledger as pending delete, removing all
channel specific data from the peer.  The routine must be invoked while the
peer is down.  Peer operators may issue the deletion by running the companion
'peer node unjoin' command from the console.

#### Type of change

- New feature

#### Description

[As a peer admin, I need a way to pause/resume a channel](https://jira.hyperledger.org/browse/FAB-16035)

Unjoining a is a helpful routine for operators managing channel lifecycles.  In some cases, a network participant may opt out of a channel, requesting a complete deletion of all channel specific data from the ledger.  While an operator may issue a node reset after pausing a channel, this is not viable in cases where the re-initialization requires the synchronization of a large (millions / billions) number of transactions. 

#### Related issues

[FAB-16035](https://jira.hyperledger.org/browse/FAB-16035)
[FAB-4481](https://jira.hyperledger.org/browse/FAB-4481)
[FAB-17787](https://jira.hyperledger.org/browse/FAB-17787)
[FAB-17801](https://jira.hyperledger.org/browse/FAB-17801)

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
        Created At 2021-07-01 13:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2731" class=".btn">#2731</a>
            </td>
            <td>
                <b>
                    Fixed grammatical errors (backport #2715)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2715 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-30 14:18:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2730" class=".btn">#2730</a>
            </td>
            <td>
                <b>
                    Fixed grammatical errors (backport #2715)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2715 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-30 14:17:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2729" class=".btn">#2729</a>
            </td>
            <td>
                <b>
                    [Docs] Added "What is a commercial paper" section. (backport #2723)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2723 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-30 14:09:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2728" class=".btn">#2728</a>
            </td>
            <td>
                <b>
                    [Docs] Added "What is a commercial paper" section. (backport #2723)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2723 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-30 14:08:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2726" class=".btn">#2726</a>
            </td>
            <td>
                <b>
                    [FAB-18509] Stop panic if collection index path is wrong
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>

#### Type of change
- Bug fix

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 09:16:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2725" class=".btn">#2725</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wuqiaomin <wuqiaomin2@huawei.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 07:31:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2724" class=".btn">#2724</a>
            </td>
            <td>
                <b>
                    [FAB-18508] ledger utility always outputs txNum
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

This patch fixes a bug reported in FAB-18508, and makes the ledger troubleshooting utility output always the record "txNum".

#### Additional details

The bug occurred when the target transaction is the first transaction of a block (txNum == 0). This patch removes the `omitempty` attributes from all the members of a record.

Note that this patch also changes the output when a key is missing in either snapshot. Instead of an empty object ({}) for the missing snapshot, the entire key (either "snapshotrecord1" or "snapshotrecord2") will be omitted.
(Refer to the changes in the test code)

#### Related issues

https://jira.hyperledger.org/projects/FAB/issues/FAB-18508
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 08:26:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2723" class=".btn">#2723</a>
            </td>
            <td>
                <b>
                    [Docs] Added "What is a commercial paper" section.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Inserted "What is the commercial paper" section. It gives better background for a reader from a non-financial background and makes it easier to understand the project from the start.

#### Type of change

- Documentation update

#### Description

While going through the Developing applications section in Fabric docs, I was not able to fully concentrate concentrate on the technical aspect of things because I kept wondering what the term "commercial paper" meant. I had to google it. 
Adding this new section in the documentation would provide for a better integrated experience for the reader.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 07:34:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2722" class=".btn">#2722</a>
            </td>
            <td>
                <b>
                    Add function to delete the ledger data for a channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Description
This PR adds a function that takes the ledger config and deletes the data for a channel

#### Additional details
This is a basic function that would be invoked in the future PR and the tests will be added in that PR

#### Related issues
[FAB-11334](https://jira.hyperledger.org/browse/FAB-11334)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 03:03:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2721" class=".btn">#2721</a>
            </td>
            <td>
                <b>
                    Fix a typo in CouchDB tutorial (backport #2714)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2714 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-28 19:43:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2720" class=".btn">#2720</a>
            </td>
            <td>
                <b>
                    Fix a typo in CouchDB tutorial (backport #2714)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2714 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-28 19:42:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2719" class=".btn">#2719</a>
            </td>
            <td>
                <b>
                    Add explanation of `--ctor` JSON string (backport #2710)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2710 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-28 19:11:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2718" class=".btn">#2718</a>
            </td>
            <td>
                <b>
                    Add explanation of `--ctor` JSON string (backport #2710)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2710 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-28 19:10:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2715" class=".btn">#2715</a>
            </td>
            <td>
                <b>
                    Fixed grammatical errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->
Fixed basic grammatical errors in the documentation.

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
        Created At 2021-06-28 08:16:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2714" class=".btn">#2714</a>
            </td>
            <td>
                <b>
                    Fix a typo in CouchDB tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Atsushi Neki <nekiaiken@gmail.com>

Fix an incorrect index document name within a sentence, which was found while translating into other language. 

#### Type of change

- Documentation update

#### Description

Fix an incorrect index document name `ownerIndexDoc` within a sentence to `indexOwnerDoc` which is the name used in chaincode index configuration in this tutorial. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-26 02:03:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2713" class=".btn">#2713</a>
            </td>
            <td>
                <b>
                    Updated enrollUser function in write_first_app tutorial
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

Updated the function called to register a user in Write First App tutorial. Function being called in the docs was `registerUser` but in the code base the function is called `registerAndEnrollUser`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 23:04:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2712" class=".btn">#2712</a>
            </td>
            <td>
                <b>
                    Use protoc-gen-go 1.3.3 for generating fabric protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A previous commit [#2113](https://github.com/hyperledger/fabric/pull/2113/files#diff-11f03b0f97705b85807a720c4608013062002af3604f046a09a2571b0ae02554L9) upgraded the protobuf in tools while the protobuf in fabric dependencies is still 1.3.3. This upgrade was caused by swagger inclusion.

In the current form, `make protos` causes to use upgraded version of protoc-gen-go. This, in turn, requires to upgrade the protobuf lib in the fabric dependancies -- which we could not until we resolve some issues. See [FAB-18363](https://jira.hyperledger.org/browse/FAB-18363).

Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Bug fix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 18:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2711" class=".btn">#2711</a>
            </td>
            <td>
                <b>
                    docker network net_test -> fabric_test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Documentation update
docker network name is `fabric_test` not `net_test` in release-2.3


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 02:25:48 +0000 UTC
    </div>
</div>

