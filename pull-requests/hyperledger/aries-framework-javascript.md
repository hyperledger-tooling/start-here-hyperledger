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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    fix: optional fields in did document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changes the logic for the did document to not set default values for the did document. This seemed convenient to me at first, but in the end it causes problems when you need to get the original form of the did document.

This PR also removes the `DidPeer` class. I thought this would be convenient (and it was for a part), but it added way to much complexity. Especially as I tried to fix the issue with `did:peer:1` method and needing the raw json bytes (to consistently calculate the hash). I now replaced it with simple methods such as `keyToNumAlgo0DidDocument` or `didDocumentJsonToNumAlgo1Did`.

@jakubkoci this affects your PR because you can't use the `DidPeer` class anymore. Please take a look at `peer-did.test.ts` on how to use it without `DidPeer`. I didn't want to add more work, but the consistent hashing is quite important for interop with other agents down the line. You should make sure that when parsing a num algo 1 (`did:peer:1`) that is received from another agent we parse the json variant of the did document (`didDocumentJsonToNumAlgo1Did`) as the transformation to the `DidDocument` class can make the resulting document structure different.

BREAKING CHANGE: The `DidDocument` class doesn't set empty array values anymore for optional fields. This means you now have to check the value exists before being able to use it. This would mean that e.g. `didDocument.authentication.map()` would become `didDocument.authentication?.map()` to deal with the optionality of the field. This change was introduced to keep the class representation of a did document more in line with the actual representation of a did document.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 21:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    refactor: replace message type constant with string literal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jakub Koci <jakub.koci@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 08:59:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    feat: Updated initPublicDid method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR reuses the public did instead of generating a new every time the wallet is opened.

Signed-off-by: Dinkar Jain <62498436+dinkar-jain@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-23 16:55:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    feat: jsonld-credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the low-level functionality that is required for the issuance and verification of JSON-LD based credentials (W3C).

The key features this PR includes are:
- The `W3cCredentialService` that can be used for signing and verifying JSON-LD based credentials and presentations.
- The `W3cCredentialRepository` that handles storage for JSON-LD based credentials.
- The `Ed25519Signature2018` signature suite that adds support for signing and verifying Ed255192018 signatures.
- The `BbsBlsSignature2020` signature suite that adds support for signing and verifying BbsBls2020 signatures.
- The `BbsBlsSignatureProof2020` signature suite that adds support for deriving, signing and verifying proofs of BbsBls2020 signed credentials.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 10:53:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    feat: add out-of-band and did exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Todo
* API
	* refactor(api): Change `acceptInvitation` param from oob record to record id @JamesKEbert 
	* feat(api): Expose remove, find, getAll oob methods @JamesKEbert 
* Implement handshake reuse handler and event emitter to react on handshake @JamesKEbert 
* Store the old did in metadata (this can have impact to migration scripts)
* Connection record migration script @TimoGlastra 
* Reuse oob invitation keys also for multiuse invitation (?)
	* @TimoGlastra Currently, I'm still creating new keys when it's multiuse invitation. I assume we don't want to do that, right?
* Add oob record state and role checks
* Emit oob state change event
* Resolve key from reference (?)
* Align connection and did-exchange protocol states @TimoGlastra Could you look at this, please? I don't see it as entirely beneficial and you already have an idea of how to do it in your mind.
* API
	* refactor(api): Rename `outOfBandMessage` to `outOfBandInvitation`
	* feat(api): store more from `receiveInvitation` config into a record and allow override in `acceptInvitation`
* refactor(core): Change `did` to `unqualifiedSovDid` or maybe `unqualifiedIndyDid`
* refactor(core): Extract connection protocol methods from service to protocol class
* Throw an error if there is more then one rule resolved by state machine
	* But I actually didn’t find beneficial the way how I implemented the did exchange state machine
* Fix naming caused by  `DecryptedMessageContext` vs. `UnpackedMessageContext`
* refactor: Rename `XxxMessageOptions` to `XxxMessageProps`

I ordered it approximately by priority. The first half before the second API point seems to be quite important, and the rest is more a nice-to-have.

I assigned names based on notes from our AFJ call last week https://wiki.hyperledger.org/display/ARIES/2022-04-14+Aries+Framework+JS+Meeting+notes, please raise your hand if it doesn't suit you. I can look at the rest of the tasks. I welcome some feedback on what you think is important and what is not.

Is there any task from the Todo list I should look at even before merging?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 08:16:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    feat: delete events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added delete events to `Connection`, `Credential` and `Proof` services so that they notify about deletion in similar way to state change events.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 06:37:19 +0000 UTC
    </div>
</div>

