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
                PR <a href="https://github.com/hyperledger/fabric/pull/3194" class=".btn">#3194</a>
            </td>
            <td>
                <b>
                    Clarify paths in core.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clarify whether paths in core.yaml may be absolute or relative.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 17:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3193" class=".btn">#3193</a>
            </td>
            <td>
                <b>
                    Update dependency fabric-protos-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

The update includes a new field in the proto message for
enabling pvt data purge.

#### Type of change
- New feature

#### Related issues

Resolves #3021 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 21:00:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3191" class=".btn">#3191</a>
            </td>
            <td>
                <b>
                    Update deploy_chaincode.md `package` command docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Define the default behavior of `peer lifecycle chaincode package`, which does *not* include node_modules in the resulting tar.gz package for chaincode. The existing step of `npm install` and quote "If the command is successful, the JavaScript packages will be installed inside a `node_modules` folder. Now that we that have our dependencies, we can create the chaincode package." would lead a reader to believe that `node_modules` are included when they are not. 

Also added more detail about what chaincode services allow `node_modules` when packaged manually.

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
        Created At 2022-01-25 18:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3190" class=".btn">#3190</a>
            </td>
            <td>
                <b>
                    Modify GetBlockByHash method to canonical style
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
- Improvement

#### Description
This PR modifies GetBlockByHash method to canonical style, similar to the other functions in the kv_ledger go code
<!--- Describe your changes in detail, including motivation. -->

#### Related issues
Issue #3101 
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
        Created At 2022-01-24 23:35:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3189" class=".btn">#3189</a>
            </td>
            <td>
                <b>
                    Address windows platform in documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #2993
Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

Address how windows users can install and contribute to fabric. The current documentation was inaccurate


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 17:20:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3188" class=".btn">#3188</a>
            </td>
            <td>
                <b>
                    remove redundant requirements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

This removes some redundant text from writing first app. You do not need windows build tools or any linux build tools for this tutorial but also this information about how to install build tools is out of date (ie not correct anymore) and in the case of linux, also specific to ubuntu (and may not work on other distros)

contributes to #2993 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 14:19:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3186" class=".btn">#3186</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.17.5 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.17.5.

First commit runs goimports to fix up build instructions.
Second commit updates unit tests and dependencies to work with Go 1.17.5.
Third commit updates docs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 05:02:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3183" class=".btn">#3183</a>
            </td>
            <td>
                <b>
                    Wire-in retroactive creation of hashed-index in pvtdatastore at peer start
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
This PR adds code for invoking the function for creating hashed-indexes in pvtdatastore at the time of peer start.

#### Related issues
issue# 3022

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 15:54:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3182" class=".btn">#3182</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.17.5 (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.17.5 (release-2.4)

Backport 3 commits from main branch related to Go 1.17 update, including dependency updates and test fixes.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 20:15:55 +0000 UTC
    </div>
</div>

