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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    fixed onboarding issues on Android
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Fixed onboarding locator issues on Android. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 22:02:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    Speed increases to receiving credential in BC Wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR adds a speedier on_this_page() method on the page object base class. 
Also cleans some steps in receive credential in bc wallet that took overly long to execute.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 23:46:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    fixed onboarding and rev error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Fixed a revocation error when notification was on. 
Fixed the BC wallet onboarding page objects due to recent test changes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 19:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    pipeline execution cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR cleans some pipeline execution issues with imports, along with removing agent files that are no longer needed, and removing code from the manage script that is no longer needed. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 23:30:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Feature/offline handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial set of Offline handling of the BC Wallet tests. These may remain flaky on iOS until we are out of the crawl stage and the test code is refined to properly use swipe to toggle WiFi on control center on iOS. 
Android in SL has issues when coming back into a closed app, biometrics at times does not display.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 00:00:31 +0000 UTC
    </div>
</div>

