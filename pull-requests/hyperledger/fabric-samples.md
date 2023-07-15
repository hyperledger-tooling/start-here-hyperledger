---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1073" class=".btn">#1073</a>
            </td>
            <td>
                <b>
                    fix typo in high-througput/README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix markdown syntax error and typo
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 08:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    Bump semver from 6.3.0 to 6.3.1 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) from 6.3.0 to 6.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v6.3.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v6.3.0...v6.3.1">6.3.1</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/928e56d21150da0413a3333a3148b20e741a920c"><code>928e56d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/591">#591</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/591">#591</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>, <a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/v6.3.1/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v6.3.0...v6.3.1">6.3.1</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/928e56d21150da0413a3333a3148b20e741a920c"><code>928e56d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/591">#591</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/591">#591</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>, <a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
<h2>6.2.0</h2>
<ul>
<li>Coerce numbers to strings when passed to semver.coerce()</li>
<li>Add <code>rtl</code> option to coerce from right to left</li>
</ul>
<h2>6.1.3</h2>
<ul>
<li>Handle X-ranges properly in includePrerelease mode</li>
</ul>
<h2>6.1.2</h2>
<ul>
<li>Do not throw when testing invalid version strings</li>
</ul>
<h2>6.1.1</h2>
<ul>
<li>Add options support for semver.coerce()</li>
<li>Handle undefined version passed to Range.test</li>
</ul>
<h2>6.1.0</h2>
<ul>
<li>Add semver.compareBuild function</li>
<li>Support <code>*</code> in semver.intersects</li>
</ul>
<h2>6.0</h2>
<ul>
<li>
<p>Fix <code>intersects</code> logic.</p>
<p>This is technically a bug fix, but since it is also a change to behavior
that may require users updating their code, it is marked as a major
version increment.</p>
</li>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/44d27bc007e4827e9b797d6145f1076c127005f2"><code>44d27bc</code></a> chore: release 6.3.1</li>
<li><a href="https://github.com/npm/node-semver/commit/928e56d21150da0413a3333a3148b20e741a920c"><code>928e56d</code></a> fix: better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/591">#591</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/39f632690ea5b1b0d64fa913aa0f96f42b9bde32"><code>39f6326</code></a> chore: <code>@​npmcli/template-oss</code><a href="https://github.com/4"><code>@​4</code></a>.16.0</li>
<li>See full diff in <a href="https://github.com/npm/node-semver/compare/v6.3.0...v6.3.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~lukekarrys">lukekarrys</a>, a new releaser for semver since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=semver&package-manager=npm_and_yarn&previous-version=6.3.0&new-version=6.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 10:05:48 +0000 UTC
    </div>
</div>

