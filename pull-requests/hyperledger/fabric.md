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
                PR <a href="https://github.com/hyperledger/fabric/pull/4438" class=".btn">#4438</a>
            </td>
            <td>
                <b>
                    add integration test in which the smartbft leader must freeze,
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                waiting for an answer.

There was a case where the leader froze up and the followers couldn't change him. 
There were two reasons for this:

1. a flaw in the behavior of the smartbft library
2. gateway was only for raft

Both reasons are fixed now.
But a test that showed this error would be nice to add.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 17:28:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4437" class=".btn">#4437</a>
            </td>
            <td>
                <b>
                    add channel to log and refactor code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Delivery is done within a channel. 
In the logs in these places it is very lacking to specify for which channel the delivery is done 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 04:45:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4435" class=".btn">#4435</a>
            </td>
            <td>
                <b>
                    Bump Fabric CA to 1.5.7
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

- Improvement (improvement to code, performance, etc)
- Documentation

#### Description

This patch bumps Fabric CA to 1.5.7 in scripts.

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
        Created At 2023-09-08 00:59:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4434" class=".btn">#4434</a>
            </td>
            <td>
                <b>
                    add docs for smartbft metrics
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
        Created At 2023-09-07 18:13:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4433" class=".btn">#4433</a>
            </td>
            <td>
                <b>
                    Document chaincode upgrade impact on state data (backport #4432)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4432 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 15:31:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4432" class=".btn">#4432</a>
            </td>
            <td>
                <b>
                    Document chaincode upgrade impact on state data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document chaincode upgrade impact on state data.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 13:51:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4431" class=".btn">#4431</a>
            </td>
            <td>
                <b>
                    Bft bp deliveryclient censorshiptimeout 2
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
        Created At 2023-09-07 09:28:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4430" class=".btn">#4430</a>
            </td>
            <td>
                <b>
                    smart BFT GRPC broadcasting invalid TX to leader test
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

Test that invalid TX broadcast to the leader is failing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:48:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4429" class=".btn">#4429</a>
            </td>
            <td>
                <b>
                    Smart BFT GRPC forwarding invalid message test
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

A test to check that if an orderer is forwarding to the leader an invalid TX, the operation should fail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:45:54 +0000 UTC
    </div>
</div>

