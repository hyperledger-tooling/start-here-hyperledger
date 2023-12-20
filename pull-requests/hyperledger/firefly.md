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
                PR <a href="https://github.com/hyperledger/firefly/pull/1433" class=".btn">#1433</a>
            </td>
            <td>
                <b>
                    Correct uniqueness lookup for nil location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's extremely hard for an external client calling the `AddContractListener` REST API to determine whether the listener already exists, because the details are a factor of a complex FFI payload.

For this reason FireFly provides a uniqueness check for the:
- `namespace`
- `topic` - allows multiple listeners to the same event, for different apps
- `location` - can be nil, or a blockchain-specific location
- `signature` - generated _by FireFly_ in a protocol specific way from the supplied FFI signature

However, the code doing a lookup in the DB was not working for the nil check, due to a `.ToString()`

Annoyingly there's a weirdness with `fftypes.JSONAny.Value()` in the `nil` case, and for some reason passing a `(*fftypes.JSONAny)(nil)` into `fb.Eq()` is not generating an `IS NULL` SQL query.

So instead this code passes actual `nil` in the nil case, and this works.

> This is really an underlying issue in `firefly-common` for a `ffapi.JSONField` case, but that's too risky a change to do in isolation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 00:56:29 +0000 UTC
    </div>
</div>

