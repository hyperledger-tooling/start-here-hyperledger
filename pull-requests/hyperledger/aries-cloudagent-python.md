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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1880" class=".btn">#1880</a>
            </td>
            <td>
                <b>
                    Allow fully qualified class names for profile managers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a small oversight that prevents specifying a qualified class name as
wallet type.

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 10:14:07 +0000 UTC
    </div>
</div>

