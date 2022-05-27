---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Update common, and defer parsing of from address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `Transaction` definition in the `ethsigner` package is very useful, but it is currently opinionated that the `from` field must be an ethereum address, which in some situations in other packages might not be true.

So this changes the field to be a `json.RawMessage` to defer parsing, and now only code that explicitly needs that value to be an address performs the parsing.

This PR also updates the dependencies - including migrating the config to the new `Section` (vs `Prefix`) terminology in `firefly-common`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 14:55:26 +0000 UTC
    </div>
</div>

