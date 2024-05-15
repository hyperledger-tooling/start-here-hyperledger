---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    [log] WithLogFields for Configuring Larger Logging Contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In several case, one might want to set several key value pairs on the context. Currently you have to chain together nested `WithLogField` funcs to do so, which isn't very readable or user friendly.

This allows the users to do so with just a list of strings. Otherwise we could require a `logrus.Fields` struct to be directly provided if we want to avoid the odd-number-check-and-panic ?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 16:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    DB-side UPSERT optimiziation support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ... still a little more work to do on this one
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 23:07:52 +0000 UTC
    </div>
</div>

