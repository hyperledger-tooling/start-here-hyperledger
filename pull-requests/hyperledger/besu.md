---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6080" class=".btn">#6080</a>
            </td>
            <td>
                <b>
                    Implement miner_setMinPriorityFee and miner_getMinPriorityFee
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Built on top of https://github.com/fab-10/besu/tree/min-priority-fee, which adds `--min-priority-fee` CLI option

Adds two new JsonRPC methods: 

- miner_setMinPriorityFee - Sets the value of `miningParameters.minPriorityFeePerGas`
- miner_getMinPriorityFee - Returns the current value of `miningParameters.minPriorityFeePerGas`

This PR does not add the transactionSelector based on `minPriorityFeePerGas`. It will be added in a different PR

Examples: 

Example:  
Request
`{"jsonrpc":"2.0","id":1,"method":"miner_setMinPriorityFee","params":[1]}`
Response:
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": true
}
```
Invalid request: 
` {"jsonrpc":"2.0","id":1,"method":"miner_setMinPriorityFee","params":[-1]}
`Response:
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": false
}
```
Get method:
` {"jsonrpc":"2.0","id":1,"method":"miner_getMinPriorityFee","params":[]}
`Response:
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": 7
}
```




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 22:53:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6079" class=".btn">#6079</a>
            </td>
            <td>
                <b>
                    Force tx replacement price bump to zero when zero base fee market is configured
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR allows to replace txs on zero base fee markets, or on gas price network, where the txs have gas price set to zero (with `min-gas-price=0`).

To achieve that we force the `tx-pool-price-bump=0` when the `zeroBaseFee:true` genesis option is present.
But this was not enough, since the transaction replacement rules were forcing the new price to be strictly greater than the price bump, that in my opinion is not intuitive, since for example if your existing tx has a gas price of 100, and the price bump is 10%, then we should accept a valid replacement a tx with a gas price of 110, and not 111 as it was before.
So the other change is to accept, as valid replacement, tx with a gas price greater than or equal to the price bump. This make also the `tx-pool-price-bump=0` case more intuitive, since you can replace a tx without increasing the gas price.

`doc-change-required` to explain that if `zeroBaseFee:true` in the genesis, then `tx-pool-price-bump=0` is forced internally, and any attempt to specify a value for it results in an error

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #6043
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 19:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6078" class=".btn">#6078</a>
            </td>
            <td>
                <b>
                    ETC 'Spiral' network upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds support to [ECIP-1109](https://ecips.ethereumclassic.org/ECIPs/ecip-1109).
Block number is set to https://github.com/ethereumclassic/ECIPs/pull/514, already set in core-geth in https://github.com/etclabscore/core-geth/pull/571
I also set the DNS discovery tree to what's in [core-geth#bootnodes_mordor.go](https://github.com/etclabscore/core-geth/blob/v1.12.14/params/bootnodes_mordor.go#L29)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 18:48:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6074" class=".btn">#6074</a>
            </td>
            <td>
                <b>
                    Trigger contextEnter/Exit for all frames, including root
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Filtering out the root context from the `context{Enter,Exit}` tracing hook leads to an asymmetry of treatment when returning from a create/call context, where the root context is blind to the event, but non-root contexts can read it.

This PR disables this restriction to address this blindspot.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-23 22:44:58 +0000 UTC
    </div>
</div>

