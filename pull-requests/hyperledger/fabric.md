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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2645" class=".btn">#2645</a>
            </td>
            <td>
                <b>
                    Update secured_private_asset_transfer_tutorial.md (backport #2636)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2636 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-07 09:30:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2644" class=".btn">#2644</a>
            </td>
            <td>
                <b>
                    Update secured_private_asset_transfer_tutorial.md (backport #2636)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2636 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-07 09:29:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2643" class=".btn">#2643</a>
            </td>
            <td>
                <b>
                    FAB-18482 Unable to specify peer's chaincode.externalBuilders as an env variable
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

- Bug fix

#### Description

As the HLF doc says, it's possible to override each config param via env variables, however, it isn't true for chaincode.externalBuilders 

#### Related issues

https://jira.hyperledger.org/browse/FAB-18482

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 23:56:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2642" class=".btn">#2642</a>
            </td>
            <td>
                <b>
                    FABGW-20 Implement TargetOrgs for Evaluate()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Implement the TargetOrganizations grpc option for the Evaluate() method.
- Rewrite logic of Evaluate() to prefer querying the local org

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 16:12:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2641" class=".btn">#2641</a>
            </td>
            <td>
                <b>
                    Update create_channel_test_net.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added missing "export " at adjusting fabric config path

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

- Bug fix (in Documentation): 
  - added missing "export " in cli code
  - added single quotes for jq cli command to prevent the json path from been interpreted somehow by the shell

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
        Created At 2021-06-04 16:10:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2636" class=".btn">#2636</a>
            </td>
            <td>
                <b>
                    Update secured_private_asset_transfer_tutorial.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed typo

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix in documentation 

#### Description

<!--- Describe your changes in detail, including motivation. -->
Org1 was mentioned twice instead of Org1 and Org2

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
        Created At 2021-06-03 14:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2635" class=".btn">#2635</a>
            </td>
            <td>
                <b>
                    Added RetrieveBlockByNumber into blockledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Description
GetBlock is used for retrieving a block in ConfigBlockOrPanic
which has overhead of Iterator. It is now simplified by exposing
a BlockStore function RetrieveBlockByNumber.

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>

#### Type of change
- Improvement (improvement to code, performance, etc)
- Test update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 18:58:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2633" class=".btn">#2633</a>
            </td>
            <td>
                <b>
                    Clarify Verify behaviour in PKCS11 Impl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

the pkcs11 verify implementation will never receive a pkcs11 key to be used to verify a signature, this change clarifies that in the code and adds tests for the verify implementation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 09:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2632" class=".btn">#2632</a>
            </td>
            <td>
                <b>
                    Pass go tags to tools container (bp #2136) 
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

Backport to version 1.4 to fix trouble: when running GO_TAGS=pkcs11 make docker, the fabric-tools docker image doesn't include a PKCS11 provider.

#### Related issues

https://lists.hyperledger.org/g/fabric/topic/error_using_hsm_in_fabric/78302231?p=
https://github.com/hyperledger/fabric/pull/2136
[FAB-18457](https://jira.hyperledger.org/browse/FAB-18457)
https://github.com/hyperledger/fabric/pull/2573
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 01:47:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2631" class=".btn">#2631</a>
            </td>
            <td>
                <b>
                    [FAB-17900] Fixes numeric env variable override bug
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

Backport fix for version 1.4 for error: when setting ORDERER_GENERAL_BCCSP_PKCS11_SECURITY orderer variable, the orderer fails saying that the security value is a string and not an int.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

[FAB-17900](https://jira.hyperledger.org/browse/FAB-17900)
[FAB-18457](https://jira.hyperledger.org/browse/FAB-18457)
https://github.com/hyperledger/fabric/pull/2573
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 01:25:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    Fix minor code comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement

#### Additional details
Address [comment](https://github.com/hyperledger/fabric/pull/2614#discussion_r642961892) in previous PR

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 15:46:42 +0000 UTC
    </div>
</div>

