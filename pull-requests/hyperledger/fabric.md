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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2978" class=".btn">#2978</a>
            </td>
            <td>
                <b>
                    Improve health checker docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add more details about health checkers, including ability
to not register Docker health checker if using
external chaincode builders.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 14:34:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2977" class=".btn">#2977</a>
            </td>
            <td>
                <b>
                    Update developer environment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

Improve the setting up dev environment section

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 09:19:22 +0000 UTC
    </div>
</div>

