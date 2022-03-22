---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Test the token transaction release function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR tests the token transaction release function that is triggered
when a context is cancelled due to a panic or an error returned by a view.
The test first locks a token and trigger the release, then
it tries to relock again the same token. The latter operation should succeed.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 14:59:23 +0000 UTC
    </div>
</div>

