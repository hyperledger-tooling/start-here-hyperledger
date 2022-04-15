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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1729" class=".btn">#1729</a>
            </td>
            <td>
                <b>
                    feat: allow querying default mediator from base wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 16:57:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1726" class=".btn">#1726</a>
            </td>
            <td>
                <b>
                    Use provided connection_id if provided
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue https://github.com/hyperledger/aries-cloudagent-python/issues/1703

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 21:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1725" class=".btn">#1725</a>
            </td>
            <td>
                <b>
                    feat: create new JWT tokens and invalidate older for multitenancy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tokens will now include an `iat` value which is also stored in the wallet record. If the `iat` of the JWT doesn't match the user won't be authorized. This means when a new token is created (using the multitenant apis) the old token becomes invalid.

Looking for some input if this is a desired approach. It is a breaking change as previously you would always get the same token, while now you always get a new token revoking the older tokens.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 14:55:14 +0000 UTC
    </div>
</div>

