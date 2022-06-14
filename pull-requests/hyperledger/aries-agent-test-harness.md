---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/510" class=".btn">#510</a>
            </td>
            <td>
                <b>
                    fix(afj): connection controller after oob
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this fixes creating connections in AFJ. There's some added complexity as AFJ doesn't return a connectionId anymore (only an oob id) when creating an invitation, but only when a request is received. I've fixed this for now by just returning the out of band id, and then looking for a connection based on the out of band id later on. 

This also adds an javascript-arm dockerfile that allows to run the AFJ container on m1 macs. Tried to create one for ACA-Py but didn't succeed yet.

Next up is tests for DIDExchange (which won't work with ACA-Py yet sadly) and ICv2 with indy credentials (which should work with ACA-Py!)

Fixes #503 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 08:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    Update services for cleaner execution and afgo-acapy interop support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 21:07:16 +0000 UTC
    </div>
</div>

