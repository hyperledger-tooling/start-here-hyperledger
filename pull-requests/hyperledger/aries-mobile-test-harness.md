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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    updated onboarding process to BCW build 1279
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjust the tests for the BC Wallet onboarding process with a new preface screen and adjusted onboarding screens as of build 1279.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 19:57:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    BCW fix wallet name tets for small devices and enhance performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a wallet naming issue where if the device is smaller and we are testing null values in the wallet name field the iOS keyboard does not close and is over the save button, causing the click save to fail. 

This PR also speeds up the restart of the app to get ready for the test. It no longer checks if the biometrics page is displayed but check a boolean flag that was set when the wallet was setup.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-30 21:56:52 +0000 UTC
    </div>
</div>

