---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3026" class=".btn">#3026</a>
            </td>
            <td>
                <b>
                    fix: wallet present proof fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixed issue where wallet is only relying parent thread id of present
proof V2

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 15:50:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3024" class=".btn">#3024</a>
            </td>
            <td>
                <b>
                    DIDComm v2 Messaging without DIDExchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Outbound Dispatcher SendToDID can now create a default connection, if a connection doesn't yet exist, allowing didcomm V2 protocols to operate without DIDExchange, as long as the recipient DID can be resolved (ie, public or otherwise previously provided to the agent).

Also fixes connection Recorder/Lookup so it makes only one database read instead of two, when fetching a record by DIDs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 18:55:10 +0000 UTC
    </div>
</div>

