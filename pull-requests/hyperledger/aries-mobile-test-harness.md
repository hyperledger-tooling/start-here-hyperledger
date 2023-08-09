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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    Handle BCW scan failures better
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This BC Wallet PR adds handling for scanning QR codes and following issue credential issues. 
When scanning a QR code, the wallet with sometimes says the QR code is invalid. At times, on android, it also just sits on the scan screen with no error. This update will now check for that, so a soft assert so that we are aware of an issue, close the scan screen, re-upload the QR Code to the device and scan again. 

If there is a problem accepting a credential offer. The tests will now check for that error, show the details if there are any, and then log it for debugging use later. 

If there is a problem initializing, the tests will now check for an error, show the details if there are any, then do a soft assert so that we are aware of the issue, and then retry initialization. 

This PR also externalizes the BCW test environments setting external of the test. So now you can specify an environment variable or a tag in the feature file to tell the tests to use a specific environment that is set in BCW developer settings. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 19:58:37 +0000 UTC
    </div>
</div>

