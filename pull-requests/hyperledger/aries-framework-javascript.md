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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1500" class=".btn">#1500</a>
            </td>
            <td>
                <b>
                    build: Update Github workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create cleanup-cache.yml

Switch build to Yarn

Update continuous-deployment.yml

- Bump actions/checkout
- Switch to `--immutable` with yarn (this is the new command)
- Fix deprecated set-output command

Add heap memory management

Update continuous-integration.yml

- Use a consistent runner
- Fix set-output issues
- Switch to setup-node

Update lint-pr.yml

Update repolinter.yml

Update cleanup-cache.yml

Update codeql-analysis.yml

Create dependabot.yml

Update dependabot.yml

Update .dockerignore

Update Dockerfile

Remove accidental --immutable

build: test large builders

Add setup functions to CodeQL

Update codeql-analysis.yml

Delete local setup-node

Update continuous-integration.yml

Change to larger runners
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 15:43:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1498" class=".btn">#1498</a>
            </td>
            <td>
                <b>
                    fix(askar): in memory wallet creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quick fix to allow the creation of an in-memory wallet (for test purposes). Previously, the parameter was supported but, due to a particular error thrown by `@hyperledger/askar-shared` it was not working.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 22:50:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1496" class=".btn">#1496</a>
            </td>
            <td>
                <b>
                    feat: Create Connection record when receive DidCommV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Added optional `autoCreateConnectionOnPing` field into Agent config and implemented corresponding logic - indicating whether we should create connection state records when receiving a trust ping message targeted to the DID in the wallet, but with a non-existing pairwise record 
* Updated MessageSender: Unified `sendDidCommV1message` and `sendDidCommV2message` functions into single method `sendMessage`. 
  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 14:41:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1495" class=".btn">#1495</a>
            </td>
            <td>
                <b>
                    fix: race condition singleton records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/aries-framework-javascript/issues/968

This just handles the multiple creation and then erroring of signleton records. 

We still have an issue with multiple writes to the same document, which we should be able to fix with locks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 12:14:03 +0000 UTC
    </div>
</div>

