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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Added biometrics authrnticate after onboarding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Calibrating to BC Wallet build 404 required the addition of biometrics authentication right after selecting to enable biometrics and clicking continue. 

This PR also includes the removal of the Sauce Labs tunnel for android test, reverting back to ngrok, which seems to work better for android when scanning the QR code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 22:56:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    fix Android issues with modals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR fixes BC Wallet test issues. One is access to the underlying page object is not accessible on android when a modal is displayed. This is different than on iOS. 

The other issue is On android the credential receiving takes longer than iOS, so a timeout increase was done. 

Another issue was @wip security tests were running because of double `Scenario` clauses on the tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 19:48:30 +0000 UTC
    </div>
</div>

