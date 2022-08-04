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

