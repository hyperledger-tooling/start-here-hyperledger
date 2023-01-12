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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Cancel existing workflows for the current PR on a new push (release-2.2)
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
        Created At 2023-01-12 14:00:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/640" class=".btn">#640</a>
            </td>
            <td>
                <b>
                    Cancel existing workflows for the current PR on a new push
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
        Created At 2023-01-12 11:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/639" class=".btn">#639</a>
            </td>
            <td>
                <b>
                    Fix scheduled build workflow syntax error
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
        Created At 2023-01-12 10:44:24 +0000 UTC
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

