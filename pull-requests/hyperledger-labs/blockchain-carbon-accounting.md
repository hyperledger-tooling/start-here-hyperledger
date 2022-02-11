---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    build(deps): bump handlebars from 4.7.6 to 4.7.7 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [handlebars](https://github.com/wycats/handlebars.js) from 4.7.6 to 4.7.7.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/handlebars-lang/handlebars.js/blob/master/release-notes.md">handlebars's changelog</a>.</em></p>
<blockquote>
<h2>v4.7.7 - February 15th, 2021</h2>
<ul>
<li>fix weird error in integration tests - eb860c0</li>
<li>fix: check prototype property access in strict-mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>) - b6d3de7</li>
<li>fix: escape property names in compat mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>) - f058970</li>
<li>refactor: In spec tests, use expectTemplate over equals and shouldThrow (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1683">#1683</a>) - 77825f8</li>
<li>chore: start testing on Node.js 12 and 13 - 3789a30</li>
</ul>
<p>(POSSIBLY) BREAKING CHANGES:</p>
<ul>
<li>the changes from version <a href="https://github.com/handlebars-lang/handlebars.js/blob/master/release-notes.md#v460---january-8th-2020">4.6.0</a> now also apply
in when using the compile-option &quot;strict: true&quot;. Access to prototype properties is forbidden completely by default, specific properties or methods
can be allowed via runtime-options. See <a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1633">#1633</a> for details. If you are using Handlebars as documented, you should not be accessing prototype properties
from your template anyway, so the changes should not be a problem for you. Only the use of undocumented features can break your build.</li>
</ul>
<p>That is why we only bump the patch version despite mentioning breaking changes.</p>
<p><a href="https://github.com/handlebars-lang/handlebars.js/compare/v4.7.6...v4.7.7">Commits</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/a9a8e403213583ca90cb7c872d3a22796c37d961"><code>a9a8e40</code></a> v4.7.7</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/e66aed5b99c1b6c93564f37d627e34e5d60eb76e"><code>e66aed5</code></a> Update release notes</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/7d4d170ce46a53084a41920c5c7387c131357989"><code>7d4d170</code></a> disable IE in Saucelabs tests</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/eb860c08998f8f506360d305d89e1f4b40f72a0a"><code>eb860c0</code></a> fix weird error in integration tests</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/b6d3de7123eebba603e321f04afdbae608e8fea8"><code>b6d3de7</code></a> fix: check prototype property access in strict-mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/f0589701698268578199be25285b2ebea1c1e427"><code>f058970</code></a> fix: escape property names in compat mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/77825f8d3522356feb8e4160fac16344104d192b"><code>77825f8</code></a> refator: In spec tests, use expectTemplate over equals and shouldThrow (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1683">#1683</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/3789a309554fd600caeae442f40881cf93eb3b54"><code>3789a30</code></a> chore: start testing on Node.js 12 and 13</li>
<li>See full diff in <a href="https://github.com/wycats/handlebars.js/compare/v4.7.6...v4.7.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=handlebars&package-manager=npm_and_yarn&previous-version=4.7.6&new-version=4.7.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 15:29:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency pathval to 1.1.1 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| pathval | [`1.1.0` -> `1.1.1`](https://renovatebot.com/diffs/npm/pathval/1.1.0/1.1.1) |

### GitHub Vulnerability Alerts

#### [CVE-2020-7751](https://nvd.nist.gov/vuln/detail/CVE-2020-7751)

This affects all versions of package pathval under 1.1.1.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 02:53:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    build(deps): bump pathval from 1.1.0 to 1.1.1 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [pathval](https://github.com/chaijs/pathval) from 1.1.0 to 1.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/chaijs/pathval/releases">pathval's releases</a>.</em></p>
<blockquote>
<h2>v1.1.1</h2>
<p>Fixes a security issue around prototype pollution.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/chaijs/pathval/commit/db6c3e39c39859564704b7f37149082689f1b172"><code>db6c3e3</code></a> chore: v1.1.1</li>
<li><a href="https://github.com/chaijs/pathval/commit/7859e0e1ce4c2c67de897edce097ed31f80661d0"><code>7859e0e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/chaijs/pathval/issues/60">#60</a> from deleonio/fix/vulnerability-prototype-pollution</li>
<li><a href="https://github.com/chaijs/pathval/commit/49ce1f41a6f65662ac4b18a91c3d9c3baad71af1"><code>49ce1f4</code></a> style: correct rule in package.json</li>
<li><a href="https://github.com/chaijs/pathval/commit/c77b9d29e4fadbbaf691c83eedc7d2224a2beb0f"><code>c77b9d2</code></a> fix: prototype pollution vulnerability + working tests</li>
<li><a href="https://github.com/chaijs/pathval/commit/49031e451c381297ea3cf90917915377998b8678"><code>49031e4</code></a> chore: remove very old nodejs</li>
<li><a href="https://github.com/chaijs/pathval/commit/57730a9baf5a4b814043e59c42f802ddd05a430d"><code>57730a9</code></a> chore: update deps and tool configuration</li>
<li><a href="https://github.com/chaijs/pathval/commit/a1230184a33a18f4eb3a92817e9b7492e8082903"><code>a123018</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/chaijs/pathval/issues/55">#55</a> from chaijs/remove-lgtm</li>
<li><a href="https://github.com/chaijs/pathval/commit/07eb4a810fbba54c084266e26689014f64befc11"><code>07eb4a8</code></a> Delete MAINTAINERS</li>
<li><a href="https://github.com/chaijs/pathval/commit/a0147cdb1df2e9e3c6e5a7865641099312ed95a8"><code>a0147cd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/chaijs/pathval/issues/54">#54</a> from astorije/patch-1</li>
<li><a href="https://github.com/chaijs/pathval/commit/aebb27810c0bcb7a0f0c6a06047242940deb9c82"><code>aebb278</code></a> Center repo name on README</li>
<li>Additional commits viewable in <a href="https://github.com/chaijs/pathval/compare/v1.1.0...v1.1.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~chai">chai</a>, a new releaser for pathval since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pathval&package-manager=npm_and_yarn&previous-version=1.1.0&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 02:21:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    Calculate estimated emissions -- placeholder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jeremy Wickersheimer <jwickers@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 19:21:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    fix orbitdb loading, seed data for ups shipping methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 00:32:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    fix(deps): pin dependency axios [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Type | Update | Change |
|---|---|---|---|
| [axios](https://axios-http.com) ([source](https://togithub.com/axios/axios)) | dependencies | pin | [`^0.19.0` -> `0.19.2`](https://renovatebot.com/diffs/npm/axios/0.19.2/0.19.2) |
| axios |  |  | [`0.21.1` -> `0.21.2`](https://renovatebot.com/diffs/npm/axios/0.21.1/0.21.2) |

### GitHub Vulnerability Alerts

#### [CVE-2020-28168](https://nvd.nist.gov/vuln/detail/CVE-2020-28168)

Axios NPM package 0.21.0 contains a Server-Side Request Forgery (SSRF) vulnerability where an attacker is able to bypass a proxy by providing a URL that responds with a redirect to a restricted host or IP address.

#### [CVE-2021-3749](https://nvd.nist.gov/vuln/detail/CVE-2021-3749)

axios is vulnerable to Inefficient Regular Expression Complexity

📌 **Important**: Renovate will wait until you have merged this Pin PR before creating any *upgrade* PRs for the affected packages. Add the preset `:preserveSemverRanges` to your config if you instead don't wish to pin dependencies.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR is behind base branch, or you tick the rebase/retry checkbox.

👻 **Immortal**: This PR will be recreated if closed unmerged. Get [config help](https://togithub.com/renovatebot/renovate/discussions) if that's undesired.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:43:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency y18n [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| y18n | [`4.0.0` -> `4.0.1`](https://renovatebot.com/diffs/npm/y18n/4.0.0/4.0.1) |
| y18n | [`3.2.1` -> `3.2.2`](https://renovatebot.com/diffs/npm/y18n/3.2.1/3.2.2) |

### GitHub Vulnerability Alerts

#### [CVE-2020-7774](https://nvd.nist.gov/vuln/detail/CVE-2020-7774)

### Overview

The npm package `y18n` before versions 3.2.2, 4.0.1, and 5.0.5 is vulnerable to Prototype Pollution. 

### POC

```
const y18n = require('y18n')();

y18n.setLocale('__proto__');
y18n.updateLocale({polluted: true});

console.log(polluted); // true
```

### Recommendation

Upgrade to version 3.2.2, 4.0.1, 5.0.5 or later.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

👻 **Immortal**: This PR will be recreated if closed unmerged. Get [config help](https://togithub.com/renovatebot/renovate/discussions) if that's undesired.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:42:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency ws [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| ws | [`5.2.2` -> `5.2.3`](https://renovatebot.com/diffs/npm/ws/5.2.2/5.2.3) |
| ws | [`7.4.0` -> `7.4.6`](https://renovatebot.com/diffs/npm/ws/7.4.0/7.4.6) |

### GitHub Vulnerability Alerts

#### [CVE-2021-32640](https://togithub.com/websockets/ws/security/advisories/GHSA-6fc8-4gx4-v693)

### Impact

A specially crafted value of the `Sec-Websocket-Protocol` header can be used to significantly slow down a ws server.

### Proof of concept

```js
for (const length of [1000, 2000, 4000, 8000, 16000, 32000]) {
  const value = 'b' + ' '.repeat(length) + 'x';
  const start = process.hrtime.bigint();

  value.trim().split(/ *, */);

  const end = process.hrtime.bigint();

  console.log('length = %d, time = %f ns', length, end - start);
}
```

### Patches

The vulnerability was fixed in ws@7.4.6 (https://github.com/websockets/ws/commit/00c425ec77993773d823f018f64a5c44e17023ff) and backported to ws@6.2.2 (https://github.com/websockets/ws/commit/78c676d2a1acefbc05292e9f7ea0a9457704bf1b) and ws@5.2.3 (https://github.com/websockets/ws/commit/76d47c1479002022a3e4357b3c9f0e23a68d4cd2).

### Workarounds

In vulnerable versions of ws, the issue can be mitigated by reducing the maximum allowed length of the request headers using the [`--max-http-header-size=size`](https://nodejs.org/api/cli.html#cli_max_http_header_size_size) and/or the [`maxHeaderSize`](https://nodejs.org/api/http.html#http_http_createserver_options_requestlistener) options.

### Credits

The vulnerability was responsibly disclosed along with a fix in private by [Robert McLaughlin](https://togithub.com/robmcl4) from University of California, Santa Barbara.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

👻 **Immortal**: This PR will be recreated if closed unmerged. Get [config help](https://togithub.com/renovatebot/renovate/discussions) if that's undesired.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency validator to 13.7.0 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| validator | [`13.1.17` -> `13.7.0`](https://renovatebot.com/diffs/npm/validator/13.1.17/13.7.0) |
| validator | [`13.6.0` -> `13.7.0`](https://renovatebot.com/diffs/npm/validator/13.6.0/13.7.0) |

### GitHub Vulnerability Alerts

#### [GHSA-xx4c-jj58-r7x6](https://togithub.com/validatorjs/validator.js/security/advisories/GHSA-xx4c-jj58-r7x6)

### Impact
Versions of `validator` prior to 13.7.0 are affected by an inefficient Regular Expression complexity  when using the `rtrim` and `trim` sanitizers.

### Patches
The problem has been patched in validator 13.7.0

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:40:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency underscore to 1.12.1 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| underscore | [`1.9.1` -> `1.12.1`](https://renovatebot.com/diffs/npm/underscore/1.9.1/1.12.1) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23358](https://nvd.nist.gov/vuln/detail/CVE-2021-23358)

The package `underscore` from 1.13.0-0 and before 1.13.0-2, from 1.3.2 and before 1.12.1 are vulnerable to Arbitrary Code Execution via the template function, particularly when a variable property is passed as an argument as it is not sanitized.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:40:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency tar to 4.4.18 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| tar | [`4.4.13` -> `4.4.18`](https://renovatebot.com/diffs/npm/tar/4.4.13/4.4.18) |

### GitHub Vulnerability Alerts

#### [CVE-2021-32803](https://togithub.com/npm/node-tar/security/advisories/GHSA-r628-mhmh-qjhw)

### Impact

Arbitrary File Creation, Arbitrary File Overwrite, Arbitrary Code Execution

`node-tar` aims to guarantee that any file whose location would be modified by a symbolic link is not extracted. This is, in part, achieved by ensuring that extracted directories are not symlinks.  Additionally, in order to prevent unnecessary `stat` calls to determine whether a given path is a directory, paths are cached when directories are created.

This logic was insufficient when extracting tar files that contained both a directory and a symlink with the same name as the directory. This order of operations resulted in the directory being created and added to the `node-tar` directory cache. When a directory is present in the directory cache, subsequent calls to mkdir for that directory are skipped. However, this is also where `node-tar` checks for symlinks occur.

By first creating a directory, and then replacing that directory with a symlink, it was thus possible to bypass `node-tar` symlink checks on directories, essentially allowing an untrusted tar file to symlink into an arbitrary location and subsequently extracting arbitrary files into that location, thus allowing arbitrary file creation and overwrite.

This issue was addressed in releases 3.2.3, 4.4.15, 5.0.7 and 6.1.2.

### Patches

3.2.3 || 4.4.15 || 5.0.7 || 6.1.2

### Workarounds

Users may work around this vulnerability without upgrading by creating a custom `filter` method which prevents the extraction of symbolic links.

```js
const tar = require('tar')

tar.x({
  file: 'archive.tgz',
  filter: (file, entry) => {
    if (entry.type === 'SymbolicLink') {
      return false
    } else {
      return true
    }
  }
})
```

Users are encouraged to upgrade to the latest patch versions, rather than attempt to sanitize tar input themselves.

#### [CVE-2021-32804](https://togithub.com/npm/node-tar/security/advisories/GHSA-3jfq-g458-7qm9)

### Impact

Arbitrary File Creation, Arbitrary File Overwrite, Arbitrary Code Execution

`node-tar` aims to prevent extraction of absolute file paths by turning absolute paths into relative paths when the `preservePaths` flag is not set to `true`. This is achieved by stripping the absolute path root from any absolute file paths contained in a tar file. For example `/home/user/.bashrc` would turn into `home/user/.bashrc`. 

This logic was insufficient when file paths contained repeated path roots such as `////home/user/.bashrc`. `node-tar` would only strip a single path root from such paths. When given an absolute file path with repeating path roots, the resulting path (e.g. `///home/user/.bashrc`) would still resolve to an absolute path, thus allowing arbitrary file creation and overwrite. 

### Patches

3.2.2 || 4.4.14 || 5.0.6 || 6.1.1

NOTE: an adjacent issue [CVE-2021-32803](https://togithub.com/npm/node-tar/security/advisories/GHSA-r628-mhmh-qjhw) affects this release level. Please ensure you update to the latest patch levels that address CVE-2021-32803 as well if this adjacent issue affects your `node-tar` use case.

### Workarounds

Users may work around this vulnerability without upgrading by creating a custom `onentry` method which sanitizes the `entry.path` or a `filter` method which removes entries with absolute paths.

```js
const path = require('path')
const tar = require('tar')

tar.x({
  file: 'archive.tgz',
  // either add this function...
  onentry: (entry) => {
    if (path.isAbsolute(entry.path)) {
      entry.path = sanitizeAbsolutePathSomehow(entry.path)
      entry.absolute = path.resolve(entry.path)
    }
  },

  // or this one
  filter: (file, entry) => {
    if (path.isAbsolute(entry.path)) {
      return false
    } else {
      return true
    }
  }
})
```

Users are encouraged to upgrade to the latest patch versions, rather than attempt to sanitize tar input themselves.

#### [CVE-2021-37701](https://togithub.com/npm/node-tar/security/advisories/GHSA-9r2w-394v-53qc)

### Impact

Arbitrary File Creation, Arbitrary File Overwrite, Arbitrary Code Execution

`node-tar` aims to guarantee that any file whose location would be modified by a symbolic link is not extracted. This is, in part, achieved by ensuring that extracted directories are not symlinks. Additionally, in order to prevent unnecessary stat calls to determine whether a given path is a directory, paths are cached when directories are created.

This logic was insufficient when extracting tar files that contained both a directory and a symlink with the same name as the directory, where the symlink and directory names in the archive entry used backslashes as a path separator on posix systems. The cache checking logic used both `\` and `/` characters as path separators, however `\` is a valid filename character on posix systems.

By first creating a directory, and then replacing that directory with a symlink, it was thus possible to bypass node-tar symlink checks on directories, essentially allowing an untrusted tar file to symlink into an arbitrary location and subsequently extracting arbitrary files into that location, thus allowing arbitrary file creation and overwrite.

Additionally, a similar confusion could arise on case-insensitive filesystems.  If a tar archive contained a directory at `FOO`, followed by a symbolic link named `foo`, then on case-insensitive file systems, the creation of the symbolic link would remove the directory from the filesystem, but _not_ from the internal directory cache, as it would not be treated as a cache hit.  A subsequent file entry within the `FOO` directory would then be placed in the target of the symbolic link, thinking that the directory had already been created. 

These issues were addressed in releases 4.4.16, 5.0.8 and 6.1.7.

The v3 branch of `node-tar` has been deprecated and did not receive patches for these issues. If you are still using a v3 release we recommend you update to a more recent version of `node-tar`. If this is not possible, a workaround is available below.

### Patches

4.4.16 || 5.0.8 || 6.1.7

### Workarounds

Users may work around this vulnerability without upgrading by creating a custom filter method which prevents the extraction of symbolic links.

```js
const tar = require('tar')

tar.x({
  file: 'archive.tgz',
  filter: (file, entry) => {
    if (entry.type === 'SymbolicLink') {
      return false
    } else {
      return true
    }
  }
})
```

Users are encouraged to upgrade to the latest patched versions, rather than attempt to sanitize tar input themselves.

### Fix

The problem is addressed in the following ways:

1. All paths are normalized to use `/` as a path separator, replacing `\` with `/` on Windows systems, and leaving `\` intact in the path on posix systems.  This is performed in depth, at every level of the program where paths are consumed.
2. Directory cache pruning is performed case-insensitively.  This _may_ result in undue cache misses on case-sensitive file systems, but the performance impact is negligible.

#### Caveat

Note that this means that the `entry` objects exposed in various parts of tar's API will now always use `/` as a path separator, even on Windows systems.  This is not expected to cause problems, as `/` is a valid path separator on Windows systems, but _may_ result in issues if `entry.path` is compared against a path string coming from some other API such as `fs.realpath()` or `path.resolve()`.

Users are encouraged to always normalize paths using a well-tested method such as `path.resolve()` before comparing paths to one another.

#### [CVE-2021-37712](https://togithub.com/npm/node-tar/security/advisories/GHSA-qq89-hq3f-393p)

### Impact
Arbitrary File Creation, Arbitrary File Overwrite, Arbitrary Code Execution

node-tar aims to guarantee that any file whose location would be modified by a symbolic link is not extracted. This is, in part, achieved by ensuring that extracted directories are not symlinks. Additionally, in order to prevent unnecessary stat calls to determine whether a given path is a directory, paths are cached when directories are created.

This logic was insufficient when extracting tar files that contained two directories and a symlink with names containing unicode values that normalized to the same value. Additionally, on Windows systems, long path portions would resolve to the same file system entities as their 8.3 "short path" counterparts. A specially crafted tar archive could thus include directories with two forms of the path that resolve to the same file system entity, followed by a symbolic link with a name in the first form, lastly followed by a file using the second form. It led to bypassing node-tar symlink checks on directories, essentially allowing an untrusted tar file to symlink into an arbitrary location and subsequently extracting arbitrary files into that location, thus allowing arbitrary file creation and overwrite.

The v3 branch of `node-tar` has been deprecated and did not receive patches for these issues. If you are still using a v3 release we recommend you update to a more recent version of `node-tar`. If this is not possible, a workaround is available below.

### Patches

6.1.9 || 5.0.10 || 4.4.18

### Workarounds

Users may work around this vulnerability without upgrading by creating a custom filter method which prevents the extraction of symbolic links.

```js
const tar = require('tar')

tar.x({
  file: 'archive.tgz',
  filter: (file, entry) => {
    if (entry.type === 'SymbolicLink') {
      return false
    } else {
      return true
    }
  }
})
```

Users are encouraged to upgrade to the latest patched versions, rather than attempt to sanitize tar input themselves.

#### Fix

The problem is addressed in the following ways, when comparing paths in the directory cache and path reservation systems:

1. The `String.normalize('NFKD')` method is used to first normalize all unicode to its maximally compatible and multi-code-point form.
2. All slashes are normalized to `/` on Windows systems (on posix systems, `\` is a valid filename character, and thus left intact).
3. When a symbolic link is encountered on Windows systems, the entire directory cache is cleared.  Collisions related to use of 8.3 short names to replace directories with other (non-symlink) types of entries may make archives fail to extract properly, but will not result in arbitrary file writes.

#### [CVE-2021-37713](https://togithub.com/npm/node-tar/security/advisories/GHSA-5955-9wpr-37jh)

### Impact

Arbitrary File Creation, Arbitrary File Overwrite, Arbitrary Code Execution

node-tar aims to guarantee that any file whose location would be outside of the extraction target directory is not extracted. This is, in part, accomplished by sanitizing absolute paths of entries within the archive, skipping archive entries that contain `..` path portions, and resolving the sanitized paths against the extraction target directory.

This logic was insufficient on Windows systems when extracting tar files that contained a path that was not an absolute path, but specified a drive letter different from the extraction target, such as `C:some\path`.  If the drive letter does not match the extraction target, for example `D:\extraction\dir`, then the result of `path.resolve(extractionDirectory, entryPath)` would resolve against the current working directory on the `C:` drive, rather than the extraction target directory.

Additionally, a `..` portion of the path could occur immediately after the drive letter, such as `C:../foo`, and was not properly sanitized by the logic that checked for `..` within the normalized and split portions of the path.

This only affects users of `node-tar` on Windows systems.

### Patches

4.4.18 || 5.0.10 || 6.1.9

### Workarounds

There is no reasonable way to work around this issue without performing the same path normalization procedures that node-tar now does.

Users are encouraged to upgrade to the latest patched versions of node-tar, rather than attempt to sanitize paths themselves.

### Fix

The fixed versions strip path roots from all paths prior to being resolved against the extraction target folder, even if such paths are not "absolute".

Additionally, a path starting with a drive letter and then two dots, like `c:../`, would bypass the check for `..` path portions.  This is checked properly in the patched versions.

Finally, a defense in depth check is added, such that if the `entry.absolute` is outside of the extraction taret, and we are not in preservePaths:true mode, a warning is raised on that entry, and it is skipped.  Currently, it is believed that this check is redundant, but it did catch some oversights in development.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:39:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency swagger-ui-dist to 4.1.3 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| swagger-ui-dist | [`3.36.0` -> `4.1.3`](https://renovatebot.com/diffs/npm/swagger-ui-dist/3.36.0/4.1.3) |

### GitHub Vulnerability Alerts

#### [GHSA-qrmm-w75w-3wpx](https://togithub.com/swagger-api/swagger-ui/security/advisories/GHSA-qrmm-w75w-3wpx)

SwaggerUI supports displaying remote OpenAPI definitions through the `?url` parameter. This enables robust demonstration capabilities on sites like `petstore.swagger.io`, `editor.swagger.io`, and similar sites, where users often want to see what their OpenAPI definitions would look like rendered.

However, this functionality may pose a risk for users who host their own SwaggerUI instances. In particular, including remote OpenAPI definitions opens a vector for phishing attacks by abusing the trusted names/domains of self-hosted instances.

An example scenario abusing this functionality could take the following form:
- `https://example.com/api-docs` hosts a version of SwaggerUI with `?url=` query parameter enabled.
- Users will trust the domain `https://example.com` and the contents of the OpenAPI definition.
- A malicious actor may craft a similar OpenAPI definition and service that responds to the defined APIs at `https://evildomain`.
- Users mistakenly click a phishing URL like `https://example.com/api-docs?url=https://evildomain/fakeapi.yaml` and enters sensitive data via the "Try-it-out" feature.

We do want to stress that this attack vector is limited to scenarios that actively trick users into divulging sensitive information. The ease of this is highly contextual and, therefore, the threat model may be different for individual users and organizations. It is *not* possible to perform non-interactive attacks (e.g., cross-site scripting or code injection) through this mechanism.

### Resolution 
We've made the decision to [disable query parameters (#&#8203;4872)](https://togithub.com/swagger-api/swagger-ui/issues/4872) by default starting with SwaggerUI version `4.1.3`. Please update to this version when it becomes available (**ETA: 2021 December**). Users will still be able to be re-enable the options at their discretion. We'll continue to enable query parameters on the Swagger demo sites.

### Workaround
If you host a version of SwaggerUI and wish to mitigate this issue immediately, you are encouraged to add the following custom plugin code:

```js
SwaggerUI({
  //  ...other configuration options,
  plugins: [function UrlParamDisablePlugin() {
    return {
      statePlugins: {
        spec: {
          wrapActions: {
            // Remove the ?url parameter from loading an external OpenAPI definition.
            updateUrl: (oriAction) => (payload) => {
              const url = new URL(window.location.href)
              if (url.searchParams.has('url')) {
                url.searchParams.delete('url')
                window.location.replace(url.toString())
              }
              return oriAction(payload)
            }
          }
        }
      }
    }
  }],
})
```

### Future UX work

Through the exploration of this issue, it became apparent that users may not be aware to which web server the Try-it-out function will send requests. While this information is currently presented at the top of the page, understanding may improve by displaying it closer to the "Execute" button where requests are actually made. We'll be exploring these UX improvements over the coming months and welcome community input. Please create a Feature Request under the GitHub Issue tab to start a conversation with us and the community.

## Reflected XSS attack

 

**Warning** in versions <= 3.36.2, it is possible to combine the URL options (as mentioned above) with a vunerability in DOMPurify (https://www.cvedetails.com/cve/CVE-2020-26870/) to create a reflected XSS vector. If your version of Swagger UI is older than or equal to 3.36.2, we suggest you upgrade or implement the workaround as mentioned above.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/425" class=".btn">#425</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency shelljs to 0.8.5 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| shelljs | [`0.8.4` -> `0.8.5`](https://renovatebot.com/diffs/npm/shelljs/0.8.4/0.8.5) |

### GitHub Vulnerability Alerts

#### [GHSA-64g7-mvw6-v9qj](https://togithub.com/shelljs/shelljs/security/advisories/GHSA-64g7-mvw6-v9qj)

### Impact
Output from the synchronous version of `shell.exec()` may be visible to other users on the same system. You may be affected if you execute `shell.exec()` in multi-user Mac, Linux, or WSL environments, or if you execute `shell.exec()` as the root user.

Other shelljs functions (including the asynchronous version of `shell.exec()`) are not impacted.

### Patches
Patched in shelljs 0.8.5

### Workarounds
Recommended action is to upgrade to 0.8.5.

### References
https://huntr.dev/bounties/50996581-c08e-4eed-a90e-c0bac082679c/

### For more information
If you have any questions or comments about this advisory:
* Ask at [https://github.com/shelljs/shelljs/issues/1058](https://togithub.com/shelljs/shelljs/issues/1058)
* Open an issue at https://github.com/shelljs/shelljs/issues/new

#### [CVE-2022-0144](https://nvd.nist.gov/vuln/detail/CVE-2022-0144)

shelljs is vulnerable to Improper Privilege Management

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:38:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/424" class=".btn">#424</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency path-parse to 1.0.7 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| path-parse | [`1.0.6` -> `1.0.7`](https://renovatebot.com/diffs/npm/path-parse/1.0.6/1.0.7) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23343](https://nvd.nist.gov/vuln/detail/CVE-2021-23343)

Affected versions of npm package `path-parse` are vulnerable to Regular Expression Denial of Service (ReDoS) via splitDeviceRe, splitTailRe, and splitPathRe regular expressions. ReDoS exhibits polynomial worst-case time complexity.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/423" class=".btn">#423</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency nth-check to 2.0.1 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| nth-check | [`1.0.2` -> `2.0.1`](https://renovatebot.com/diffs/npm/nth-check/1.0.2/2.0.1) |
| nth-check | [`2.0.0` -> `2.0.1`](https://renovatebot.com/diffs/npm/nth-check/2.0.0/2.0.1) |

### GitHub Vulnerability Alerts

#### [CVE-2021-3803](https://nvd.nist.gov/vuln/detail/CVE-2021-3803)

nth-check is vulnerable to Inefficient Regular Expression Complexity

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency normalize-url to 4.5.1 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| normalize-url | [`4.5.0` -> `4.5.1`](https://renovatebot.com/diffs/npm/normalize-url/4.5.0/4.5.1) |

### GitHub Vulnerability Alerts

#### [CVE-2021-33502](https://nvd.nist.gov/vuln/detail/CVE-2021-33502)

The normalize-url package before 4.5.1, 5.x before 5.3.1, and 6.x before 6.0.1 for Node.js has a ReDoS (regular expression denial of service) issue because it has exponential performance for data: URLs.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:34:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency node-forge to 1.0.0 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| node-forge | [`0.10.0` -> `1.0.0`](https://renovatebot.com/diffs/npm/node-forge/0.10.0/1.0.0) |

### GitHub Vulnerability Alerts

#### [GHSA-gf8q-jrpm-jvxq](https://togithub.com/digitalbazaar/forge/security/advisories/GHSA-gf8q-jrpm-jvxq)

### Impact
The regex used for the `forge.util.parseUrl` API would not properly parse certain inputs resulting in a parsed data structure that could lead to undesired behavior.

### Patches
`forge.util.parseUrl` and other very old related URL APIs were removed in 1.0.0 in favor of letting applications use the more modern WHATWG URL Standard API.

### Workarounds
Ensure code does not directly or indirectly call `forge.util.parseUrl` with untrusted input.

### References
- https://www.huntr.dev/bounties/41852c50-3c6d-4703-8c55-4db27164a4ae/

### For more information
If you have any questions or comments about this advisory:
* Open an issue in [forge](https://togithub.com/digitalbazaar/forge)
* Email us at support@digitalbazaar.com

#### [GHSA-5rrq-pxf6-6jx5](https://togithub.com/digitalbazaar/forge/security/advisories/GHSA-5rrq-pxf6-6jx5)

### Impact
The `forge.debug` API had a potential prototype pollution issue if called with untrusted input. The API was only used for internal debug purposes in a safe way and never documented or advertised.  It is suspected that uses of this API, if any exist, would likely not have used untrusted inputs in a vulnerable way.

### Patches
The `forge.debug` API and related functions were removed in 1.0.0.

### Workarounds
Don't use the `forge.debug` API directly or indirectly with untrusted input.

### References
- https://www.huntr.dev/bounties/1-npm-node-forge/

### For more information
If you have any questions or comments about this advisory:
* Open an issue in [forge](https://togithub.com/digitalbazaar/forge).
* Email us at support@digitalbazaar.com.

#### [CVE-2022-0122](https://nvd.nist.gov/vuln/detail/CVE-2022-0122)

parseUrl functionality in node-forge mishandles certain uses of backslash such as https:/\/\/\ and interprets the URI as a relative path.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:34:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency node-fetch [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| node-fetch | [`2.6.1` -> `2.6.7`](https://renovatebot.com/diffs/npm/node-fetch/2.6.1/2.6.7) |
| node-fetch | [`2.1.2` -> `2.6.1`](https://renovatebot.com/diffs/npm/node-fetch/2.1.2/2.6.1) |

### GitHub Vulnerability Alerts

#### [CVE-2022-0235](https://nvd.nist.gov/vuln/detail/CVE-2022-0235)

node-fetch is vulnerable to Exposure of Sensitive Information to an Unauthorized Actor

#### [CVE-2020-15168](https://togithub.com/node-fetch/node-fetch/security/advisories/GHSA-w7rc-rwvf-8q5r)

### Impact
Node Fetch did not honor the `size` option after following a redirect, which means that when a content size was over the limit, a `FetchError` would never get thrown and the process would end without failure.

For most people, this fix will have a little or no impact. However, if you are relying on node-fetch to gate files above a size, the impact could be significant, for example: If you don't double-check the size of the data after `fetch()` has completed, your JS thread could get tied up doing work on a large file (DoS) and/or cost you money in computing.

### Patches
We released patched versions for both stable and beta channels:

- For `v2`: 2.6.1
- For `v3`: 3.0.0-beta.9

### Workarounds
None, it is strongly recommended to update as soon as possible.

### For more information
If you have any questions or comments about this advisory:
* Open an issue in [node-fetch](https://togithub.com/node-fetch/node-fetch/issues/new?assignees=&labels=question&template=support-or-usage.md&title=Question%3A+)
* Contact one of the core maintainers.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

👻 **Immortal**: This PR will be recreated if closed unmerged. Get [config help](https://togithub.com/renovatebot/renovate/discussions) if that's undesired.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:32:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency nanoid to 3.1.31 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| nanoid | [`3.1.25` -> `3.1.31`](https://renovatebot.com/diffs/npm/nanoid/3.1.25/3.1.31) |
| nanoid | [`3.1.20` -> `3.1.31`](https://renovatebot.com/diffs/npm/nanoid/3.1.20/3.1.31) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23566](https://nvd.nist.gov/vuln/detail/CVE-2021-23566)

The package nanoid before 3.1.31 are vulnerable to Information Exposure via the valueOf() function which allows to reproduce the last id generated.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:29:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/418" class=".btn">#418</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency json-schema to 0.4.0 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| json-schema | [`0.2.3` -> `0.4.0`](https://renovatebot.com/diffs/npm/json-schema/0.2.3/0.4.0) |

### GitHub Vulnerability Alerts

#### [CVE-2021-3918](https://nvd.nist.gov/vuln/detail/CVE-2021-3918)

json-schema is vulnerable to Improperly Controlled Modification of Object Prototype Attributes ('Prototype Pollution')

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:28:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency immer to 9.0.6 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| immer | [`8.0.1` -> `9.0.6`](https://renovatebot.com/diffs/npm/immer/8.0.1/9.0.6) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23436](https://nvd.nist.gov/vuln/detail/CVE-2021-23436)

This affects the package immer before 9.0.6. A type confusion vulnerability can lead to a bypass of CVE-2020-28477 when the user-provided keys used in the path parameter are arrays. In particular, this bypass is possible because the condition (p === "__proto__" || p === "constructor") in applyPatches_ returns false if p is ['__proto__'] (or ['constructor']). The === operator (strict equality operator) returns false if the operands have different type.

#### [CVE-2021-3757](https://nvd.nist.gov/vuln/detail/CVE-2021-3757)

immer is vulnerable to Improperly Controlled Modification of Object Prototype Attributes ('Prototype Pollution')

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:27:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency hosted-git-info to 2.8.9 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| hosted-git-info | [`2.8.8` -> `2.8.9`](https://renovatebot.com/diffs/npm/hosted-git-info/2.8.8/2.8.9) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23362](https://nvd.nist.gov/vuln/detail/CVE-2021-23362)

The npm package `hosted-git-info` before 3.0.8 are vulnerable to Regular Expression Denial of Service (ReDoS) via regular expression shortcutMatch in the fromUrl function in index.js. The affected regular expression exhibits polynomial worst-case time complexity

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:25:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency handlebars to 4.7.7 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| handlebars | [`4.7.6` -> `4.7.7`](https://renovatebot.com/diffs/npm/handlebars/4.7.6/4.7.7) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23369](https://nvd.nist.gov/vuln/detail/CVE-2021-23369)

The package handlebars before 4.7.7 are vulnerable to Remote Code Execution (RCE) when selecting certain compiling options to compile templates coming from an untrusted source.

#### [CVE-2021-23383](https://nvd.nist.gov/vuln/detail/CVE-2021-23383)

The package handlebars before 4.7.7 are vulnerable to Prototype Pollution when selecting certain compiling options to compile templates coming from an untrusted source.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:24:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency grpc to 1.24.4 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| grpc | [`1.24.3` -> `1.24.4`](https://renovatebot.com/diffs/npm/grpc/1.24.3/1.24.4) |

### GitHub Vulnerability Alerts

#### [CVE-2020-7768](https://nvd.nist.gov/vuln/detail/CVE-2020-7768)

"The package grpc before 1.24.4 and the package @&#8203;grpc/grpc-js before 1.1.8 are vulnerable to Prototype Pollution via loadPackageDefinition."

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:24:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency glob-parent to 5.1.2 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| glob-parent | [`3.1.0` -> `5.1.2`](https://renovatebot.com/diffs/npm/glob-parent/3.1.0/5.1.2) |
| glob-parent | [`5.1.1` -> `5.1.2`](https://renovatebot.com/diffs/npm/glob-parent/5.1.1/5.1.2) |

### GitHub Vulnerability Alerts

#### [CVE-2020-28469](https://nvd.nist.gov/vuln/detail/CVE-2020-28469)

This affects the package glob-parent before 5.1.2. The enclosure regex used to check for strings ending in enclosure containing path separator.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:23:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency follow-redirects to 1.14.7 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| follow-redirects | [`1.14.4` -> `1.14.7`](https://renovatebot.com/diffs/npm/follow-redirects/1.14.4/1.14.7) |
| follow-redirects | [`1.13.0` -> `1.14.7`](https://renovatebot.com/diffs/npm/follow-redirects/1.13.0/1.14.7) |

### GitHub Vulnerability Alerts

#### [CVE-2022-0155](https://nvd.nist.gov/vuln/detail/CVE-2022-0155)

follow-redirects is vulnerable to Exposure of Private Personal Information to an Unauthorized Actor

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:21:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency engine.io to 6.1.1 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| engine.io | [`6.0.0` -> `6.1.1`](https://renovatebot.com/diffs/npm/engine.io/6.0.0/6.1.1) |

### GitHub Vulnerability Alerts

#### [CVE-2022-21676](https://togithub.com/socketio/engine.io/security/advisories/GHSA-273r-mgr4-v34f)

### Impact

A specially crafted HTTP request can trigger an uncaught exception on the Engine.IO server, thus killing the Node.js process.

> RangeError: Invalid WebSocket frame: RSV2 and RSV3 must be clear
>   at Receiver.getInfo (/.../node_modules/ws/lib/receiver.js:176:14)
>   at Receiver.startLoop (/.../node_modules/ws/lib/receiver.js:136:22)
>   at Receiver._write (/.../node_modules/ws/lib/receiver.js:83:10)
>   at writeOrBuffer (internal/streams/writable.js:358:12)

This impacts all the users of the [`engine.io`](https://www.npmjs.com/package/engine.io) package starting from version `4.0.0`, including those who uses depending packages like [`socket.io`](https://www.npmjs.com/package/socket.io).

### Patches

A fix has been released for each major branch:

| Version range | Fixed version |
| --- | --- |
| `engine.io@4.x.x` | `4.1.2` |
| `engine.io@5.x.x` | `5.2.1` |
| `engine.io@6.x.x` | `6.1.1` |

Previous versions (`< 4.0.0`) are not impacted.

For `socket.io` users:

| Version range | `engine.io` version | Needs minor update? |
| --- | --- | --- |
| `socket.io@4.4.x` | `~6.1.0` | -
| `socket.io@4.3.x` | `~6.0.0` | Please upgrade to `socket.io@4.4.x`
| `socket.io@4.2.x` | `~5.2.0` | -
| `socket.io@4.1.x` | `~5.1.1` | Please upgrade to `socket.io@4.4.x`
| `socket.io@4.0.x` | `~5.0.0` | Please upgrade to `socket.io@4.4.x`
| `socket.io@3.1.x` | `~4.1.0` | -
| `socket.io@3.0.x` | `~4.0.0` | Please upgrade to `socket.io@3.1.x` or `socket.io@4.4.x` (see [here](https://socket.io/docs/v4/migrating-from-3-x-to-4-0/))

In most cases, running `npm audit fix` should be sufficient. You can also use  `npm update engine.io --depth=9999`.

### Workarounds

There is no known workaround except upgrading to a safe version.

### For more information

If you have any questions or comments about this advisory:

* Open an issue in [`engine.io`](https://togithub.com/socketio/engine.io)

Thanks to Marcus Wejderot from Mevisio for the responsible disclosure.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:20:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency elliptic to 6.5.4 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| elliptic | [`6.3.3` -> `6.5.4`](https://renovatebot.com/diffs/npm/elliptic/6.3.3/6.5.4) |
| elliptic | [`6.5.3` -> `6.5.4`](https://renovatebot.com/diffs/npm/elliptic/6.5.3/6.5.4) |

### GitHub Vulnerability Alerts

#### [CVE-2020-13822](https://nvd.nist.gov/vuln/detail/CVE-2020-13822)

The Elliptic package before version 6.5.3 for Node.js allows ECDSA signature malleability via variations in encoding, leading '\0' bytes, or integer overflows. This could conceivably have a security-relevant impact if an application relied on a single canonical signature.

#### [CVE-2020-28498](https://nvd.nist.gov/vuln/detail/CVE-2020-28498)

The npm package `elliptic` before version 6.5.4 are vulnerable to Cryptographic Issues via the secp256k1 implementation in elliptic/ec/key.js. There is no check to confirm that the public key point passed into the derive function actually exists on the secp256k1 curve. This results in the potential for the private key used in this implementation to be revealed after a number of ECDH operations are performed.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:20:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency browserslist to 4.16.5 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| browserslist | [`4.14.2` -> `4.16.5`](https://renovatebot.com/diffs/npm/browserslist/4.14.2/4.16.5) |

### GitHub Vulnerability Alerts

#### [CVE-2021-23364](https://nvd.nist.gov/vuln/detail/CVE-2021-23364)

The package browserslist from 4.0.0 and before 4.16.5 are vulnerable to Regular Expression Denial of Service (ReDoS) during parsing of queries.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:19:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/408" class=".btn">#408</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency ansi-regex to 5.0.1 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| ansi-regex | [`3.0.0` -> `5.0.1`](https://renovatebot.com/diffs/npm/ansi-regex/3.0.0/5.0.1) |
| ansi-regex | [`4.1.0` -> `5.0.1`](https://renovatebot.com/diffs/npm/ansi-regex/4.1.0/5.0.1) |

### GitHub Vulnerability Alerts

#### [CVE-2021-3807](https://nvd.nist.gov/vuln/detail/CVE-2021-3807)

ansi-regex is vulnerable to Inefficient Regular Expression Complexity

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:16:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/407" class=".btn">#407</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency @openzeppelin/contracts [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| @&#8203;openzeppelin/contracts | [`3.4.2` -> `4.4.1`](https://renovatebot.com/diffs/npm/@openzeppelin%2fcontracts/3.4.2/4.4.1) |
| @&#8203;openzeppelin/contracts | [`4.4.1` -> `4.4.2`](https://renovatebot.com/diffs/npm/@openzeppelin%2fcontracts/4.4.1/4.4.2) |

### GitHub Vulnerability Alerts

#### [GHSA-9c22-pwxw-p6hx](https://togithub.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9c22-pwxw-p6hx)

### Impact

Initializer functions that are invoked separate from contract creation (the most prominent example being minimal proxies) may be reentered if they make an untrusted non-view external call.

Once an initializer has finished running it can never be re-executed. However, an exception put in place to support multiple inheritance made reentrancy possible in the scenario described above, breaking the expectation that there is a single execution.

Note that upgradeable proxies are commonly initialized together with contract creation, where reentrancy is not feasible, so the impact of this issue is believed to be minor.

### Patches

A fix is included in the version v4.4.1 of `@openzeppelin/contracts` and `@openzeppelin/contracts-upgradeable`.

### Workarounds

Avoid untrusted external calls during initialization.

### References
https://github.com/OpenZeppelin/openzeppelin-contracts/pull/3006

### Credits

This issue was identified and reported by @&#8203;chaitinblockchain through [our bug bounty on Immunefi](https://immunefi.com/bounty/openzeppelin/).

### For more information

If you have any questions or comments about this advisory, or need assistance executing the mitigation, email us at security@openzeppelin.com.

#### [GHSA-m6w8-fq7v-ph4m](https://togithub.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-m6w8-fq7v-ph4m)

### Impact

The `GovernorCompatibilityBravo` module may lead to the creation of governance proposals that execute function calls with incorrect arguments due to bad ABI encoding. This happens if the proposal is created using explicit function signatures, e.g. a proposal to invoke the function `foo(uint256)` is created as `propose([target], [0], ["foo(uint256)"], ["0x00..01"])`. If the function selector is provided as part of the encoded proposal data the issue is not present, e.g. the same proposal is created as `propose([target], [0], ["0x2fbebd3800..01"])`, where `2fbebd38` is the function selector.

We've assessed the instances of this contract found on chain, and did not find any occurrence of this bug in the past. Proposal creation through Tally or OpenZeppelin Defender is not affected. The core `Governor` contract on its own is not affected.

### Patches

A fix is included in version v4.4.2 of `@openzeppelin/contracts` and `@openzeppelin/contracts-upgradeable`.

### Workarounds

Do not create proposals using explicit function signatures. Instead, use the `propose` function without the `signatures` argument, and create the proposal using the fully ABI-encoded function call including the function selector in the `calldatas` argument as explained above.

### References

https://github.com/OpenZeppelin/openzeppelin-contracts/issues/3099

### Credits

This issue was identified and reported by @&#8203;GeraldHost.

### For more information

If you have any questions, comments, or need assistance regarding this advisory, email us at security@openzeppelin.com.

To submit security reports please use [our bug bounty on Immunefi](https://immunefi.com/bounty/openzeppelin/).

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

👻 **Immortal**: This PR will be recreated if closed unmerged. Get [config help](https://togithub.com/renovatebot/renovate/discussions) if that's undesired.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:13:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    chore(deps): roll back dependency ws-identity to ^1.0.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Type | Update | Change |
|---|---|---|---|
| [ws-identity](https://togithub.com/brioux/blockchain-carbon-accounting) | devDependencies | rollback | [`^1.0.13` -> `^1.0.12`](https://renovatebot.com/diffs/npm/ws-identity//1.0.12) |

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:12:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    initial supply chain emissions calculation: distance of UPS package by tracking number.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will let you calculate the travel distance of UPS package with its tracking number.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 18:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    initial commit of simple script to get UPS shipment tracking info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 23:59:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    build(deps): bump simple-get from 2.8.1 to 2.8.2 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 2.8.1 to 2.8.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/4e156b6bb19e11ccfad05fad310ea799d63f890d"><code>4e156b6</code></a> 2.8.2</li>
<li><a href="https://github.com/feross/simple-get/commit/43c272db3e4b1383cb03d80338dba3e08c451641"><code>43c272d</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=2.8.1&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 18:46:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    build(deps): bump simple-get from 3.1.0 to 3.1.1 in /net-emissions-token-network/interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 3.1.0 to 3.1.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/496166d2fff21b4ec1d4ab9e7c8d4b2ab11ebf18"><code>496166d</code></a> 3.1.1</li>
<li><a href="https://github.com/feross/simple-get/commit/6eb82c090e30e7146fa5e9ae7212ca16b24b08b4"><code>6eb82c0</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v3.1.0...v3.1.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=3.1.0&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 18:46:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    build(deps): bump simple-get from 2.8.1 to 2.8.2 in /utility-emissions-channel/typescript_app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 2.8.1 to 2.8.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/4e156b6bb19e11ccfad05fad310ea799d63f890d"><code>4e156b6</code></a> 2.8.2</li>
<li><a href="https://github.com/feross/simple-get/commit/43c272db3e4b1383cb03d80338dba3e08c451641"><code>43c272d</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=2.8.1&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 00:09:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    build(deps): bump simple-get from 3.1.0 to 3.1.1 in /net-emissions-token-network/interface/packages/subgraph
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 3.1.0 to 3.1.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/496166d2fff21b4ec1d4ab9e7c8d4b2ab11ebf18"><code>496166d</code></a> 3.1.1</li>
<li><a href="https://github.com/feross/simple-get/commit/6eb82c090e30e7146fa5e9ae7212ca16b24b08b4"><code>6eb82c0</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v3.1.0...v3.1.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=3.1.0&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 00:09:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    feat(OrbitDB): add OrbitDB service to use it outside of chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a service class for interacting with the OrbitDB database containing all the emissions factors and lookup identifiers. Instructions for how to use the service:
* Move into the `utility-emissions-channel/docker-compose-setup/data` directory
* Load in the emissions factors and identifiers using the `src/dataLoader.ts` script
* Fetch or query for emissions factors using the methods provided by the service. An example for usage has been given in the `src/getData.ts` file. Please note that this file must be run with the current working directory being `data` and not `data/src`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 18:57:55 +0000 UTC
    </div>
</div>

