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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Test/connections proto mediator id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                some tests for mediator id being used in connection protocol. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 09:17:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    fix: Use make-error-cause that works in RN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I forked [make-error-cause](https://github.com/blakeembrey/make-error-cause) and replaced Node.js `inspect` dependency with [util-inspect](https://github.com/Automattic/util-inspect). I'm not saying this is the final solution but it should make it work at least for now (I tested it with RN).

The issue describing the problem is #281.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 08:54:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    refactor: Rename samples to test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The initial goal with `samples` was to represent API and how to use the framework. However, the content of the folder is more about e2e tests so we can rename it. It doesn't change anything on the fact that it still could (and should) be a good place where the user can see examples of how to use it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:36:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    fix: convert from buffer now also accepts uint8Array
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also decodes from uint8Array now instead of only a Buffer.

Necessary for anything that is not in NodeJs.

Signed-off-by: blu3beri <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 17:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    fix: test failing because of moved import
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the failing CI.

The CI jobs are now required so it won't be possible to get bad commits into main


The problem was because I moved `toBeConnected` with to setup so each test file doesn't have to do it anymore. However this caused (i think?) some cyclic dependencies
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 17:11:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    refactor: Move a transport protocol-related logic from the framework core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I did some refactorings to help me add support for multiple transports in the following PR:
* Add test to `MessageSender`
* Move up a logic from `EnvelopeService` to `MessageSender`
* Remove transport-related details from the `TransportService` and from the core of the framework.
* Rename `transport` to `session` which hopefully express the meaning better.

As a next step I'm considering:
* Rename transporters to transports
* Move up more logic from `MessageSender.packMessage` and pass `service` object to `packMessage`
* Then we could call `packMessage` and `sendMessage` for every available service. Eventually, we could remove the logic from `createOutboundMessage`.
* Improve validation of `outboundMessage` inside `OutboundTransporter` and error handling
* Add multiple transports

If you think it doesn't make sense to merge this without full functionality I can continue with adding changes. But I realized that it contains a good amount of changes already and it could be worth merging sooner.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 08:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    fix: connection record type was BaseRecord 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 16:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    refactor: Re-use ws outbound transport in mediator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small refactor.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 16:55:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    refactor: replace all errors with framework errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a base `AriesFrameworkError` that is now thrown instead of the generic `Error`. It also adds `RecordNotFoundError` and `RecordDuplicateError` that is now used when storing/retrieving records. It could be hard to find out why an indy operation was failing. This gives a lot more context to the framework consumer.

Over time we can add more specific error classes for other parts of the codebase, but I thought this was already a great start.

Fixes #78
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 13:18:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    refactor: use single event emitter for all events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 23:21:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    feat: only connect to ledger when needed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - only connect to ledger when needed
- allow to pass `genesisTransactions` so you don't have to deal with storing the genesis yourself

Fixes #219 
Fixes #265 

The ledger management can be improved, but I think this is a simple first step. Only open the ledger connection if a ledger call is made


---

Tested in both NodeJS and React Native
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 21:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Dev/mediation config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @DavidClawson work on configuration for meditation recipient. 
Introduces an initialize method to the recipient module(src/modules/routing/RecipientModule.ts).
- initialize is called from agent.init() after wallet, ledger, and transport are set up. 
- recipient.init() checks for provided configurations to automatically set up mediation at the start.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 17:57:49 +0000 UTC
    </div>
</div>

