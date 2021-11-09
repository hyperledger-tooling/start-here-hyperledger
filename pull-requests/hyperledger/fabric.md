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

