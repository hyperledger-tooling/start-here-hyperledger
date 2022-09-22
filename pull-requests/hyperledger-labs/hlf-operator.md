---
layout: default
title: hlf-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-operator
---

# hlf-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-operator/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    Support for peer hostAliases in create and update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Let users specify host aliases, so that /etc/hosts on peer containers can be easily managed. Peers need to be able to resolve the ordering node names - needed when using Istio and no real DNS.
- Introduce peer update command - for now to let users change host aliases even after the peer has been created.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 19:53:49 +0000 UTC
    </div>
</div>

