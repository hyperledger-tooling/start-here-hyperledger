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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    Fix decline credential screen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Added the credential summary card to the declined screen as per designs.


![IMG_71BC2BB19A01-1](https://user-images.githubusercontent.com/390891/166338427-50ac68cb-facf-424c-8d0f-7de840933420.jpeg)


# Related Issues

na/

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
        Created At 2022-05-02 22:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    Various miscellaneous fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

Various style fixes including:
* Settings font size
* Empty credential list text
* Hides remove button in credential details until AFJ/hooks are updated
* Share button is hidden for proof request screen unless a valid proof can be presented

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [ ] Updated documentation as needed for changed code and new or modified features;
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
        Created At 2022-05-02 13:54:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    Shore up animations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Cleaned up credential pending and completed animations along with updates to the image assets.

# Related Issues

n/a

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
        Created At 2022-04-29 18:19:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    Bump cross-fetch from 3.1.4 to 3.1.5 in /core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [cross-fetch](https://github.com/lquixada/cross-fetch) from 3.1.4 to 3.1.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/lquixada/cross-fetch/releases">cross-fetch's releases</a>.</em></p>
<blockquote>
<h2>v3.1.5</h2>
<h2>What's Changed</h2>
<ul>
<li>chore: updated node-fetch version to 2.6.7 by <a href="https://github.com/dlafreniere"><code>@​dlafreniere</code></a> in <a href="https://github-redirect.dependabot.com/lquixada/cross-fetch/pull/124">lquixada/cross-fetch#124</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/dlafreniere"><code>@​dlafreniere</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/lquixada/cross-fetch/pull/124">lquixada/cross-fetch#124</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/lquixada/cross-fetch/compare/v3.1.4...v3.1.5">https://github.com/lquixada/cross-fetch/compare/v3.1.4...v3.1.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lquixada/cross-fetch/commit/c6089dfafc1fd6253b4d204d37c0439eea631cd0"><code>c6089df</code></a> chore(release): 3.1.5</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/a3b3a9481091ddd06b8f83784ba9c4e034dc912a"><code>a3b3a94</code></a> chore: updated node-fetch version to 2.6.7 (<a href="https://github-redirect.dependabot.com/lquixada/cross-fetch/issues/124">#124</a>)</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/efed703489d591eee76a15d12b088538d04f668b"><code>efed703</code></a> chore: updated node-fetch version to 2.6.5</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/694ff77b367cff4be7e16366988b394016717e88"><code>694ff77</code></a> refactor: removed ora from dependencies</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/efc5956f740440cf4684e982fd4ceef85f2a2c67"><code>efc5956</code></a> refactor: added .vscode to .gitignore</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/da605d5ab026e7986f6633307fbd3018f1eebb58"><code>da605d5</code></a> refactor: renamed test/fetch/ to test/fetch-api/ and test/module/ to test/mod...</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/0f0d51de7f07f5202ee9de472d88c71911da9cb9"><code>0f0d51d</code></a> chore: updated minor and patch versions of dev dependencies</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/c6e34ead1bb70845eccf9ec83c3144ccf4a73f2e"><code>c6e34ea</code></a> refactor: removed sinon.js</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/f524a522ecda60db99f57798beac8e7af3349580"><code>f524a52</code></a> fix: yargs was incompatible with node 10</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/7906fcf4c2d3fa300690baa72dc6b8fa30ac02ea"><code>7906fcf</code></a> chore: updated dev dependencies</li>
<li>Additional commits viewable in <a href="https://github.com/lquixada/cross-fetch/compare/v3.1.4...v3.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cross-fetch&package-manager=npm_and_yarn&previous-version=3.1.4&new-version=3.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 01:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Allow splash override
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Allow for Splash screen override and a few small tweaks after some refactoring.

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
        Created At 2022-04-27 23:09:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Fix animation and layout issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fixed a number of layout issues and test runs when animations are used:
- Fix style on connection screen;
- Fix tests with loop animations;
- Fix test warnings when Animations used;
- Shore up offer accept layout

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
        Created At 2022-04-26 22:12:21 +0000 UTC
    </div>
</div>

