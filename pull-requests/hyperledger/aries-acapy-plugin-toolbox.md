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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    feat: Add revocation support to credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently running into an error saving credentials with the `support_revocation` flag. Data appears to be successfully received from the client, however, saving the details is another matter. Every time the credential definition is retrieved by the toolbox, `support_revocation` is set to `false` (the default value).

Signed-off-by: Colton Wolkins <colton@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 19:56:48 +0000 UTC
    </div>
</div>

