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
                    feat/jsonld-credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                > I'm reopening this PR (this time originating from the Animo fork) because I wasn't able to push to upstream anymore all of a sudden. This PR is identical to the previous `feat/jsonld-credentials` PR (apart from a few extra commits).
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
                    feat: Delete events
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/715" class=".btn">#715</a>
            </td>
            <td>
                <b>
                    fix: close session early if no return route
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `close` method to all transport session so it can be closed from within the agent. This allows us to close the session early if the message doesn't have return routing enabled. Specifically this resolves the following issue raised:

> Hi Timo, I'm debugging our DIDCOMM protocol engine, and it seems that AFJ doesn't respond immediately after it has received the payload by HTTP POST. Our protocol state-machine keeps waiting for the response, but instead of that, AFJ sends a new HTTP POST request. Naturally, we could handle that, but could you please confirm that this is the case? Does your HTTP handlers block, i.e. process the payload and send the new request before responding?

Although it's not necesarily a wrong doing in AFJ, there is no need to keep the session open for longer than needed. Draft as this is dependant on some changes in this PR: https://github.com/hyperledger/aries-framework-javascript/pull/712
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 15:46:54 +0000 UTC
    </div>
</div>

