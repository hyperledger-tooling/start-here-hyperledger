---
layout: default
title: Scorex
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/Scorex
---

# Scorex <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/Scorex){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/Scorex/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    fixing PeerConnectionHandler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Problem: false positive peer bans, ie. peers are getting banned even though they communicate properly.

Explanation: 
Logic of this whole incoming data deserialization is as follows : 
 1. ByteString is received 
 2. if length properties don't comply with full message length, keep on reading next ByteString as we have not enough bytes yet
 3. otherwise try to deserialize it into a message

The bug is caused by the fact that we are testing for `magic` and grabbing `msgCode` before checking the length, which means it fails (incorrectly) at time when not enough bytes is read to be able to deserialize it into a message.

Fix outcome: 
No bans happen now and more peers are connected, tested on Ergo.

The test failure is just a timeout, tests pass locally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 14:33:48 +0000 UTC
    </div>
</div>

