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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1960" class=".btn">#1960</a>
            </td>
            <td>
                <b>
                    fix: Safely shutdown when root_profile uninitialized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If an exception was thrown during the initialization of the root_profile, we would throw an exception during shutdown and fail to end the process. This would leave ACA-Py running, without accepting/handling any further requests. Adding guards for shutdown code that uses the root_profile should avoid this situation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 15:32:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1957" class=".btn">#1957</a>
            </td>
            <td>
                <b>
                    key type registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes key types pluggable to enable plugins to define and register new ones.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 23:15:15 +0000 UTC
    </div>
</div>

