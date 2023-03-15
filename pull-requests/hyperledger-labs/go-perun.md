---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/389" class=".btn">#389</a>
            </td>
            <td>
                <b>
                    Grant access to SignedState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new channel wrapper `TransparentChannel` that grants access to the channel's `SignedState`.

In the context of light clients using the Perun WebSocket, the ability to send them the signed state of their channel as a backup allows the light clients to register the channel on-chain even if the WebSocket should be offline.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 14:07:04 +0000 UTC
    </div>
</div>

