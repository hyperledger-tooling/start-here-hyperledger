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
                PR <a href="https://github.com/hyperledger/firefly/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    Consistency in JSON/Blob codepaths for validation of "none" datatype
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In testing #207 we found the following error when using `validator: "none"` on a JSON upload of `data`, that was not seen on the BLOB upload.

```
FF10200: Unknown validator type: ‘none’
```

I found a discrepancy in the validation on upload between the two paths. This PR should reconcile that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 20:57:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    Add "created" field to token pools, add some extra E2E checks
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
        Created At 2021-09-27 20:47:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Announce token pool info via broadcast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than requiring all token pool metadata (namespace, name, id) to be written
to the blockchain, send it out via a broadcast message after creating the actual
pool on chain.
 
~~Note: this contains the commit from #210 as a pre-req.~~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 18:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    Move TokenPoolCreated handler into AssetManager
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
        Created At 2021-09-27 18:20:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    Factor out PersistTransaction helper
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
        Created At 2021-09-27 16:01:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Move various top-level folders for smart contracts into 'smart_contracts' folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moved these top-level contract folders to a consolidated `smart_contracts` directory, with sub-folders corresponding to the supported ledger protocol:

```
smart_contracts
  \_ fabric
  \_ ethereum
  \_ corda
```

Note that "smart contracts" is a commonly accepted term in all 3 communities (ethereum, fabric, corda)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 15:25:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    Allow null value with blob data, and allow "none" validator to tag datatype on unstructured data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #198 

- Fixes handling of `null` on `data.value` - including as part of a FORM post upload
  - Stored as the bytes `null` in the database (as today)
  - Does not contribute to the hash, when there is a blob
  - Returned as `null` in the JSON payload on `GET`
- Adds a new `validator` of `none`
  - Must be set explicitly - `json` remains the default
  - Disabled any checking of the `datatype.name`/`datatype.value` when set
  - Allows you to just use the `datatype` for tagging purposes, without validating the `value` JSON payload itself
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-25 06:00:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Docs updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix links and TOCs in docs
- Add new docs page
- Add new Hyperledger logo
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 17:40:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Remove references to labs
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
        Created At 2021-09-23 18:36:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    Use Operation ID for tracking ethconnect requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Transaction ID is longer-lived, while Operation ID is more appropriate for
a single request (since a transaction may contain multiple operations).

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 18:30:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Rename tokens "https" plugin to "fftokens"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The name "https" is too generic - the plugin represents a way to map token operations
like pool, mint, and transfer into a specific HTTP+websocket protocol. Therefore a
specific, unique name is appropriate.

Also changed the config key from "connector" to "plugin" (since its purpose is to
affect which plugin FireFly loads from the map).

Added migration paths for both changes so that the CLI and any existing stacks can
have time to be updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 14:41:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Add additional fields to TokenPool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All token pools should record the connector that created them, may optionally
include a token symbol, and may (in the near future) be linked to a message.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 00:50:30 +0000 UTC
    </div>
</div>

