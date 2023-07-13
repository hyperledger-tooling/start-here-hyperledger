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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1508" class=".btn">#1508</a>
            </td>
            <td>
                <b>
                    fix(samples): mediator wallet and http transport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds `IndySdkModule` to `Agent` modules in order to allow it to have a default Wallet and Storage implementation (it could be Askar once we solve the performance issue for node <18 and/or drop support for it).

In `HttpInboundTransport`, It also moves content-type validation to the specific endpoint rather than the whole HTTP server. This is needed to allow using an invitation endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 18:30:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1504" class=".btn">#1504</a>
            </td>
            <td>
                <b>
                    build(deps): bump semver from 5.7.1 to 5.7.2
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 01:54:32 +0000 UTC
    </div>
</div>

