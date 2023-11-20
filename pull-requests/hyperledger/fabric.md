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
                PR <a href="https://github.com/hyperledger/fabric/pull/4548" class=".btn">#4548</a>
            </td>
            <td>
                <b>
                    Remove legacy chaincode deploy from snapshot integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit takes care to remove deprecate legacy chaincode deploy from the ledger snapshot integration test.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-19 23:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4547" class=".btn">#4547</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.4

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 21:12:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4545" class=".btn">#4545</a>
            </td>
            <td>
                <b>
                    add integration test in which the smartbft leader must freeze,
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                waiting for an answer.

There was a case where the leader froze up and the followers couldn't change him.
There were two reasons for this:

a flaw in the behavior of the smartbft library
gateway was only for raft
Both reasons are fixed now.
But a test that showed this error would be nice to add.

For some reason, https://github.com/hyperledger/fabric/pull/4438 conflicts with main.
Second, clean attempt.

@C0rWin FYI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 11:38:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4544" class=".btn">#4544</a>
            </td>
            <td>
                <b>
                    Doc improvement - Chaincode access control
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clarify chaincode access control and add link to
client identity library APIs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 06:02:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4543" class=".btn">#4543</a>
            </td>
            <td>
                <b>
                    Improve the compare logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I3d86e409e8aafb013cd289809b1b6a1d26ccc6b6

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Use plain compare to clear the logic.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 23:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4542" class=".btn">#4542</a>
            </td>
            <td>
                <b>
                    Block deliverer test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Type of change : Test update
Description: The test aims to create an environment that emulates the behavior of a malicious orderer.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 19:34:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4541" class=".btn">#4541</a>
            </td>
            <td>
                <b>
                    Fix compilation break in main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix compilation break caused by conflicting commits.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 18:57:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4539" class=".btn">#4539</a>
            </td>
            <td>
                <b>
                    Bump github.com/IBM/idemix and github.com/consensys/gnark-crypto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/IBM/idemix to get updated github.com/consensys/gnark-crypto.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 18:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4537" class=".btn">#4537</a>
            </td>
            <td>
                <b>
                    Docs - Update legacy SDK references to Gateway SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This documentation change updates many of the remaining references to the legacy SDKs, and replaces them with Gateway SDK references where applicable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 04:37:06 +0000 UTC
    </div>
</div>

