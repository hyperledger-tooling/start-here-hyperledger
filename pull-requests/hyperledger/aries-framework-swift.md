---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Fix ack message expect response problem
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Checklist

- [x] have run AriesFrameworkTests
- [x] I have run AllTests

# Description

Some agents, such as aca-py, wait for a response from it's handler with holding the inbound transport when the transport decorator is received. So, when client sends ack message with transport decorator with return_route attribute, the result is that client get a connection timeout error.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 09:37:03 +0000 UTC
    </div>
</div>

