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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Fix BCW iOS 14 remove contact failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should fix an issue in the remove contact test where we try and select view on the credential revocation notification. On iOS 14 and below the testID is not displayed (this is an issue we have not found a solution to), so the element is retrieved based on a partial xpath match and then clicked.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 20:54:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    BCW working revocation notification test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a BC Wallet related PR that adds a working revocation notification test scenario. The remaining revocation notification scenario set to WIP is blocked by a bug in BC Wallet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 16:11:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    Feature/remove contact test dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One working BC Wallet Test Scenario for Remove Contact. Others are stubbed into the feature file but will remain WIP until the Contacts UI is reworked. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 14:40:17 +0000 UTC
    </div>
</div>

