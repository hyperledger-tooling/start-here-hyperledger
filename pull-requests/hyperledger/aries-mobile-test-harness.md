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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    updated bc wallet tests to build 317
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Moved tests forward to build 317 adjusting test IDS on credentials and handling biometrics on all tests. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 23:51:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Fix error in import for security
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR removes an unnecessary import in the security tests that was causing the nightly runs to fail. 

It also adds the extra camera message handling to the connectionless test scenario.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 00:28:49 +0000 UTC
    </div>
</div>

