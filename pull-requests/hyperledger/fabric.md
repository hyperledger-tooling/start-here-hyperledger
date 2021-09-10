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
                PR <a href="https://github.com/hyperledger/fabric/pull/2905" class=".btn">#2905</a>
            </td>
            <td>
                <b>
                    Updates in main for v2.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and scripts in main branch for v2.3.3 release.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:40:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2903" class=".btn">#2903</a>
            </td>
            <td>
                <b>
                    Release commit for v2.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.3.3.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 18:58:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2901" class=".btn">#2901</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.2.4.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 18:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2900" class=".btn">#2900</a>
            </td>
            <td>
                <b>
                    updated chaincode4ade.rst("Writing your first chaincode") showing good practise on how to achieve determinism in json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: fraVlaca <ocsenarf@outlook.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 15:00:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2899" class=".btn">#2899</a>
            </td>
            <td>
                <b>
                    Minor code clean-up in Gateway ChaincodeEvents handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove code duplication and improve readability of `ChaincodeEvents()` function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 06:05:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2897" class=".btn">#2897</a>
            </td>
            <td>
                <b>
                    install-fabric.sh script - updated version of bootstrap.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Background:  I've always found the existing bootstrap.sh script to confusing... do the versions come first or last.  Having to think what components I want to NOT have.

I wanted to offer up this alternative way of working for discussion.

Uses positional arguments and opt-in logic to control the components to install
Uses options to define the optional fabric and ca versions

Order of arguments and options is not important

eg
```
install-fabric.sh docker binary samples         # install docker images, binaries and clones samples dir
install-fabric.sh d b s                         # install all components but with short-hand
install-fabric.sh -f 2.4.0-beta b               # 2.4.0-beta for binaries only
install-fabric.sh docker -c 1.5.1 -f 2.4.0-beta # docker images but for 1.5.1 CA and 2.4.0-beta
```
it is an error to NOT specify a component

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>

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
        Created At 2021-09-06 15:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2896" class=".btn">#2896</a>
            </td>
            <td>
                <b>
                    Implement chaincode event replay for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2792 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 14:01:40 +0000 UTC
    </div>
</div>

