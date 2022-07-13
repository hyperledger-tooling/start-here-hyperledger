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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/946" class=".btn">#946</a>
            </td>
            <td>
                <b>
                    fix: no return routing and wait for ping
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds some improvements to return routing. Mainly it adds two things:
1. Messages returned as a http response are now emitted using an event, meaning the sendMessage await won't wait for the returned message to be processed. This could lead to a chain of send / receive messages that would take a long time to resolve. Especially if the socket was kept open because no response was returned this could lead to unwanted behaviour. (see https://github.com/hyperledger/aries-cloudagent-python/pull/1853 for more context on socket staying open)
2. Do not include the return route decorator if not response is expected. The return route decorator is automatically added if we don't have an endpoint. This only happens with the mediator in most cases. What would happen is that the trust ping was sent to complete the connection, and we didn't receive a response. This would lead to the socket staying open for 15 seconds, before the mediation request message was sent. Now if the return route is already set (in this case to none) we won't add it in the message sender.. 

As mentioned in https://github.com/hyperledger/aries-cloudagent-python/pull/1853, this reduces the connection + request mediation flow time from ~17 seconds to around 1.5 seconds :)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 10:47:01 +0000 UTC
    </div>
</div>

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

