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
                PR <a href="https://github.com/hyperledger/firefly/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Do not return an error from status if node lookup fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In `v0.14.0` if you register your org (only), and then call `/api/v1/status` you receive:

```js
{"error":"FF10277: Identity could not be resolved via DID 'did:firefly:node/zzhc7hdmc0'"}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:15:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.3] v0.6.3 release of ui in manifest
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
        Created At 2022-03-25 19:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Simplfy solc compilation of BatchPin contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a slight simplification to the way the BatchPin contract is compiled at build time. This allows us to remove some deprecated code in the FireFly CLI and goes along with the changes in https://github.com/hyperledger/firefly-cli/pull/165
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 19:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Add pool config to activate call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/36
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 18:40:07 +0000 UTC
    </div>
</div>

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

