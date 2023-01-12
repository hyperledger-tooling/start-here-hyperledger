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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    fix: problems with zoom screen on create PIN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

# Summary of Changes

Added a scroll view to the create PIN screen to stop the keyboard from blocking the second pin input in IOS zoomed mode

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
        Created At 2023-01-11 19:55:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    chore(deps): bump luxon from 1.28.0 to 1.28.1 in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [luxon](https://github.com/moment/luxon) from 1.28.0 to 1.28.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/luxon/blob/master/CHANGELOG.md">luxon's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1>3.2.0 (2022-12-29)</h1>
<ul>
<li>Allow timeZone to be specified as an intl option</li>
<li>Fix for diff's handling of end-of-month when crossing leap years (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1340">#1340</a>)</li>
<li>Add Interval.toLocaleString() (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1320">#1320</a>)</li>
</ul>
<h1>3.1.1 (2022-11-28)</h1>
<ul>
<li>Add Settings.twoDigitCutoffYear</li>
</ul>
<h1>3.1.0 (2022-10-31)</h1>
<ul>
<li>Add Duration.rescale</li>
</ul>
<h1>3.0.4 (2022-09-24)</h1>
<ul>
<li>Fix quarters in diffs (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1279">#1279</a>)</li>
<li>Export package.json in package (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1239">#1239</a>)</li>
</ul>
<h1>3.0.2 (2022-08-28)</h1>
<ul>
<li>Lots of doc changes</li>
<li>Added DateTime.expandFormat</li>
<li>Added support for custom conversion matrices in Durations</li>
</ul>
<h1>3.0.1 (2022-07-09)</h1>
<ul>
<li>Add DateTime.parseFormatForOpts</li>
</ul>
<h1>3.0.0 (2022-07-09)</h1>
<ul>
<li>Add &quot;default&quot; as an option for specifying a zone, and change &quot;system&quot; to really mean the system zone (breaking change)</li>
</ul>
<h1>2.5.0 (2022-07-09)</h1>
<ul>
<li>Support for ESM-style node imports</li>
<li>Fix Wednesday parsing for RFC 850 strings</li>
<li>Increase number of digits allowed in ISO durations</li>
</ul>
<h2>2.4.0 (2022-05-08)</h2>
<ul>
<li>Add support for parsing the ISO zone extension, like <code>2022-05-08T20:42:00.000-04:00[America/New_York]</code></li>
<li>Add an <code>extendedZone</code> option to <code>toISO()</code> and <code>toISOTime</code></li>
<li>Improvements to <code>DateTime.isInDST()</code></li>
<li>Fix for parsing in Vietnames (and probably other languages)</li>
</ul>
<h2>2.3.2 (2022-04-17)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/luxon/commit/16a1aa3ee95a80a7e9c4ccbc740c378064449ec4"><code>16a1aa3</code></a> bump to 1.38.1</li>
<li><a href="https://github.com/moment/luxon/commit/612e0c778d2dedb947f3e5160c46601688ea4959"><code>612e0c7</code></a> fix rfc2822 regex</li>
<li>See full diff in <a href="https://github.com/moment/luxon/compare/1.28.0...1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=luxon&package-manager=npm_and_yarn&previous-version=1.28.0&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-10 01:03:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    chore(deps): bump luxon from 1.28.0 to 1.28.1 in /core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [luxon](https://github.com/moment/luxon) from 1.28.0 to 1.28.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/luxon/blob/master/CHANGELOG.md">luxon's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1>3.2.0 (2022-12-29)</h1>
<ul>
<li>Allow timeZone to be specified as an intl option</li>
<li>Fix for diff's handling of end-of-month when crossing leap years (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1340">#1340</a>)</li>
<li>Add Interval.toLocaleString() (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1320">#1320</a>)</li>
</ul>
<h1>3.1.1 (2022-11-28)</h1>
<ul>
<li>Add Settings.twoDigitCutoffYear</li>
</ul>
<h1>3.1.0 (2022-10-31)</h1>
<ul>
<li>Add Duration.rescale</li>
</ul>
<h1>3.0.4 (2022-09-24)</h1>
<ul>
<li>Fix quarters in diffs (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1279">#1279</a>)</li>
<li>Export package.json in package (<a href="https://github-redirect.dependabot.com/moment/luxon/issues/1239">#1239</a>)</li>
</ul>
<h1>3.0.2 (2022-08-28)</h1>
<ul>
<li>Lots of doc changes</li>
<li>Added DateTime.expandFormat</li>
<li>Added support for custom conversion matrices in Durations</li>
</ul>
<h1>3.0.1 (2022-07-09)</h1>
<ul>
<li>Add DateTime.parseFormatForOpts</li>
</ul>
<h1>3.0.0 (2022-07-09)</h1>
<ul>
<li>Add &quot;default&quot; as an option for specifying a zone, and change &quot;system&quot; to really mean the system zone (breaking change)</li>
</ul>
<h1>2.5.0 (2022-07-09)</h1>
<ul>
<li>Support for ESM-style node imports</li>
<li>Fix Wednesday parsing for RFC 850 strings</li>
<li>Increase number of digits allowed in ISO durations</li>
</ul>
<h2>2.4.0 (2022-05-08)</h2>
<ul>
<li>Add support for parsing the ISO zone extension, like <code>2022-05-08T20:42:00.000-04:00[America/New_York]</code></li>
<li>Add an <code>extendedZone</code> option to <code>toISO()</code> and <code>toISOTime</code></li>
<li>Improvements to <code>DateTime.isInDST()</code></li>
<li>Fix for parsing in Vietnames (and probably other languages)</li>
</ul>
<h2>2.3.2 (2022-04-17)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/luxon/commit/16a1aa3ee95a80a7e9c4ccbc740c378064449ec4"><code>16a1aa3</code></a> bump to 1.38.1</li>
<li><a href="https://github.com/moment/luxon/commit/612e0c778d2dedb947f3e5160c46601688ea4959"><code>612e0c7</code></a> fix rfc2822 regex</li>
<li>See full diff in <a href="https://github.com/moment/luxon/compare/1.28.0...1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=luxon&package-manager=npm_and_yarn&previous-version=1.28.0&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-10 01:03:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/582" class=".btn">#582</a>
            </td>
            <td>
                <b>
                    Allow projects to supply custom notification type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

# Summary of Changes

Added configurations for custom notifications. Allows projects to extend the notification functionality and have custom actions for their notifications. Made notifications more consistent with wireframes, added cancellation button to notification box

![image](https://user-images.githubusercontent.com/36937407/211638862-295374dd-7584-4d94-94ae-f795fae42019.png)
![image](https://user-images.githubusercontent.com/36937407/211638917-4d86e0ac-54a9-4eb8-8c27-d1332d466083.png)


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
        Created At 2023-01-06 22:15:55 +0000 UTC
    </div>
</div>

