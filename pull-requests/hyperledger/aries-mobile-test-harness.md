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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    BCW updated request and offer TestIDs on Contact page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the TestID locators on the contact page for the Credential Offer and the Proof Request view buttons changed in BC Wallet build 1087.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 13:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    fix: appium 2 alignment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR brings the Appium, Selenium, and WebDriver Manager libraries to the latest releases. This allows for the usage of Appium 2 in Sauce Labs (and other device cloud services if they support it).   This was done at the recommendation of Sauce Labs to isolate a skipped test issue in the nightly test pipeline for BC Wallet testing. 

There may be some repercussions here to other AMTH users and will need to be executed by someone using LambdaTest. If the library upgrades in requirements.txt work well LambdaTest then we can merge, if not, then LambdaTest support should be fixed or we can have separate requirements.txt files.  @fc-santos If you or someone on your team could check this that would be great?

@AmarjeetAkv Can you look at these in regards to NB?

There is one issue that is outstanding and that is on Apple Silicon with the proper workaround in place for the test harness container, Chromium will still not start in that container. Issue it still under investigation. It should be ok in the test pipelines in GitHub however. This affects any test that uses selenium to control a web based issuer or verifier. 
Closes #178 


This PR also slips in an update to the manage script to check for Apple Silicon and apply the workaround for docker containers on the platform.
Closes #180
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 19:16:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    BCW fix double call of open cred from contact
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 14:47:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    BCW fix QR Code border to allow scanning on iPad/tablets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the occasional inability of some tablets to scan the QR code from test agents. With the new BC Wallet full width iPad feature, on some devices the QR code was too big. This was solved by increasing the border of the QR code if the device is a tablet. This is done easily on iOS devices by checking the name, but android is a little more difficult and is using a pixel ratio to determine if it is likely to be a tablet. The threshold for this ratio may require some calibration, but the devices I tried worked with the existing threshold of 1.7.

Also snuck in here is a small fix to a revocation test that no longer looks for the ability to redisplay the revocation message. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 22:12:12 +0000 UTC
    </div>
</div>

