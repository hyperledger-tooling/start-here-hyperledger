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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/930" class=".btn">#930</a>
            </td>
            <td>
                <b>
                    feat: OOB public did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pavel Zarecky <zarecky@procivis.ch>

First attempt to add support for receiving OOB invitations with public did.

Currently this is working together with the aca-py agent, when  oob invitation is created using:
```
POST /out-of-band/create-invitation
{
  "handshake_protocols": [
    "did:sov:BzCbsNYhMrjHiqZDTUASHg;spec/connections/1.0"
  ],
  "use_public_did": true,
  ...
}
```

* refactored `OutOfBandInvitation.services` to tackle the issues with `String` coming from the transformer. Exposing only a getter `getServices` method to get simplified representation.
* resolving public DID services procedure moved from the `MessageSender` into the `DidResolverService` as it needs to be performed when sending the connection request as well as handling the connection response
  * We should maybe think about some caching to not run the resolution multiple times
* The service `recipientKey` lookup procedure had to be adjusted, to work together with aca-py. There's a strange Ed25519/X25519 key specification historical convention (https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html#did-document-notes)

TODO: 
* check OOB invitation with `didexchange` protocol
* fix tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 11:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    fix: missing module exports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 21:02:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/926" class=".btn">#926</a>
            </td>
            <td>
                <b>
                    feat(oob): allow to append attachments to invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds an optional `appendedAttachments` field for OOB invitations (and legacy Connection Invitation messages) that allows to append attachments as per [Aries RFC 0017](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0017-attachments#appending).

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 20:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    chore: update afj dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just some housekeeping
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 13:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/922" class=".btn">#922</a>
            </td>
            <td>
                <b>
                    refactor!: add agent context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                This is the same PR as #919 , but based off the 0.3.0-pre branch instead of main. There's no changes compared to #919 

Dependant on #920 and #921 

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 12:12:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    feat: add agent context provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                This is the same PR as #898, but based off the 0.3.0-pre branch instead of main. There's no changes compared to #898

Dependant on #920

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 11:29:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    refactor!: add agent context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span><span class="chip">breaking change</span>
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

This is the same PR as #881, but based off the 0.3.0-pre branch instead of main. There's no changes compared to #881 except for making it work with this branch (making the new w3c services stateless). Due to the breaking changes we don't want to have this in main just yet. 

BREAKING CHANGE: To make AFJ multi-tenancy ready, all services and repositories have been made stateless. A new `AgentContext` is introduced that holds the current context, which is passed to each method call. The public API hasn't been affected, but due to the large impact of this change it is marked as breaking.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 11:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    feat: add method to fetch KeyType by proof type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 13:32:56 +0000 UTC
    </div>
</div>

