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
                PR <a href="https://github.com/hyperledger/fabric/pull/4244" class=".btn">#4244</a>
            </td>
            <td>
                <b>
                    Make AmMemberOf to use only the mspIDs in collection policy
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

https://github.com/hyperledger/fabric/issues/4229

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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 18:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4242" class=".btn">#4242</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: verify attestation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Ia34ff4536453581895c4f13b2d73f0e7066ce125

#### Type of change

- New feature

#### Description

BFT Block Puller: verify attestation. 
Verify a block attestation, which is a block with block.Data=nil.
Verification is the same as verifying a regular block, except computing the data hash and comparing it to the hash in the header, and extracting the channel ID.

#### Related issues
#4240 
#4243 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 09:06:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4239" class=".btn">#4239</a>
            </td>
            <td>
                <b>
                    configtxgen - add a check for V3 style signature - BFT consensus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a check for V3 style signature - BFT consensus

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Related issues

Issue: #4228 .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-28 15:55:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4238" class=".btn">#4238</a>
            </td>
            <td>
                <b>
                    system channel cleanup - configtxgen document system channel no longer supported
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                configtxgen - document system channel no longer supported

#### Type of change

- Test update
- Documentation update

#### Related issues

Issue: #4211 .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-28 12:18:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4237" class=".btn">#4237</a>
            </td>
            <td>
                <b>
                    Fixes #4180 peer chaincode error message formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix #4180

#### Description

Uses proto.MarshalTextString to insert the protocol buffer response message into the error string

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 23:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4236" class=".btn">#4236</a>
            </td>
            <td>
                <b>
                    delete unnecessary preallocated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is no need to exceed the memory allocation.
Because more items can be added than you have allocated.
It is misleading.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 14:32:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4235" class=".btn">#4235</a>
            </td>
            <td>
                <b>
                    Method AppRootCAsByChain() not thread safe
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

As described in issue #4233 

#### Related issues

issue: #4233 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 14:03:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4234" class=".btn">#4234</a>
            </td>
            <td>
                <b>
                    Improved sentences
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
        Created At 2023-05-24 12:07:46 +0000 UTC
    </div>
</div>

