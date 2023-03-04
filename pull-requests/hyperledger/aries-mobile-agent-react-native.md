---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    docs : Design proposal document for Verifier functionality in Aries Mobile Agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR includes the proposed design document covering adding Verifier functionality in Aries Mobile Agent.
For some aspects, provided multiple options to choose which one will be included in the final design and implemented.

# Related Issues

BC Wallet Issue: https://github.com/bcgov/bc-wallet-mobile/issues/800

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 08:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/648" class=".btn">#648</a>
            </td>
            <td>
                <b>
                    feat: added connection image to proof & cred offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Added connection Image URL to proof request and credential offer page:

Note, I will need to change some of the images in the bc wallet demo since they're still pointing to some animo images
![Screen Shot 2023-03-01 at 3 33 58 PM](https://user-images.githubusercontent.com/36937407/222291327-45ba059a-897e-4baa-beaf-c46b11cf8c06.png)
![Screen Shot 2023-03-01 at 3 34 31 PM](https://user-images.githubusercontent.com/36937407/222291369-77d4fb88-ad9a-4ad9-a178-f0c9250d2bbf.png)

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 23:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/647" class=".btn">#647</a>
            </td>
            <td>
                <b>
                    fix: reset navigation stack for problematic screens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Resetting the navigation stack when navigating from problematic screens that we don't want users to be able to navigate back to (either with swipe back on iOS or hardware back button on Android)

# Related Issues

Resolves #460 

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 22:59:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    feat: added error message if biometrics fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Added error text to the PIN enter screen if the biometrics fails:
![image](https://user-images.githubusercontent.com/36937407/221679186-b3c83dd7-6a6c-43f6-b054-d1f93e5a17cb.png)


# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 20:33:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/645" class=".btn">#645</a>
            </td>
            <td>
                <b>
                    fix: improve scroll/keyboard use of create and enter pin scrns
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Refactored the create pin and enter pin screens so that they are uniform and use the same approach for keyboard handling. They now scroll nicely with the keyboard being hidden when the user taps outside of the keyboard in empty space and the buttons are kept at the bottom of the screen for easy access. 
Note 1: I also fixed some spacing issues, one of which included a lot of extra margin caused by the secondary logo being made very large by percentage-defined height and then resized while still taking up the same space. To do this I had to set the image height and width explicitly (it's only used in the one place.)
Note 2: I removed a redundant `AlertModal` in the enter pin screen. There was always a `PopupModal` over it with the same conditional logic
 
Prepare for a lot of gifs...

Create PIN screen, iOS, default:
![pin_create_ios](https://user-images.githubusercontent.com/32586431/221493834-d8caacc7-3294-4f2c-9b73-821a5cb33357.gif)
Create PIN screen, iOS, max zoom + font:
![pin_create_ios_zoom](https://user-images.githubusercontent.com/32586431/221493902-88be9e79-c0a6-4701-8da6-b68643bf01ab.gif)
Create PIN screen, Android, default:
![pin_create_android](https://user-images.githubusercontent.com/32586431/221493965-0ea55236-d747-4d2d-8904-08d00cd5191e.gif)
Create PIN screen, Android, max zoom + font:
![pin_create_android_zoom](https://user-images.githubusercontent.com/32586431/221494024-f68f2dd4-5e61-46f1-b8cb-99575b187aae.gif)
Enter PIN screen, iOS, default:
![pin_enter_ios](https://user-images.githubusercontent.com/32586431/221494132-a4b6b799-bf50-4a88-b9ac-149027e762e2.gif)
Enter PIN screen, iOS, max zoom + font:
![pin_enter_ios_zoom](https://user-images.githubusercontent.com/32586431/221494194-c51d2990-3a68-46eb-a7cd-8ca531ca1fbf.gif)
Enter PIN screen, Android, default - note that on Android, logo images don't show up during local development:
![pin_enter_android](https://user-images.githubusercontent.com/32586431/221494271-3771046b-2760-48a2-9b08-59cc505b3d63.gif)
Enter PIN screen, Android, max zoom + font:
![pin_enter_android_zoom](https://user-images.githubusercontent.com/32586431/221494470-b003e3cc-f2ba-4e67-a5b2-86fe19748f3c.gif)

Phew.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 06:57:07 +0000 UTC
    </div>
</div>

