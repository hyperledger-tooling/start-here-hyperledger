---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5628" class=".btn">#5628</a>
            </td>
            <td>
                <b>
                    Make fork id the default and try to recover the DiscoveryPeer for incoming connections from the PeerTable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR introduces these changes:
- Make "--filter-on-enr-fork-id" default to true. That means that Besu by default will request the ENR from peers it has bonded with, which usually contains the fork id. The fork id then is used to find out whether that peer is on the same chain.
- When other peers are initiating a handshake with us we now will check our PeerTable to see whether we have bonded with that peer. If the peer is found in the PeerTable we can check if the fork id is available to find out whether that peer is on the same chain.

Only if the fork id indicates that the peer is on the same chain we will try to establish a connection with that peer.

## Fixed Issue(s)
#5272 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 07:01:49 +0000 UTC
    </div>
</div>

