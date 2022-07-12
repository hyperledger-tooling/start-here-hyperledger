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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/945" class=".btn">#945</a>
            </td>
            <td>
                <b>
                    Feat/indy namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #944 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 14:15:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/943" class=".btn">#943</a>
            </td>
            <td>
                <b>
                    feat(credentials): credential module config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">modularization</span>
            </td>
            <td>
                Adds a CredentialModuleConfig to showcase how module configuration would work. For now the module is still internal and takes config from the agent config, but it shows how custom module configuration works. This is one step closer to configurable modules.

Basically how you'd use it (if we have full modularization):

```ts
const agent = new Agent({
  modules: {
    credentials: new CredentialsModule({
        autoAcceptCredentials: AutoAcceptCredential.always
    })
  }
})
```

The credentials api can then depend on it like this:

```ts
CredentialsApi {
  public constructor(
    credentialsModuleConfig: CredentialsModuleConfig
  ) {
   const autoAcceptCredentials = this.credentialsModuleConfig.autoAcceptCredentials
  }
}
```


@karimStekelenburg @blu3beri @genaris @2byrds @JamesKEbert Thoughts? If we can agree on the approach for configuration, I can update it for all modules. We can still keep it in init config (so there won't be much breaking changes for now). But from then on it will be trivial to start extracting modules out of core
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 15:57:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/942" class=".btn">#942</a>
            </td>
            <td>
                <b>
                    feat(tenants): tenant lifecycle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                Adds lifecycle management to the tenants module (especially the `TenantSessionCoordinator` and the `TenantAgentContextProvider`). 

There's an internal registry of open sessions (`TenantSessionMutex`). This is configured with a max number of sessions (currently set to 10.000, I hope to add custom module config with modularization soon). It also adds a timeout for how long it can take to acquire a session (also hardcoded for now, will become configurable). It's important that sessions are always ended. You can either do that using `withAgentContext` which will end the session for you, or you need to call `.destroy` after you're done using the tenant agent. After a message has been processed the session will also be ended.

This doesn't include caching of agent context yet. So if the last session for a tenant is ended, the wallet will be closed. In the future we could look at keeping the wallet open for a while, but with RAW key derivation I have this process to be quite fast. I first wanted to make sure we can handle a lot of sessions for different and same tenants at the same time and don't break.

Some notes:
- I've updated most of the codebase to work with multiple contexts, and making sure we aren't creating events based on contexts that may have been expired. The exception is the mediation recipient module. This will need more work, and as you probably won't use mediation as a tenant is lower priority for now.
- max session count, session acquire timeout are hardcoded for now. Will be configurable soon
- Added some e2e tests that open 5 sessions each for 20 tenants in parallel. WE should add some proper benchmark tests soon
- I've updated the wallet to use RAW key derivation (we use `generateWalletKey`) which means the wallet key generation process has been sped up significantly.
- There's improvements to be made in how we weigh sessions. Currently 10 sessions for 1 tenant weigh equal to 10 sessions spread over 10 tenants. In theory in the first case we only open 1 wallet, while in the latter we open 10. We could make the first session have 5 weight points, and the concurrent sessions 1. This means it's cheaper to have multiple sessions for the same tenant than sessions for different tenants. Server environments should make sure to use sticky sessions and route the same tenants to the same agent.

One thing we should still look at is that you can call tenantAgent.wallet.close() at any time which will corrupt all current sessions. I'm not sure if we can avoid this, and we should probably document this.

Also see: https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g?view#Tenant-Lifecycle

Usage:

```ts
// manual: FAILURE TO CALL .destroy() CAN LEAD TO DEADLOCKS. SECOND APPROACH ADVISED
const tenantAgent = await agent.tenants.getTenantAgent({ tenantId: 'tenant-id' })
const invitation = await tenantAgent.oob.createInvitation()
await tenantAgent.destroy()

// auto
const tenantAgent = await agent.tenants.withTenantAgent({ tenantId: 'tenant-id' }, async tenantAgent => {
	const invitation = await tenantAgent.oob.createInvitation()
})
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 14:46:45 +0000 UTC
    </div>
</div>

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

