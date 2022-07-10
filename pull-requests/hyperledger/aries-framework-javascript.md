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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/941" class=".btn">#941</a>
            </td>
            <td>
                <b>
                    ci: fix changelog generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I removed this last time, but seems it is needed after all to correctly generate the changelog. See the changelog in #940 for what's the issue
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 09:32:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/940" class=".btn">#940</a>
            </td>
            <td>
                <b>
                    chore(release): v0.2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.2.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 09:24:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/938" class=".btn">#938</a>
            </td>
            <td>
                <b>
                    fix: clone record before emitting event
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
        Created At 2022-07-06 19:35:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/937" class=".btn">#937</a>
            </td>
            <td>
                <b>
                    build(deps): bump parse-url from 6.0.0 to 6.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [parse-url](https://github.com/IonicaBizau/parse-url) from 6.0.0 to 6.0.2.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/IonicaBizau/parse-url/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=parse-url&package-manager=npm_and_yarn&previous-version=6.0.0&new-version=6.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 01:11:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/936" class=".btn">#936</a>
            </td>
            <td>
                <b>
                    docs: initial contributing checklist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                see https://github.com/hyperledger/aries-framework-javascript/issues/918
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:59:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/935" class=".btn">#935</a>
            </td>
            <td>
                <b>
                    fix: change pubKey input from Buffer to Uint8Array
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses an issue that occurred when running the `deriveProof` test case in the `W3cCredentialService` tests. Strangely enough this issue only occurred when running in a NodeJS environment (which uses node-bbs-signatures) instead of the WASM fallback.

Huge thanks to @blu3beri for helping debug this issue. This one wasn't easy to catch.

Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:14:06 +0000 UTC
    </div>
</div>

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

