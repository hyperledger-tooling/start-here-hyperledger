---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1367" class=".btn">#1367</a>
            </td>
            <td>
                <b>
                    fix(anoncreds): Buffer not imported from core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Subtle omission that was causing `encodeCredentialValue` to fail under React Native.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 23:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1362" class=".btn">#1362</a>
            </td>
            <td>
                <b>
                    feat(indy-vdr)!: extend did:indy support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Same changes as in #1347, but now for indy-vdr.

It updates the anoncreds registry to support both legacy and did:indy identifiers.

There's one issue that needs to be resolved, but I'd like to do that in a separate PR, is that currently the code isn't set up in a way yet that we support using both did:indy and legacy identifiers in anoncreds for _issuance_. As the holder and verifier only do resolving, it works with both now. 

What still needs to be done:
- when a credential with legacy identifiers or vice versa is received, allow it to be shared as the other format. I want to store all credentials using the new did:indy identifiers, and we can optionally transform the identifiers to legacy when needed (in the credential/proof format services)
- creating an offer for legacy format as the record always stores using the did:indy format. I'd also like to handle this in the format services, so the storage / issuer/holder/verifier services always use the new formats. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 13:26:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1361" class=".btn">#1361</a>
            </td>
            <td>
                <b>
                    test: various improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a few improvements to the test setup that should hopefully prevent timeouts, but also make sure we test the askar setup:
- only run askar related tests in node18
- add ref-napi resolution in node18
- increase timeout for some packages that often timeout
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 13:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1359" class=".btn">#1359</a>
            </td>
            <td>
                <b>
                    fix(tenant): Correctly configure storage for multi tenant agents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes hyperledger/aries-framework-javascript#1353
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 12:36:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1356" class=".btn">#1356</a>
            </td>
            <td>
                <b>
                    fix(core): repository event when calling deleteById
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling Repository method `deleteById`, no `RecordEvent` event is emitted. This PR fixes this by emitting the Event with the information we have about the record: its id and type. This makes the event suitable for filtering in handlers used in hooks. The limitation, of course, will be that no other information about it could be retrieved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 14:39:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1355" class=".btn">#1355</a>
            </td>
            <td>
                <b>
                    fix: isNewSocket logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `isNewSocket` was holding whether the socket already exists to an endpoint. I think the logic for closing the socket in `sendMessage` should be : 
```ts
    const socket = await this.resolveSocket({ socketId: endpoint, endpoint, connectionId })

    socket.send(Buffer.from(JSON.stringify(payload)))

    // If the socket was created for this message and we don't have return routing enabled
    // We can close the socket as it shouldn't return messages anymore
    if (socket && !outboundPackage.responseRequested) {
      socket.close()
    }
```
As per current logic, the socket is closed only when a message has `responseRequested=false` and a new socket is created just for this message. Let's suppose a message (`responseRequested=false` and socket already exists), in this case sender won't call `socket.close()`. But the receiver will close the socket

https://github.com/hyperledger/aries-framework-javascript/blob/1bda3f0733a472b536059cee8d34e25fb04c9f2d/packages/core/src/agent/MessageReceiver.ts#L138-L156

it's true, when the receiver closes the socket from his side, the sender will also close the socket based on `socket.onclose` event. But the sender might send a message before receiving the `socket.onclose` event. I got this bug, while I was testing for an edge agent to setup a mediation with an afj mediator. This was console log (at agent/MessageReceiver.tsL#139 and L#154) from the mediator

```
received message with return routes session_id:  3018a3bb-c37b-4b22-a1f6-66c494fc3d14 <<< This is connection/1.0/request
closing session for session_id:  a1de283b-0e9c-421e-a0d6-c59ac311d048 <<<< This is didcom/trust_ping
received message with return routes session_id:  a1de283b-0e9c-421e-a0d6-c59ac311d048 <<<< this mediate-request.
```
@TimoGlastra 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 14:19:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1354" class=".btn">#1354</a>
            </td>
            <td>
                <b>
                    refactor!: remove Dispatcher.registerMessageHandler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was marked as deprecated since 0.3.0

BREAKING CHANGE:

`Dispatcher.registerMessageHandler` has been removed in favour of `MessageHandlerRegistry.registerMessageHandler`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 13:42:27 +0000 UTC
    </div>
</div>

