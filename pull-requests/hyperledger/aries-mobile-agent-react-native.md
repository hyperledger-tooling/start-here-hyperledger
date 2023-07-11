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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/879" class=".btn">#879</a>
            </td>
            <td>
                <b>
                    fix: issue on mobile verifier after wallet lockout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously if the wallet timeout was reached and the user was locket out, it wouldn't close the wallet. This resulted in the mobile verifier feature not working, the loading screen would hang on the presenter side and they would never receive a proof request. I added functionality to close the wallet on a timeout and it seems to have resolved the issue.

https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/2f68f096-f14c-4d36-8a0c-fd6b038c0e18


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
        Created At 2023-07-10 19:47:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/878" class=".btn">#878</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tough-cookie from 4.1.2 to 4.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tough-cookie](https://github.com/salesforce/tough-cookie) from 4.1.2 to 4.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/salesforce/tough-cookie/releases">tough-cookie's releases</a>.</em></p>
<blockquote>
<h2>4.1.3</h2>
<p>Security fix for Prototype Pollution discovery in <a href="https://redirect.github.com/salesforce/tough-cookie/issues/282">#282</a>. This is a minor release, although output from the <code>inspect</code> utility is affected by this change, we felt this change was important enough to be pushed into the next patch.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4ff4d29f6cefd279a412b8d62a21142ebd410b36"><code>4ff4d29</code></a> 4.1.3 release preparation, update the package and lib/version to 4.1.3. (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/284">#284</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/12d474791bb856004e858fdb1c47b7608d09cf6e"><code>12d4747</code></a> Prevent prototype pollution in cookie memstore (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/283">#283</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/f06b72d1d447f33dfa6222c0a3c0c5e063558248"><code>f06b72d</code></a> Fix documentation for store.findCookies, missing allowSpecialUseDomain proper...</li>
<li>See full diff in <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.2...v4.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tough-cookie&package-manager=npm_and_yarn&previous-version=4.1.2&new-version=4.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 02:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/877" class=".btn">#877</a>
            </td>
            <td>
                <b>
                    feat: dev only templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Sheldon asked for Unverified Person templates for ease of testing, Decided to make them development only templates so they don't end up in prod.
- Added extra toggle on developer menu to include development templates
- Bound inputs so that when the dev templates toggle is on, verifier feature must be enabled. Conversely when the verifier feature is turned off, dev template must also be turned off 

https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/d2910669-c842-4501-b2da-3d351cb80ed2


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
        Created At 2023-07-07 21:02:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/876" class=".btn">#876</a>
            </td>
            <td>
                <b>
                    feat: adding toast notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Adding toast notifications to `Decline` action where they were missing:
- Proof Request
- Credential Offer

Before

https://github.com/hyperledger/aries-mobile-agent-react-native/assets/97122568/5f167b91-f093-4d80-926b-30fc7a6c2d87

Now

https://github.com/hyperledger/aries-mobile-agent-react-native/assets/97122568/fbb91d43-aec7-4743-9890-47dec74a7da4

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
- [X] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._











            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 18:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/875" class=".btn">#875</a>
            </td>
            <td>
                <b>
                    fix:fixing problem with the amount of attributes in the proof request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

When the proof request contains more than ten attributes, the card keep blinking. This happens because the `initialNumToRender` variable has a default value of ten.

Before

https://github.com/hyperledger/aries-mobile-agent-react-native/assets/97122568/d834cb28-d15a-43ba-bf62-f846b805dccf

Now

https://github.com/hyperledger/aries-mobile-agent-react-native/assets/97122568/9bff3a04-3eab-4cea-bd8f-031b638730b8

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
- [X] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 18:32:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/874" class=".btn">#874</a>
            </td>
            <td>
                <b>
                    fix: verifier notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously I removed mobile verifier notifications in the home screen. This change adds them back in as well as fixes bugs while viewing or deleting the notification.
<img width="389" alt="image" src="https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/6a43b5b7-6d9d-471c-98a4-a2e69ab95cff">
<img width="389" alt="image" src="https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/7cd2e0ef-20f1-4c4f-ae21-15b178e6e136">

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
        Created At 2023-07-06 17:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    fix: mob ver proof notif
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously the notification functionality was listing any proof record that was in the done state. This doesn't really make sense since the notification list is supposed to contain proofs and credential offers that haven't been completed yet. The functionality to list completed proof requests in the notification list has been removed

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
        Created At 2023-07-04 23:07:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/872" class=".btn">#872</a>
            </td>
            <td>
                <b>
                    fix: make sure walletName is not undefined when fetching from ls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously, if an older instance of the wallet that had already gone through onboarding was initialized it would have an undefined walletName in preferences, which would then overwrite the default value. This caused errors in connections because the label was missing. This fix is two-pronged, first it will convert undefined `walletName` values in localstorage to `generateRandomWalletName` when preferences are loaded, then it will use a backup value of `Aries Bifold` if `walletName` is still somehow undefined.

EDIT: I also removed the check for the wallet being named from the onboarding completeness check, so that older already-initialized wallets don't end up having to go back to onboarding. (Something I did for BC Wallet already but not for Bifold)

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
        Created At 2023-07-04 20:30:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    chore: add codecov
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add CodeCov checker to our quality workflow.

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
        Created At 2023-07-04 18:36:41 +0000 UTC
    </div>
</div>

