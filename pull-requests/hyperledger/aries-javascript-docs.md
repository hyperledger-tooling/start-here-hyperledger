---
layout: default
title: aries-javascript-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-javascript-docs
---

# aries-javascript-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-javascript-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-javascript-docs/pull/89" class=".btn">#89</a>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-javascript-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 01:23:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-javascript-docs/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    build(deps): bump json5 from 2.2.1 to 2.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 2.2.1 to 2.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
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
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=2.2.1&new-version=2.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-javascript-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 18:19:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-javascript-docs/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    fix: android setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 02:02:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-javascript-docs/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    fix: agent setup for 0.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 15:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-javascript-docs/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    fix: add expo workaround for yarn
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a workaround that allows you to use expo in AFJ 0.3.0 with yarn.

Sort of addresses https://github.com/hyperledger/aries-framework-javascript/issues/1189, but only as a hacky workaround, not an actual fix.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 15:09:32 +0000 UTC
    </div>
</div>

