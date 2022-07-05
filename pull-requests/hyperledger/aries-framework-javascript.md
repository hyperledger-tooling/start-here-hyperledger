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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/932" class=".btn">#932</a>
            </td>
            <td>
                <b>
                    feat(tenants): initial tenants module 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                Initial version of the tenants module. This is not fully finished yet and ready for prime time, but it contains most of the things needed for multi-tenancy. It doesn't introduce any breaking changes (those were addressed in the PRs this PR depends on).

Dependant on:
- #920
- #921 
- #922 

Until the modularization is fully here the API for registering module is not really nice, but I see that as a separate task that we can address after multi-tenancy has been merged. This is how you use it:

```ts
import { DependencyManager, Agent } from '@aries-framework/core'
import { TenantsApi, TenantsModule } from '@aries-framework/module-tenants'
import { agentDependencies } from '@aries-framework/node'

// create dependency manager and register module
const dependencyManager = new DependencyManager()
dependencyManager.registerModules(TenantsModule)

// create agent, and resolve tenants api
const agent = new Agent({ /* config */, agentDependencies , dependencyManager)
const tenantsApi = agent.dependencyManager.resolve(TenantsApi)

const tenantRecord = await tenantsApi.createTenant({
  config: {
   label: 'Tenant 1',
  },
})

const tenantAgent = await tenantsApi.getTenantAgent({
  tenantId: tenantRecord.id,
})

// Create oob invitation in scope of tenant
const outOfBandRecord = await tenantAgent.oob.createInvitation()
```

I would like to already merge so we can keep PRs reasonable (this is already getting quite large).

Basically the only thing that's left to do is correctly managing the tenant lifecycle and managing tenant sessions (see https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g?view#Tenant-Lifecycle). Currently, wallets are being opened when needed and will not be closed afterwards. That means over time the number of open wallets keeps increasing. Correctly opening wallets and avoiding race conditions if two sessions would like to open the same wallet is handled (using `async-mutex` library). This does need some improvements in not waiting indefinitely.

Concrete what's still todo:
- Agent lifecycle. Currently you call `getTenantAgent` with no proper way to dispose of the agent (session count won't be reduced)
- Check we're not using context after a process is complete (e.g. by setting an event listener). This should always start a new session instead of using the session from the upper scope

I'm quite happy with how it turned out and how multi-tenancy is an optional addon without having the code in the core package.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 13:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    fix(oob): support legacy prefix in attachments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix issue of the oob module not being able to handle the legacy did sov prefix on attachment in oob invitations.

Issue as reported on discord:

> AFJ is throwing an error when i accept an oob invitation with a present-proof/credential-offer attachment from acapy,   Error msg: There is no message in requests~attach supported by agent.  It's due to LegacyDidSovPrefix in the message type.  It fails at this step : https://github.com/hyperledger/aries-framework-javascript/blob/main/packages/core/src/modules/oob/OutOfBandModule.ts#L599 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 13:22:27 +0000 UTC
    </div>
</div>

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
                    feat: add base agent class 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                This is the same PR as #919 , but based off the 0.3.0-pre branch instead of main. There's no changes compared to #919 

Dependant on:
- #920
- #921 

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

Dependant on:
- #920

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

