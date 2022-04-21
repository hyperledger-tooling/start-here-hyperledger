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
                PR <a href="https://github.com/hyperledger/firefly/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    Format JSON errors from fftokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
Parse a JSON error of the form:
  {"error": "Bad Request", "message": "Field 'x' is required"}
into a message of the form:
  "Bad Request: Field 'x' is required"
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 01:04:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/747" class=".btn">#747</a>
            </td>
            <td>
                <b>
                    Add table name to debug on every SQL call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently we take the first three words of the SQL to try and provide a debug statement that's useful, without printing the massive bundle of SQL. However, that is insufficient as for something like `SELECT` it just contains the first two fields from the select.

This PR introduces an explicit table name being passed on every call and put in the logs.

I did find what I think was one bug where `GetContractAPIs` was using the `contract_interfaces` table
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 21:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/746" class=".btn">#746</a>
            </td>
            <td>
                <b>
                    Resolve pool activation operations more cleanly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #743
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 20:26:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    Ensuring Senders Do Not Download Their Own Batches in Response to Pin Events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #694, we were seeing the sender's aggregator process pins before a batch was ever persisted. So although message confirmed events were still being sent by the dispatchers, the database updates to mark the message pending (what is done as part of persisting a batch) were occurring after the messages were already confirmed.

When persisting the batch, we guarantee that the batch is not cached until its successfully persisted:
```
	valid, err = em.validateAndPersistBatchContent(ctx, batch)
	if err != nil || !valid {
		return nil, valid, err
	}
	em.aggregator.cacheBatch(em.aggregator.getBatchCacheKey(persistedBatch.ID, persistedBatch.Hash), persistedBatch, manifest)
	return persistedBatch, true, err
```

so if the aggregator repolls any pins who's batch is not in the cache this should avoid the issue. Other option is instead of repolling, letting the aggregators rewind handle processing the pins.

See https://github.com/hyperledger/firefly/pull/745/files#discussion_r854706368 for a more up-to-date explanation of the cause and fix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 17:26:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/742" class=".btn">#742</a>
            </td>
            <td>
                <b>
                    Update dependencies for v1.0.0-rc.5 release
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
        Created At 2022-04-20 12:55:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/741" class=".btn">#741</a>
            </td>
            <td>
                <b>
                    UI v0.7.1
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
        Created At 2022-04-20 12:54:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/740" class=".btn">#740</a>
            </td>
            <td>
                <b>
                    Add first step of FireFly Transaction Manager support - separate URL for submit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the first step, to allow a URL to be specified, and use it only for `SendTransaction`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 12:18:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Add change events to operations, by adding namespace to ResolveOperation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR chain with #738 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 08:01:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    Merge wsconfig to wsclient so microservices can use it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 07:07:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/737" class=".btn">#737</a>
            </td>
            <td>
                <b>
                    Configurable JSON Formatter and Caller Reporting for Logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #713, useful for parsing logs w/ `jq` or searching through logs using log aggregators like Filebeat + OpenSearch

Using a slightly modified config from a default `dev` stack:
```yaml
log:
  level: debug
  reportCaller: true
  json:
    enabled: true
```

and running the image locally:

```shell
make docker
docker run -v ${HOME}/.firefly/stacks/dev/init/config/:/etc/firefly -it hyperledger/firefly -f /etc/firefly/firefly_core_0.yml
```

results in:

```json
{"@timestamp":"2022-04-20T04:53:12.477Z","file":"/firefly/pkg/config/config.go:528","func":"github.com/hyperledger/firefly/pkg/config.SetupLogging","level":"debug","message":"Log level: debug","prefix":"node_0"}
{"@timestamp":"2022-04-20T04:53:12.477Z","file":"/firefly/cmd/firefly.go:105","func":"github.com/hyperledger/firefly/cmd.run","level":"info","message":"Project Firefly","prefix":"node_0"}
{"@timestamp":"2022-04-20T04:53:12.477Z","file":"/firefly/cmd/firefly.go:106","func":"github.com/hyperledger/firefly/cmd.run","level":"info","message":"© Copyright 2021 Kaleido, Inc.","prefix":"node_0"}
{"@timestamp":"2022-04-20T04:53:12.479Z","file":"/firefly/cmd/firefly.go:159","func":"github.com/hyperledger/firefly/cmd.startFirefly","level":"debug","message":"Debug HTTP endpoint listening on localhost:6060","prefix":"node_0"}

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 05:02:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/734" class=".btn">#734</a>
            </td>
            <td>
                <b>
                    Add event for failed token pool creation operations
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
        Created At 2022-04-20 00:31:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/733" class=".btn">#733</a>
            </td>
            <td>
                <b>
                    Use blank type for JSONAny in OpenAPI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Type is unknown, as it may be any valid JSON.

See https://github.com/hyperledger/firefly-sdk-nodejs/issues/18
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 18:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    Accept "decimals" from token plugins on pool creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pairs with https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/46

This does not give any way to set `decimals` from FireFly when creating a pool, and it does not change the formatting of any values exposed on the FireFly API (ie for token balances). It simply accepts `decimals` if it is provided by a token connector upon pool creation, stores it, and returns it when querying token pools.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 16:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/730" class=".btn">#730</a>
            </td>
            <td>
                <b>
                    Allow config suffix to be changed by microservices using config package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 04:51:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/729" class=".btn">#729</a>
            </td>
            <td>
                <b>
                    Fix account creation for nightly integration runs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We recently merged a change in how blockchain accounts are created for the E2E tests. This worked fine for a normal run. The nightly integration test also stops all the services, starts them up again, and re-runs all the tests. This meant that there weren't enough "extra" test blockchain accounts allocated for the second test run after the restart. This PR fixes that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 01:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/728" class=".btn">#728</a>
            </td>
            <td>
                <b>
                    Adjustments to the FAQ documents page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Trevor Scanlon <trevorscanlon@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 20:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Fix image link in Sandbox docs
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
        Created At 2022-04-18 19:03:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Add "tx.blockchainId" to BlockchainEvent type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Every blockchain event will have a blockchain TX ID (such as an Ethereum
transaction hash), whether or not it has a FireFly transaction. This is
useful to record as another indexed field on the table.

It will also allow manually correlating blockchain events to FireFly transactions
in the case that the blockchain doesn't pass through enough data to do the
correlation based on FireFly IDs (such as custom smart contracts, ERC20 transfers
without a "data" argument, etc).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 17:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Parse input params for /query endpoints in ffi2swagger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #718
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 17:12:41 +0000 UTC
    </div>
</div>

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
                ~~In a PR chain with #720~~ (rebased now)

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

