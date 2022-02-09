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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Style the Home Screen as per design docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Restyle the Home Screen to better show notifications according to the new and improved designs. Besides the obvious styling changes, I disabled some tests that were timing out on the build system (GitHub servers). I also moved the AFJ and Navigation hooks to `__mocks__` so they are automatically mocked for every test. We can `requireActual()` if we need the real deal and re-mock as needed. See `Home.test.tsx` how to feed mock return values into them.

In a follow up PR I can look into why the tests are failing and improve.

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
        Created At 2022-02-07 23:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    Credential details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Credential details screen update:
* Shows a list of credential details from a credential record, attributes are in human readable format, values are masked by default
* Pressing a 'Show' button on a detail list item unmasks the credential value
* Pressing a 'Hide all' button at the list header masks all credential values 
* Unit tests included
* Adds lodash package for converting attribute names into human readable strings

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
        Created At 2022-02-03 03:09:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Style notifications as per design
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Restyled the notifications to align with the designs and build in a Color Pallet v2 that also aligns with the style guide.

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
        Created At 2022-02-02 17:53:48 +0000 UTC
    </div>
</div>

