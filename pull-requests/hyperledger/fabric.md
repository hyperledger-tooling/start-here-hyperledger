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
                PR <a href="https://github.com/hyperledger/fabric/pull/4551" class=".btn">#4551</a>
            </td>
            <td>
                <b>
                    Return the struct directly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I3e1622c0c7ee144c3164cecc49f5cf6d75b9ec32

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

No need to create an empty struct and then fill in the data.

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
        Created At 2023-11-20 22:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4550" class=".btn">#4550</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: verifier in the monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- New feature

#### Description

Integration of the stand alone verifier with the censorship monitor.


#### Related issues
#4353 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 16:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4549" class=".btn">#4549</a>
            </td>
            <td>
                <b>
                    migration raft2bft - WIP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

This PR aims to update the migration test. The goal is to migrate from Raft to BFT.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 10:00:26 +0000 UTC
    </div>
</div>

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

