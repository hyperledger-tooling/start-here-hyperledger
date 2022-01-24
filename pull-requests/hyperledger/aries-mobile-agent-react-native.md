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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Display credential offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

* Add full notification screen modals and navigation changes for credential offer workflow
  - Modals include a pending, credential received and credential arrived
  - Modal component is generic and reusable
* Refactors some navigation params into exported module
* Adds unit tests for credential offer workflow

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 17:29:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    Misc cleanup and fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

- Removed old `globalStyles.ts` file;
- Set the root stack tab bar text color for onboarding;
- Fixed theme color name in `Button.tsx`

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 23:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Renaming cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

General app cleanup:
* Group react components under `components/` folder
* Group helpers into utils
* Group provider and context related files into `store/' folder
* Align file renaming (camelCase for `.ts` files, PascalCase for `.tsx`) 

# Related Issues

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 16:59:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    Refactor stack params into separate file to prevent import cycle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

Refactors stack params from screens to exported module in an effort to remove import cycles and to keep app components focussed.

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 16:32:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    Displays invalid QR code message on scan screen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

* Displays an 'Invalid QR code' message on the Scan screen if one is encountered. Message remains displayed until a valid QR code is scanned.
* Introduces throwable QRCodeScanError 
* Updates Color theming file

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 23:14:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    Style terms and conditions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add styling and bring Theme through the terms and conditions screen.

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 22:50:45 +0000 UTC
    </div>
</div>

