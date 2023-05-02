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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/162" class=".btn">#162</a>
            </td>
            <td>
                <b>
                    BCW fix remove contact test to select testID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is for the BC Wallet Remove Contact test scenarios. The info/settings element for contacts has a new TestID and a changed accessibility label. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 13:43:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    BCW stop Scrolling for iOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR stops BC Wallet scrolling for iOS when a cred offer or proof request comes in. With large credentials it takes a long time to scroll. iOS will find the element anyway even if it is not in the viewport, unlike Android where scrolling has to happen. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 22:06:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    Fix BCW environment setting for security tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR changes the ending of the security tests for BC Wallet which use to go ahead and change the environment to the test env. There is no need to do that in these tests, and saves minutes off of each test to remove it. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 18:48:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    BCW Dismiss app guide in dev mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is for BC Wallet. The latest build, when dev mode is toggled redisplays the app guide on the home screen. This update dismisses that modal to continue with testing. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 10:57:21 +0000 UTC
    </div>
</div>

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

