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
                PR <a href="https://github.com/hyperledger/fabric/pull/2586" class=".btn">#2586</a>
            </td>
            <td>
                <b>
                    NewSnapshotReader Nil Error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

- Edited NewSnapshotReader so it now creates and returns a new error if the passed in filename does not exist

#### Related issues

- [FAB-18469](https://jira.hyperledger.org/browse/FAB-18469)

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
        Created At 2021-05-10 18:38:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2585" class=".btn">#2585</a>
            </td>
            <td>
                <b>
                    Update chaincode4ade.rst
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
        Created At 2021-05-10 16:27:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2584" class=".btn">#2584</a>
            </td>
            <td>
                <b>
                    Documentation updated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kestutis Gudynas <44440041+kemi04@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 12:34:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2583" class=".btn">#2583</a>
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
        Created At 2021-05-10 10:48:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2582" class=".btn">#2582</a>
            </td>
            <td>
                <b>
                    Correcting a possible typo
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
I believe it should be "Now that R3 is able to fully participate in channel C1" instead of "Now that R3 is able to fully participate in channel C2" because the latter one doesn't make sense to me as R3 already had the permission to participate in channel C2 and given the context having C1 makes sense.

P.S: Apologies if perhaps I got something wrong, I just started learning Hyperledger Fabric :)

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
        Created At 2021-05-09 10:30:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2581" class=".btn">#2581</a>
            </td>
            <td>
                <b>
                    Add vendor directories into chaincode code package tar when install golang chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: xuchengli <lixucheng@aliyun.com>

If chaincode dependency have multi-level directory, only META-INF metadata directory will be added into chaincode code package tar, other dependency directories will be skipped. So when instantiate chaincode it will throw error of missing file or directory. By adding vendor directory at the root of chaincode directory will avoid the issue.

Jira issue: https://jira.hyperledger.org/browse/FAB-18467

- Bug fix

Test:
1. Compile peer binary based on the patch.
2. Restart peer using the latest peer binary.
3. Install and instantiate the chaincode with multi-level vendor dependency directories. The test chaincode is: https://github.com/xuchengli/fabric-chaincode/tree/main/src/test-1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 10:51:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2579" class=".btn">#2579</a>
            </td>
            <td>
                <b>
                    Revert "Simplify GitHub Action for AZP Triggering"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit b1f43299ac7a3325bd686e1d34869b170b1fcc51.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 13:09:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2578" class=".btn">#2578</a>
            </td>
            <td>
                <b>
                    FABGW-20 Specify endorsing organizations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implementation of endorsingOrgs in gateway Endorse method.
- The set of endorsing peers from the discovery service is filtered down to only include those from the specified orgs.
- The discovery handling code has been upgraded to step through all given layouts to find a layout that satisfies the endorsingOrgs constraint.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 09:56:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2577" class=".btn">#2577</a>
            </td>
            <td>
                <b>
                    modify some errors in tutorial document for secured_private_asset_transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The modified command can be directly copied and run on the linux server

Signed-off-by: c20liu <diandian.yong@163.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
Refer to the tutorial document of the previous version to  the test case,  I found it is necessary to manually modify the command to execute it successfully.

So some errors have been fixed

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
        Created At 2021-05-07 07:30:47 +0000 UTC
    </div>
</div>

