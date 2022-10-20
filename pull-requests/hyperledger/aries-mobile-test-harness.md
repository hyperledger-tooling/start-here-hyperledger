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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    fix webdriver-manager package issue and calibrate to 447
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Webdriver-manager was updated on the 18th and issues in that library caused the BC Wallet test pipeline to fail completely. Reverted to the older version.

Also calibrated the BC wallet tests to build 447. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 00:23:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    restrict matrix entry in main run all runset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Added if condition to the main run all runset for BC Wallet test pipeline. That runset was running for all projects giving all the results for all tests in restricted runsets with different issuers. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 17:42:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    update to affect the BCSC runset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Update to for the BC Services Card/Person credential BC Wallet tests in the nightly test pipeline. Added `@wip` to unfinished scenarios and changed the tag set in the run command, along with updated credential names for the Person credential. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 21:02:40 +0000 UTC
    </div>
</div>

