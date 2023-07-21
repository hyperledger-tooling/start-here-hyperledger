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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    Align BCW tests to new scan/connection flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the BC Wallet test flows to the new Scan and Connection workflow in the app. 

It also sneaks in a fix to another test that was still looking at the decline proof request done screen.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 21:45:30 +0000 UTC
    </div>
</div>

