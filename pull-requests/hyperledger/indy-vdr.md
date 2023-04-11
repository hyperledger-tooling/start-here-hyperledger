---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    fix(js): return body as string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to prevent the reqId (which is a large number) from overflowing and changing

We were running into this when implementing endorsement and needing to get the body of a request and send it to another agent. ACA-Py / the python wrapper als returns a string representation of the request when calling body
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 09:22:21 +0000 UTC
    </div>
</div>

