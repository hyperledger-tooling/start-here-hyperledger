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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Fix project LINTing and update husky
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

- Updated husky;
- Updated husky config to recommended `.husky` format;
- Added `lint-staged` package to LINT as pre-commit hook via husky;
- Ported commit message check to new husky format;
- Fixed LINT issues in existing code.

# Related Issues

Fixes #92 

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 22:16:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Expire old build cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

- Expire the old build cache to fix build issues on iOS due to outdated pod dependency;
- Align the iOS target version in the project (was 10, now 11) with the one specified in the Podfile (11.0).

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 17:38:56 +0000 UTC
    </div>
</div>

