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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    feat: add support for alias, label, and unknown issuer names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add support for connection alias, connection label, and a fallback to `Unknown` for issuer names (so we don't end up using their `connectionId` so often)

What it looked like before:
![IMG_0017](https://user-images.githubusercontent.com/32586431/228086257-f47e3669-379a-47e8-b95f-5f85259a016f.PNG)
What it looks like now:
![IMG_0018](https://user-images.githubusercontent.com/32586431/228086299-aafb7cca-c389-4dbd-8a02-706b1abca7d7.PNG)

# Related Issues

#660

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
        Created At 2023-03-27 23:04:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/679" class=".btn">#679</a>
            </td>
            <td>
                <b>
                    fix: Re-run CI checks on PR Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fixes the CI to re-run checks (quality and mobile builds) on updates to PRs

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
        Created At 2023-03-24 16:08:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/673" class=".btn">#673</a>
            </td>
            <td>
                <b>
                    chore: add namespace to indy ledgers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes
- Add namespace identifier to indy ledger genesis files
- Up the minimum version of node to 18.5 (latest stable)

This is to comply with the DID Indy specs having a namespace portion for faster parsing of sub name spaces
The debate here might be to use "-" versus ":" in su namespaces, in AFJ test suite, I found them using "-" while in the RFCs I found ":" this needs a discussion in Bifold sync meetings

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 12:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/672" class=".btn">#672</a>
            </td>
            <td>
                <b>
                    fix: text wrap for cred name + issuer name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Recently updated credential style allowed longer text (for cred name and issuer name) to go off the screen. This fixes that

Old (broken) branded creds:
<img width="374" alt="branded_broken" src="https://user-images.githubusercontent.com/32586431/226756576-835e987e-d4c1-4163-a160-9246f8912f64.png">
Old (broken) generic creds with long issuer name:
<img width="377" alt="generic_broken" src="https://user-images.githubusercontent.com/32586431/226756636-d12a7b25-eda1-470b-a07e-47bd22a6ee88.png">
New (fixed) branded creds:
<img width="374" alt="branded_fixed" src="https://user-images.githubusercontent.com/32586431/226756694-5cd29772-e809-46eb-a2fa-15998b85f87d.png">
New (fixed) generic creds with long issuer name:
<img width="371" alt="generic_fixed" src="https://user-images.githubusercontent.com/32586431/226756757-25af297c-9a06-40ff-98cf-14a80bf0926d.png">

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
        Created At 2023-03-21 22:33:56 +0000 UTC
    </div>
</div>

