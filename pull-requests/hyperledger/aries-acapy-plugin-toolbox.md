---
layout: default
title: aries-acapy-plugin-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugin-toolbox
---

# aries-acapy-plugin-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugin-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    fix: acapy-endpoint.sh to send correct ws endpoint to ACA-Py
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was noticed that the Toolbox was "unable to connect" to the demos due
to the fact that the websocket endpoint was not set properly. When the
toolbox would attempt to discover the features of the ACA-Py instance,
it was sending the request to ws://host/ws (which isn't a valid
endpoint) instead of sending it to ws://host/.

Signed-off-by: Colton Wolkins (Indicio work address) <colton@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 19:16:41 +0000 UTC
    </div>
</div>

