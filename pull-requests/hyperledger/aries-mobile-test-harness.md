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
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    testing if the CANdy BC Wallet tests will work without starting tunnels
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR is an attempt to see if the CANdy tests (which pass locally) will pass in the GitHub test pipeline if the tunnels are not started. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 19:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    fix for pervasive connection issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This BC WAllet Test PR changes the Sauce Connect tunnel to allow connections to the Prod Mediator instead of the Test Mediator. Switching to the Test env in the app doesn't switch to the test mediator, it remains on prod. 

There was also a new issue introduced in the previous PR that caused the send credential not to fire because the test code was waiting for the connecting image to disappear. That test code was moved to after the send credential. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 20:32:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    Fix for getting version element on settings page on iOS < 15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR works around a problem with the BC wallet where the testID does not show for the version label on the settings page. It now gets the elements by partial text. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 20:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Develop settings toggle to Test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>
This PR includes the following enhancements to BC Wallet tests and AMTH itself.

BC Wallet:

- Test environment Toggle to Test env for all tests

- Streamlined waiting for connecting, initializing, and cred offer

AMTH:
- The BasePage that every PageObject should inherit from now has a scroll_to_bottom() that may come in handy if you just need to get to the bottom of a page instead of scrolling to an element. 

- There is a new class called WaitCondition which is an ENUM. So instead of using the default `presence_of_element_located` in the find_by method, you can now use `element_to_be_clickable`, visibility_of _element_located`, or `invisibility_of_element_located`, the latter is great for waiting for temporary progress elements like loading, initializing, connecting, to disappear before continuing.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 22:10:45 +0000 UTC
    </div>
</div>

