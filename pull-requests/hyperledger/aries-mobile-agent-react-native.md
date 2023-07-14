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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/885" class=".btn">#885</a>
            </td>
            <td>
                <b>
                    fix: add iPad and iOS simulator support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR addresses a few changes around adding support for the iOS tablets (iPads) to better alight with the supported Android devices (Android supports tables by default). Changes include:

- enable iPad support for iOS;
- enable iOS simulator support (iPad and iPhone);
- fix the tab button layout on tablets;
- fix the QR size on tablets (somewhat smaller on tablets).



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
        Created At 2023-07-13 18:13:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    fix: chat details for cred and proof notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fixed the chat message detail button not showing up in certain instances when it should. Also changed the display logic on the proofDetails screen to allow holders to review their proof information after they've sent it.

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
        Created At 2023-07-13 00:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/883" class=".btn">#883</a>
            </td>
            <td>
                <b>
                    feat: implement the remote OCA resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Implementing the remote OCA resolver.

# Related Issues

#676 

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
        Created At 2023-07-12 16:52:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    chore(deps): bump semver from 5.7.1 to 5.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) from 5.7.1 to 5.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v5.7.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">5.7.2</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/585">#585</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>) (<a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/v5.7.2/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">5.7.2</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/585">#585</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>) (<a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>5.7</h2>
<ul>
<li>Add <code>minVersion</code> method</li>
</ul>
<h2>5.6</h2>
<ul>
<li>Move boolean <code>loose</code> param to an options object, with
backwards-compatibility protection.</li>
<li>Add ability to opt out of special prerelease version handling with
the <code>includePrerelease</code> option flag.</li>
</ul>
<h2>5.5</h2>
<ul>
<li>Add version coercion capabilities</li>
</ul>
<h2>5.4</h2>
<ul>
<li>Add intersection checking</li>
</ul>
<h2>5.3</h2>
<ul>
<li>Add <code>minSatisfying</code> method</li>
</ul>
<h2>5.2</h2>
<ul>
<li>Add <code>prerelease(v)</code> that returns prerelease components</li>
</ul>
<h2>5.1</h2>
<ul>
<li>Add Backus-Naur for ranges</li>
<li>Remove excessively cute inspection methods</li>
</ul>
<h2>5.0</h2>
<ul>
<li>Remove AMD/Browserified build artifacts</li>
<li>Fix ltr and gtr when using the <code>*</code> range</li>
<li>Fix for range <code>*</code> with a prerelease identifier</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/f8cc313550691a50d9662d8c94f0c033717efd7d"><code>f8cc313</code></a> chore: release 5.7.2</li>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> fix: better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/deb5ad51bf58868fa243c1683775305fe9e0e365"><code>deb5ad5</code></a> chore: <code>@​npmcli/template-oss</code><a href="https://github.com/4"><code>@​4</code></a>.16.0</li>
<li>See full diff in <a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~lukekarrys">lukekarrys</a>, a new releaser for semver since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=semver&package-manager=npm_and_yarn&previous-version=5.7.1&new-version=5.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-07-12 09:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/881" class=".btn">#881</a>
            </td>
            <td>
                <b>
                    feat: add new feature flagged scan screen flows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Now, if you enable connection invitations in developer settings, there are few new features. There is now a menu option to share your QR code, an additional header button to add contacts, and a new two-tab scan screen where you can tab between scanning other people's QRs and sharing your own. Upon successful scanning of a shared QR code, both users are propelled to the chat screen through the connection screen. It's so fast that you don't really see the connection screen (loading screen basically) but oh well.

Here is what it looks like: 
![new_scan_screen](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/ec239144-fd24-42a2-8a72-f8cfb96008f1)

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
        Created At 2023-07-12 03:08:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    feat: restore verifier flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

becuase we didn't have goal codes set up before, when Jason implemented the changes to the connection flow, he had to remove the loading screen functionality in the mobile verifier flow. This PR restores the origional flow and adds a hook to fetch the oob record from a conneciton ID which gives you the goal code. 

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
        Created At 2023-07-11 22:34:13 +0000 UTC
    </div>
</div>

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

