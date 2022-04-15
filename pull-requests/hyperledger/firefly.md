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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    Rename "contract" field to "interface" on FFIMethod/FFIEvent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                This is consistent with the underlying database field name and with the
naming of the field on other related objects (like contract APIs and
listeners).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 01:01:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    Fix postgres migrations and add to PR checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a regression that was introduced recently into PostgreSQL migrations. The issue first occurred when the `payload_ref` column was removed in this commit: https://github.com/hyperledger/firefly/commit/7b02d90d85c1632b65c11f73667a1f35f9f5ac20#diff-aace6955c9ca1493ae6a4a7f8bb03aa93f8d12ea4ca6f4b7ee74321bc875d379L12. 

A later postgres migration (number `21`) referenced this column but it was no longer, so it failed to migrate the database with the following message:

```
Error: FF10163: Database migration failed: FF10163: Database migration failed: 2 errors occurred:
	* migration failed: column "payload_ref" does not exist (column 70) in line 8: BEGIN;

ALTER TABLE data DROP COLUMN blobstore;
ALTER TABLE data ADD blob_hash CHAR(64);
ALTER TABLE data ADD blob_public VARCHAR(1024);

-- Make payload_ref larger and a varchar, to accomodate more flexible IDs for non-IPFS shared storage plugins
ALTER TABLE batches ALTER COLUMN payload_ref TYPE VARCHAR(256) USING payload_ref;

CREATE INDEX data_blobs ON data(blob_hash);

COMMIT;
 (details: pq: column "payload_ref" does not exist)
	* pq: current transaction is aborted, commands ignored until end of transaction block in line 0: SELECT pg_advisory_unlock($1)
```

A misguided attempt to fix this issue was merged in https://github.com/hyperledger/firefly/pull/683. That PR removed postgres migrations `20` and `21` in an attempt to match the sqlite migrations. However, that "fix" did not work.

This PR undoes https://github.com/hyperledger/firefly/pull/683 by adding `20` and `21` back again. It also fixes the original problem, by not attempting to alter the column in `21` that no longer exists.

This PR also adds postgres to the test matrix for PR approval which should prevent us from winding up in this situation again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 23:06:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Status plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `GET /api/v1/status` now returns a `plugin` key:
```json
{
  "node": {...},
  "org": {...},
  "defaults": {...},
  "plugins": {
    "blockchain": [
      {
        "pluginType": "ethereum"
      }
    ],
    "database": [
      {
        "pluginType": "sqlite3"
      }
    ],
    "dataExchange": [
      {
        "pluginType": "ffdx"
      }
    ],
    "events": [
      {
        "pluginType": "system"
      },
      {
        "pluginType": "websockets"
      },
      {
        "pluginType": "webhooks"
      }
    ],
    "identity": [
      {
        "pluginType": "onchain"
      }
    ],
    "sharedStorage": [
      {
        "pluginType": "ipfs"
      }
    ],
    "tokens": [
      {
        "name": "erc1155",
        "pluginType": "fftokens"
      }
    ]
  }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 22:27:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Move ffresty to pkg for use by other microservices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The logging, retry and other configuration features we have in the FireFly wrapper on resty, should be available to other microservices. That way we can have consistency in how you configure it and the features you get.

In PR chain with #668 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 21:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Include interface metadata routes in FFI-generated Swagger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows fetching info about the associated FFI, including the details of all
methods and events.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 16:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Add contract listeners only by event definition or event pathname
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Previously, contract listeners could be added in 3 ways:
1. By passing a full event definition inline
2. By passing a partial event definition (containing just an event name) along with an interface reference
3. By passing an event ID

Number (2) is slightly confusing in how it is expressed and differentiated from (1), and also has been slightly broken since we don't actually support event lookup by "name" (rather it's by "pathname", and "pathname" isn't a field available on the FFIEventDefinition type).

To clean all this up, I'm proposing here that we drop the existing (2) and (3) and instead end up with only these two ways to add a listener:
1. By passing a full event definition inline
2. By passing an interface reference and event pathname

Technically there's no reason to drop the lookup by event ID, so if there is a strong argument to keep it, we can. But I like the simplicity of these two codepaths that I anticipate will be the most common.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 12:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Remove extra postgres migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It looks like at some point we removed sqlite migrations 20 and 21, but did not remove the corresponding postgres migrations. This was causing FireFly to fail to start when attempting to apply postgres migrations. This PR aligns the postgres migrations with the working sqlite migrations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 12:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Fix make docker command in release build GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 02:10:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Enforce config descriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 20:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/680" class=".btn">#680</a>
            </td>
            <td>
                <b>
                    Add /api/v1/status/websockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #679
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 19:57:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    Configuration docs, and packaging config/i18n for re-use by microservices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A bunch of changes to improve our config docs (thanks @nguyer for your work there), and some structural changes to the `config` and `i18n` packages to allow them to be used by other microservices building in Go within the FireFly project.

- `pkg/config` - moved out the package for configuration, including the facility for Markdown generation
  - Split out the configuration that is base (just `log` and `lang`) from the Core configuration
  - `internal/coreconfig` contains the core configuration
  - Note that `coreconfig.Reset()` initializes all the defaults in a lock (needed to avoid concurrent map errors)
- `pkg/i18n` - moved out the translation framework
  - All the framework for translation moved
  - Tweak to how the default `en` translations are initialized, to allow sub-modules to keep adding keys
  - Split out `ErrorMessageKey` from `MessageKey` - with the distinction that errors have to have a registered prefix, that means microservices will not re-use message codes from other microservices
  - `FF10` errors are the FireFly Core errors
  - `FF00` errors are raised from the common utilities in `pkg` - note this mean renames of some codes
  - `FF201` errors are for the new Transaction Manager microservice being split out of EthConnect (the reason for doing this work now)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 18:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/677" class=".btn">#677</a>
            </td>
            <td>
                <b>
                    Update manifest for v1.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 17:52:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/676" class=".btn">#676</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.10] manifest
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
        Created At 2022-04-08 17:29:57 +0000 UTC
    </div>
</div>

