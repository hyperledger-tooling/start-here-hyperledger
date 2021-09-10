---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Split "contracts" package into "contractgateway" and "contractregistry"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The new "contractregistry" package has minimal dependencies and can be used from anywhere
to lookup contracts/ABIs, while the "contractgateway" package remains large and pulls in nearly
everything.

This will facilitate future enhancements where we want to do ABI lookups from outside the gateway
(such as from the "events" package).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:29:27 +0000 UTC
    </div>
</div>

