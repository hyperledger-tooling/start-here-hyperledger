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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/522" class=".btn">#522</a>
            </td>
            <td>
                <b>
                    chore: add candy test and prod ledgers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add CANDy-test and CANDy-prod ledgers to Bifold. 

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
        Created At 2022-11-08 21:40:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/521" class=".btn">#521</a>
            </td>
            <td>
                <b>
                    chore(deps): bump @xmldom/xmldom from 0.7.5 to 0.7.9 in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@xmldom/xmldom](https://github.com/xmldom/xmldom) from 0.7.5 to 0.7.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/releases"><code>@​xmldom/xmldom</code>'s releases</a>.</em></p>
<blockquote>
<h2>0.7.9</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.8...0.7.9">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Properly check nodes before replacement <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/457"><code>[#457](https://github.com/xmldom/xmldom/issues/457)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/455"><code>[#455](https://github.com/xmldom/xmldom/issues/455)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/456"><code>[#456](https://github.com/xmldom/xmldom/issues/456)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/edemaine"><code>@​edemaine</code></a>, <a href="https://github.com/pedro-l9"><code>@​pedro-l9</code></a>, for your contributions</p>
<h2>0.7.8</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.7...0.7.8">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2>0.7.7</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.6...0.7.7">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Security: Prevent inserting DOM nodes when they are not well-formed <a href="https://github.com/xmldom/xmldom/security/advisories/GHSA-crh6-fp67-6883"><code>CVE-2022-39353</code></a>
In case such a DOM would be created, the part that is not well-formed will be transformed into text nodes, in which xml specific characters like <code>&lt;</code> and <code>&gt;</code> are encoded accordingly.
In the upcoming version 0.9.0 those text nodes will no longer be added and an error will be thrown instead.
This change can break your code, if you relied on this behavior, e.g. multiple root elements in the past. We consider it more important to align with the specs that we want to be aligned with, considering the potential security issues that might derive from people not being aware of the difference in behavior.
Related Spec: <a href="https://dom.spec.whatwg.org/#concept-node-ensure-pre-insertion-validity">https://dom.spec.whatwg.org/#concept-node-ensure-pre-insertion-validity</a></li>
</ul>
<p>Thank you, <a href="https://github.com/frumioj"><code>@​frumioj</code></a>, <a href="https://github.com/cjbarth"><code>@​cjbarth</code></a>, <a href="https://github.com/markgollnick"><code>@​markgollnick</code></a> for your contributions</p>
<h2>0.7.6</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/441"><code>[#441](https://github.com/xmldom/xmldom/issues/441)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/jftanner"><code>@​jftanner</code></a>, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/blob/master/CHANGELOG.md"><code>@​xmldom/xmldom</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.8...0.7.9">0.7.9</a></h2>
<h3>Fixed</h3>
<ul>
<li>Properly check nodes before replacement <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/457"><code>[#457](https://github.com/xmldom/xmldom/issues/457)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/455"><code>[#455](https://github.com/xmldom/xmldom/issues/455)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/456"><code>[#456](https://github.com/xmldom/xmldom/issues/456)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/edemaine"><code>@​edemaine</code></a>, <a href="https://github.com/pedro-l9"><code>@​pedro-l9</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.5...0.9.0-beta.6">0.9.0-beta.6</a></h2>
<h3>Fixed</h3>
<ul>
<li>Properly check nodes before replacement <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/457"><code>[#457](https://github.com/xmldom/xmldom/issues/457)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/455"><code>[#455](https://github.com/xmldom/xmldom/issues/455)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/456"><code>[#456](https://github.com/xmldom/xmldom/issues/456)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/edemaine"><code>@​edemaine</code></a>, <a href="https://github.com/pedro-l9"><code>@​pedro-l9</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.4...0.9.0-beta.5">0.9.0-beta.5</a></h2>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.4...0.8.5">0.8.5</a></h2>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.7...0.7.8">0.7.8</a></h2>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.3...0.9.0-beta.4">0.9.0-beta.4</a></h2>
<h3>Fixed</h3>
<ul>
<li>Security: Prevent inserting DOM nodes when they are not well-formed <a href="https://github.com/xmldom/xmldom/security/advisories/GHSA-crh6-fp67-6883"><code>CVE-2022-39353</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/xmldom/xmldom/commit/927392f627e8f9cf1ea051612c7996596a904c78"><code>927392f</code></a> 0.7.9</li>
<li><a href="https://github.com/xmldom/xmldom/commit/99cfe62576e563234b928db9305290dfb3a96c03"><code>99cfe62</code></a> fix: Properly check nodes before replacement (<a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/457">#457</a>)</li>
<li><a href="https://github.com/xmldom/xmldom/commit/a627fbcd8b75304abe9142ca963c25ca773685d7"><code>a627fbc</code></a> chore: Preconfigure &quot;patch&quot; version in release script</li>
<li><a href="https://github.com/xmldom/xmldom/commit/0d6e3a132ec6eb32a67cfca327477a2098d4b55c"><code>0d6e3a1</code></a> 0.7.8</li>
<li><a href="https://github.com/xmldom/xmldom/commit/74e25a6763cc6afd0100b82b137f78af649741f8"><code>74e25a6</code></a> fix: Restore ES5 compatibility (<a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/452">#452</a>)</li>
<li><a href="https://github.com/xmldom/xmldom/commit/fe5b043fd07bbfed7f039b77d0b9e1a1eb832a2a"><code>fe5b043</code></a> 0.7.7</li>
<li><a href="https://github.com/xmldom/xmldom/commit/8a3173dc3bb7edb8619e914b8a2d366cc7cc8401"><code>8a3173d</code></a> docs: Prepare CHANGELOG for 0.7.7</li>
<li><a href="https://github.com/xmldom/xmldom/commit/c02f786216bed70825f9a351c65e61500f51e931"><code>c02f786</code></a> Merge pull request from GHSA-crh6-fp67-6883</li>
<li><a href="https://github.com/xmldom/xmldom/commit/3ca016d7da634686dbcadd076dda07d28a8ffd45"><code>3ca016d</code></a> 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/b28e631b8bc42edca9df6eb68e5b84f78529b3cb"><code>b28e631</code></a> docs: Prepare CHANGELOG for 0.7.6</li>
<li>Additional commits viewable in <a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@xmldom/xmldom&package-manager=npm_and_yarn&previous-version=0.7.5&new-version=0.7.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-08 17:28:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/517" class=".btn">#517</a>
            </td>
            <td>
                <b>
                    fix: change the react-native dependency version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thiago Romano <thiagoromano.s@gmail.com>

# Summary of Changes

When trying to compile the android application (running `npm run android` or `./gradlew assembleRelease` in app/android folder), the compilation crashes. This is a known error, which has a fix describe in [this issue](https://github.com/facebook/react-native/issues/35210). I just applied the fix mentioned in the issue link, and the compilation works fine.

Fixed #518

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
        Created At 2022-11-08 02:01:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/516" class=".btn">#516</a>
            </td>
            <td>
                <b>
                    feat: add developer settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add developer settings so that certain features can be enabled or changed by someone with expert level knowledge of the application.

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
        Created At 2022-11-04 19:32:39 +0000 UTC
    </div>
</div>

