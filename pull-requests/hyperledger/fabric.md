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
                PR <a href="https://github.com/hyperledger/fabric/pull/3093" class=".btn">#3093</a>
            </td>
            <td>
                <b>
                    Randomize endorsement layouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry pick of https://github.com/hyperledger/fabric/commit/7c736c44b5b9d2ba4d64d148a8fca2be2bb59341 from main branch

For improved load balancing and fairer workload distribution across organizations, then gateway should randomize the endorsement layouts

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 08:43:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3092" class=".btn">#3092</a>
            </td>
            <td>
                <b>
                    Create HashedIndex in Pvtdata Store retroactively
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: manish <manish.sethi@gmail.com>

- Add functions in the pvtdata store package that would be used for creating the HashedIndex in Pvtdata Store retroactively.
- We use this opportunity to upgrade the data format from V11 to V12, so we can simplify the reading code in the future releases.
- Small refactoring is included to simplify the usage of update batch.

#### Type of change
- New feature

#### Related issues
- [RFC](https://github.com/hyperledger/fabric-rfcs/blob/main/text/0000-private_data_purge.md)
- [Issue](https://github.com/hyperledger/fabric/issues/3022) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 20:49:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3091" class=".btn">#3091</a>
            </td>
            <td>
                <b>
                    Final peer for gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peers topic for new gateway service, updates following WebEx with @andrew-coleman 

#### Type of change

- New feature
- Documentation update

#### Description

gateway service running on peers in Fabric v2.4

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 16:43:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3090" class=".btn">#3090</a>
            </td>
            <td>
                <b>
                    Final network orderers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Final doc for Networks and Orderers, following WebEx with @andrew-coleman

#### Type of change

- New feature
- Documentation update

#### Description

Updates for the gateway service now managing Tx proposals and endorsements.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 16:13:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3089" class=".btn">#3089</a>
            </td>
            <td>
                <b>
                    Randomize endorsement layouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For improved load balancing and fairer workload distribution across organizations, then gateway should randomize the endorsement layouts

Resolves https://github.com/hyperledger/fabric-gateway/issues/338

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 11:58:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3088" class=".btn">#3088</a>
            </td>
            <td>
                <b>
                    Corrected container names in commercial paper tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Corrected container names in commercial paper tutorial

#### Type of change

- Documentation update

#### Description
Corrected container names in commercial paper tutorial. The container names for Org1 and Org2 were swapped with each other.

Signed-off-by: Nidhi Singh <nidhi2894@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 11:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3087" class=".btn">#3087</a>
            </td>
            <td>
                <b>
                    Add command reference doc for ledgerutil
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add command reference doc for ledgerutil.
Includes minor edits to the command's user messages.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 17:10:01 +0000 UTC
    </div>
</div>

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
                PR <a href="https://github.com/hyperledger/fabric/pull/3078" class=".btn">#3078</a>
            </td>
            <td>
                <b>
                    Release commit for v2.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add What's New for v2.4.0.
Update install doc and scripts for v2.4.0.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 15:37:29 +0000 UTC
    </div>
</div>

