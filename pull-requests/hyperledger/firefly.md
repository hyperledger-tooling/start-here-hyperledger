---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Config map length fix, fix bug with missing events by closing the websocket
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
        Created At 2021-12-23 19:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/365" class=".btn">#365</a>
            </td>
            <td>
                <b>
                    Validate message topics/tag before sending
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently these fields are verified only by the receiver, which can lead to
sending a bad message that is rejected on the other end.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 19:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/364" class=".btn">#364</a>
            </td>
            <td>
                <b>
                    Update manifest ready for v0.11.3 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 22:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/363" class=".btn">#363</a>
            </td>
            <td>
                <b>
                    Fix send-to-self for private messages, and add group query URLs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I noticed that when I was only sending to myself, I was still getting data being pushed by FireFly core to DX.

Looks like when we made the identity change to introduce DIDs, we broke the code here:
https://github.com/hyperledger/firefly/blob/24d075b4ec5b08601780ebac04fefc61aebbd427/internal/privatemessaging/privatemessaging.go#L188-L191

Also @hfuss mentioned to me that we've seen problems where the config has to have the full Key specification exactly as it gets resolved by the blockchain connector (so `0x` prefix for ethereum, and the full `CN=xyz...` syntax for fabric), or things do not work correctly.

This PR:
- Ensures we always use the blockchain connector to get the resolved signing key
- Compares `Owner` of a `Node` to the signing key of the local org, not the DID
- Adds APIs to query groups, which seemed to be missing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 19:52:26 +0000 UTC
    </div>
</div>

