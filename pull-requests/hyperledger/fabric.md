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
                PR <a href="https://github.com/hyperledger/fabric/pull/3424" class=".btn">#3424</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix code issues from the updated staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 20:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3423" class=".btn">#3423</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update staticcheck to a version that works with Go 1.18.
Fix code issues with the new staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 19:45:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3420" class=".btn">#3420</a>
            </td>
            <td>
                <b>
                    Log proposal response differences
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the gateway, if proposal responses from different endorsing peers don’t match, then it’s very difficult for the end user to diagnose why.  This commit adds extra logging to help identify the cause of the mismatch.

If the log level is set to ‘debug’ for the ‘gateway’, then the proposal response payloads are unmarshalled and analysed to log specific differences between individual key/values in the read/write sets, SBE policy write differences, event differences and chaincode response differences.  For private collections, only the hashes are logged if they are different.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 12:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3418" class=".btn">#3418</a>
            </td>
            <td>
                <b>
                    Fix mistake change 'curl' to 'git'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-14 14:23:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3408" class=".btn">#3408</a>
            </td>
            <td>
                <b>
                    Fix doc to handle $PWD containing whitepaces (backport #2298)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A backport of pull requset #2298

Note: the file `docs/source/peer-chaincode-devmode.md` does not exist in release-2.2, so I deleted it from the commit.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 14:39:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3406" class=".btn">#3406</a>
            </td>
            <td>
                <b>
                    Update README build badge link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 13:18:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3404" class=".btn">#3404</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.2

Update staticcheck to a version that works with Go 1.18.
Fix code issues with the new staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 16:27:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3403" class=".btn">#3403</a>
            </td>
            <td>
                <b>
                    Update boostrap.sh for test network (backport #2735)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A backport of pull request #2735 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 15:59:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3402" class=".btn">#3402</a>
            </td>
            <td>
                <b>
                    Update links for Jira to GitHub issue transition in README (backport #2956)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A backport of pull request #2956
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 15:36:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3401" class=".btn">#3401</a>
            </td>
            <td>
                <b>
                    Update documentation to include Go SDK (backport #2377)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A backport of pull request #2377
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 14:22:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3400" class=".btn">#3400</a>
            </td>
            <td>
                <b>
                    Fix link to security bug reporting process (backport #2160)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #2160
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 14:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3399" class=".btn">#3399</a>
            </td>
            <td>
                <b>
                    Remove an unused config parameter from peer
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
After the commit of 6c58b2, a config parameter 'DeliverClientKeepaliveOptions' is no longer used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 06:11:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3398" class=".btn">#3398</a>
            </td>
            <td>
                <b>
                    UpdatePrerequisite.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have updated the line which tells to have docker toolbox as the development prerequisite but on official documentation it's support has been depreciates. Hence, I thought to contribute to help people,

Signed-off-by: Ali Akbar <48174866+BCdeveloper98@users.noreply.github.com>

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
        Created At 2022-05-10 05:43:28 +0000 UTC
    </div>
</div>

