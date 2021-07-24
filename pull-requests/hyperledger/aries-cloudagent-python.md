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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1331" class=".btn">#1331</a>
            </td>
            <td>
                <b>
                    Initial DIDComm v2 envelope support via Askar backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also cleans up and relocates the (incomplete) in-memory ECDH-1PU support.

This does not make the DIDComm v2 envelope format(s) available for communication yet, it only establishes some of the basic functionality.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 20:10:36 +0000 UTC
    </div>
</div>

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

