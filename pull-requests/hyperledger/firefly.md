---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Honor "confirm" parameter for blockchain invoke
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a PR chain with #720.

Unit tests are not yet complete, but wanted to validate the approach before finishing them.

Summary of the changes:
* The `confirm` parameter for `/invoke` will now be honored (previously it was ignored)
* The `fftypes.ContractCallResponse` type is removed, and `/invoke` requests now just return `fftypes.Operation`
* Two new event types are added - `EventTypeBlockchainInvokeOpSucceeded` and `EventTypeBlockchainInvokeOpFailed` - which reference an operation ID (open to thoughts on whether `topic` and `correlator` should be filled in)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 18:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    New Getting Started Guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - All of the content under "Getting Started" is completely new.
- This is now completely tailored for someone who is completely new to FireFly and needs a walkthrough on how to get started with it
- Existing "Getting Started Guides" have moved to a new "Tutorials" section

A live preview of these new docs can be viewed at: https://nguyer.github.io/firefly/gettingstarted/gettingstarted.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 18:15:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    Move "special" operation update handling out of Operations Manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Feels like these should be farmed out instead of Operations Manager having knowledge of the various specific operation types.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 17:26:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    OpenAPI cleanup items
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 17:17:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Rename contract listener "protocol_id" to "backend_id"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This doesn't align with other "protocol_id" fields in the system, so it should have a different name.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 20:19:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    DID rewind
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #692 
In PR chain with #707

This PR adds a new reason for a rewind - to go back and confirm messages that were previously parked because the author was not known.

We cannot assure that the identity verification for an identity, will be processed by the aggregator before messages sent by that identity, or child identities registered under that identity. Because they are all sent on different topics.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 19:00:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/714" class=".btn">#714</a>
            </td>
            <td>
                <b>
                    WebSocket disconnections should be info messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 16:04:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/712" class=".btn">#712</a>
            </td>
            <td>
                <b>
                    Restore getting started section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was an accidental deletion in #708 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 13:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    Add token provider to container logs name to make it unique
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When trying to investigate https://github.com/hyperledger/firefly/runs/6001824099?check_suite_focus=true I found that I didn't have the container logs.

Looks like it's due to a clash in the names between the token tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 12:25:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/709" class=".btn">#709</a>
            </td>
            <td>
                <b>
                    Fix token approvals and clarify fields "protocolId", "locator", and "subject"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Depends on https://github.com/hyperledger/firefly-tokens-erc1155/pull/67 and https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/42

This started as a quest to clean up token approvals, but ended up encompassing a few related items:

* The term "protocolId" has come to mean (fairly specifically) "an ID meaningful in the context of an underlying blockchain protocol".
  * The existing "protocolId" of token approvals is renamed to "subject", and token approvals get a new "protocolId" field that better aligns with the above.
  * Token transfers keep their "protocolId" unchanged, as it already aligns.
  * The existing "protocolId" of token pools is renamed to "locator".
  * Blockchain events will be de-duplicated based on their "protocolId" - only one event per namespace+listener+protocolId will be recorded, to avoid recording the same blockchain event multiple times.
* Token approvals will record _all_ historical approvals (instead of sometimes overwriting old ones). As a convenience for query purposes, the most recent approval for each subject will be notated with a new field "active=true".
* When matching token approval (and transfer) events to operations, event manager will now consider the operation ID _and_ the token connector and pool embedded in the operation inputs before considering it a match. This ensures that side-effects in other pools will not be matched with the wrong operation and return unexpected results for synchronous actions (when using confirm=true). Resolves #661.

This does introduce changes in the interface with token connectors, so will require connectors to be upgraded alongside it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 05:06:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Readme and documentation updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are quite a substantial batch of updates here. Highlights:
- New README.md that is hopefully much more friendly, and highlights some great new V1 features like the Sandbox
- Updates to the ASCII art repo detail (in README and docs)
- New docs landing page
- New main architecture diagram
- Combining `Maintainers` section into `Contributors` section
- Renaming `Key concepts` to `Understanding FireFly`
- New doc article summarizing what FireFly is - `Introduction to Supernodes`
- New doc article on `Public and Permissioned Blockchain`
- New slides
- New screenshots
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 02:47:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/707" class=".btn">#707</a>
            </td>
            <td>
                <b>
                    E2E account creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes only testing changes, which are necessary for the upcoming `v0.0.47` release of the FireFly CLI.

It moves the responsibility for blockchain account creation to the CLI, and uses the new `stackState.json` file generated by the CLI to get a list of available accounts that can be used in tests.

This PR also enables the identity E2E tests for Fabric and Besu based FireFly stacks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 02:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/705" class=".btn">#705</a>
            </td>
            <td>
                <b>
                    Reject Contract API updates with an ID mismatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #703

More work can be done to reject upfront for a better user experience, but this fixes the important bug that blocks event processing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 21:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/702" class=".btn">#702</a>
            </td>
            <td>
                <b>
                    Add descriptions for all API routes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds descriptions for all API routes and path parameters. Just like configuration descriptions, the tests will panic if a new route is created that doesn't have a description.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 18:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/701" class=".btn">#701</a>
            </td>
            <td>
                <b>
                    [ui-v0.7.0] manifest and image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 17:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    Update readme images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix #699.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 17:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    Update ruby deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dependabot is encouraging upgrades
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 14:12:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Make http server framework re-usable by microservices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a PR chain with #688
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 22:07:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    Add helpers at /apis/{apiName}/listeners/{eventPath}
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This includes the commit from #693.

Add helper URLs:

```
GET /apis/{apiName}/listeners/{eventPath} - list all listeners matching this event on this API
POST /apis/{apiName}/listeners/{eventPath} - create a new listener for this event on this API
```

Also makes `topic` a required field for contract listeners, and enforces uniqueness of listeners across these 2 dimensions:
* namespace + name
* topic + contract location + event signature

Violating either uniqueness constraint when attempting to create a listener will result in HTTP 409, so applications can rely on this behavior to perform "create this listener if it does not already exist". Note that `name` is still optional, and a unique one will be assigned at creation time if none is specified.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 21:08:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/695" class=".btn">#695</a>
            </td>
            <td>
                <b>
                    Add completed configuration descriptions and types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The main thing this PR adds is completed descriptions for all configuration options. It also adds a new `ffc()` for FireFly Configuration message keys for translations. The configuration key requires that a `fieldType` be set as another parameter in addition to the configuration description. The `fieldType` is a `string` that describes the Go type that FireFly Core will parse the field as.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 20:48:47 +0000 UTC
    </div>
</div>

