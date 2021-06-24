---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Fix peeradd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I found that `addSecureContext` was not reliably causing a working TLS context on startup of the firefly CLI with the e2e test.
It looks like simplifying to `setSecureContext ` instead (without supplying a particular hostname) is the right thing to do.

Note in PR chain with #25
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 17:47:32 +0000 UTC
    </div>
</div>

