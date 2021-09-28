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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/474" class=".btn">#474</a>
            </td>
            <td>
                <b>
                    feat(core): support multiple indy ledgers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for using multiple indy ledgers simultaneously. I'd really like some input on the approach before wrapping up and merging.

- Only supports multiple ledgers for reading, writing to the ledger still only supports one pool, which is currently always first configured pool.
- `genesisPath`, `poolName` and `genesisTransactions` in the `InitConfig` are replaced by the `indyLedgers` array property with the following structure: (@MosCD3)
- 
```ts
interface IndyPoolConfig {
  genesisPath?: string
  genesisTransactions?: string
  id: string
  isProduction: boolean
}
```
- caching is not implemented yet, I'll do that after validating the approach/implementation
- Algorithm to decide which ledger to use is based on this google doc by @swcurran: https://docs.google.com/document/d/109C_eMsuZnTnYe2OAd02jAts1vC4axwEKIq7_4dnNVA/edit#heading=h.564c8ed7spl8

Before each read operation in `IndyLedgerService` a new method is called, `IndyPoolService.getPoolForDid`. The method will, if successful, return the pool that should be used for the operation. The process is a follows:

1. If no pools are configured, an error will be thrown immediately
1. loop through all configured pools and performs a getNymRequest.
	1. If one of the responses is not successful, and is other than LedgerNotFound, an error will be thrown immediately. This means if one requests fails with an unknown error, the process fails. This is to prevent an incorrect pool from being returned.
	1. If all pools couldn't find the did, a LedgerNotFoundError will be thrown
1. A divide between production and non production ledgers is made.
	1. If there is one or more successful responses from production ledgers, this is assigned as the `remaining` group
	1. If there are no successful responses from production ledgers, and there are one or more successful responses from non production ledgers, the non production results are assigned as the `remaining` group.
1. If there is only one response in the `remaining` group, return the pool associated with the response
1. Loop through all `remaining` responses and check for each if the did is self certifying.
	1. If exactly one of the DIDs is self certifying, return the pool associated with it.
1. If there's still no pool selected, sort all items in the `remaning` group based on `txnTime`. The pool associated with the earliest `txnTime` will be returned.

@swcurran @shaangill025 I'm not so sure on 6. in the process. From the google document I understand that the txnTime is not the same as the time the DID was registered. In the HackMD document from @shaangill025 (https://hackmd.io/BVye073CTiqgNEMXxDeVdQ) the following step is described: "return production ledger with oldest/min datetime". Where does the oldest/min datetime property come from? I'd rather not have a service that tracks DIDs that are on multiple ledgers, and would be inclined to just throw an error instead that the DID couldn't be resolved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-26 21:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    fix(core): remove unused url import
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
        Created At 2021-09-23 12:56:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    docs: fix meeting time in readme and add link to meetings page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 22:40:56 +0000 UTC
    </div>
</div>

