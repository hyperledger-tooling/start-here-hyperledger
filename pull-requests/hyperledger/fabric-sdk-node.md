---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/638" class=".btn">#638</a>
            </td>
            <td>
                <b>
                    Fix chaincode dependencies to v2.2.x in test fixtures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                v2.5.x introduced some changes that broke the tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 11:38:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/637" class=".btn">#637</a>
            </td>
            <td>
                <b>
                    Reduce reliance on exact error message text in scenario tests (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some testing of error scenarios checked for exact error message text produced by Fabric and/or the chaincode runtime, which are outside the scope of control of the SDK and failed when the text of those messages changed slightly. This change minimises the checking to text that should either be reasonably expected to be included in the runtime error message, or is produced by the smart contract used for testing and can therefore be relied on.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 17:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    Decompose build into reusable workflows (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This enables scheduled builds to be run across multiple branches while keeping the build logic local to each branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 17:40:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    Scheduled build matrix for main and release-2.2 branches
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Decompose build into a reusable GitHub Actions workflows to facilitate matrix build across multiple branches.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 17:10:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    Reduce reliance on exact error message text in scenario tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some testing of error scenarios checked for exact error message text produced by Fabric and/or the chaincode runtime, which are outside the scope of control of the SDK and failed when the text of those messages changed slightly. This change minimises the checking to text that should either be reasonably expected to be included in the runtime error message, or is produced by the smart contract used for testing and can therefore be relied on.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 16:19:24 +0000 UTC
    </div>
</div>

