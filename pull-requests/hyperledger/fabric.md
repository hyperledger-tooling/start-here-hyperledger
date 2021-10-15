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
                PR <a href="https://github.com/hyperledger/fabric/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    Gateway endorsement retry logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than selecting one layout from the discovery endorsement plan and failing if one of the endorsers fails, this commit attempts to create a set of endorsements by retrying the proposal on other endorser until one of the layouts is satisfied.
Additionally, rather than connect to all peers in a channel once on first usage and then never update that cache, this commit adds support for later additions and removals to/from the cache and closing stale connections to peers.

Resolves #2914 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 15:20:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2982" class=".btn">#2982</a>
            </td>
            <td>
                <b>
                    Extra info in log message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the transaction ID and the orderer endpoint address to the log message before sending the transaction to the orderer.

Resolves https://github.com/hyperledger/fabric-gateway/issues/250

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 07:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2981" class=".btn">#2981</a>
            </td>
            <td>
                <b>
                    Add `calculatepackageid` command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch `calculatepackageid` command to calculate the package ID for a packaged chaincode rather than an installed chaincode.

#### Type of change

- New feature

#### Description

This patch `calculatepackageid` command to calculate the package ID for a packaged chaincode rather than an installed chaincode.

The new command will be useful, for example, the following cases:
* When multiple chaincode packages with the same label name are installed,
it is possible to identify which ID corresponds to which package later.
* To check whether a particular chaincode package is installed or not on a peer
without installing that package.

#### Additional details

After this patch is merged, I'm going to submit the following related patches as separate PRs in sequence:

- For the integration tests:
  - https://github.com/satota2/fabric/commit/666a5ca4b941ee92c2da665d619c43df9350399d

#### Related issues

- https://github.com/hyperledger/fabric/issues/2976
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 04:21:58 +0000 UTC
    </div>
</div>

