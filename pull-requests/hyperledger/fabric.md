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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2710" class=".btn">#2710</a>
            </td>
            <td>
                <b>
                    Add explanation of `--ctor` JSON string
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

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

Neither the documentation nor the source code of peer mention the exact format of `--ctor` JSON string. Beginners are likely to frown at that.

By looking at the source and asking questions online, I think I figured out the format of  `--ctor` JSON string. 
In this PR, I add the format explanation on the docs of the peer command.

I am also a newbie. Please check if the explanation is correct and revise. 

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
        Created At 2021-06-24 07:47:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2709" class=".btn">#2709</a>
            </td>
            <td>
                <b>
                    File Location Flag
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

- New feature

#### Description

- New flag allows the user to specify the location of the resulting json file.

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

- [FAB-18425](https://jira.hyperledger.org/browse/FAB-18425)


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
        Created At 2021-06-23 22:23:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2708" class=".btn">#2708</a>
            </td>
            <td>
                <b>
                    Compare Snapshots Utility First 10
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

- New feature
- Test update

#### Description

- Snapshot comparison tool now only finds the first 10 divergences by default. A flag has been added to let the user allow for all divergences to be found.

<!--- Describe your changes in detail, including motivation. -->

#### Related issues

- [FAB-18425](https://jira.hyperledger.org/browse/FAB-18425)


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
        Created At 2021-06-23 22:04:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2707" class=".btn">#2707</a>
            </td>
            <td>
                <b>
                    WIP: prepare for etcd version bump.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jay Guo <guojiannan1101@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 16:15:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2706" class=".btn">#2706</a>
            </td>
            <td>
                <b>
                    Clarify orderers seeing the transaction data (backport #2689)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2689 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-22 19:16:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2705" class=".btn">#2705</a>
            </td>
            <td>
                <b>
                    Clarify orderers seeing the transaction data (backport #2689)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2689 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-22 19:10:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2704" class=".btn">#2704</a>
            </td>
            <td>
                <b>
                    Retire Will Lahti as maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's been wonderful contributing alongside all of you since 2016. I've moved on from fabric for the time-being so it's time for me to retire as a maintainer. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 16:03:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2703" class=".btn">#2703</a>
            </td>
            <td>
                <b>
                    Mandate TLS 1.2 or higher in fabhttp package (backport #2701)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2701 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-22 05:23:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2701" class=".btn">#2701</a>
            </td>
            <td>
                <b>
                    Mandate TLS 1.2 or higher in fabhttp package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit ensures that the HTTP server that is spawned by the fabhttp package
only accepts TLS handshakes from clients that attempt to use TLS 1.2 or higher.

Change-Id: Ia25482d9c96f68506724a58258451311b3d63208
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 20:06:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2699" class=".btn">#2699</a>
            </td>
            <td>
                <b>
                    [FAB-18485]Fabric orderer - add config option for client keepalives
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added config option for orderer client keepalives.  Defaults defined as per the
existing hard coded values. 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 10:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2698" class=".btn">#2698</a>
            </td>
            <td>
                <b>
                    Address PR comments in Gateway integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 09:29:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2697" class=".btn">#2697</a>
            </td>
            <td>
                <b>
                    Fix two typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Eyers <dme@cs.otago.ac.nz>

Fixed two minor typographical errors in the documentation.

#### Type of change

- Documentation update

#### Description

Fixed two minor typographical errors in the documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 04:19:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2695" class=".btn">#2695</a>
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
        Created At 2021-06-21 02:53:11 +0000 UTC
    </div>
</div>

