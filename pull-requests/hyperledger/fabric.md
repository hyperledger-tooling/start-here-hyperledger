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
                PR <a href="https://github.com/hyperledger/fabric/pull/4418" class=".btn">#4418</a>
            </td>
            <td>
                <b>
                    Whats New doc for v3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add What's New doc for v3.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 20:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4417" class=".btn">#4417</a>
            </td>
            <td>
                <b>
                    change submit bft
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/fabric/issues/4415
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 12:20:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4416" class=".btn">#4416</a>
            </td>
            <td>
                <b>
                    Change evaluation method in gateway.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since RAFT node is able to run with capability turned on, changed the gateway code to evaluate consensus type rather than evaluating channel capabilities.

#### Type of change
- Bug fix

#### Description
Since RAFT node is able to run with capability turned on, changed the gateway code to evaluate consensus type rather than evaluating channel capabilities.
Following that changed the [https://github.com/hyperledger/fabric/blob/main/internal/pkg/gateway/submit.go#L53](url) file to check the consensus type.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 11:40:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4414" class=".btn">#4414</a>
            </td>
            <td>
                <b>
                    [WIP] delete in test "Resubmitting the same transaction", …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ... but the test completes successfully

Illustration of gateway submit (broadcastToAll) malfunction returning an error when it should return success.
In my opinion, the broadcastToAll function is implemented incorrectly

https://github.com/hyperledger/fabric/issues/4415
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 11:18:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4413" class=".btn">#4413</a>
            </td>
            <td>
                <b>
                    Tutorial doc on test network with BFT ordering service
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

Since v3.0.0-preview users will be expected to be very interested in trying out the BFT ordering service,
I think it would be beneficial for the users to easily try its end-to-end operation, like other features (CouchDB, CCaaS, etc.).

This patch updates test_network.md:
- To update the network.sh help text output
- Add brief instructions for running a test network with BFT ordering service

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

- https://github.com/hyperledger/fabric/issues/4296
- https://github.com/hyperledger/fabric/issues/4332

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
        Created At 2023-08-30 08:57:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4412" class=".btn">#4412</a>
            </td>
            <td>
                <b>
                    Fix orderer endpoints in add_orderer.md
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

- Bug fix
- Documentation update

#### Description

This patch fixes orderer endpoints in add_orderer.md.


#### Additional details

#### Related PRs

https://github.com/hyperledger/fabric-samples/pull/1085

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 07:19:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4411" class=".btn">#4411</a>
            </td>
            <td>
                <b>
                    Fix occurring unexpected cert expiration warnings in orderer
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

This patch adds setting a cert's expireAt in RemoteContext so that checkExpiration() will not occur cert expiraration warnings that were not expected.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

https://github.com/hyperledger/fabric/issues/4404

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
        Created At 2023-08-30 06:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4410" class=".btn">#4410</a>
            </td>
            <td>
                <b>
                    Add BFT to ordering service overview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 00:24:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4409" class=".btn">#4409</a>
            </td>
            <td>
                <b>
                    Bft bp deliveryclient block censorship timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code)
- Test update


#### Description

As described in issue #4401 


#### Related issues

issue #4401 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 22:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4408" class=".btn">#4408</a>
            </td>
            <td>
                <b>
                     BFT Block Puller: a common block verifier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- New feature

#### Description
 BFT Block Puller: a common block verifier to the peer the orderer.

The new implementation verifies the integrity and signatures of a block stream, while keeping a copy of the latest configuration.

Every time a config block arrives, it must first be verified using VerifyBlock and then used as an argument to the UpdateConfig method.  

The block stream could be composed of either:

- full blocks, which are verified using the VerifyBlock method, or
- block attestations (a header+metadata, with nil data) which are verified using the VerifyBlockAttestation method.

In both cases, config blocks must arrive in full.

This commit also moved `BlockVerifierAssembler` form `orderer/common/cluster/util.go` to `common/deliverclient/verifier_assembler.go`, as it is now used by both orderer and peer. In addition, `VerificationRegistry` was removed from  `orderer/common/cluster/util.go`  as it is no longer in use.

#### Related issues

#4346 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 13:19:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4407" class=".btn">#4407</a>
            </td>
            <td>
                <b>
                    timestamp encoding bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #4406

#### Type of change

- Bug fix

#### Description

#4406
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 14:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4405" class=".btn">#4405</a>
            </td>
            <td>
                <b>
                    Update install scripts for v2.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix
- Documentation update

#### Description

Update install script and bootstrap script for v2.5.4.

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 05:20:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4402" class=".btn">#4402</a>
            </td>
            <td>
                <b>
                    CFT Block Puller: reset total sleep 
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

In internal/pkg/peer/blocksprovider/deliverer.go:150

Local variable `totalDuration` measures the total sleep during retries. If it exceeds `reconnectTotalTimeThreshold` the Deliverer may exit if `MaxRetryDurationExceededHandler` returns true. 

However, it does not reset on success (block reception), so `DeliverBlocks()` may exit eventually if the cumulative sleep time is large, but no consecutive reconnect failure sequence exceeds the threshold for stopping retries.

The solution is to reset `totalDuration` together when we reset `failureCounter`.


#### Related issues

Issue: #4394 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-27 11:56:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4398" class=".btn">#4398</a>
            </td>
            <td>
                <b>
                    up smartbft library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 05:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4397" class=".btn">#4397</a>
            </td>
            <td>
                <b>
                    Improve add_orderer.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates add_orderer.md to improve it from the user's perspective.

#### Type of change
- Documentation update

#### Description
I'm trying out the BFT samples in fabric-samples recently.
As part of this process, I also tried to add an orderer following the instructions in the doc added by https://github.com/hyperledger/fabric/pull/4390.

I've identified some areas from a user's perspective that might benefit from further improvements.
This PR updates add_orderer.md for the above improvements.

#### Other possible improvements, or points that were not clear after trying the procedure

- I interpreted that [such a file path description](https://github.com/hyperledger/fabric/blob/17b77cf1d8750263df89316cd0c888f18b872022/docs/source/create_channel/add_orderer.md?plain=1#L185) in Add the fifth orderer to the config should actually be filled in with the result of base64 encoding of the certificate in the file, but some readers may overlook it.
  - It may be less misleading to explicitly state in a snippet, such as `<The result of base64 encoding of the contents in ...>`.

- It might be more user-friendly if the command snippets for entering `cli` container and copying between cli and local were also illustrated in the doc.

#### Related issues
https://github.com/hyperledger/fabric/issues/4332

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 03:56:10 +0000 UTC
    </div>
</div>

