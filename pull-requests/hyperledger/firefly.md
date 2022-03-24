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
                PR <a href="https://github.com/hyperledger/firefly/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Re-read configuration on restart of orchestrator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that we are using more standard deployment of Ethereum contracts in the FireFly CLI, where a unique Eth address is generated each time, we need to set that configuration.

Rather than having configuration like this that's only in the DB, this PR proposes we re-read the configuration after the reset to pick up patched YAML configuration containing the instance address.

We still need to use the `preInit` trick in the CLI to let it start in a zombie mode so Docker compose is happy, while we're using EthConnect to deploy the contract, but the only thing we use the DB config patch for is to unset this flag (which is true already today).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 03:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    [fetchreferences2] Adding event enrichment for all event types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `GET /events?fetchreferences` now returns enriched events for all event types:

```go
type EnrichedEvent struct {
	Event
	BlockchainEvent   *BlockchainEvent `json:"blockchainevent,omitempty"`
	ContractAPI       *ContractAPI     `json:"contractAPI,omitempty"`
	ContractInterface *FFI             `json:"contractInterface,omitempty"`
	Datatype          *Datatype        `json:"datatype,omitempty"`
	Identity          *Identity        `json:"identity,omitempty"`
	Message           *Message         `json:"message,omitempty"`
	NamespaceDetails  *Namespace       `json:"namespaceDetails,omitempty"`
	TokenApproval     *TokenApproval   `json:"tokenApproval,omitempty"`
	TokenPool         *TokenPool       `json:"tokenPool,omitempty"`
	Transaction       *Transaction     `json:"transaction,omitempty"`
	TokenTransfer     *TokenTransfer   `json:"tokenTransfer,omitempty"`
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 19:12:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.0-release] new ui release
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
        Created At 2022-03-22 17:24:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.0] PR for new UI release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Will get exact release hash once it's released
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 14:05:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Add route to lookup identity by DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #583

This is more of a starting point - the functionality works, but I'm pretty certain the API spelling is not what we want.

I was struggling with the best way to provide this functionality - it seems like it must be a query param, because `/` is a valid char for query params but not for path params. Assuming we do use a query param, it would also be nice to flag it as "required" from the Swagger perspective.

Side note: you can already query the `/namespaces/{ns}/identities` endpoint with a query param for `did`, but you have to know the namespace you're looking for in that case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 21:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Change node/org lookups to support name or ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #583
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 21:20:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Update microservices versions for v0.14.0
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
        Created At 2022-03-18 20:06:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Dependency updates for v0.14 testing
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
        Created At 2022-03-18 16:32:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    [blockchainevents-charts] support for blockchain event charting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding support for blockchain event charting, so that the new UI can include blockchain event histograms.
This was a bigger change than expected since blockchain events have no `type` field, and are also timestamped by a `timestamp` field rather than a `created` field. This resulted in a `getHistogramNoTypes()` method and a `getHistogramWithTypes()` method.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 12:25:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    Add E2E test support for ERC20/ERC721
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/33
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 03:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    Restart stack and re-run E2E tests in daily integration job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This does not affect the PR test runs - only the daily integration test job - or if a `RESTART` environment variable is set to `true`.

Resolves https://github.com/hyperledger/firefly/issues/566
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 15:58:09 +0000 UTC
    </div>
</div>

