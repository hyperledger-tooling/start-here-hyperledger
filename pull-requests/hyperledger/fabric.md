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
                PR <a href="https://github.com/hyperledger/fabric/pull/3005" class=".btn">#3005</a>
            </td>
            <td>
                <b>
                    Add integration tests for `calculatepackageid` command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds integration tests for `calculatepackageid` command.

#### Type of change

- Test update

#### Description

This patch adds integration tests for `calculatepackageid` command.

#### Additional details

#### Related issues

- https://github.com/hyperledger/fabric/issues/2976
- https://github.com/hyperledger/fabric/pull/2981
 
After this PR is merged, I'm going to submit some patches to add some output options as a separate PR in sequence.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 16:44:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3004" class=".btn">#3004</a>
            </td>
            <td>
                <b>
                    Don’t close connection if already closing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a peer is shutdown, if the gateway attempts to send a proposal to it, it will fail and the gateway will close the connection and remove it from its registry.
Under stress, with multiple concurrent goroutines all attempting to use and then close the connection, the log gets flooded with the messages:
- (INFO) Attempting to close
- (ERROR) Failed to close.

This commit changes the behaviour so that it checks the grpc state before logging and attempting to close.  If it’s already shutting down, then it’s a no-op.

Resolves https://github.com/hyperledger/fabric-gateway/issues/265

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 15:00:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3002" class=".btn">#3002</a>
            </td>
            <td>
                <b>
                    Add explanation of stringArray (--peerAddresses)
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

I searched the documentations but didn't find they explain stringArray. 

I looked at the source code of github.com/spf13/pflag and guess I should use

 `--peerAddresses localhost:9051--peerAddresses localhost:7051` rather than `--peerAddresses "localhost:9051
localhost:7051"`.

I think this information should be added to the docs.


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
        Created At 2021-10-29 02:31:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3000" class=".btn">#3000</a>
            </td>
            <td>
                <b>
                    Move to better IsAbs Implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #2998 

Signed-off-by: D <d_kelsey@uk.ibm.com>


- Bug fix

#### Description

path.IsAbs is a poor implementation in Go, filepath.IsAbs looks to be much better 
and addresses the problem where a windows absolute path is not recognised


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 08:42:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2999" class=".btn">#2999</a>
            </td>
            <td>
                <b>
                    Retry logic for evaluate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify the evaluate method to retry processing of a transaction proposal on another peer in the case of an error.

resolves #2913 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2997" class=".btn">#2997</a>
            </td>
            <td>
                <b>
                    Protobuf and etcd upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Update protobuf and etcd to their latest versions.

#### Additional details

This is a reprisal of the work on updating protobuf by #2185

#### Related issues

FAB-18363


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 15:57:35 +0000 UTC
    </div>
</div>

