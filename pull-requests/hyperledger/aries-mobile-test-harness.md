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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/220" class=".btn">#220</a>
            </td>
            <td>
                <b>
                    Turned off flakey Offline BCW tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Temporarily broken Offline wallet handling tests until there is a chance to fix them. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 16:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    update final verified state check in OOB BCW test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added handling for the verified check in the OOB case in the BC Wallet tests. This will wait and try again if the proof is not verified in the first check. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 22:38:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    BCW added a verified check to the agent after the connectionless proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the OOB with proof attachment is now working, I've added the final check at the end of the proof to make sure the proof was actually verified. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 23:00:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    fixes to the connectionless oob tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This update fixes the BC Wallet tests in the OOB Connectionless proof scenario. Most important thing here is the added step to select the credential on the contact screen which was overlooked when the credential and proof flows were updated. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 19:20:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    update path for retrieving screenshots
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
        Created At 2023-11-28 21:47:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    updated wallet naming for android
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TestiD not working on Android for edit wallet name. Using accessibility id instead. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 18:29:17 +0000 UTC
    </div>
</div>

