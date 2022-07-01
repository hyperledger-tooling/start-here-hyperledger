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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/911" class=".btn">#911</a>
            </td>
            <td>
                <b>
                    ci: fix next version bump output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Last one I hope...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    ci: fix next version bump variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CI is hard...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    feat(routing): add routing service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                Adds a routing service that handles the creating of keys for routing and integrates with the mediation recipient service to add routing for the mediator.

The extraction is just to make sure we don't have to depend on a mediator dependency all across the framework. 

What this also adds is an event for when routing keys are created. This allows the tenant module to listen for created routing keys and can then create a mapping of it in the base wallet. I first started with a middleware approach (As described in the design document: https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g), but this added _ A LOT_ of complexity and didn't abstract away the mediator functionality as that is a part of the core API. So I went for the less generic but simpler API, that is just fine I think.

Again no changes to the public api, so we can merge this without issues



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 07:46:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/908" class=".btn">#908</a>
            </td>
            <td>
                <b>
                    ci: add correct version bump
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We are using patch version for feature releases and minor versions for breaking releases, this change makes sure that's enforced. 

This should be merged before all other PRs to make sure we aren't going to release 0.3.0-alpha.1 but 0.2.1-alpha.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 15:39:53 +0000 UTC
    </div>
</div>

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

A module is declared like below:

```ts
import { module } from '@aries-framework/core'

@module()
class MyModule {
  public static register(dependencyManager: DependencyManager) {
    dependencyManager.registerContextScoped(MyApi)

    dependencyManager.registerSingleton(MyService)
    dependencyManager.registerSingleton(MyRepository)
  }
}
```

For now all module classes declare the module itself, but as discussed previously the current module classes will be renamed to `xxxApi`, and a module will act as the combination off everything that module adds (so more than just the public api)

It's not mean to be used publicly yet (and will have breaking changes), but you can then register the module on the dependency manager:

```ts
dependencyManager.registerModules(MyModule)
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

