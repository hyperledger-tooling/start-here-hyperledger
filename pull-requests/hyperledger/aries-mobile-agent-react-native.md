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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1055" class=".btn">#1055</a>
            </td>
            <td>
                <b>
                    fix: in app guides orientation on ipad
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Potential fix for the orientation issues the in app guides have on ipads

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
        Created At 2024-01-02 19:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1054" class=".btn">#1054</a>
            </td>
            <td>
                <b>
                    feat: inject global screen configuration into core config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add more UI customization options by optionally customizing screen options from wrapper wallet

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [ ] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-31 15:01:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1053" class=".btn">#1053</a>
            </td>
            <td>
                <b>
                    fix: iOS app permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

iOS 14+ uses local network permissions at app start which triggers permissions package to start, incorrectly configured Podfile and outdated package version cause an exception trigger at iOS app startup
Updated `react-native-permissions` package and added configuration in Podfile
Also tested Android to make sure updating package doesn't affect the flow

![IMG_0272](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/46829557/62aee451-c763-42e2-99c2-164b13168254)


# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [ ] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-31 02:19:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1052" class=".btn">#1052</a>
            </td>
            <td>
                <b>
                    feat: disable sharing proof if it is in a bad state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

If a proof is not in the request-received state then it will error out when sending. I've added functionality to disable the share button if a proof is not in the request received state

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
        Created At 2023-12-29 19:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1051" class=".btn">#1051</a>
            </td>
            <td>
                <b>
                    fix:disabling going back function on connectionless proof flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Disabling going back function on connectionless proof flow.

### Expected behavior
Users should not exit this screen using the device's back button, just the home icon.

### Actual behavior
Users can go back and on android it shows up a black screen, on iOS returns to the scan screen.

### To fix
I added `gestureEnabled` for ios (didn't work on android) and `Backhandler API` for android, both already used in the project.
https://reactnavigation.org/docs/stack-navigator/#gestureenabled
https://reactnative.dev/docs/backhandler


https://github.com/hyperledger/aries-mobile-agent-react-native/assets/97122568/7c10d844-e5c3-4190-871e-dc279a89cb4f


# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
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
        Created At 2023-12-27 18:29:10 +0000 UTC
    </div>
</div>

