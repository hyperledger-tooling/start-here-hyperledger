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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/170" class=".btn">#170</a>
            </td>
            <td>
                <b>
                    BCW remove credential declined page object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The BC Wallet has changed the flow when declining a cred or proof, there is no longer a final Credential Declined page. When the credential decline is confirmed, it goes directly to the Home screen. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 19:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    Anchor Appium at 2.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Android test may fail with 2.9.1+ of the Appium Python Client. The BCW tests that restarted the app, gave a message Unknown mobile command "activateApp". Pinning at 2.9.0 resolved this issue. May be able unpin when this issue is fixed in the library. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 18:17:53 +0000 UTC
    </div>
</div>

