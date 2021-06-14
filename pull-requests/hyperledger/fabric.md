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
                PR <a href="https://github.com/hyperledger/fabric/pull/2675" class=".btn">#2675</a>
            </td>
            <td>
                <b>
                    [FAB-18484] Return transaction forwarding result back to the client synchronously (backport #2666)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit makes a Raft follower wait for the transaction forwarded to the leader to be sent into
the gRPC stream, and returns the result (success or failure) back to the client accordingly.

Before this commmit, the behavior was that it returns success after enqueueing it into the message queue,
which might have resulted in the transaction being dropped but a success being returned to the client.

Change-Id: I0cd45540be4988845663eb0c68f76fed2ff25b94
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-13 22:28:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2672" class=".btn">#2672</a>
            </td>
            <td>
                <b>
                    [FAB-18484] Return transaction forwarding result back to the client synchronously (backport #2666)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2666 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-13 21:57:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2671" class=".btn">#2671</a>
            </td>
            <td>
                <b>
                    Update email address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updating my email address to the active one. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-13 20:21:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    [FAB-18487] Update broken link in 2.2 branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                
#### Type of change

- Bug fix
- Documentation update

#### Description

Fix broken links in the Fabric 2.2 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 20:06:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2668" class=".btn">#2668</a>
            </td>
            <td>
                <b>
                    [FAB-18490] Link fixes detailed in FAB-18490 (backport #2667)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2667 done by [Mergify](https://mergify.io).
Cherry-pick of c81f265d79c797a133f92c346b813ee7a0710134 has failed:
```
On branch mergify/bp/release-2.3/pr-2667
Your branch is up to date with 'origin/release-2.3'.

You are currently cherry-picking commit c81f265d7.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
	modified:   docs/source/advice_for_writers.md
	modified:   docs/source/capabilities_concept.md
	modified:   docs/source/config_update.md
	modified:   docs/source/create_channel/create_channel_config.md
	modified:   docs/source/create_channel/create_channel_test_net.md
	modified:   docs/source/developapps/gateway.md
	modified:   docs/source/developapps/transactionhandler.md
	modified:   docs/source/developapps/wallet.md
	modified:   docs/source/kafka_raft_migration.md
	modified:   docs/source/tutorial/commercial_paper.md

Unmerged paths:
  (use "git add <file>..." to mark resolution)
	both modified:   docs/source/secured_asset_transfer/secured_private_asset_transfer_tutorial.md

```


To fix up this pull request, you can check it out locally. See documentation: https://help.github.com/articles/checking-out-pull-requests-locally/

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
        Created At 2021-06-11 16:28:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2667" class=".btn">#2667</a>
            </td>
            <td>
                <b>
                    [FAB-18490] Link fixes detailed in FAB-18490
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>


#### Type of change

- Bug fix
- Documentation update

#### Description

Fix links found in the broken link report. Will backport this PR back to 2.3, though will probably need a new PR for 2.2. Note that the broken link in the ordererplan doc was fixed in another PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 15:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2666" class=".btn">#2666</a>
            </td>
            <td>
                <b>
                    [FAB-18484] Return transaction forwarding result back to the client synchronously
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit makes a Raft follower wait for the transaction forwarded to the leader to be sent into
the gRPC stream, and returns the result (success or failure) back to the client accordingly.

Before this commmit, the behavior was that it returns success after enqueueing it into the message queue,
which might have resulted in the transaction being dropped but a success being returned to the client.

Change-Id: I0cd45540be4988845663eb0c68f76fed2ff25b94
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 13:02:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2665" class=".btn">#2665</a>
            </td>
            <td>
                <b>
                    Update private_data_tutorial.rst
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

fabric-samples branch:release-2.2 does not exist anymore.
This break the document link


#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 14:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2664" class=".btn">#2664</a>
            </td>
            <td>
                <b>
                    Update discovery PeersOfChannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update PeersOfChannel behaviour to match Peers function,
i.e. include endpoint in self memeber, only the peers that
have an external endpoint, and sanitizes the envelopes

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 11:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2663" class=".btn">#2663</a>
            </td>
            <td>
                <b>
                    Typo fix in peer deployment guide in main (backport #2660)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2660 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-09 22:29:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2662" class=".btn">#2662</a>
            </td>
            <td>
                <b>
                    Fix jq commands in create channel tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Cherry pick jq command fixes that were made in release-2.3 to the 2.2 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 21:28:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2661" class=".btn">#2661</a>
            </td>
            <td>
                <b>
                    Link fixes in create channel tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Cherry pick link fixes made in the 2.3 branch to main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:57:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2660" class=".btn">#2660</a>
            </td>
            <td>
                <b>
                    Typo fix in peer deployment guide in main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Cherry pick typo fix that was made in the 2.3 branch to main branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:21:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2659" class=".btn">#2659</a>
            </td>
            <td>
                <b>
                    Fix link in orderer deployment guide in main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Cherry picking a link fix that was put into the 2.3 branch into main

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2658" class=".btn">#2658</a>
            </td>
            <td>
                <b>
                    Update ordererplan.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify link "create-channel_participation.html" to "create_channel_participation.html"

Signed-off-by: Corey Lin <514971757@qq.com>

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
        Created At 2021-06-09 02:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2657" class=".btn">#2657</a>
            </td>
            <td>
                <b>
                    Added RetrieveBlockByNumber into blockledger (backport #2635)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2635 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-08 11:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2656" class=".btn">#2656</a>
            </td>
            <td>
                <b>
                    Update peerchecklist.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                modify "tp" to "to"

Signed-off-by: CoreyLin <514971757@qq.com>

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
        Created At 2021-06-08 09:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2655" class=".btn">#2655</a>
            </td>
            <td>
                <b>
                    Clarify doc for readset validations (backport #2647)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2647 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-07 19:38:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2654" class=".btn">#2654</a>
            </td>
            <td>
                <b>
                    Clarify doc for readset validations (backport #2647)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2647 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-07 19:38:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2649" class=".btn">#2649</a>
            </td>
            <td>
                <b>
                    Improve mvcc log warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                MVCC invalidations generated a log warning but did not
indicate which versions are mismatched.
This change adds a log warning indicating the specific
version mismatch to help users troubleshoot MVCC invalidations.

Also the version formatting in the log was updated from format:

   &version.Height{BlockNum:0x6, TxNum:0x0}

to user friendly format:

   {BlockNum: 6, TxNum: 0}

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 18:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2648" class=".btn">#2648</a>
            </td>
            <td>
                <b>
                    Back port 2023 - skip empty ledge and 2635 - RetrieveBlockByNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix
- Improvement (improvement to code, performance, etc)

#### Description
Back porting these 2 fixes:
1. FAB-18276 Ch.Part.API: extractSystemChannel must skip empty ledger (#2023)
2.  Added RetrieveBlockByNumber into blockledger (#2635)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 17:20:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2647" class=".btn">#2647</a>
            </td>
            <td>
                <b>
                    Clarify doc for readset validations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clarify that both prior blocks and prior transactions in the same block
are considered during readset validation.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 15:56:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2646" class=".btn">#2646</a>
            </td>
            <td>
                <b>
                    Use protobuf Getters to avoid nil reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the gateway registry, use the proto generated Get… methods to access the proto structures rather than direct field references.
This protects against dereferencing nil pointers for incomplete structures.  Some unit tests added.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 15:15:58 +0000 UTC
    </div>
</div>

