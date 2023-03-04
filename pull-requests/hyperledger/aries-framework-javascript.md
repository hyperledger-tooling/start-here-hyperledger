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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1351" class=".btn">#1351</a>
            </td>
            <td>
                <b>
                    fix(anoncreds-rs): save revocation registry index
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When storing AnonCreds credentials, we weren't saving the revocation registry index, making it impossible to properly search for the credential in `RevocationNotificationService`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 17:34:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1350" class=".btn">#1350</a>
            </td>
            <td>
                <b>
                    refactor!: remove getKeyDidMappingByVerificationMethod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes hyperledger/aries-framework-javascript#1256
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 14:58:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1349" class=".btn">#1349</a>
            </td>
            <td>
                <b>
                    feat: add set up for indy-vdr optional peer dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR provides the guide to set up indy-vdr optional peer dependencies

**Work funded by the Government of Ontario**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 11:40:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    feat(oob): implicit invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for Out-of-Band protocol 'implicit invitations', meaning by that to connect to a public DID given it has a DID Communication service in its DidDocument. 

The API consists on the method `oob.receiveImplicitInvitation`, similar to regular `oob.receiveInvitation` but it of course receiving a resolvable did instead of a Connection Invitation.

It can use both Connection and DID Exchange protocols and it's possible to create multiple connections from the same public DID. By querying `connections.findByInvitationDid(publicDid)` it's possible for an application to know if it's already connected to a public entity.

Using AFJ agents it's working, but didn't test it against ACA-Py yet. Hopefully with these changes we can pass some DID Exchange tests in the AATH.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-25 16:51:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1347" class=".btn">#1347</a>
            </td>
            <td>
                <b>
                    feat(indy-sdk)!: move to did:indy with limited support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds full did:indy support for the indy-sdk package, while still keeping support for did:sov dids in interactions with other agents.

The `IndySdkAnonCredsRegistry` now supports resolving both `did:indy` and legacy unqualified anoncreds objects. I wasn't sure on making it two separate classes due to the duplication. I think it's okay that they're combined for now, but it may be nice to split them up at some point so users could choose to e.g. not support the legacy identifiers anymore.

 In addition a new `IndySdkIndyDidRegistrar` has been added. This doesn't support the `diddocContent`. The `IndySdkSovDidRegistrar` has been removed. From now on you can create did:indy dids, which contain the namespace, but you can keep on using the `did:sov` resolvers.

For registering anoncreds object you can now only use `did:indy` identifiers as this will contain the namespace, but you can still use the unqualified ones in using the legacy indy credential format services.

~~There's some additional work needed to the indy sdk issuer/holder/verifier services to make sure we can handle but qualified and unqualified dids and can also use them interchangeably.~~

> **Note**
> I don't think we're able to support did:indy using the indy-sdk as the identifiers are part of the credential meaning the identifiers in the credentials always must be unqualfiied as indy-sdk doesn't allow qualified input. I still think primarily supporting did:indy when creating objects is a good choice, as it allows us to prevent a lot of the ambiguity around which ledger to use. 

I'll make a similar PR for the indy-vdr package so they'll be in feature parity.

BREAKING CHANGE: The `IndySdkSovDidRegistrar` has been removed in favour of the new `IndySdkIndyDidRegistar`. you can register the same dids as you could do with the `IndySdkSovDidRegistrar`, but now with less ambiguity on which ledger should be used as that's encoded in the did itself.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-25 15:30:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1346" class=".btn">#1346</a>
            </td>
            <td>
                <b>
                    fix(indy-sdk): import from core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A relative import from core was preventing indy-sdk from being built correctly.

Here we add an eslint plugin to check these relative imports and other stuff that can be useful now we have plenty of packages in this repo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-25 13:34:43 +0000 UTC
    </div>
</div>

