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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    BCW fixed Give Feedback test for android
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was an issue with the BC Wallet tests where getting the EXIT locator on the feedback entry page was not locatable by the Accessibility id of EXIT on Android as it is on iOS. Changed the Android locator to XPATH with text of EXIT.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 13:43:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Feature/pin update test dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a suite of test scenarios for Change PIN in BC Wallet. It tests the Acceptance Criteria to Change a PIN and also goes through the error cases that are done on the PIN create functionality to make sure they behave the same here. 

Also slipped in here is a fix to a "magic number" that is a separator used for devices that swipe down for control panel and  devices that swipe up for control panel.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 20:23:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Fix for feature "Scan QR code to recieve a credential offer" in connect.feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Error existed**
Not able to find Scan button as the Biometric page was not handled 
![image](https://github.com/hyperledger/aries-mobile-test-harness/assets/79985154/711e4746-463f-43ec-8781-bf55eda5683c)

**Changes made**

> Added line to use biometrics
> Changed the way to find Allow button on IOS devices

Test Result
![image](https://github.com/hyperledger/aries-mobile-test-harness/assets/79985154/3ae0989e-55d1-4fd4-81b2-832586ccc9f2)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 22:33:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Appium upgrade remove mobileby
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A recent upgrade to appium-python-client (3.0.0) has removed some deprecated ways of doing a couple things that were still lingering around in the Aries Mobile Test Harness. This PR adjusts the Test Harness and the BC Wallet for this update. 

1/ In the Test Harness, we were still using desired_capabilities when creating the appium driver. This has been replaced with AppiumOptions. 

This may affect the LamdaTest and the localAndroid device handlers. So those may have to change as well. 

2/ MobileBy locator types has been removed and now only supports AppiumBy. All BC Wallet page objects and the test harness page object base class has been updated to use strictly AppiumBy. 

All users of AMTH will have to adjust their page objects if they have any lingering MobileBy references. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 18:23:36 +0000 UTC
    </div>
</div>

