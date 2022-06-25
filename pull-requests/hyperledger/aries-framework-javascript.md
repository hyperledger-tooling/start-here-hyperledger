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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    feat: initial plugin api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span><span class="chip">modularization</span>
            </td>
            <td>
                Adds an initial (mostly internal for now) plugin API that will be used as part of modularization. The changes from this PR are also needed for multi-tenancy.

I've not made breaking changes yet, so we can already get this merged and start releasing it, and we can do some clean up of the old custom module approach once we're ready to make the next breaking change release.

As this doesn't contain any breaking changes, I think we should merge this before #881 and #898

The biggest change in this PR is to move from a more implicit registration of services and modules, to a more explicit way to declare services and modules.

Instead of declarating a class with `@scoped(Lifecycle.ContainerScoped)` it now just needs `@injectable` (which is exported from the `src/plugins` directory. Then you can define a plugin to register modules and services. There's currently tow types of plugins, where a module plugin extends a default plugin.

A normal plugin is declared like below, this doesn't expose a public API through a module. We already use this internally for some services without public api (e.g. the indy plugin that adds the `IndyIssuerService`, etc..)

```ts
const myPlugin: Plugin = {
  register(dependencyManager: DependencyManager) {
    dependencyManager.registerSingleton(MyService)
    dependencyManager.registerSingleton(MyRepository)
  }
}
```

The you have the module plugin which works the same but is declared directly on the module itself:

```ts
class MyModule {
  register(dependencyManager: DependencyManager) {
    dependencyManager.registerSingleton(MyService)
    dependencyManager.registerSingleton(MyRepository)
  }
}
```


It's not mean to be used publicly yet (and will have breaking changes), but you can then register the module on the dependency manager:

```ts
dependencyManager.registerModulePlugins([MyModule])

// or if no module
dependencyManager.registerPlugins([myPlugin])
```

This will make sure the services are registered and in case of the module plugin the module is also registered. The reason why we need this for multitenancy is that we're going to create child container for each tenant agent, that share most of the services from the base agent, but will have some differences. The `@scoped(Lifecycle.ContainerScoped)` won't do the job anymore. 

I've exported some of the tsyringe methods and wrote a simple DependencyManager class to abstract away most of the `TSyringe` functionality so that you don't need to import from that dependench to write plugins, the needed primivities are exported from AFJ itself.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 10:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/906" class=".btn">#906</a>
            </td>
            <td>
                <b>
                    feat(credentials): added credential sendProblemReport method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pavel Zarecky <zarecky@procivis.ch>

Adding a convenience method to send problem report as part of RFC's 0036 and 0453 unhappy flow.
It is a complementary implementation to the `agent.proofs.sendProblemReport`. But for credentials it was still missing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 12:21:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/904" class=".btn">#904</a>
            </td>
            <td>
                <b>
                    fix(connections): fix log of object in string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes issue where logs would print `[object Object]`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 13:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/903" class=".btn">#903</a>
            </td>
            <td>
                <b>
                    refactor(credentials): remove formats for version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Just to make the type a bit simpler
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 13:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/900" class=".btn">#900</a>
            </td>
            <td>
                <b>
                    feat: Smart schema and credential definition registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Moriarty <moritz@animo.id>

closes #859 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 13:18:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    feat!: add agent context provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                > - Dependant on #881 (until that one is merged this is kinda hard to review)
> - Design: https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g#Agent-Context-Provider

Adds an `AgentContextProvider` with default `DefaultAgentContextProvider` implementation that always returns the same agent context (for a single tenant agent). 

This allows the tenant module (will be added as a separate module) to implement its own `TenantAgentContextProvider` that will find provide the agent context for a specific tenant. This allows to keep the core lean, while providing more advanced usages of providing the agent context.

I added a `contextCorrelationId` to the `AgentContext` interface. For now this is not really needed, but this will become really useful when we add tenants. The `contextCorrelationId` allows to correlate the context with an identifier to make it easier to provide the context for an incoming message. By default we find the tenant based on the recipient public keys of a message, but there's numerous cases where we are processing plaintext messages. By providing the contextCorrelationId we can use this in the `AgentContextProvider` to correlate the message to a specific context. In the case of the `TenantContextProvider` the `contextCorrelationId` will be the `tenantId`.


BREAKING CHANGE: the `agent.receiveMessage` method should only be used if you want to process the message in the context of the current agent. This means it fine to use for e.g. processing plaintext connection-less messages, but it shouldn't be used anymore by outbound and inbound transports to process messages. Instead, inject the `MessageReceiver` class and call `receiveMessage` on that class instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 17:22:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    fix(connections): set image url in create request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Amit-Padmani <amit.padmani@ontario.ca>

Image URL is missing in connection record [#895](https://github.com/hyperledger/aries-framework-javascript/issues/895)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 11:56:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/893" class=".btn">#893</a>
            </td>
            <td>
                <b>
                    test(credentials): fix flaky tests with events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the flaky e2e test for icv2. We only start event listeners action the has been performed (sendProposal -> start proposal received listener) while we should be starting the listener before performing the action (start proposal received listener -> sendProposal) to prevent flaky tests.

I've fixed it for one file now, but we should look at all ICv2 and PPv2 tests (that's where we use evens A LOT).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 17:06:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    fix(credentials): do not store offer attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes #891 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 15:36:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/890" class=".btn">#890</a>
            </td>
            <td>
                <b>
                    chore: move to docs repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Should not be merged until https://aries.js.org is live.

Removes all docs that have been moved to the Aries JavaScript docs repo. Have kept some getting started docs in place until we can add sections for that in the aries javascript docs repo.

Related PR in https://github.com/animo/aries-javascript-docs/pull/30 (should be merged first)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 14:02:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/889" class=".btn">#889</a>
            </td>
            <td>
                <b>
                    fix(oob): allow legacy did sov prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes #875 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/888" class=".btn">#888</a>
            </td>
            <td>
                <b>
                    fix: remove usage of const enum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes #884, see the issue for why we can't use const enums
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 08:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/887" class=".btn">#887</a>
            </td>
            <td>
                <b>
                    feat(credentials): find didcomm message methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Adds `findProposalMessage`, `findOfferMessage`, `findRequestMessage`, `findCredentialMessage` methods to the credentials module to be able to access the did comm message associated with a credential exchange.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 07:45:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/886" class=".btn">#886</a>
            </td>
            <td>
                <b>
                    feat: delete w3c credential record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a method to the W3cCredentialService to remove a credential record from storage. I also renamed a few properties and methods because their previous names were somewhat misleading.

- feat: add method to remove w3c credential
- refactor: rename methods and props for consistancy

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 18:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    fix(connections): allow ; to convert legacy did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Older dids use `;` as an identifier separator instead of the now used `#`. So an id of `did:sov:123;indy` would be normalized to `#did:sov:123;indy`. We now check when converting a legacy did doc to a new did doc whether an `;` character is in place and the `#` isn't and we will handle it correclty so it parses to `#indy`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 15:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/881" class=".btn">#881</a>
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
                This is a big pull request, but doesn't change any functionality of the agent. All services, repositories etc.. now use agent context so we can start using them as stateless services for multitenancy (as described here: https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g#Agent-Context).

This doesn't change the public API of the framework, but because of the large number of changes and also the implications for custom modules I've marked this as a breaking change.

Will add more detailed migration docs later on, but generally you have to update your modules to now inject the agent context object and pass that around to services. See the `DummyModule` for an example: https://github.com/TimoGlastra/aries-framework-javascript/blob/317dc779d8ff88921fa6333ed3490ae77784f1ff/samples/extension-module/dummy/DummyModule.ts


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 10:02:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    fix(credentials): miscellaneous typing issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes some issues encountered in the typing. Mainly:
- export the messages types from the core packages
- prepend `V1` and `V2 to all credential interfaces to avoid conflicts in interface names
- use `string` as type for `protocolVersion` instead of `v${string}` to make it work with tsoa
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 08:47:26 +0000 UTC
    </div>
</div>

