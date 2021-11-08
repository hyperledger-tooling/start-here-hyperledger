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
                PR <a href="https://github.com/hyperledger/fabric/pull/3019" class=".btn">#3019</a>
            </td>
            <td>
                <b>
                    docs: fix typo in comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
 * Documentation update
 
#### Description
This change fixes a typo in a comment in `main/common/ledger/blkstorage/blockfile_mgr.go`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 03:48:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3017" class=".btn">#3017</a>
            </td>
            <td>
                <b>
                    Better gRPC error on context error from CommitStatus service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than always return a FailedPrecondition error on failure obtaining commit status, return either a DeadlineExceeded or Canceled error on a context error. This may happen if the call is cancelled from the client end, either by an explicit context cancel or timeout.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 18:13:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3016" class=".btn">#3016</a>
            </td>
            <td>
                <b>
                    Fix typo in comment
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

This change fixes a typo in a comment in `gossip/privdata/pvtdataprovider.go`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 12:37:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3013" class=".btn">#3013</a>
            </td>
            <td>
                <b>
                    Add chaincode err message to Evaluate err message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a previous commit which implemented retry logic for the evaluate method, the error(s) produced by remote endorsers were added to the Details field of the gateway error with a generic error message at the top level.
In the case of a proposal response containing a chaincode generated error, no retry is performed and so the error message should also be at the top level (as it used to be before that earlier commit).

This commit adds the chaincode error message back into the message returned by the gateway, and will restore the behaviour expected by the scenario tests in the SDKs.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 16:33:01 +0000 UTC
    </div>
</div>

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

> Error: could not assemble transaction: ProposalResponsePayloads do not match with version:1 response:<status:200 payload:"true" > payload:"\n \265\277\020\265\226D\035\361\001n\371K\013\274\021F\227\002?\261\204\370\327\363r\347\010\221\313\214\031\230\022\230\001\n|\0227\n\n_lifecycle\022)\n'\n..." endorsement:<endorser:"\n\007Org1MSP\022\252\006-----BEGIN CERTIFICATE-----\nMIICKDCCAc6gAwIBAgIQEO..." signature:"0E\002!\000\331p\034A\353t\261{\026#\177\211\371g\232\213\331\323\..." >
> &#45; proposal response: version:1 response:<status:200 payload:"true" > payload:"\n \265\277\020\265\226D\035\361\001n\371K\013\274\021F\227\002?\261\204\370\327\363r\347\010\221\313\214\031\230\022\213\001\no\0227\n\n_lifecycle\022)\n'..." endorsement:<endorser:"\n\007Org2MSP\022\252\006-----BEGIN CERTIFICATE-----\nMIICKDCCAc+gA..." signature:"0D\002 J\\\300\307~\350\236\026\245H\003\337\2732\020\312\n\017Fa\306~\367x\356\347K\225\..." > 


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
                <span class="chip">docs</span>
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

