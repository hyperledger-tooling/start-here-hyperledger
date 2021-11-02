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
                PR <a href="https://github.com/hyperledger/fabric/pull/3012" class=".btn">#3012</a>
            </td>
            <td>
                <b>
                    Show what do not match
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: gqqnbig <gqqnb2005@gmail.com>

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

When  `peer chaincode invoke`  submits a request, if chaincode has bugs, it may return different responses on different nodes.

Before, the error message is like

> Error: could not assemble transaction: ProposalResponsePayloads do not match  - proposal response: version:1 response:<status:200 payload:"true" > payload:"\n \265\277\020\265\226D\035\361\001n\371K\013\274\021F\227\002?\261\204\370\327\363r\347\010\221\313\214\031\230\022\213\001\no\0227\n\n_lifecycle\022)\n'..." endorsement:<endorser:"\n\007Org2MSP\022\252\006-----BEGIN CERTIFICATE-----\nMIICKDCCAc+gA..." signature:"0D\002 J\\\300\307~\350\236\026\245H\003\337\2732\020\312\n\017Fa\306~\367x\356\347K\225\..." > 

That is it. Developers have no idea what mismatch what.

Now, with this PR, the error message is like 

> Error: could not assemble transaction: ProposalResponsePayloads do not match with version:1 response:<status:200 payload:"true" > payload:"\n \265\277\020\265\226D\035\361\001n\371K\013\274\021F\227\002?\261\204\370\327\363r\347\010\221\313\214\031\230\022\230\001\n|\0227\n\n_lifecycle\022)\n'\n..." endorsement:<endorser:"\n\007Org1MSP\022\252\006-----BEGIN CERTIFICATE-----\nMIICKDCCAc6gAwIBAgIQEO..." signature:"0E\002!\000\331p\034A\353t\261{\026#\177\211\371g\232\213\331\323\..." > - proposal response: version:1 response:<status:200 payload:"true" > payload:"\n \265\277\020\265\226D\035\361\001n\371K\013\274\021F\227\002?\261\204\370\327\363r\347\010\221\313\214\031\230\022\213\001\no\0227\n\n_lifecycle\022)\n'..." endorsement:<endorser:"\n\007Org2MSP\022\252\006-----BEGIN CERTIFICATE-----\nMIICKDCCAc+gA..." signature:"0D\002 J\\\300\307~\350\236\026\245H\003\337\2732\020\312\n\017Fa\306~\367x\356\347K\225\..." > 


With this error message, developers can use text comparison tools to find out where the two responses start to differ, and they may get some cues.


Technically, only the payload part needs to be displayed, but I don't know how to format bytes as the toString method of  ProposalResponse does.

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
        Created At 2021-11-02 11:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3011" class=".btn">#3011</a>
            </td>
            <td>
                <b>
                    Update Sphinx to v1.8.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A recent commit updated the doc generation tool, sphinx, from v1.7.2 to v1.8.0.  However, this broke the ability to generate and review the docs from a forked branch.
This is due to a known bug in Sphinx which was fixed on v1.8.2 (https://github.com/sphinx-doc/sphinx/issues/5519).
This commit updates the dependency to this version.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 10:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3010" class=".btn">#3010</a>
            </td>
            <td>
                <b>
                    Update transaction flow doc for peer gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update transaction flow doc for the new v2.4 flow with the peer gateway.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 10:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3009" class=".btn">#3009</a>
            </td>
            <td>
                <b>
                    Improve output formats of calculatepackageid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR improves the output formats of `calculatepackageid` command.

#### Type of change
- New feature
- Documentation update

#### Description

This patch removes the prefix from the output format of calculatepackageid.
With this patch, the command returns only the package ID by default.

Also, this PR adds an output option for `calculatepackageid` command:
- `-O json`: to output as JSON format

#### Additional details

#### Related issues
- https://github.com/hyperledger/fabric/issues/2976

#### Related PRs
- https://github.com/hyperledger/fabric/pull/2981

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 00:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3008" class=".btn">#3008</a>
            </td>
            <td>
                <b>
                    Add gateway architecture page to docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #2807 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 17:55:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3007" class=".btn">#3007</a>
            </td>
            <td>
                <b>
                    Reword duplicate error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are two error paths that produce the same message.  Reword the second one to a more acurate description of the problem.

Resolves https://github.com/hyperledger/fabric-gateway/issues/271

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 13:45:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3006" class=".btn">#3006</a>
            </td>
            <td>
                <b>
                    Add logging for identity, policy, and signature troubleshooting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Most identity, policy, and signature issues return a fairly generic error
message to the user, e.g. "not authorized".
This is often intentional so as to not disclose information to malicious users that
may be probing for information about the system.

This commit adds logging on the orderer and peer side so that identity issues
can more easily be troubleshooted by users setting up sample networks,
and by administrators and SREs in production networks.

For any identity, policy, or signature error, the identity is now logged in a warning message.
Additionally, the identity of every signature that is verified can be seen if tracing is enabled.

The new logging can help with the following types of issue resolution:
User cert and MSP membership errors
Determine which user is unauthorized to perform an action
Determine which MSPs and user signatures are included in a config transaction that was invalidated
Determine which peers participated in an endorsement invalidation
Determine which peer signature doesn't match the others in a proposal response

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 12:15:19 +0000 UTC
    </div>
</div>

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

