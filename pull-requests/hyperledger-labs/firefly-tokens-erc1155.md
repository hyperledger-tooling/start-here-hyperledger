---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Add automated Docker builds
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
        Created At 2021-08-12 13:59:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Support deferred initialization
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
        Created At 2021-08-11 20:42:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Add README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 18:03:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Add GitHub action for unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 16:19:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    Include author in token-pool event
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
        Created At 2021-08-11 16:03:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Add Solidity contract and Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 20:17:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Initial code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The purpose of this repository is to provide a thin shim between [FireFly](https://github.com/hyperledger-labs/firefly) and an ERC1155 contract exposed via [ethconnect](https://github.com/hyperledger-labs/firefly-ethconnect). It must take logical inputs from FireFly (namespace, pool name & UUID, token type) and pack them into the standard fields provided by ERC1155 (token ID, URI). It must also take the events emitted from ERC1155 (URI, transfer) and map them to logical events needed by FireFly (pool creation, mint, transfer).

The API is very flat and non REST-ful at the moment, but open to input. The FireFly tokens API itself was proposed on [a recent community call](https://wiki.hyperledger.org/display/labs/2021-06-30+FireFly+Community+Call), but the API for this micro-service will have a much smaller service area and notably very few GETs (as the goal is for this service to be stateless). Ideally the exact same API will be used for future implementations built on other token contracts or chains.

Current proposed APIs:
* `POST /pool` - Create a new token pool (inputs: type, namespace, name, client_id)
* `POST /mint` - Mint new tokens (inputs: pool_id, to, amount)
* `POST /transfer` - Transfer tokens (inputs: pool_id, token_index, from, to, amount)
* `GET /balance` - Get token balance (inputs: pool_id, token_index, account)

All POST APIs are async and return 202 immediately, and results are reported by a websocket event of the form `{event: string, data: any}`, with the following event types:
* `token-pool` - Token pool created (outputs: pool_id, type, namespace, name, client_id)
* `token-mint` - Tokens minted (outputs: pool_id, token_index, to, amount)
* `token-transfer` - Tokens transferred (outputs: pool_id, token_index, from, to, amount)

The TypeScript code is tightly coupled to the Solidity contract in terms of how data is packed and unpacked. For the purposes of this first pass, [this reference contract](https://github.com/hyperledger-labs/firefly/pull/124/commits/7989ce583960fb040d68c855de8959a34f3685cb) is assumed, which is in turn based on a fungible/non-fungible [example from Enjin](https://github.com/enjin/erc-1155/blob/master/contracts/ERC1155MixedFungibleMintable.sol). The actual contract will be finalized for review in a future PR.

At a high level, the 256-bit token ID from the contract is used to pack the token type, pool ID, and (for non-fungible only) token index. The string URI from the contract is used to pack the FireFly data such as namespace, name, and UUID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 14:25:58 +0000 UTC
    </div>
</div>

