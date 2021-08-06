---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Handle spurious acks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently there are two cases where the ack processing can get stuck:
- An application sends a spurious additional ack
  - The WS code tries to deliver this to the eventstream code, while the ES code is trying to wait for a message
  - Eventually results in `We were not available to process it after ... seconds` in the logs
- The ES code receives an update to the eventstream, while it's waiting for an ack
  - This results in the WS code never being able to deliver the ack, so never delivering the next message

The proposed change in this PR adds a buffer of 1 to the channel between the WS and ES code, and changes the timeout into a `default` when delivering the ack. This prevents the deadlock possibility. There are always either `0` or `1` acks in the pipe.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 19:01:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/135" class=".btn">#135</a>
            </td>
            <td>
                <b>
                    Avoid panic on concurrent stream update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #134
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 20:38:08 +0000 UTC
    </div>
</div>

