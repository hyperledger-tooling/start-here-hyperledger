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
                PR <a href="https://github.com/hyperledger/fabric/pull/3038" class=".btn">#3038</a>
            </td>
            <td>
                <b>
                    Reword evaluate() error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When no suitable peers are available to evaluate a transaction, the registry returns an error.  The message should be reworded to make clear it is being used for evaluation rather than endorsement.

Resolves https://github.com/hyperledger/fabric-gateway/issues/282

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 13:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3037" class=".btn">#3037</a>
            </td>
            <td>
                <b>
                    no gateway via cli - tutorials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

The new Fabric Gateway peer function is being documented, but the CLI cannot yet access the gateway peer. So these tutorials which call the `peer chaincode invoke` command need a mention of the requirement to still specify all endorsement peers. 

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

https://github.com/hyperledger/fabric/issues/2807

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
        Created At 2021-11-09 21:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    Add extra info to error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When processing an endorsement plan, failure to connect to remote peers could lead to an error saying there aren’t enough endorsers to satisfy the policy.  This commit add the list of peers that failed to commit.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 17:48:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    Use correct timeout option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway’s endpoint connection factory is currently using the EndorsementTimeout option when making connections.  It should be using the DialTimeout.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 13:34:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3031" class=".btn">#3031</a>
            </td>
            <td>
                <b>
                    ProposalResponse error should return error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A transaction proposal can fail for two reasons:
1) The chaincode return an error (status 500) response
2) Some infrastructure error occurs or error generated in the peer.

For case (1), the ProcessProposal() function will return the ProposalResponse and a nil error.
For case (2), most error paths return both a newly generated status 500 response and the error.  There is one path though (the one that invokes the simulateProposal) that just returns a status 500 response, but a nil error.
This means that client applications (via SDKs or Gateway) cannot destinguish between chaincode raised errors (case 1) and infrastructure errors (case 2).  This is a problem for the gateway which needs to destinguish these two situations in its retry logic.

This commit fixes this by returning the original error (instead of nil) as well as the generated ProposalResponse for this error path.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 13:18:54 +0000 UTC
    </div>
</div>

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

