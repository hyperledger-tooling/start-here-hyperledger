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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    Only check for Camera Policy on iOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is an attempt to fix the connection timeout issue that is frequently happening on Android in the test pIpeline. I have removed the check for the Camera policy for Android since that does take a little time determining if we are on that page. That policy doesn't show on Android when the `autoGrantPermissions` is set in the appium config. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 20:28:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Fix BCW iOS 14 remove contact failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should fix an issue in the remove contact test where we try and select view on the credential revocation notification. On iOS 14 and below the testID is not displayed (this is an issue we have not found a solution to), so the element is retrieved based on a partial xpath match and then clicked.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 20:54:11 +0000 UTC
    </div>
</div>

