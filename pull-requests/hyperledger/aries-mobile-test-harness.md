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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    workaround for iOS input fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR implements a workaround for a problem in the BC wallet PIN Creation screen with iOS where input fields may have multiple elements with the same accessibility id (label). We now do a get elements (plural) and pick the one for the input before we do a sendKeys(). This is a workaround and hopefully we can get a build where the accessibility id is unique. However, it may be an idiosyncrasy with iOS.

For AMTH in general this PR contains an update to BasePage with a new method to get the multiple elements by accessibility id. fyi @dipeshnb
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 00:53:11 +0000 UTC
    </div>
</div>

