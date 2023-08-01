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

