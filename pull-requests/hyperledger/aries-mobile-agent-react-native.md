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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/1056" class=".btn">#1056</a>
            </td>
            <td>
                <b>
                    fix: adjust safeareaview and remove unneeded styles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fixes button placement on verifier proof requesting screen. See below

Old:
![proof_requesting_old](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/86dd7815-cb53-43d9-96de-7f2432145b1d)

New: 
![proof_requesting_new](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/ebd7c8b0-81cd-46cb-a59e-1ac0a2006614)

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
        Created At 2024-01-03 21:24:01 +0000 UTC
    </div>
</div>

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

