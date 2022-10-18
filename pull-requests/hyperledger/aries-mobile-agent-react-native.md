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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    chore(deps): bump @xmldom/xmldom from 0.7.5 to 0.7.6 in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@xmldom/xmldom](https://github.com/xmldom/xmldom) from 0.7.5 to 0.7.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/releases"><code>@​xmldom/xmldom</code>'s releases</a>.</em></p>
<blockquote>
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
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">0.7.6</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/441"><code>[#441](https://github.com/xmldom/xmldom/issues/441)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/jftanner"><code>@​jftanner</code></a>, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.3...0.8.2">0.8.3</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.1...0.9.0-beta.2">0.9.0-beta.2</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.3...0.8.2">0.8.3</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.2...0.9.0-beta.1">0.9.0-beta.1</a></h2>
<h3>Fixed</h3>
<p><strong>Only use HTML rules if mimeType matches</strong> <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/338"><code>[#338](https://github.com/xmldom/xmldom/issues/338)</code></a>, fixes <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/203"><code>[#203](https://github.com/xmldom/xmldom/issues/203)</code></a></p>
<p>In the living specs for parsing XML and HTML, that this library is trying to implement,
there is a distinction between the different types of documents being parsed:
There are quite some rules that are different for parsing, constructing and serializing XML vs HTML documents.</p>
<p>So far xmldom was always &quot;detecting&quot; whether &quot;the HTML rules should be applied&quot; by looking at the current namespace. So from the first time an the HTML default namespace (<code>http://www.w3.org/1999/xhtml</code>) was found, every node was treated as being part of an HTML document. This misconception is the root cause for quite some reported bugs.</p>
<p>BREAKING CHANGE: HTML rules are no longer applied just because of the namespace, but require the <code>mimeType</code> argument passed to <code>DOMParser.parseFromString(source, mimeType)</code> to match <code>'text/html'</code>. Doing so implies all rules for handling casing for tag and attribute names when parsing, creation of nodes and searching nodes.</p>
<p>BREAKING CHANGE: Correct the return type of <code>DOMParser.parseFromString</code> to <code>Document | undefined</code>. In case of parsing errors it was always possible that &quot;the returned <code>Document</code>&quot; has not been created. In case you are using Typescript you now need to handle those cases.</p>
<p>BREAKING CHANGE: The instance property <code>DOMParser.options</code> is no longer available, instead use the individual <code>readonly</code> property per option (<code>assign</code>, <code>domHandler</code>, <code>errorHandler</code>, <code>normalizeLineEndings</code>, <code>locator</code>, <code>xmlns</code>). Those also provides the default value if the option was not passed. The 'locator' option is now just a boolean (default remains <code>true</code>).</p>
<p>BREAKING CHANGE: The following methods no longer allow a (non spec compliant) boolean argument to toggle &quot;HTML rules&quot;:</p>
<ul>
<li><code>XMLSerializer.serializeToString</code></li>
<li><code>Node.toString</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/xmldom/xmldom/commit/3ca016d7da634686dbcadd076dda07d28a8ffd45"><code>3ca016d</code></a> 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/b28e631b8bc42edca9df6eb68e5b84f78529b3cb"><code>b28e631</code></a> docs: Prepare CHANGELOG for 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/1f20aee8ef1a8f3964add1a188f723bbc54862a0"><code>1f20aee</code></a> fix: Backport PR-437 to 0.7.x branch</li>
<li>See full diff in <a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@xmldom/xmldom&package-manager=npm_and_yarn&previous-version=0.7.5&new-version=0.7.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-17 21:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    feat: oca image display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR let us use OCA format overlay to display images in the credential details.

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
        Created At 2022-10-17 13:07:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    fix: OCA fix credential logo display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes
Fixing display of credential logo

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
        Created At 2022-10-13 22:58:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/483" class=".btn">#483</a>
            </td>
            <td>
                <b>
                    feat: new style for settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Style the settings screen as per the designs.

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
        Created At 2022-10-12 22:14:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    Bump shell-quote and @react-native-community/cli-tools in /core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/substack/node-shell-quote) and [@react-native-community/cli-tools](https://github.com/react-native-community/cli/tree/HEAD/packages/tools). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.3
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/substack/node-shell-quote/commits">compare view</a></li>
</ul>
</details>
<br />

Updates `@react-native-community/cli-tools` from 6.1.0 to 6.2.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/react-native-community/cli/releases"><code>@​react-native-community/cli-tools</code>'s releases</a>.</em></p>
<blockquote>
<h2>v6.2.0</h2>
<h2>Features</h2>
<ul>
<li>support renamed <code>-PreactNativeArchitectures</code> (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1496">#1496</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li>better Handle EPERM on Windows (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1495">#1495</a>)</li>
<li>use <code>simclt</code> instead of deprecated <code>instruments</code> (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1484">#1484</a>)</li>
<li>platform-ios: add missing <code>ora</code> dependency (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1483">#1483</a>)</li>
</ul>
<h2>Chore &amp; Maintenance</h2>
<ul>
<li>bump lerna to 4 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1504">#1504</a>)</li>
<li>bump chalk to 4.x (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1505">#1505</a>)</li>
<li>GH Actions: lint &amp; unit tests (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1499">#1499</a>)</li>
<li>remove mkdirp (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1500">#1500</a>)</li>
<li>add 6.1.0 release to compatibility table (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1501">#1501</a>)</li>
<li>replace azure with github actions (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1494">#1494</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-native-community/cli/commit/7a10b39160d53caf43f36ae9e62d4bed942003ea"><code>7a10b39</code></a> Publish</li>
<li><a href="https://github.com/react-native-community/cli/commit/a327ac86983d8b1dc8020f4d10c27d0764695a25"><code>a327ac8</code></a> chore(deps): bump shell-quote to 1.7.3 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1642">#1642</a>)</li>
<li><a href="https://github.com/react-native-community/cli/commit/908eac093d84ef0a5786e3de0f480519ddcc3ecb"><code>908eac0</code></a> v6.2.0</li>
<li><a href="https://github.com/react-native-community/cli/commit/1ac43cce3df75bff069558ac13e8314a17d892e4"><code>1ac43cc</code></a> bump chalk to 4.x (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1505">#1505</a>)</li>
<li><a href="https://github.com/react-native-community/cli/commit/ad0883d8e9b20e30e85adacbfc0b525df5d72840"><code>ad0883d</code></a> chore(deps): remove mkdirp (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1500">#1500</a>)</li>
<li>See full diff in <a href="https://github.com/react-native-community/cli/commits/@react-native-community/cli-tools@6.2.1/packages/tools">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-10-11 23:49:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    Bump hermes-engine and react-native in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [hermes-engine](https://github.com/facebook/hermes). It's no longer used after updating ancestor dependency [react-native](https://github.com/facebook/react-native). These dependencies need to be updated together.

Removes `hermes-engine`

Updates `react-native` from 0.66.1 to 0.70.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/releases">react-native's releases</a>.</em></p>
<blockquote>
<h2>0.70.2</h2>
<h3>Added</h3>
<h4>iOS specific</h4>
<ul>
<li>Add support for &quot;Prefer Cross-Fade Transitions&quot; into AccessibilityInfo (<a href="https://github.com/facebook/react-native/commit/be7c50fefd7f13201fb538ded93d91b374341173">be7c50fefd</a> by <a href="https://github.com/gabrieldonadel"><code>@​gabrieldonadel</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Bump CLI to 9.1.3 and Metro to 0.72.3 (<a href="https://github.com/facebook/react-native/commit/f1645560376b734a87f0eba1fef69f6cba312cc1">f164556037</a> by <a href="https://github.com/kelset"><code>@​kelset</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Inform ScrollView of Keyboard Events Before Mount (<a href="https://github.com/facebook/react-native/commit/26d148029c7fde117f33b0d6c8b34286c45a0ef2">26d148029c</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Fix port as -1 if dev server without specifying port on Android (<a href="https://github.com/facebook/react-native/commit/3d7e1380b4e609f5340ee80c19d566b17e620427">3d7e1380b4</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
</ul>
<hr />
<p>You can participate in the conversation on the status of this release in this <a href="https://github.com/reactwg/react-native-releases/discussions/36">discussion</a>.</p>
<hr />
<p>To help you upgrade to this version, you can use the <a href="https://react-native-community.github.io/upgrade-helper/">upgrade helper</a> ⚛️</p>
<hr />
<p>You can find the whole changelog history in the <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG.md">changelog.md file</a>.</p>
<h2>0.70.1</h2>
<!-- raw HTML omitted -->
<!-- raw HTML omitted -->
<h3>Added</h3>
<ul>
<li>Add more debugging settings for <em>HermesExecutorFactory</em> (<a href="https://github.com/facebook/react-native/commit/32d12e89f864a106433c8e54c10691d7876333ee">32d12e89f8</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
<li>Support TypeScript array types for turbo module (component only) (<a href="https://github.com/facebook/react-native/commit/33d1291e1a96497a4f994e9d622248a745ee1ea6">33d1291e1a</a> by <a href="https://github.com/ZihanChen-MSFT"><code>@​ZihanChen-MSFT</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Accept TypeScript type <code>T | null | undefined</code> as a maybe type of T in turbo module. (<a href="https://github.com/facebook/react-native/commit/9ecd203eec97e7d21d10311d950c9f8f30c7a4b1">9ecd203eec</a> by <a href="https://github.com/ZihanChen-MSFT"><code>@​ZihanChen-MSFT</code></a>)</li>
<li>Bump react-native-gradle-plugin to 0.70.3 (<a href="https://github.com/facebook/react-native/commit/e33633644c70ea39af6e450fcf31d9458051fd5f">e33633644c</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
<li>Bump react-native-codegen to 0.70.5 (<a href="https://github.com/facebook/react-native/commit/6a8c38eef272e79e52a35941afa9c3fe9e8fc191">6a8c38eef2</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
<li>Hermes version bump for 0.70.1 (<a href="https://github.com/facebook/react-native/commit/5132211228a5b9e36d58c1f7e2c99ccaabe1ba3d">5132211228</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
</ul>
<h3>Fixed</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG.md">react-native's changelog</a>.</em></p>
<blockquote>
<h2>v0.70.2</h2>
<h3>Added</h3>
<h4>iOS specific</h4>
<ul>
<li>Add support for &quot;Prefer Cross-Fade Transitions&quot; into AccessibilityInfo (<a href="https://github.com/facebook/react-native/commit/be7c50fefd7f13201fb538ded93d91b374341173">be7c50fefd</a> by <a href="https://github.com/gabrieldonadel"><code>@​gabrieldonadel</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Bump CLI to 9.1.3 and Metro to 0.72.3 (<a href="https://github.com/facebook/react-native/commit/f1645560376b734a87f0eba1fef69f6cba312cc1">f164556037</a> by <a href="https://github.com/kelset"><code>@​kelset</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Inform ScrollView of Keyboard Events Before Mount (<a href="https://github.com/facebook/react-native/commit/26d148029c7fde117f33b0d6c8b34286c45a0ef2">26d148029c</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Fix port as -1 if dev server without specifying port on Android (<a href="https://github.com/facebook/react-native/commit/3d7e1380b4e609f5340ee80c19d566b17e620427">3d7e1380b4</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
</ul>
<h2>v0.70.1</h2>
<h3>Added</h3>
<ul>
<li>Add more debugging settings for <em>HermesExecutorFactory</em> (<a href="https://github.com/facebook/react-native/commit/32d12e89f864a106433c8e54c10691d7876333ee">32d12e89f8</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
<li>Support TypeScript array types for turbo module (component only) (<a href="https://github.com/facebook/react-native/commit/33d1291e1a96497a4f994e9d622248a745ee1ea6">33d1291e1a</a> by <a href="https://github.com/ZihanChen-MSFT"><code>@​ZihanChen-MSFT</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Accept TypeScript type <code>T | null | undefined</code> as a maybe type of T in turbo module. (<a href="https://github.com/facebook/react-native/commit/9ecd203eec97e7d21d10311d950c9f8f30c7a4b1">9ecd203eec</a> by <a href="https://github.com/ZihanChen-MSFT"><code>@​ZihanChen-MSFT</code></a>)</li>
<li>Bump react-native-gradle-plugin to 0.70.3 (<a href="https://github.com/facebook/react-native/commit/e33633644c70ea39af6e450fcf31d9458051fd5f">e33633644c</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
<li>Bump react-native-codegen to 0.70.5 (<a href="https://github.com/facebook/react-native/commit/6a8c38eef272e79e52a35941afa9c3fe9e8fc191">6a8c38eef2</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
<li>Hermes version bump for 0.70.1 (<a href="https://github.com/facebook/react-native/commit/5132211228a5b9e36d58c1f7e2c99ccaabe1ba3d">5132211228</a> by <a href="https://github.com/dmytrorykun"><code>@​dmytrorykun</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix hermes profiler (<a href="https://github.com/facebook/react-native/commit/81564c1a3dae4222858de2a9a34089097f665e82">81564c1a3d</a> by <a href="https://github.com/janicduplessis"><code>@​janicduplessis</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Support PlatformColor in borderColor (<a href="https://github.com/facebook/react-native/commit/2d5db284b061aec33af671b25065632e20217f62">2d5db284b0</a> by <a href="https://github.com/danilobuerger"><code>@​danilobuerger</code></a>)</li>
<li>Avoid crash in ForwardingCookieHandler if webview is disabled (<a href="https://github.com/facebook/react-native/commit/5451cd48bd0166ba70d516e3a11c6786bc22171a">5451cd48bd</a> by <a href="https://github.com/Pajn"><code>@​Pajn</code></a>)</li>
<li>Correctly resolve classes with FindClass(..) (<a href="https://github.com/facebook/react-native/commit/361b310bcc8dddbff42cf63495649291c894d661">361b310bcc</a> by <a href="https://github.com/evancharlton"><code>@​evancharlton</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>Fix KeyboardAvoidingView height when &quot;Prefer Cross-Fade Transitions&quot; is enabled (<a href="https://github.com/facebook/react-native/commit/4b9382c250261aab89b271618f8b68083ba01785">4b9382c250</a> by <a href="https://github.com/gabrieldonadel"><code>@​gabrieldonadel</code></a>)</li>
<li>Fix React module build error with swift integration on new architecture mode (<a href="https://github.com/facebook/react-native/commit/3afef3c16702cefa5115b059a08741fba255b2db">3afef3c167</a> by <a href="https://github.com/Kudo"><code>@​Kudo</code></a>)</li>
<li>Fix ios pod install error (<a href="https://github.com/facebook/react-native/commit/0cae4959b750ea051dcd04e4c9374e02b1de6e7a">0cae4959b7</a> by <a href="https://github.com/Romick2005"><code>@​Romick2005</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react-native/commit/b9c297537a5eda68621ba77ead272cfd8b4c6e2c"><code>b9c2975</code></a> [0.70.2] Bump version numbers</li>
<li><a href="https://github.com/facebook/react-native/commit/13a2b117becd7bfb983080a330149362ebed8816"><code>13a2b11</code></a> Minor: Rename AccessibilityInfo.sendAccessibilityEvent_unstable to sendAccess...</li>
<li><a href="https://github.com/facebook/react-native/commit/2de4cf03cfc91aec4b594e17d584ce40189c4a2e"><code>2de4cf0</code></a> chore(deps): bump CLI to 9.1.3 and Metro to 0.72.3 (<a href="https://github-redirect.dependabot.com/facebook/react-native/issues/34803">#34803</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/7b53a244cd85b894497939e1a5776812a510763c"><code>7b53a24</code></a> Fix port as -1 if dev server without specifying port on Android (<a href="https://github-redirect.dependabot.com/facebook/react-native/issues/34705">#34705</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/b03f536279f423acdd525a2284e4aac3a9d6d1dd"><code>b03f536</code></a> fix: KeyboardAvoidingView height when &quot;Prefer Cross-Fade Transitions&quot; is enab...</li>
<li><a href="https://github.com/facebook/react-native/commit/764f58461583243228f55d9eb610c3f2d0df3fbe"><code>764f584</code></a> Let ScrollView Know About Keyboard Opened Before Mount</li>
<li><a href="https://github.com/facebook/react-native/commit/75d567970141967acc1681247f64a45a99243b78"><code>75d5679</code></a> feat: Add support for &quot;Prefer Cross-Fade Transitions&quot; into AccessibilityInfo ...</li>
<li><a href="https://github.com/facebook/react-native/commit/73e55334b070797ead720f6831cd15597a102522"><code>73e5533</code></a> Add a pseudo flow declaration for AccessibilityInfo</li>
<li><a href="https://github.com/facebook/react-native/commit/9fd764388a0963cddbeafdcea2d830937ad716b2"><code>9fd7643</code></a> Revert &quot;fix: KeyboardAvoidingView height when &quot;Prefer Cross-Fade Transitions&quot;...</li>
<li><a href="https://github.com/facebook/react-native/commit/a54ba33305621abb778085fc01ff954b621ce57b"><code>a54ba33</code></a> [0.70.1] Bump version numbers</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/react-native/compare/v0.66.1...v0.70.2">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-10-11 23:48:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    Bump shell-quote and @react-native-community/cli-tools in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/substack/node-shell-quote) and [@react-native-community/cli-tools](https://github.com/react-native-community/cli/tree/HEAD/packages/tools). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.3
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/substack/node-shell-quote/commits">compare view</a></li>
</ul>
</details>
<br />

Updates `@react-native-community/cli-tools` from 6.2.0 to 6.2.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-native-community/cli/commit/7a10b39160d53caf43f36ae9e62d4bed942003ea"><code>7a10b39</code></a> Publish</li>
<li><a href="https://github.com/react-native-community/cli/commit/a327ac86983d8b1dc8020f4d10c27d0764695a25"><code>a327ac8</code></a> chore(deps): bump shell-quote to 1.7.3 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1642">#1642</a>)</li>
<li>See full diff in <a href="https://github.com/react-native-community/cli/commits/@react-native-community/cli-tools@6.2.1/packages/tools">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-10-11 23:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    Bump @xmldom/xmldom and react-native-windows in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [@xmldom/xmldom](https://github.com/xmldom/xmldom). It's no longer used after updating ancestor dependency [react-native-windows](https://github.com/microsoft/react-native-windows/tree/HEAD/vnext). These dependencies need to be updated together.

Removes `@xmldom/xmldom`

Updates `react-native-windows` from 0.69.1 to 1.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/microsoft/react-native-windows/releases">react-native-windows's releases</a>.</em></p>
<blockquote>
<h2>React Native Windows 0.70.3</h2>
<p>This is patch release of react-native-windows, fixing bugs or adding non-breaking enhancements. To see a summary of changes in this major release, see <a href="https://github.com/microsoft/react-native-windows/releases/tag/react-native-windows_v0.70.0">release notes for React Native Windows 0.70.0</a>.</p>
<h3>New changes</h3>
<ul>
<li>66f46b19 Set Origin HTTP header during CORS (<a href="https://github.com/microsoft/react-native-windows/tree/HEAD/vnext/issues/10700">#10700</a>) (<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>)</li>
<li>bf355fcb Set User-Agent header in Origin Policy filter (<a href="https://github.com/microsoft/react-native-windows/tree/HEAD/vnext/issues/10695">#10695</a>) (<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>)</li>
</ul>
<h2>React Native Windows 0.70.2</h2>
<p>This is patch release of react-native-windows, fixing bugs or adding non-breaking enhancements. To see a summary of changes in this major release, see <a href="https://github.com/microsoft/react-native-windows/releases/tag/react-native-windows_v0.70.0">release notes for React Native Windows 0.70.0</a>.</p>
<h3>New changes</h3>
<ul>
<li>77bf7205 Export OriginPolicy.h to NuGet package (<a href="https://github.com/microsoft/react-native-windows/tree/HEAD/vnext/issues/10615">#10615</a>) (<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>)</li>
<li>ecd361d5 Consolidate JavaScript HTTP module specifications (<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>)</li>
<li>5c1c0839 Move required PackageRestore properties into shared property sheets (<a href="mailto:jthysell@microsoft.com">jthysell@microsoft.com</a>)</li>
</ul>
<h2>React Native Windows 0.70.1</h2>
<p>This is patch release of react-native-windows, fixing bugs or adding non-breaking enhancements. To see a summary of changes in this major release, see <a href="https://github.com/microsoft/react-native-windows/releases/tag/react-native-windows_v0.70.0">release notes for React Native Windows 0.70.0</a>.</p>
<h3>New changes</h3>
<ul>
<li>4161b2c6 Implement HTTP redirection (<a href="https://github.com/microsoft/react-native-windows/tree/HEAD/vnext/issues/10534">#10534</a>) (<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>)</li>
<li>76794bf8 Fixes bug introduced by pointerEvents change (<a href="mailto:ericroz@fb.com">ericroz@fb.com</a>)</li>
</ul>
<h2>React Native Windows 0.70.0</h2>
<p>We're excited to release React Native Windows 0.70.0-preview.1 targeting React Native 0.70.0-rc.3. There have been many changes to both react-native-windows and react-native itself and we would love your feedback on anything that doesn't work as expected.
How to upgrade
You can view the changes made to the default new React Native Windows applications for C++ and C# using <a href="https://react-native-community.github.io/upgrade-helper/?package=react-native-windows">React Native Upgrade Helper</a>. See <a href="https://microsoft.github.io/react-native-windows/docs/next/upgrade-app">this document</a> for more details.</p>
<h2>What's new from React Native</h2>
<ul>
<li>React Native is now using <code>@​react-native-community/cli</code><a href="https://github.com/9"><code>@​9</code></a>.0.0-alpha.3. See Upgrade <code>@​react-native-community/cli</code>.</li>
<li>Folly is now on version v2021.07.22.0.</li>
</ul>
<h3>Debuggability</h3>
<ul>
<li>Fixes a crash when enabling Yoga logging.</li>
<li>Fixes metro config when using <code>--useDevMode</code>.</li>
</ul>
<h3>Reliability</h3>
<ul>
<li>Improved Supply Chain security by updating NuGet config files.</li>
<li>Fixes floating point conversions in non en-US locales.</li>
<li>Updates autolinking to not error if a dependency is misconfigured.</li>
<li>Fixes matrix multiplication logic for transforms to match iOS/Android.</li>
<li>Fixes ExecuteJsi on instance shutdown.</li>
<li>Fixes bug when UTF-8 characters are in bundle path.</li>
<li>Updates autolinking to update project paths in solution files rather than including new paths, upon not finding the exact project entry for a given GUID.</li>
<li>Fixes skew transforms for degree inputs.</li>
<li>Fixes bug in <code>onLongPress</code> functionality. Now <code>onLongPress</code> is only allowed during left clicks.\</li>
<li>Fixes crash in DynamicAutomationPeer::GetContentName.</li>
</ul>
<h3>Accessibility</h3>
<ul>
<li>Updates visual of TextInput if <code>focusable == false</code>.</li>
<li>Fixes color customization bug for Text component during High Contrast mode.</li>
</ul>
<h3>Other</h3>
<ul>
<li>Supports PreparedScriptStore for V8 Node-API.</li>
<li>Exposes <code>LoadingState</code> on ReactContext.</li>
<li>Implements Blob module.</li>
<li>Adds partial PlatformColor support for Image's tintColor.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/microsoft/react-native-windows/blob/main/vnext/CHANGELOG.json">react-native-windows's changelog</a>.</em></p>
<blockquote>
<p>{
&quot;name&quot;: &quot;react-native-windows&quot;,
&quot;entries&quot;: [
{
&quot;date&quot;: &quot;Tue, 11 Oct 2022 05:11:41 GMT&quot;,
&quot;tag&quot;: &quot;react-native-windows_v0.0.0-canary.562&quot;,
&quot;version&quot;: &quot;0.0.0-canary.562&quot;,
&quot;comments&quot;: {
&quot;prerelease&quot;: [
{
&quot;author&quot;: &quot;<a href="mailto:erozell@outlook.com">erozell@outlook.com</a>&quot;,
&quot;package&quot;: &quot;react-native-windows&quot;,
&quot;commit&quot;: &quot;fa9658fa1dc03799cddf594ba82dd638cf7839f3&quot;,
&quot;comment&quot;: &quot;Always synchronize focusable and accessible props&quot;
}
]
}
},
{
&quot;date&quot;: &quot;Sat, 08 Oct 2022 05:11:18 GMT&quot;,
&quot;tag&quot;: &quot;react-native-windows_v0.0.0-canary.561&quot;,
&quot;version&quot;: &quot;0.0.0-canary.561&quot;,
&quot;comments&quot;: {
&quot;prerelease&quot;: [
{
&quot;author&quot;: &quot;<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>&quot;,
&quot;package&quot;: &quot;react-native-windows&quot;,
&quot;commit&quot;: &quot;635a86b1f8c85de006f8faa9f5d881b13f667a78&quot;,
&quot;comment&quot;: &quot;Set Origin HTTP header during CORS&quot;
},
{
&quot;author&quot;: &quot;<a href="mailto:34109996+chiaramooney@users.noreply.github.com">34109996+chiaramooney@users.noreply.github.com</a>&quot;,
&quot;package&quot;: &quot;react-native-windows&quot;,
&quot;commit&quot;: &quot;59c2ab9fa9f859d5df99c3726c6ebdc14f1e9ec8&quot;,
&quot;comment&quot;: &quot;Add Snapshots&quot;
},
{
&quot;author&quot;: &quot;<a href="mailto:julio.rocha@microsoft.com">julio.rocha@microsoft.com</a>&quot;,
&quot;package&quot;: &quot;react-native-windows&quot;,
&quot;commit&quot;: &quot;9ded99c24ff2e211fa6a4e4e20f21e4562bff9c4&quot;,
&quot;comment&quot;: &quot;Set User-Agent header in Origin Policy filter&quot;
}
]
}
},
{
&quot;date&quot;: &quot;Fri, 07 Oct 2022 05:11:46 GMT&quot;,
&quot;tag&quot;: &quot;react-native-windows_v0.0.0-canary.560&quot;,
&quot;version&quot;: &quot;0.0.0-canary.560&quot;,
&quot;comments&quot;: {</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/microsoft/react-native-windows/commits/HEAD/vnext">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2022-10-11 23:47:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    updated PIN screen wording
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

# Summary of Changes

Updated wording on PIN screen to match wireframes
![2022-10-11_16-12](https://user-images.githubusercontent.com/36937407/195215282-1313e3d0-0583-4842-948a-ff1e3b2dcb60.png)

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
        Created At 2022-10-11 23:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    chore: cleanup unused code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

The WebView is no longer needed for any features so I removed it as part of this change.

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
        Created At 2022-10-11 21:20:05 +0000 UTC
    </div>
</div>

