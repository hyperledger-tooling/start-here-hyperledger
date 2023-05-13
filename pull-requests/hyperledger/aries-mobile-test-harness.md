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

