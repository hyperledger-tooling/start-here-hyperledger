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
        Created At 2023-12-27 18:29:10 +0000 UTC
    </div>
</div>

