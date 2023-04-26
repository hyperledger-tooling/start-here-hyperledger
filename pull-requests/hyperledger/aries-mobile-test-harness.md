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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    Fix Test harness BasePage iOS scroll_to_bottom
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an iOS scroll_to_bottom issue where it would occasionally fail, this is because the x and y of the window rect would come back as zeros in some cases. Now with iOS it does comparison on page source at after a scroll to determine is it is at the bottom. 

This PR also contains a fix to the BCW app guides select dismiss button. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 20:26:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    Calibrate Tests to BCW build 318
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR Accounts for the new In App Guide selection that shows on the Home page when the app starts. At this point it just dismisses the guide selector to continue with the tests. App Guide tests will come in the future. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 15:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    Turn off retry attempts on failure for BCW tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR turns off the Test Failure Retry Attempts. The BC Wallet iOS full test run is taking up to 6 hours to run and is getting cancelled. This should cut the time down for the run so it doesn't get cancelled. When test failure are more infrequent, this can be turned back on.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 18:13:18 +0000 UTC
    </div>
</div>

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

