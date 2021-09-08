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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    bump ui to v0.2.4
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
        Created At 2021-09-03 13:26:04 +0000 UTC
    </div>
</div>

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

