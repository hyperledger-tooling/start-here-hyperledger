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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    build: make indy-sdk dev dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently when installing AFJ from npm it tries to install indy-sdk. Moving it back to dev dependencies so this isn't the case anymore. This requires a bit more setup as yarn install now requires indy to be installed.

I created a local action setup-libindy that handles this and is reused by all jobs.

related to discussion over here https://github.com/hyperledger/aries-mobile-agent-react-native/issues/41
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 08:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    feat: add internal ws outbound transporter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add internal ws outbound transporter. Same as with HTTP. Next step is multi outbound transport support. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 15:31:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    feat: Added attachment extension
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added the extension to the attachment decorator and renamed the attachment property on the issue and verify messages to avoid confliction.

Has been added for the support of linking credentials to attachments.

Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 15:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    ci: do not run concurrent release jobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the issues with the release. Github added a `concurrency` key a few weeks ago that allows us to prevent concurrent jobs from running. See the comment in the action file for more context


https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idconcurrency


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 08:58:48 +0000 UTC
    </div>
</div>

