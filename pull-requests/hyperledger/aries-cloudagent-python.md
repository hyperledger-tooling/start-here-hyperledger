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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1886" class=".btn">#1886</a>
            </td>
            <td>
                <b>
                    Use did:key for recipient keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of #1859, I have made it so the coordinate-mediation protocol uses did:key representation. Apologies that this took as long as it did. Implementing this impacted more of ACA-Py than I realized it would while keeping it compatible with existing agents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 18:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1885" class=".btn">#1885</a>
            </td>
            <td>
                <b>
                    fix: schema class can set Meta.unknown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables the Schema class of a model to determine the default `unknown` behavior. Without this, if you have a schema where you expect extra values to be present, every time `deserialize` or `serialize` is called, you must set `unknown=INCLUDE`. Now, in the `Meta` class of the Schema, `unknown` can be set to some value that will be respected as the default if not overrided by method parameter.

While I was at it, I also touched up some of the typing. I'm not fond of using `@overload` but I think it's the best way to address typing a method where a bool flag impacts the return type.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 16:54:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1881" class=".btn">#1881</a>
            </td>
            <td>
                <b>
                    fix: didx request cannot be accepted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi everyone,

this PR fixes a few problems which were apparently introduced by #1710:

- A didx request which is received in response to an explicit oob invitation cannot be accepted because the state of the corresponding connection record is not updated to `'request-received'`

- The admin api incorrectly indicates that the `/out-of-band/receive-invitation` endpoint returns a `ConnRecord` instead of the new `OobRecord` (which is also why the `OobRecord` is not included in the `swagger.json`)

@TimoGlastra: maybe you want to take a look to make sure I didn't break the connectionless exchange feature by saving the updated connection record?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 16:44:08 +0000 UTC
    </div>
</div>

