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
                PR <a href="https://github.com/hyperledger/fabric/pull/4441" class=".btn">#4441</a>
            </td>
            <td>
                <b>
                    fix network diagrams R4 error (#4436)
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

I've fixed 4 diagrams on network page in documentation based on @satota2's suggestion.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 16:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4440" class=".btn">#4440</a>
            </td>
            <td>
                <b>
                    smart BFT GRPC leader sends proposal to follower test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                SmartBFT integration test:
The leader is using GRPC to send a proposal to the follower, checking that the signature validation is correct.

#### Type of change

- Test update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 12:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4438" class=".btn">#4438</a>
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

1. a flaw in the behavior of the smartbft library
2. gateway was only for raft

Both reasons are fixed now.
But a test that showed this error would be nice to add.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 17:28:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4437" class=".btn">#4437</a>
            </td>
            <td>
                <b>
                    add channel to log and refactor code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Delivery is done within a channel. 
In the logs in these places it is very lacking to specify for which channel the delivery is done 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 04:45:49 +0000 UTC
    </div>
</div>

