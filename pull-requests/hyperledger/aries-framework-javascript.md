---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1200" class=".btn">#1200</a>
            </td>
            <td>
                <b>
                    feat(indy-sdk): add indy-sdk package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commits add the `@aries-framework/indy-sdk` package. It implements all the new interfaces based on the anonreds package. Testing is still light, but I want to add it in upcoming prs when we add the anoncreds api.

The classes aren't used yet, and all old Indy implementations are still in the core package. Once we have finished the new classes we can deprecate the old ones and point to the new ones.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 10:30:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1197" class=".btn">#1197</a>
            </td>
            <td>
                <b>
                    feat: add minimal oidc-client package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the very minimum of the new `oidc-client` package. It doesn't contain any logic so far.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 00:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1196" class=".btn">#1196</a>
            </td>
            <td>
                <b>
                    build(deps): bump luxon from 1.28.0 to 1.28.1
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
Dependabot will merge this PR once CI passes on it, as requested by @TimoGlastra.

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 00:38:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    build(deps): bump json5 from 1.0.1 to 1.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 1.0.1 to 1.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v1.0.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>). This has been backported to v1. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/298">#298</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>Unreleased [<a href="https://github.com/json5/json5/tree/main">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.3...HEAD">diff</a>]</h3>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/a62db1e51e1031d92ac260f5bb38bbed1fdbc754"><code>a62db1e</code></a> 1.0.2</li>
<li><a href="https://github.com/json5/json5/commit/e0c23fe458a77c0b2cdb271376be5d8d0908133c"><code>e0c23fe</code></a> docs: update CHANGELOG for v1.0.2</li>
<li><a href="https://github.com/json5/json5/commit/62a65408408d40aeea14c7869ed327acead12972"><code>62a6540</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li>See full diff in <a href="https://github.com/json5/json5/compare/v1.0.1...v1.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=1.0.1&new-version=1.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
Dependabot will merge this PR once CI passes on it, as requested by @TimoGlastra.

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 13:23:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    chore(release): v0.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.3.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 11:48:55 +0000 UTC
    </div>
</div>

