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
                PR <a href="https://github.com/hyperledger/fabric/pull/2607" class=".btn">#2607</a>
            </td>
            <td>
                <b>
                    Updated setting up environment documentation to reflect "brew cask" no longer being a valid command
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

Replaced "brew cask install --appdir=“/Applications” docker" with "brew install --cask docker"

Cask is no longer a brew command. When you want to install a Cask, you just do brew install or brew install --cask instead of brew cask install.

#### Additional details

N/A

#### Related issues

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2606" class=".btn">#2606</a>
            </td>
            <td>
                <b>
                    Optionally disable gossip block forwarding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds a new configuration option to the peer which makes peers
not forward blocks that they pull from the ordering service.

If all peers in an organization explictly set "peer.deliveryclient.blockGossipEnabled" to false, 
no peer in the organization gossips blocks to any other peer in that organization.

Change-Id: I5d9b278ae72f239129827c044fa78179f6ba87ab
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:11:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2604" class=".btn">#2604</a>
            </td>
            <td>
                <b>
                    FABGW-21: Return block number in CommitStatusResponse
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor Gateway's CommitStatus service in line with updated protobufs, so the returned CommitStatusResponse message includes the block number in which the transaction committed. This required a refactor to the commit finder implementation and a switch from Counterfeiter to Mockery as the mocking framework for that package due to cyclic import limitations with Counterfeiter.

First step towards implementing chaincode event listening. A dummy implementation of that service that returns an error is included.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 17:42:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    Fixed JIRA issue FLY2- 64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have updated chain.go  Submit and ordered method..

#Fixed FLY2-64
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 09:36:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2601" class=".btn">#2601</a>
            </td>
            <td>
                <b>
                    Maintain order of transactions in the commit notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Maintain order of transactions in the commit notification so the gateway can deliver the clients the chaincode events in the same and consistent order.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 18:21:07 +0000 UTC
    </div>
</div>

