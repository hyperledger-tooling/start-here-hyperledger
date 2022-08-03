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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Re-enable the sauce tunnel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Connecting to agents didn't work in the pipeline without the Sauce Connect Tunnel. Re-enabling it. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 23:09:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Fixed bcw init timeout and try pipeline without tunnel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

The BC Wallet test timeout check for initialization of the wallet was in the wrong location and would never get checked. 

Also removes the Sauce Tunnel from the test pipeline to see if the android runs will work better on initialization. iOS has no issue. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 16:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    added a 5 minute timeout to the bc wallet initialzation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

The BC wallet has no timeout on the app initialization. When the tests have an issue connecting to the mediator, initialization can go on for hours, resulting in jobs getting cancelled in the test pipeline. This PR add a 5 minute default timeout on initialization.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 23:29:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    fixed biometrics call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

The biometrics authentication calls were ignoring the boolean passed into the handler. Fixed that. 

Found a couple of changed test IDs in the BC wallet revocation page objects. And also fixed an isolated scrolling issue on android for a BC Wallet test. 

Moved fullReset from a hard coded value in the capabilities to the json files. This will allow keeping the app installed in its post test state which may be useful for debugging. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 22:09:56 +0000 UTC
    </div>
</div>

