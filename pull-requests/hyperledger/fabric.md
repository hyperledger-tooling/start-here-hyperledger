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
                PR <a href="https://github.com/hyperledger/fabric/pull/3085" class=".btn">#3085</a>
            </td>
            <td>
                <b>
                    Add read version to the example in read-write set
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


Per discussion, we want to add read version to the example in read-write set so that

1. the read version described in the earlier description appears in this example.
2. show readers clearly that a transaction is rejected due to read version mismatch.

#### Related issues

Fixes #3015 

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
        Created At 2021-11-29 08:16:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3083" class=".btn">#3083</a>
            </td>
            <td>
                <b>
                    Clarify v2.x upgrade docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Combine the v2.x to v2.x instructions in a single section.

For v1.x to v2.x, clarify which steps should occur prior to updating peers,
while updating peers, and after updating peers, by adding a section header for each.

Finally, clarify that existing chaincodes will automatically shift from old lifecycle framework
to new lifecycle framework upon the first install/approve/commit after enabling the
v2.x lifecycle (i.e., after updating the V2_0 application capability).

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 02:56:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3082" class=".btn">#3082</a>
            </td>
            <td>
                <b>
                    Update v2.4.0 release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update v2.4.0 release notes

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 01:59:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3080" class=".btn">#3080</a>
            </td>
            <td>
                <b>
                    Other key concepts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature
- Documentation update

#### Description

Other Key Concepts - Network and Ordering Service topics for gateway

#### Related issues

https://github.com/hyperledger/fabric/issues/2807 
- Other Key Concepts items


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 23:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3079" class=".btn">#3079</a>
            </td>
            <td>
                <b>
                    Peers for Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

Final review of Peers page/topic for Fabric Gateway GA

#### Type of change

- New feature
- Documentation update

#### Description

Fabric Gateway service - new model for peers and apps for transaction proposals and endorsements.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-27 20:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3078" class=".btn">#3078</a>
            </td>
            <td>
                <b>
                    What's New for v2.4.0 doc topic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add What's New for v2.4.0

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 15:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    Refine Gateway gRPC error status codes
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
        Created At 2021-11-23 16:34:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3074" class=".btn">#3074</a>
            </td>
            <td>
                <b>
                    EndorsementTimeout should apply to each endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently the options.EndorsementTimeout creates a context that is shared by all endorsement requests in the Endose() and Evaluate() methods.
This commit changes it so It is applied individually to each endorsing peer.
The overall timeout for Endorse/Evaluate is set in the client SDK

Resolves https://github.com/hyperledger/fabric-gateway/issues/292

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 14:15:06 +0000 UTC
    </div>
</div>

