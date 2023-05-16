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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Fix BCW security tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR fixes some test errors resulting from some BC Wallet PIN entry screen rework recently. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 20:55:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    feat: Add LambdaTest support to manage script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## New Features ##

* Added script for uploading app to LambdaTest
* Added new device service handler for LambdaTest
* Added new json config for LambdaTest (Android & iOS) 

### Important ###

LambdaTest only supports at the moment [camera image injection](https://www.lambdatest.com/support/docs/camera-image-injection/). Biometrics is not a feature that this platform can offer for now.

Also, for iOS the minimum platformVersion they have for real devices is 14, which needs to be considered since the wallet app has the target configured for minimum deployments at 11.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 15:26:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    pin selenium at 4.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR sets the selenium version to 4.9.0 since 4.9.1 caused driver not to instantiate in the test harness. This can be removed when 4.9.1 is fixed. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 20:52:36 +0000 UTC
    </div>
</div>

