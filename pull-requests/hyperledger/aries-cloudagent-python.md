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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1439" class=".btn">#1439</a>
            </td>
            <td>
                <b>
                    Fixed potential deadlocks by opening sessions only on demand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removed potential deadlocks in Multitenancy, Issue credential v2, Present proof v2 and mediation protocols by opening sessions on demand and closing them asap.

Additional info in this issue: https://github.com/hyperledger/aries-cloudagent-python/issues/1417
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 10:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1438" class=".btn">#1438</a>
            </td>
            <td>
                <b>
                    fix: incorrect return type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small fix in the type hinting of the store_credential method

In general I think it may be good to look into static type checking tools for ACA-Py. E.g. tools like [pyright](https://github.com/microsoft/pyright) can help find errors in typing (and thus implementation)

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 07:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    Fix issue with cred limit on presentation endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue https://github.com/hyperledger/aries-cloudagent-python/issues/1436
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 23:24:01 +0000 UTC
    </div>
</div>

