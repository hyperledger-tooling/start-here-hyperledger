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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4232" class=".btn">#4232</a>
            </td>
            <td>
                <b>
                    WIP: BFT: orderer can deliver header+sigs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                


Change-Id: I47e9767e7f322145291a8ffa498500ee99714cc6


#### Type of change

- New feature

#### Description
When the SeekInfo message SeekContentType is HEADER_WITH_SIGS, send a block with nil block.data.


#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 11:41:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4231" class=".btn">#4231</a>
            </td>
            <td>
                <b>
                    test that a join block does not define a system channel by verifying consortiums
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

Addition of an integration test to validate that when channel participation receives a join block, this block does not define a system channel

#### Related issues

issue: #4019 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 17:02:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4230" class=".btn">#4230</a>
            </td>
            <td>
                <b>
                    system channel cleanup - cleanup docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removal of system channel from docs.

#### Type of change

- Documentation update

#### Description

Removal of system channel from docs.

#### Related issues

Issue: #4211 .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 10:31:40 +0000 UTC
    </div>
</div>

