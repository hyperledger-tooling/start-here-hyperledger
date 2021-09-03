---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    Pack all token pool info into "data" field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The separate fields for the /pool API are going away. Any arbitrary
data should now be packed (as a JSON string) into the "data" field.

Depends on https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/19
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 17:00:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Fabric plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dependent on https://github.com/hyperledger-labs/firefly-fabconnect/pull/41

The plugin provides:
- `BatchPin` transactions and events support
- Identity resolution (note that pending enhancement for https://github.com/hyperledger-labs/firefly/issues/182 is left for a future PR given its significant implications to the identity plugin). For now these workaround are used when comparing the persisted tx signer with the event signer, which will be re-implemented as part of the solution for #182:
  - `internal/events/batch_pin_complete.go`: `subjectMatch()` 
  - `internal/events/persist_batch.go`: `persistBatchFromBroadcast()`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 22:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Add self-describing enum support to OpenAPI definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One step on the journey to #111, allowing us to list the possible values for an `FFEnum` type (renaming `LowerCasedType`).

This builds on a feature added to the OpenAPI schema generator in https://github.com/getkin/kin-openapi/pull/411

Using the same approach in follow-on PRs, we can:
- Add in field-level descriptions with translation keys
- Remove the need for hard-coded schemas for complex objects like `Message`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 14:13:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Only download lint if not present
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
        Created At 2021-08-31 15:59:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    Supply requestId when creating token pools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/18
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 15:45:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Add skeleton functionality for token accounts
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
        Created At 2021-08-30 20:50:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Read "operator" field instead of "author" for token-pool event
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
        Created At 2021-08-30 20:13:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    Align the "additional info" for blockchain and token transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Both will contain keys for blockNumber, transactionIndex, and transactionHash
(at least on Ethereum). Prune higher and lower level nested items from the
JSON body.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 19:58:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Remove unneeded "allowExisting" param from some db methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the param is always true, no need to have a param.

Note that token pools were sometimes erroneously passing false, but
should have been passing true (passing false would result in infinite
retries for a name conflict).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 18:40:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    Support multi-threaded "make mocks"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Generating mocks can be sped up significantly by splitting each file out
as a separate target and using e.g. "make mocks -j8".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 17:22:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    Add unit tests for tokens HTTPS plugin
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
        Created At 2021-08-27 20:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    Remove unnecessary streamID param to ethconnect
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
        Created At 2021-08-27 12:59:36 +0000 UTC
    </div>
</div>

