---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1325" class=".btn">#1325</a>
            </td>
            <td>
                <b>
                    fix: error on deserializing conn record with protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes error when deserializing a connection record that has a `connection_protocol` value set:
```
marshmallow.exceptions.ValidationError: {'connection_protocol': ['Must be one of: c, o, n, n, e, c, t, i, o, n, s, /, 1, ., 0, d, i, d, e, x, c, h, a, n, g, e, /, 1, ., 0.']}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 20:01:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1324" class=".btn">#1324</a>
            </td>
            <td>
                <b>
                    Handle unpadded protected header in PackWireFormat::get_recipient_keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I believe this only affects connection establishment when using an Askar wallet together with multi-tenant wallets.

Fixes #1323 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 19:19:51 +0000 UTC
    </div>
</div>

