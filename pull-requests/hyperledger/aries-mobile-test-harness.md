---
layout: default
title: aries-mobile-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-test-harness
---

# aries-mobile-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    streamline the iOS scroll to bottom
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR streamlines the scroll to bottom function for iOS. Something changed in the infrastructure that now returns the different page xml even if it looks the same, we were using xml compare to determine if we were at the bottom of the page. This was causing some BC Wallet tests using this scroll to continue the scroll attempt to over an hour. The routine now checks for the last app element in the viewport and compares it to the before scroll last app element. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 21:17:04 +0000 UTC
    </div>
</div>

