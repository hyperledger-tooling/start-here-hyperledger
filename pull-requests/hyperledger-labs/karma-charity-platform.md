---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Bump semver from 6.3.0 to 6.3.1 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 09:57:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    Bump semver, @angular/cli, @ts-core/angular, @angular-devkit/build-angular and @babel/core in /platform/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) to 7.5.4 and updates ancestor dependencies [semver](https://github.com/npm/node-semver), [@angular/cli](https://github.com/angular/angular-cli), [@ts-core/angular](https://github.com/ManhattanDoctor/ts-core-frontend-angular), [@angular-devkit/build-angular](https://github.com/angular/angular-cli) and [@babel/core](https://github.com/babel/babel/tree/HEAD/packages/babel-core). These dependencies need to be updated together.

Updates `semver` from 7.3.5 to 7.5.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2>v7.5.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2>v7.4.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/36cd334708ec1f85a71445622fb1864bceee0f4e"><code>36cd334</code></a> chore: release 7.5.4</li>
<li><a href="https://github.com/npm/node-semver/commit/8456d87971a447ce295d9f1a396b37b29a972a63"><code>8456d87</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dde1f002baadf7b4cc45504c4046d13586de11b7"><code>dde1f00</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dffcd1b07ec6a192bc0fb405d30d19da46fdc690"><code>dffcd1b</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.16.0 to 4.17.0</li>
<li><a href="https://github.com/npm/node-semver/commit/d619f66513a0fa953177882ecee2c365a65efe97"><code>d619f66</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/3bc42477d1a69361eb79978851be090e5fb4bc2a"><code>3bc4247</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.15.1 to 4.16.0</li>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> fix: trim each range set before parsing</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> fix: correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/4f0f6b19a54b1ba7e1c62af2dfba61f7a4fa68d5"><code>4f0f6b1</code></a> chore: fix arguments in whitespace test (<a href="https://redirect.github.com/npm/node-semver/issues/574">#574</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6bd1a37f95904512015353a3a5dd726f785c9eb8"><code>6bd1a37</code></a> chore: remove duplicate test in semver class (<a href="https://redirect.github.com/npm/node-semver/issues/575">#575</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v7.3.5...v7.5.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~npm-cli-ops">npm-cli-ops</a>, a new releaser for semver since your current version.</p>
</details>
<br />

Updates `@angular/cli` from 13.3.9 to 16.1.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/releases"><code>@​angular/cli</code>'s releases</a>.</em></p>
<blockquote>
<h2>v16.1.4</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><img src="https://img.shields.io/badge/7016cee57-fix-green" alt="fix - 7016cee57" /></a></td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<h2>v16.1.3</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><img src="https://img.shields.io/badge/b56ab0798-fix-green" alt="fix - b56ab0798" /></a></td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<h2>v16.1.2</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.2 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/3475e0281da3298f288a5f8836155c0b8c971372"><img src="https://img.shields.io/badge/3475e0281-fix-green" alt="fix - 3475e0281" /></a></td>
<td>update direct <code>semver</code> dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8108b8c2da3ebfdb74f0f9d3554df01f484670bd"><img src="https://img.shields.io/badge/8108b8c2d-fix-green" alt="fix - 8108b8c2d" /></a></td>
<td>allow linker JIT support with prebundling with esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><img src="https://img.shields.io/badge/502365037-fix-green" alt="fix - 502365037" /></a></td>
<td>use all style language watch files in esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.1</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.1 (2023-06-22)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f017fee2e93a4207b7bfd69c838991546b398753"><img src="https://img.shields.io/badge/f017fee2e-fix-green" alt="fix - f017fee2e" /></a></td>
<td>actually disable Vite prebundling file discovery</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2b4beaca2c32c11508078e082b3338d1edb414a0"><img src="https://img.shields.io/badge/2b4beaca2-fix-green" alt="fix - 2b4beaca2" /></a></td>
<td>experimental esbuild pipeline, add <code>es2015</code> to main fields for RxJS v6 compatibility</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/e3c85e00e6b3390f239aaeb3db6a38fe4b4d2523"><img src="https://img.shields.io/badge/e3c85e00e-fix-green" alt="fix - e3c85e00e" /></a></td>
<td>track postcss provided file dependencies in esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/1419fff887173e331690fb0a664a081154842554"><img src="https://img.shields.io/badge/1419fff88-fix-green" alt="fix - 1419fff88" /></a></td>
<td>unpin and downgrade <code>browserslist</code></td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/950a4b60f046117867755ccd005f0e04bcc403a7"><img src="https://img.shields.io/badge/950a4b60f-fix-green" alt="fix - 950a4b60f" /></a></td>
<td>watch all bundler provided inputs with esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.0 (2023-06-13)</h1>
<h3><code>@​schematics/angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b14b959901d5a670da0df45e082b8fd4c3392d14"><img src="https://img.shields.io/badge/b14b95990-feat-blue" alt="feat - b14b95990" /></a></td>
<td>add bootstrap-agnostic utilities for writing ng-add schematics</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<p>| Commit | Description |</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/blob/main/CHANGELOG.md"><code>@​angular/cli</code>'s changelog</a>.</em></p>
<blockquote>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f">7016cee57</a></td>
<td>fix</td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8">b56ab0798</a></td>
<td>fix</td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>15.2.9 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f36e38a913b454ec340d6bf2311391c5df1cee24">f36e38a91</a></td>
<td>fix</td>
<td>update direct semver dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.2.0-next.0 (2023-06-28)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/c05c83be7c6c8bcdad4be8686a6e0701a55304cc">c05c83be7</a></td>
<td>feat</td>
<td>add initial application builder implementation</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2a3fc68460152a48758b9353bff48193641861c5">2a3fc6846</a></td>
<td>feat</td>
<td>add preload hints based on transitive initial files</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f42f10135c1e2184a9080b726dc5e41669937b13">f42f10135</a></td>
<td>fix</td>
<td>ensure preload hints for external stylesheets are marked as styles</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular-cli/commit/e009075e9024751c5ed1535b1f4903db7b9e343a"><code>e009075</code></a> release: cut the v16.1.4 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/68cbf1229d692940ca90ac797215489781d2ea05"><code>68cbf12</code></a> build: update <code>@babel/generator</code> to <code>7.22.8</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/258cde5462a6ddfb81cb64dc695ac43a21b6adda"><code>258cde5</code></a> test: convert e2e_runner <code>ignore</code> to array</li>
<li><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><code>7016cee</code></a> fix(<code>@​angular-devkit/build-angular</code>): normalize paths in loader cache with esbuild</li>
<li><a href="https://github.com/angular/angular-cli/commit/d3310b230bdf936b745fa6d6e9dd37fc43a8231a"><code>d3310b2</code></a> release: cut the v16.1.3 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><code>b56ab07</code></a> fix(<code>@​angular-devkit/build-angular</code>): use absolute watch paths for postcss depe...</li>
<li><a href="https://github.com/angular/angular-cli/commit/da6ec6f695a6333c16f873efd62ee1ee197c595f"><code>da6ec6f</code></a> build: update Angular peer dependencies to <code>^16.0.0</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/f039ee9af68be2dcd84846393cab530739ead202"><code>f039ee9</code></a> release: cut the v16.1.2 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/f8aff00a924073ae3fd9e68123c52ba5c58ff0dd"><code>f8aff00</code></a> refactor: remove <code>keepNames</code> esbuild option for server builds</li>
<li><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><code>5023650</code></a> fix(<code>@​angular-devkit/build-angular</code>): use all style language watch files in esb...</li>
<li>Additional commits viewable in <a href="https://github.com/angular/angular-cli/compare/13.3.9...16.1.4">compare view</a></li>
</ul>
</details>
<br />

Updates `@ts-core/angular` from 13.1.34 to 15.0.27
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/ManhattanDoctor/ts-core-frontend-angular/commits">compare view</a></li>
</ul>
</details>
<br />

Updates `@angular-devkit/build-angular` from 13.3.9 to 16.1.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/releases"><code>@​angular-devkit/build-angular</code>'s releases</a>.</em></p>
<blockquote>
<h2>v16.1.4</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><img src="https://img.shields.io/badge/7016cee57-fix-green" alt="fix - 7016cee57" /></a></td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<h2>v16.1.3</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><img src="https://img.shields.io/badge/b56ab0798-fix-green" alt="fix - b56ab0798" /></a></td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<h2>v16.1.2</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.2 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/3475e0281da3298f288a5f8836155c0b8c971372"><img src="https://img.shields.io/badge/3475e0281-fix-green" alt="fix - 3475e0281" /></a></td>
<td>update direct <code>semver</code> dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8108b8c2da3ebfdb74f0f9d3554df01f484670bd"><img src="https://img.shields.io/badge/8108b8c2d-fix-green" alt="fix - 8108b8c2d" /></a></td>
<td>allow linker JIT support with prebundling with esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><img src="https://img.shields.io/badge/502365037-fix-green" alt="fix - 502365037" /></a></td>
<td>use all style language watch files in esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.1</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.1 (2023-06-22)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f017fee2e93a4207b7bfd69c838991546b398753"><img src="https://img.shields.io/badge/f017fee2e-fix-green" alt="fix - f017fee2e" /></a></td>
<td>actually disable Vite prebundling file discovery</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2b4beaca2c32c11508078e082b3338d1edb414a0"><img src="https://img.shields.io/badge/2b4beaca2-fix-green" alt="fix - 2b4beaca2" /></a></td>
<td>experimental esbuild pipeline, add <code>es2015</code> to main fields for RxJS v6 compatibility</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/e3c85e00e6b3390f239aaeb3db6a38fe4b4d2523"><img src="https://img.shields.io/badge/e3c85e00e-fix-green" alt="fix - e3c85e00e" /></a></td>
<td>track postcss provided file dependencies in esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/1419fff887173e331690fb0a664a081154842554"><img src="https://img.shields.io/badge/1419fff88-fix-green" alt="fix - 1419fff88" /></a></td>
<td>unpin and downgrade <code>browserslist</code></td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/950a4b60f046117867755ccd005f0e04bcc403a7"><img src="https://img.shields.io/badge/950a4b60f-fix-green" alt="fix - 950a4b60f" /></a></td>
<td>watch all bundler provided inputs with esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.0 (2023-06-13)</h1>
<h3><code>@​schematics/angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b14b959901d5a670da0df45e082b8fd4c3392d14"><img src="https://img.shields.io/badge/b14b95990-feat-blue" alt="feat - b14b95990" /></a></td>
<td>add bootstrap-agnostic utilities for writing ng-add schematics</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<p>| Commit | Description |</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/blob/main/CHANGELOG.md"><code>@​angular-devkit/build-angular</code>'s changelog</a>.</em></p>
<blockquote>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f">7016cee57</a></td>
<td>fix</td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8">b56ab0798</a></td>
<td>fix</td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>15.2.9 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f36e38a913b454ec340d6bf2311391c5df1cee24">f36e38a91</a></td>
<td>fix</td>
<td>update direct semver dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.2.0-next.0 (2023-06-28)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/c05c83be7c6c8bcdad4be8686a6e0701a55304cc">c05c83be7</a></td>
<td>feat</td>
<td>add initial application builder implementation</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2a3fc68460152a48758b9353bff48193641861c5">2a3fc6846</a></td>
<td>feat</td>
<td>add preload hints based on transitive initial files</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f42f10135c1e2184a9080b726dc5e41669937b13">f42f10135</a></td>
<td>fix</td>
<td>ensure preload hints for external stylesheets are marked as styles</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular-cli/commit/e009075e9024751c5ed1535b1f4903db7b9e343a"><code>e009075</code></a> release: cut the v16.1.4 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/68cbf1229d692940ca90ac797215489781d2ea05"><code>68cbf12</code></a> build: update <code>@babel/generator</code> to <code>7.22.8</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/258cde5462a6ddfb81cb64dc695ac43a21b6adda"><code>258cde5</code></a> test: convert e2e_runner <code>ignore</code> to array</li>
<li><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><code>7016cee</code></a> fix(<code>@​angular-devkit/build-angular</code>): normalize paths in loader cache with esbuild</li>
<li><a href="https://github.com/angular/angular-cli/commit/d3310b230bdf936b745fa6d6e9dd37fc43a8231a"><code>d3310b2</code></a> release: cut the v16.1.3 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><code>b56ab07</code></a> fix(<code>@​angular-devkit/build-angular</code>): use absolute watch paths for postcss depe...</li>
<li><a href="https://github.com/angular/angular-cli/commit/da6ec6f695a6333c16f873efd62ee1ee197c595f"><code>da6ec6f</code></a> build: update Angular peer dependencies to <code>^16.0.0</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/f039ee9af68be2dcd84846393cab530739ead202"><code>f039ee9</code></a> release: cut the v16.1.2 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/f8aff00a924073ae3fd9e68123c52ba5c58ff0dd"><code>f8aff00</code></a> refactor: remove <code>keepNames</code> esbuild option for server builds</li>
<li><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><code>5023650</code></a> fix(<code>@​angular-devkit/build-angular</code>): use all style language watch files in esb...</li>
<li>Additional commits viewable in <a href="https://github.com/angular/angular-cli/compare/13.3.9...16.1.4">compare view</a></li>
</ul>
</details>
<br />

Updates `@babel/core` from 7.18.10 to 7.22.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.22.5 (2023-06-08)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15675">#15675</a> Fix using <code>syntax-unicode-sets-regex</code> in standalone (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-core</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15683">#15683</a> Suggest <code>-transform-</code> when resolving missing plugins (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 4</h4>
<ul>
<li>Avery (<a href="https://github.com/nullableVoidPtr"><code>@​nullableVoidPtr</code></a>)</li>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
</ul>
<h2>v7.22.4 (2023-05-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15649">#15649</a> Set <code>shorthand: false</code> when renaming an identifier inside an object property (<a href="https://github.com/coderaiser"><code>@​coderaiser</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li><code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15666">#15666</a> Add missing <code>attributes</code>/<code>assertions</code> to <code>VISITOR_KEYS</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15667">#15667</a> Mark <code>assert</code> attributes with <code>extra.deprecatedAssertSyntax</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>coderaiser (<a href="https://github.com/coderaiser"><code>@​coderaiser</code></a>)</li>
</ul>
<h2>v7.22.3 (2023-05-27)</h2>
<ul>
<li>Re-publish all the package published in 7.22.0 that hadn't been republished yet. We accidentally published them with a <code>package.json</code> file containing <code>&quot;type&quot;: &quot;script&quot;</code> instead of <code>&quot;type&quot;: &quot;commonjs&quot;</code> (<a href="https://redirect.github.com/babel/babel/issues/15664">#15664</a>).</li>
</ul>
<h2>v7.22.2 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15660">#15660</a> Fix importing symbol polyfill in <code>@babel/runtime-corejs2</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
<h2>v7.22.1 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.22.5 (2023-06-08)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15675">#15675</a> Fix using <code>syntax-unicode-sets-regex</code> in standalone (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-core</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15683">#15683</a> Suggest <code>-transform-</code> when resolving missing plugins (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.4 (2023-05-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15649">#15649</a> Set <code>shorthand: false</code> when renaming an identifier inside an object property (<a href="https://github.com/coderaiser"><code>@​coderaiser</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li><code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15666">#15666</a> Add missing <code>attributes</code>/<code>assertions</code> to <code>VISITOR_KEYS</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15667">#15667</a> Mark <code>assert</code> attributes with <code>extra.deprecatedAssertSyntax</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.3 (2023-05-27)</h2>
<ul>
<li>Re-publish all the package published in 7.22.0 that hadn't been republished yet. We accidentally published them with a <code>package.json</code> file containing <code>&quot;type&quot;: &quot;script&quot;</code> instead of <code>&quot;type&quot;: &quot;commonjs&quot;</code> (<a href="https://redirect.github.com/babel/babel/issues/15664">#15664</a>).</li>
</ul>
<h2>v7.22.2 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15660">#15660</a> Fix importing symbol polyfill in <code>@babel/runtime-corejs2</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.1 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15658">#15658</a> Workaround for broken babel-preset-react-app (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.0 (2023-05-26)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>babel-parser</code>, <code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15497">#15497</a> [ts] Support <code>import ... =</code> and <code>export =</code> in scripts (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-core</code>, <code>babel-plugin-proposal-unicode-sets-regex</code>, <code>babel-plugin-transform-unicode-sets-regex</code>, <code>babel-preset-env</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15636">#15636</a> Add <code>unicode-sets-regex</code> transform to <code>preset-env</code> (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-runtime</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15633">#15633</a> Implement transform support for <code>using</code> declarations (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-import-attributes-to-assertions</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15620">#15620</a> Create <code>@babel/plugin-proposal-import-attributes-to-assertions</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-core</code>, <code>babel-generator</code>, <code>babel-parser</code>, <code>babel-plugin-syntax-import-attributes</code>, <code>babel-preset-env</code>, <code>babel-standalone</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15536">#15536</a> Add support for the updated import attributes proposal (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>, <code>babel-parser</code>, <code>babel-traverse</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15520">#15520</a> Parse <code>await using</code> declarations (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/08564ea23070524f31ddf12c6677e9699073dd69"><code>08564ea</code></a> v7.22.5</li>
<li><a href="https://github.com/babel/babel/commit/17162e5d8d900817aa95acf0636ed0539320a12f"><code>17162e5</code></a> Suggest <code>-transform-</code> when resolving missing plugins (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15683">#15683</a>)</li>
<li><a href="https://github.com/babel/babel/commit/72006cb657ae3f587bf1624a1ed4df4ff297e059"><code>72006cb</code></a> Use Prettier v3.0.0-alpha.12 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15617">#15617</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ecc819bf75dac9173ecf0e772a3257d811f94de7"><code>ecc819b</code></a> [babel 8] Require Node.js <code>^16.20.0 || ^18.16.0 || &gt;=20.0.0</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15585">#15585</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ae5f07376b79a2cab9d178e68d57bbfddc674a11"><code>ae5f073</code></a> v7.22.1</li>
<li><a href="https://github.com/babel/babel/commit/f64974d6ac747154845d1fd123b1abe56b07332e"><code>f64974d</code></a> chore: Improve development experience about global variables (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15646">#15646</a>)</li>
<li><a href="https://github.com/babel/babel/commit/389ecb08ed502cd13671928c1ab9caccb72f0a6f"><code>389ecb0</code></a> v7.22.0</li>
<li><a href="https://github.com/babel/babel/commit/696784a43367857a774eb2764fd5c3efdcf94002"><code>696784a</code></a> Add <code>unicode-sets-regex</code> transform to <code>preset-env</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15636">#15636</a>)</li>
<li><a href="https://github.com/babel/babel/commit/4b5ebdc9b3921b4dab7f0e10a37779788208a96a"><code>4b5ebdc</code></a> Add support for the updated import attributes proposal (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15536">#15536</a>)</li>
<li><a href="https://github.com/babel/babel/commit/920b78c0c22b242a86178dc3556e54e442a05aec"><code>920b78c</code></a> Enable regexp unicode sets parsing by default (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15638">#15638</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.22.5/packages/babel-core">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 11:16:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/115" class=".btn">#115</a>
            </td>
            <td>
                <b>
                    Bump semver from 7.3.8 to 7.5.4 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [semver](https://github.com/npm/node-semver) from 7.3.8 to 7.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2>v7.5.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2>v7.4.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/36cd334708ec1f85a71445622fb1864bceee0f4e"><code>36cd334</code></a> chore: release 7.5.4</li>
<li><a href="https://github.com/npm/node-semver/commit/8456d87971a447ce295d9f1a396b37b29a972a63"><code>8456d87</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dde1f002baadf7b4cc45504c4046d13586de11b7"><code>dde1f00</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dffcd1b07ec6a192bc0fb405d30d19da46fdc690"><code>dffcd1b</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.16.0 to 4.17.0</li>
<li><a href="https://github.com/npm/node-semver/commit/d619f66513a0fa953177882ecee2c365a65efe97"><code>d619f66</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/3bc42477d1a69361eb79978851be090e5fb4bc2a"><code>3bc4247</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.15.1 to 4.16.0</li>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> fix: trim each range set before parsing</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> fix: correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/4f0f6b19a54b1ba7e1c62af2dfba61f7a4fa68d5"><code>4f0f6b1</code></a> chore: fix arguments in whitespace test (<a href="https://redirect.github.com/npm/node-semver/issues/574">#574</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6bd1a37f95904512015353a3a5dd726f785c9eb8"><code>6bd1a37</code></a> chore: remove duplicate test in semver class (<a href="https://redirect.github.com/npm/node-semver/issues/575">#575</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.5.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~npm-cli-ops">npm-cli-ops</a>, a new releaser for semver since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=semver&package-manager=npm_and_yarn&previous-version=7.3.8&new-version=7.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 11:15:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Bump semver, @angular/cli, @angular-devkit/build-angular and @babel/core in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) to 7.5.4 and updates ancestor dependencies [semver](https://github.com/npm/node-semver), [@angular/cli](https://github.com/angular/angular-cli), [@angular-devkit/build-angular](https://github.com/angular/angular-cli) and [@babel/core](https://github.com/babel/babel/tree/HEAD/packages/babel-core). These dependencies need to be updated together.

Updates `semver` from 7.3.5 to 7.5.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2>v7.5.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2>v7.4.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/36cd334708ec1f85a71445622fb1864bceee0f4e"><code>36cd334</code></a> chore: release 7.5.4</li>
<li><a href="https://github.com/npm/node-semver/commit/8456d87971a447ce295d9f1a396b37b29a972a63"><code>8456d87</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dde1f002baadf7b4cc45504c4046d13586de11b7"><code>dde1f00</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/dffcd1b07ec6a192bc0fb405d30d19da46fdc690"><code>dffcd1b</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.16.0 to 4.17.0</li>
<li><a href="https://github.com/npm/node-semver/commit/d619f66513a0fa953177882ecee2c365a65efe97"><code>d619f66</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/3bc42477d1a69361eb79978851be090e5fb4bc2a"><code>3bc4247</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.15.1 to 4.16.0</li>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> fix: trim each range set before parsing</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> fix: correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/4f0f6b19a54b1ba7e1c62af2dfba61f7a4fa68d5"><code>4f0f6b1</code></a> chore: fix arguments in whitespace test (<a href="https://redirect.github.com/npm/node-semver/issues/574">#574</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6bd1a37f95904512015353a3a5dd726f785c9eb8"><code>6bd1a37</code></a> chore: remove duplicate test in semver class (<a href="https://redirect.github.com/npm/node-semver/issues/575">#575</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v7.3.5...v7.5.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~npm-cli-ops">npm-cli-ops</a>, a new releaser for semver since your current version.</p>
</details>
<br />

Updates `@angular/cli` from 13.2.3 to 16.1.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/releases"><code>@​angular/cli</code>'s releases</a>.</em></p>
<blockquote>
<h2>v16.1.4</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><img src="https://img.shields.io/badge/7016cee57-fix-green" alt="fix - 7016cee57" /></a></td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<h2>v16.1.3</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><img src="https://img.shields.io/badge/b56ab0798-fix-green" alt="fix - b56ab0798" /></a></td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<h2>v16.1.2</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.2 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/3475e0281da3298f288a5f8836155c0b8c971372"><img src="https://img.shields.io/badge/3475e0281-fix-green" alt="fix - 3475e0281" /></a></td>
<td>update direct <code>semver</code> dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8108b8c2da3ebfdb74f0f9d3554df01f484670bd"><img src="https://img.shields.io/badge/8108b8c2d-fix-green" alt="fix - 8108b8c2d" /></a></td>
<td>allow linker JIT support with prebundling with esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><img src="https://img.shields.io/badge/502365037-fix-green" alt="fix - 502365037" /></a></td>
<td>use all style language watch files in esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.1</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.1 (2023-06-22)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f017fee2e93a4207b7bfd69c838991546b398753"><img src="https://img.shields.io/badge/f017fee2e-fix-green" alt="fix - f017fee2e" /></a></td>
<td>actually disable Vite prebundling file discovery</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2b4beaca2c32c11508078e082b3338d1edb414a0"><img src="https://img.shields.io/badge/2b4beaca2-fix-green" alt="fix - 2b4beaca2" /></a></td>
<td>experimental esbuild pipeline, add <code>es2015</code> to main fields for RxJS v6 compatibility</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/e3c85e00e6b3390f239aaeb3db6a38fe4b4d2523"><img src="https://img.shields.io/badge/e3c85e00e-fix-green" alt="fix - e3c85e00e" /></a></td>
<td>track postcss provided file dependencies in esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/1419fff887173e331690fb0a664a081154842554"><img src="https://img.shields.io/badge/1419fff88-fix-green" alt="fix - 1419fff88" /></a></td>
<td>unpin and downgrade <code>browserslist</code></td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/950a4b60f046117867755ccd005f0e04bcc403a7"><img src="https://img.shields.io/badge/950a4b60f-fix-green" alt="fix - 950a4b60f" /></a></td>
<td>watch all bundler provided inputs with esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.0 (2023-06-13)</h1>
<h3><code>@​schematics/angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b14b959901d5a670da0df45e082b8fd4c3392d14"><img src="https://img.shields.io/badge/b14b95990-feat-blue" alt="feat - b14b95990" /></a></td>
<td>add bootstrap-agnostic utilities for writing ng-add schematics</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<p>| Commit | Description |</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/blob/main/CHANGELOG.md"><code>@​angular/cli</code>'s changelog</a>.</em></p>
<blockquote>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f">7016cee57</a></td>
<td>fix</td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8">b56ab0798</a></td>
<td>fix</td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>15.2.9 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f36e38a913b454ec340d6bf2311391c5df1cee24">f36e38a91</a></td>
<td>fix</td>
<td>update direct semver dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.2.0-next.0 (2023-06-28)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/c05c83be7c6c8bcdad4be8686a6e0701a55304cc">c05c83be7</a></td>
<td>feat</td>
<td>add initial application builder implementation</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2a3fc68460152a48758b9353bff48193641861c5">2a3fc6846</a></td>
<td>feat</td>
<td>add preload hints based on transitive initial files</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f42f10135c1e2184a9080b726dc5e41669937b13">f42f10135</a></td>
<td>fix</td>
<td>ensure preload hints for external stylesheets are marked as styles</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular-cli/commit/e009075e9024751c5ed1535b1f4903db7b9e343a"><code>e009075</code></a> release: cut the v16.1.4 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/68cbf1229d692940ca90ac797215489781d2ea05"><code>68cbf12</code></a> build: update <code>@babel/generator</code> to <code>7.22.8</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/258cde5462a6ddfb81cb64dc695ac43a21b6adda"><code>258cde5</code></a> test: convert e2e_runner <code>ignore</code> to array</li>
<li><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><code>7016cee</code></a> fix(<code>@​angular-devkit/build-angular</code>): normalize paths in loader cache with esbuild</li>
<li><a href="https://github.com/angular/angular-cli/commit/d3310b230bdf936b745fa6d6e9dd37fc43a8231a"><code>d3310b2</code></a> release: cut the v16.1.3 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><code>b56ab07</code></a> fix(<code>@​angular-devkit/build-angular</code>): use absolute watch paths for postcss depe...</li>
<li><a href="https://github.com/angular/angular-cli/commit/da6ec6f695a6333c16f873efd62ee1ee197c595f"><code>da6ec6f</code></a> build: update Angular peer dependencies to <code>^16.0.0</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/f039ee9af68be2dcd84846393cab530739ead202"><code>f039ee9</code></a> release: cut the v16.1.2 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/f8aff00a924073ae3fd9e68123c52ba5c58ff0dd"><code>f8aff00</code></a> refactor: remove <code>keepNames</code> esbuild option for server builds</li>
<li><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><code>5023650</code></a> fix(<code>@​angular-devkit/build-angular</code>): use all style language watch files in esb...</li>
<li>Additional commits viewable in <a href="https://github.com/angular/angular-cli/compare/13.2.3...16.1.4">compare view</a></li>
</ul>
</details>
<br />

Updates `@angular-devkit/build-angular` from 13.2.3 to 16.1.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/releases"><code>@​angular-devkit/build-angular</code>'s releases</a>.</em></p>
<blockquote>
<h2>v16.1.4</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><img src="https://img.shields.io/badge/7016cee57-fix-green" alt="fix - 7016cee57" /></a></td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<h2>v16.1.3</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><img src="https://img.shields.io/badge/b56ab0798-fix-green" alt="fix - b56ab0798" /></a></td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<h2>v16.1.2</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.2 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/3475e0281da3298f288a5f8836155c0b8c971372"><img src="https://img.shields.io/badge/3475e0281-fix-green" alt="fix - 3475e0281" /></a></td>
<td>update direct <code>semver</code> dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8108b8c2da3ebfdb74f0f9d3554df01f484670bd"><img src="https://img.shields.io/badge/8108b8c2d-fix-green" alt="fix - 8108b8c2d" /></a></td>
<td>allow linker JIT support with prebundling with esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><img src="https://img.shields.io/badge/502365037-fix-green" alt="fix - 502365037" /></a></td>
<td>use all style language watch files in esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.1</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.1 (2023-06-22)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f017fee2e93a4207b7bfd69c838991546b398753"><img src="https://img.shields.io/badge/f017fee2e-fix-green" alt="fix - f017fee2e" /></a></td>
<td>actually disable Vite prebundling file discovery</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2b4beaca2c32c11508078e082b3338d1edb414a0"><img src="https://img.shields.io/badge/2b4beaca2-fix-green" alt="fix - 2b4beaca2" /></a></td>
<td>experimental esbuild pipeline, add <code>es2015</code> to main fields for RxJS v6 compatibility</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/e3c85e00e6b3390f239aaeb3db6a38fe4b4d2523"><img src="https://img.shields.io/badge/e3c85e00e-fix-green" alt="fix - e3c85e00e" /></a></td>
<td>track postcss provided file dependencies in esbuild builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/1419fff887173e331690fb0a664a081154842554"><img src="https://img.shields.io/badge/1419fff88-fix-green" alt="fix - 1419fff88" /></a></td>
<td>unpin and downgrade <code>browserslist</code></td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/950a4b60f046117867755ccd005f0e04bcc403a7"><img src="https://img.shields.io/badge/950a4b60f-fix-green" alt="fix - 950a4b60f" /></a></td>
<td>watch all bundler provided inputs with esbuild builder</td>
</tr>
</tbody>
</table>
<h2>v16.1.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.0 (2023-06-13)</h1>
<h3><code>@​schematics/angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b14b959901d5a670da0df45e082b8fd4c3392d14"><img src="https://img.shields.io/badge/b14b95990-feat-blue" alt="feat - b14b95990" /></a></td>
<td>add bootstrap-agnostic utilities for writing ng-add schematics</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<p>| Commit | Description |</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/blob/main/CHANGELOG.md"><code>@​angular-devkit/build-angular</code>'s changelog</a>.</em></p>
<blockquote>
<h1>16.1.4 (2023-07-06)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f">7016cee57</a></td>
<td>fix</td>
<td>normalize paths in loader cache with esbuild</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.1.3 (2023-06-29)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8">b56ab0798</a></td>
<td>fix</td>
<td>use absolute watch paths for postcss dependency messages</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>15.2.9 (2023-06-28)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f36e38a913b454ec340d6bf2311391c5df1cee24">f36e38a91</a></td>
<td>fix</td>
<td>update direct semver dependencies to 7.5.3</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>16.2.0-next.0 (2023-06-28)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/c05c83be7c6c8bcdad4be8686a6e0701a55304cc">c05c83be7</a></td>
<td>feat</td>
<td>add initial application builder implementation</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2a3fc68460152a48758b9353bff48193641861c5">2a3fc6846</a></td>
<td>feat</td>
<td>add preload hints based on transitive initial files</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f42f10135c1e2184a9080b726dc5e41669937b13">f42f10135</a></td>
<td>fix</td>
<td>ensure preload hints for external stylesheets are marked as styles</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular-cli/commit/e009075e9024751c5ed1535b1f4903db7b9e343a"><code>e009075</code></a> release: cut the v16.1.4 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/68cbf1229d692940ca90ac797215489781d2ea05"><code>68cbf12</code></a> build: update <code>@babel/generator</code> to <code>7.22.8</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/258cde5462a6ddfb81cb64dc695ac43a21b6adda"><code>258cde5</code></a> test: convert e2e_runner <code>ignore</code> to array</li>
<li><a href="https://github.com/angular/angular-cli/commit/7016cee5783b2762d550db8f2a4f29e7b56f317f"><code>7016cee</code></a> fix(<code>@​angular-devkit/build-angular</code>): normalize paths in loader cache with esbuild</li>
<li><a href="https://github.com/angular/angular-cli/commit/d3310b230bdf936b745fa6d6e9dd37fc43a8231a"><code>d3310b2</code></a> release: cut the v16.1.3 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/b56ab07980c5d990606ddb1e298fc1c4ecf8a2a8"><code>b56ab07</code></a> fix(<code>@​angular-devkit/build-angular</code>): use absolute watch paths for postcss depe...</li>
<li><a href="https://github.com/angular/angular-cli/commit/da6ec6f695a6333c16f873efd62ee1ee197c595f"><code>da6ec6f</code></a> build: update Angular peer dependencies to <code>^16.0.0</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/f039ee9af68be2dcd84846393cab530739ead202"><code>f039ee9</code></a> release: cut the v16.1.2 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/f8aff00a924073ae3fd9e68123c52ba5c58ff0dd"><code>f8aff00</code></a> refactor: remove <code>keepNames</code> esbuild option for server builds</li>
<li><a href="https://github.com/angular/angular-cli/commit/502365037bf7dbacd0e28d29a074a246971848ea"><code>5023650</code></a> fix(<code>@​angular-devkit/build-angular</code>): use all style language watch files in esb...</li>
<li>Additional commits viewable in <a href="https://github.com/angular/angular-cli/compare/13.2.3...16.1.4">compare view</a></li>
</ul>
</details>
<br />

Updates `@babel/core` from 7.16.12 to 7.22.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.22.5 (2023-06-08)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15675">#15675</a> Fix using <code>syntax-unicode-sets-regex</code> in standalone (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-core</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15683">#15683</a> Suggest <code>-transform-</code> when resolving missing plugins (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 4</h4>
<ul>
<li>Avery (<a href="https://github.com/nullableVoidPtr"><code>@​nullableVoidPtr</code></a>)</li>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
</ul>
<h2>v7.22.4 (2023-05-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15649">#15649</a> Set <code>shorthand: false</code> when renaming an identifier inside an object property (<a href="https://github.com/coderaiser"><code>@​coderaiser</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li><code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15666">#15666</a> Add missing <code>attributes</code>/<code>assertions</code> to <code>VISITOR_KEYS</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15667">#15667</a> Mark <code>assert</code> attributes with <code>extra.deprecatedAssertSyntax</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 3</h4>
<ul>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>coderaiser (<a href="https://github.com/coderaiser"><code>@​coderaiser</code></a>)</li>
</ul>
<h2>v7.22.3 (2023-05-27)</h2>
<ul>
<li>Re-publish all the package published in 7.22.0 that hadn't been republished yet. We accidentally published them with a <code>package.json</code> file containing <code>&quot;type&quot;: &quot;script&quot;</code> instead of <code>&quot;type&quot;: &quot;commonjs&quot;</code> (<a href="https://redirect.github.com/babel/babel/issues/15664">#15664</a>).</li>
</ul>
<h2>v7.22.2 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15660">#15660</a> Fix importing symbol polyfill in <code>@babel/runtime-corejs2</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 1</h4>
<ul>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
<h2>v7.22.1 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.22.5 (2023-06-08)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15675">#15675</a> Fix using <code>syntax-unicode-sets-regex</code> in standalone (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-core</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15683">#15683</a> Suggest <code>-transform-</code> when resolving missing plugins (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.4 (2023-05-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15649">#15649</a> Set <code>shorthand: false</code> when renaming an identifier inside an object property (<a href="https://github.com/coderaiser"><code>@​coderaiser</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li><code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15666">#15666</a> Add missing <code>attributes</code>/<code>assertions</code> to <code>VISITOR_KEYS</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15667">#15667</a> Mark <code>assert</code> attributes with <code>extra.deprecatedAssertSyntax</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.3 (2023-05-27)</h2>
<ul>
<li>Re-publish all the package published in 7.22.0 that hadn't been republished yet. We accidentally published them with a <code>package.json</code> file containing <code>&quot;type&quot;: &quot;script&quot;</code> instead of <code>&quot;type&quot;: &quot;commonjs&quot;</code> (<a href="https://redirect.github.com/babel/babel/issues/15664">#15664</a>).</li>
</ul>
<h2>v7.22.2 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15660">#15660</a> Fix importing symbol polyfill in <code>@babel/runtime-corejs2</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.1 (2023-05-26)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15658">#15658</a> Workaround for broken babel-preset-react-app (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.22.0 (2023-05-26)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>babel-parser</code>, <code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15497">#15497</a> [ts] Support <code>import ... =</code> and <code>export =</code> in scripts (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-core</code>, <code>babel-plugin-proposal-unicode-sets-regex</code>, <code>babel-plugin-transform-unicode-sets-regex</code>, <code>babel-preset-env</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15636">#15636</a> Add <code>unicode-sets-regex</code> transform to <code>preset-env</code> (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-runtime</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>, <code>babel-standalone</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15633">#15633</a> Implement transform support for <code>using</code> declarations (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-import-attributes-to-assertions</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15620">#15620</a> Create <code>@babel/plugin-proposal-import-attributes-to-assertions</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-core</code>, <code>babel-generator</code>, <code>babel-parser</code>, <code>babel-plugin-syntax-import-attributes</code>, <code>babel-preset-env</code>, <code>babel-standalone</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15536">#15536</a> Add support for the updated import attributes proposal (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>, <code>babel-parser</code>, <code>babel-traverse</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15520">#15520</a> Parse <code>await using</code> declarations (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/08564ea23070524f31ddf12c6677e9699073dd69"><code>08564ea</code></a> v7.22.5</li>
<li><a href="https://github.com/babel/babel/commit/17162e5d8d900817aa95acf0636ed0539320a12f"><code>17162e5</code></a> Suggest <code>-transform-</code> when resolving missing plugins (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15683">#15683</a>)</li>
<li><a href="https://github.com/babel/babel/commit/72006cb657ae3f587bf1624a1ed4df4ff297e059"><code>72006cb</code></a> Use Prettier v3.0.0-alpha.12 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15617">#15617</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ecc819bf75dac9173ecf0e772a3257d811f94de7"><code>ecc819b</code></a> [babel 8] Require Node.js <code>^16.20.0 || ^18.16.0 || &gt;=20.0.0</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15585">#15585</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ae5f07376b79a2cab9d178e68d57bbfddc674a11"><code>ae5f073</code></a> v7.22.1</li>
<li><a href="https://github.com/babel/babel/commit/f64974d6ac747154845d1fd123b1abe56b07332e"><code>f64974d</code></a> chore: Improve development experience about global variables (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15646">#15646</a>)</li>
<li><a href="https://github.com/babel/babel/commit/389ecb08ed502cd13671928c1ab9caccb72f0a6f"><code>389ecb0</code></a> v7.22.0</li>
<li><a href="https://github.com/babel/babel/commit/696784a43367857a774eb2764fd5c3efdcf94002"><code>696784a</code></a> Add <code>unicode-sets-regex</code> transform to <code>preset-env</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15636">#15636</a>)</li>
<li><a href="https://github.com/babel/babel/commit/4b5ebdc9b3921b4dab7f0e10a37779788208a96a"><code>4b5ebdc</code></a> Add support for the updated import attributes proposal (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15536">#15536</a>)</li>
<li><a href="https://github.com/babel/babel/commit/920b78c0c22b242a86178dc3556e54e442a05aec"><code>920b78c</code></a> Enable regexp unicode sets parsing by default (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/15638">#15638</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.22.5/packages/babel-core">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 11:15:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.2.2 to 4.2.4 in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.2.2 to 4.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>4.2.4</h2>
<h3>Bug Fixes</h3>
<ul>
<li>ensure reserved events cannot be used as event names (<a href="https://github.com/socketio/socket.io-parser/commit/d9db4737a3c8ce5f1f49ecc8d928a74f3da591f7">d9db473</a>)</li>
<li>properly detect plain objects (<a href="https://github.com/socketio/socket.io-parser/commit/b0e6400c93b5c4aa25e6a629d6448b8627275213">b0e6400</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.2.3...4.2.4">https://github.com/socketio/socket.io-parser/compare/4.2.3...4.2.4</a></li>
</ul>
<h2>4.2.3</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot convert object to primitive value
       at Socket.emit (node:events:507:25)
       at .../node_modules/socket.io/lib/socket.js:531:14
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/main/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.3...4.2.4">4.2.4</a> (2023-05-31)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>ensure reserved events cannot be used as event names (<a href="https://github.com/socketio/socket.io-parser/commit/d9db4737a3c8ce5f1f49ecc8d928a74f3da591f7">d9db473</a>)</li>
<li>properly detect plain objects (<a href="https://github.com/socketio/socket.io-parser/commit/b0e6400c93b5c4aa25e6a629d6448b8627275213">b0e6400</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/3.4.2...3.4.3">3.4.3</a> (2023-05-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/2dc3c92622dad113b8676be06f23b1ed46b02ced">2dc3c92</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">4.2.3</a> (2023-05-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/164ba2a11edc34c2f363401e9768f9a8541a8b89"><code>164ba2a</code></a> chore(release): 4.2.4</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b0e6400c93b5c4aa25e6a629d6448b8627275213"><code>b0e6400</code></a> fix: properly detect plain objects</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/d9db4737a3c8ce5f1f49ecc8d928a74f3da591f7"><code>d9db473</code></a> fix: ensure reserved events cannot be used as event names</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/6a5a004d1e1fd7b7250fdc6fb148e0d9015f8368"><code>6a5a004</code></a> docs(changelog): include changelog for release 3.4.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b6c824f82421aa44dfd5ef395f5132866543de59"><code>b6c824f</code></a> chore(release): 4.2.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/dcc70d9678ac896de08294d6e8d668be6a68680a"><code>dcc70d9</code></a> refactor: export typescript declarations for the commonjs build</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3"><code>3b78117</code></a> fix: check the format of the event name</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/0841bd562351c3d45a5288e2adf9707cc8a3131d"><code>0841bd5</code></a> chore: bump ua-parser-js from 1.0.32 to 1.0.33 (<a href="https://redirect.github.com/socketio/socket.io-parser/issues/121">#121</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.2.2&new-version=4.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 11:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie from 4.0.0 to 4.1.3 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tough-cookie](https://github.com/salesforce/tough-cookie) from 4.0.0 to 4.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/salesforce/tough-cookie/releases">tough-cookie's releases</a>.</em></p>
<blockquote>
<h2>4.1.3</h2>
<p>Security fix for Prototype Pollution discovery in <a href="https://redirect.github.com/salesforce/tough-cookie/issues/282">#282</a>. This is a minor release, although output from the <code>inspect</code> utility is affected by this change, we felt this change was important enough to be pushed into the next patch.</p>
<h2>4.1.2 -- Patch and Bugfix Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow set cookies with localhost by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/253">salesforce/tough-cookie#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2">https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2</a></p>
<h2>4.1.1</h2>
<h2>Patch Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow special use domains by default by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/249">salesforce/tough-cookie#249</a></li>
<li>4.1.1 Patch -- allow special use domains by default by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/250">salesforce/tough-cookie#250</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1">https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1</a></p>
<h2>4.1.0</h2>
<p>v4.1.0</p>
<p>Minor release, focused mainly on resolving reported issues and some minor feature work.</p>
<h2>What's Changed</h2>
<ul>
<li>Create CHANGELOG.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/189">salesforce/tough-cookie#189</a></li>
<li>Missing param validation issue145 by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/193">salesforce/tough-cookie#193</a></li>
<li>Create SECURITY.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/201">salesforce/tough-cookie#201</a></li>
<li>Create CODE_OF_CONDUCT.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/200">salesforce/tough-cookie#200</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/195">#195</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/202">salesforce/tough-cookie#202</a></li>
<li>Add explanation and more special-use domains by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/203">salesforce/tough-cookie#203</a></li>
<li>Sync of constructor options for serialization by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/204">salesforce/tough-cookie#204</a></li>
<li>Returned null in case of empty cookie value by <a href="https://github.com/vsin12"><code>@​vsin12</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/196">salesforce/tough-cookie#196</a></li>
<li>132 str trim not a function by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/209">salesforce/tough-cookie#209</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/153">#153</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/210">salesforce/tough-cookie#210</a></li>
<li>Fix permuteDomain with trailing dot by <a href="https://github.com/ruoho-sfdc"><code>@​ruoho-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/216">salesforce/tough-cookie#216</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/213">#213</a> -- added gh-actions flow for building and testing tough-co… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/218">salesforce/tough-cookie#218</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/210">#210</a> -- Updated workflow to use npm install. by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/220">salesforce/tough-cookie#220</a></li>
<li>@<a href="https://redirect.github.com/salesforce/tough-cookie/issues/215">GH-215</a> -- Tests that document localhost behavior when set as domain. by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/221">salesforce/tough-cookie#221</a></li>
<li>fix: MemoryCookieStore methods should exist on the prototype, not on the class. by <a href="https://github.com/wjhsf"><code>@​wjhsf</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/226">salesforce/tough-cookie#226</a></li>
<li>Unit test cases for <code>allowSpecialUseDomain</code> option by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/225">salesforce/tough-cookie#225</a></li>
<li>[Snyk] Upgrade universalify from 0.1.2 to 0.2.0 by <a href="https://github.com/snyk-bot"><code>@​snyk-bot</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/228">salesforce/tough-cookie#228</a></li>
<li>React Native Support by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/227">salesforce/tough-cookie#227</a></li>
<li>Adding Updating CODEOWNERS with ECCN as per Export Control Compliance by <a href="https://github.com/svc-scm"><code>@​svc-scm</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/223">salesforce/tough-cookie#223</a></li>
<li>fix: domain match routine by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/236">salesforce/tough-cookie#236</a></li>
<li>Stop using the internal NodeJS punycode module by <a href="https://github.com/gboer"><code>@​gboer</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/238">salesforce/tough-cookie#238</a></li>
<li>Initial documentation review by <a href="https://github.com/mcarey86"><code>@​mcarey86</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/234">salesforce/tough-cookie#234</a></li>
<li>fix: distinguish between no samesite and samesite=none by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/240">salesforce/tough-cookie#240</a></li>
<li>Prepare tough-cookie 4.1 for publishing (updated GitHub actions, move… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/242">salesforce/tough-cookie#242</a></li>
<li>4.1.0 release to NPM by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/245">salesforce/tough-cookie#245</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4ff4d29f6cefd279a412b8d62a21142ebd410b36"><code>4ff4d29</code></a> 4.1.3 release preparation, update the package and lib/version to 4.1.3. (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/284">#284</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/12d474791bb856004e858fdb1c47b7608d09cf6e"><code>12d4747</code></a> Prevent prototype pollution in cookie memstore (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/283">#283</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/f06b72d1d447f33dfa6222c0a3c0c5e063558248"><code>f06b72d</code></a> Fix documentation for store.findCookies, missing allowSpecialUseDomain proper...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b1a8898ee3f8af52c6c1c355555d9f50ebe626ce"><code>b1a8898</code></a> fix: allow set cookies with localhost (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/253">#253</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/ec707966e68a48199e646e2fa6b3055df6a280f0"><code>ec70796</code></a> 4.1.1 Patch -- allow special use domains by default (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/250">#250</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/d4ac5801dd2c2d53eec51329e5380bbffb23bfaf"><code>d4ac580</code></a> fix: allow special use domains by default (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/249">#249</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/79c2f7d373e39918605c270ecd965f507701233d"><code>79c2f7d</code></a> 4.1.0 release to NPM (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/245">#245</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4fafc179a798a570e32fc698034f0480c07d9afa"><code>4fafc17</code></a> Prepare tough-cookie 4.1 for publishing (updated GitHub actions, move Dockerf...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/aa4396da7abcb2dbe607db7b31606f7dd0f45709"><code>aa4396d</code></a> fix: distinguish between no samesite and samesite=none (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/240">#240</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b8d751188da697157e5eed81fa1e5f806fdfb541"><code>b8d7511</code></a> Modernize README (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/234">#234</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/salesforce/tough-cookie/compare/v4.0.0...v4.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tough-cookie&package-manager=npm_and_yarn&previous-version=4.0.0&new-version=4.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 17:17:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie from 4.0.0 to 4.1.3 in /platform/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tough-cookie](https://github.com/salesforce/tough-cookie) from 4.0.0 to 4.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/salesforce/tough-cookie/releases">tough-cookie's releases</a>.</em></p>
<blockquote>
<h2>4.1.3</h2>
<p>Security fix for Prototype Pollution discovery in <a href="https://redirect.github.com/salesforce/tough-cookie/issues/282">#282</a>. This is a minor release, although output from the <code>inspect</code> utility is affected by this change, we felt this change was important enough to be pushed into the next patch.</p>
<h2>4.1.2 -- Patch and Bugfix Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow set cookies with localhost by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/253">salesforce/tough-cookie#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2">https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2</a></p>
<h2>4.1.1</h2>
<h2>Patch Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow special use domains by default by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/249">salesforce/tough-cookie#249</a></li>
<li>4.1.1 Patch -- allow special use domains by default by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/250">salesforce/tough-cookie#250</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1">https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1</a></p>
<h2>4.1.0</h2>
<p>v4.1.0</p>
<p>Minor release, focused mainly on resolving reported issues and some minor feature work.</p>
<h2>What's Changed</h2>
<ul>
<li>Create CHANGELOG.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/189">salesforce/tough-cookie#189</a></li>
<li>Missing param validation issue145 by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/193">salesforce/tough-cookie#193</a></li>
<li>Create SECURITY.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/201">salesforce/tough-cookie#201</a></li>
<li>Create CODE_OF_CONDUCT.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/200">salesforce/tough-cookie#200</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/195">#195</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/202">salesforce/tough-cookie#202</a></li>
<li>Add explanation and more special-use domains by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/203">salesforce/tough-cookie#203</a></li>
<li>Sync of constructor options for serialization by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/204">salesforce/tough-cookie#204</a></li>
<li>Returned null in case of empty cookie value by <a href="https://github.com/vsin12"><code>@​vsin12</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/196">salesforce/tough-cookie#196</a></li>
<li>132 str trim not a function by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/209">salesforce/tough-cookie#209</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/153">#153</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/210">salesforce/tough-cookie#210</a></li>
<li>Fix permuteDomain with trailing dot by <a href="https://github.com/ruoho-sfdc"><code>@​ruoho-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/216">salesforce/tough-cookie#216</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/213">#213</a> -- added gh-actions flow for building and testing tough-co… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/218">salesforce/tough-cookie#218</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/210">#210</a> -- Updated workflow to use npm install. by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/220">salesforce/tough-cookie#220</a></li>
<li>@<a href="https://redirect.github.com/salesforce/tough-cookie/issues/215">GH-215</a> -- Tests that document localhost behavior when set as domain. by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/221">salesforce/tough-cookie#221</a></li>
<li>fix: MemoryCookieStore methods should exist on the prototype, not on the class. by <a href="https://github.com/wjhsf"><code>@​wjhsf</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/226">salesforce/tough-cookie#226</a></li>
<li>Unit test cases for <code>allowSpecialUseDomain</code> option by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/225">salesforce/tough-cookie#225</a></li>
<li>[Snyk] Upgrade universalify from 0.1.2 to 0.2.0 by <a href="https://github.com/snyk-bot"><code>@​snyk-bot</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/228">salesforce/tough-cookie#228</a></li>
<li>React Native Support by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/227">salesforce/tough-cookie#227</a></li>
<li>Adding Updating CODEOWNERS with ECCN as per Export Control Compliance by <a href="https://github.com/svc-scm"><code>@​svc-scm</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/223">salesforce/tough-cookie#223</a></li>
<li>fix: domain match routine by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/236">salesforce/tough-cookie#236</a></li>
<li>Stop using the internal NodeJS punycode module by <a href="https://github.com/gboer"><code>@​gboer</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/238">salesforce/tough-cookie#238</a></li>
<li>Initial documentation review by <a href="https://github.com/mcarey86"><code>@​mcarey86</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/234">salesforce/tough-cookie#234</a></li>
<li>fix: distinguish between no samesite and samesite=none by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/240">salesforce/tough-cookie#240</a></li>
<li>Prepare tough-cookie 4.1 for publishing (updated GitHub actions, move… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/242">salesforce/tough-cookie#242</a></li>
<li>4.1.0 release to NPM by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/245">salesforce/tough-cookie#245</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4ff4d29f6cefd279a412b8d62a21142ebd410b36"><code>4ff4d29</code></a> 4.1.3 release preparation, update the package and lib/version to 4.1.3. (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/284">#284</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/12d474791bb856004e858fdb1c47b7608d09cf6e"><code>12d4747</code></a> Prevent prototype pollution in cookie memstore (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/283">#283</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/f06b72d1d447f33dfa6222c0a3c0c5e063558248"><code>f06b72d</code></a> Fix documentation for store.findCookies, missing allowSpecialUseDomain proper...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b1a8898ee3f8af52c6c1c355555d9f50ebe626ce"><code>b1a8898</code></a> fix: allow set cookies with localhost (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/253">#253</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/ec707966e68a48199e646e2fa6b3055df6a280f0"><code>ec70796</code></a> 4.1.1 Patch -- allow special use domains by default (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/250">#250</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/d4ac5801dd2c2d53eec51329e5380bbffb23bfaf"><code>d4ac580</code></a> fix: allow special use domains by default (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/249">#249</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/79c2f7d373e39918605c270ecd965f507701233d"><code>79c2f7d</code></a> 4.1.0 release to NPM (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/245">#245</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4fafc179a798a570e32fc698034f0480c07d9afa"><code>4fafc17</code></a> Prepare tough-cookie 4.1 for publishing (updated GitHub actions, move Dockerf...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/aa4396da7abcb2dbe607db7b31606f7dd0f45709"><code>aa4396d</code></a> fix: distinguish between no samesite and samesite=none (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/240">#240</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b8d751188da697157e5eed81fa1e5f806fdfb541"><code>b8d7511</code></a> Modernize README (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/234">#234</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/salesforce/tough-cookie/compare/v4.0.0...v4.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tough-cookie&package-manager=npm_and_yarn&previous-version=4.0.0&new-version=4.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 17:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Bump protobufjs and fabric-network in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) and [fabric-network](https://github.com/hyperledger/fabric-sdk-node). These dependencies needed to be updated together.
Updates `protobufjs` from 6.11.3 to 7.2.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>protobufjs: v7.2.4</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2>protobufjs: v7.2.3</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
<h2>protobufjs: v7.2.2</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.1...protobufjs-v7.2.2">7.2.2</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab">14f0536</a>)</li>
</ul>
<h2>protobufjs: v7.2.1</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.0...protobufjs-v7.2.1">7.2.1</a> (2023-02-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>cli:</strong> fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2">e42eea4</a>)</li>
<li>Revert &quot;fix: error should be thrown&quot; (<a href="https://github.com/protobufjs/protobuf.js/commit/4489fa771464bcb49b57149760e9cc4131e8077e">4489fa7</a>)</li>
<li>use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83">dce9a2e</a>)</li>
<li>use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745">64e8936</a>)</li>
</ul>
<h2>protobufjs: v7.2.0</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.2...protobufjs-v7.2.0">7.2.0</a> (2023-01-24)</h2>
<h3>Features</h3>
<ul>
<li><strong>cli:</strong> generate static files at the granularity of proto messages (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1840">#1840</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/32f2d6a68b27997bd0f7619998695a9fa7a4fd70">32f2d6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>error should be thrown (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1817">#1817</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e7a34897a122342485468999a507626f1ea91507">e7a3489</a>)</li>
</ul>
<h2>protobufjs: v7.1.2</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.1...protobufjs-v7.1.2">7.1.2</a> (2022-09-22)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/master/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.1...protobufjs-v7.2.2">7.2.2</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab">14f0536</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.0...protobufjs-v7.2.1">7.2.1</a> (2023-02-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>cli:</strong> fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2">e42eea4</a>)</li>
<li>Revert &quot;fix: error should be thrown&quot; (<a href="https://github.com/protobufjs/protobuf.js/commit/4489fa771464bcb49b57149760e9cc4131e8077e">4489fa7</a>)</li>
<li>use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83">dce9a2e</a>)</li>
<li>use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745">64e8936</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.2...protobufjs-v7.2.0">7.2.0</a> (2023-01-24)</h2>
<h3>Features</h3>
<ul>
<li><strong>cli:</strong> generate static files at the granularity of proto messages (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1840">#1840</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/32f2d6a68b27997bd0f7619998695a9fa7a4fd70">32f2d6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>error should be thrown (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1817">#1817</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e7a34897a122342485468999a507626f1ea91507">e7a3489</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.1...protobufjs-v7.1.2">7.1.2</a> (2022-09-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>types:</strong> nested object can be a oneof (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1812">#1812</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/119d90aa1ce14d7bff20bb1dcc1ddc4544a80c23">119d90a</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/42e5a9ca85044800b16e193020e1d4d2e6b4010c"><code>42e5a9c</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1900">#1900</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d"><code>e66379f</code></a> fix: do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/56b1e64979dae757b67a21d326e16acee39f2267"><code>56b1e64</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1879">#1879</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8"><code>8817ee6</code></a> fix: type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e721d04dad42603e2f7f262b03cb9bd01f8adaa1"><code>e721d04</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1867">#1867</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab"><code>14f0536</code></a> fix: do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/644d588c0495da6a570344248e1b5af901bc3b0c"><code>644d588</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1865">#1865</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2"><code>e42eea4</code></a> fix(cli): fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83"><code>dce9a2e</code></a> fix: use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745"><code>64e8936</code></a> fix: use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.3...protobufjs-v7.2.4">compare view</a></li>
</ul>
</details>
<br />

Updates `fabric-network` from 2.2.14 to 2.2.18
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/fabric-sdk-node/releases">fabric-network's releases</a>.</em></p>
<blockquote>
<h2>v2.2.18</h2>
<h2>What's Changed</h2>
<ul>
<li>Correctly clean up network connections after use in CA client by <a href="https://github.com/rajat-dlt"><code>@​rajat-dlt</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/674">hyperledger/fabric-sdk-node#674</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/rajat-dlt"><code>@​rajat-dlt</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/674">hyperledger/fabric-sdk-node#674</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.17...v2.2.18">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.17...v2.2.18</a></p>
<h2>v2.2.17</h2>
<h2>What's Changed</h2>
<ul>
<li>Add support for getting CA server information by <a href="https://github.com/redegade"><code>@​redegade</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/510">hyperledger/fabric-sdk-node#510</a></li>
<li>Close Client in Gateway disconnect by <a href="https://github.com/davidkhala"><code>@​davidkhala</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/287">hyperledger/fabric-sdk-node#287</a></li>
<li>Include timestamp in transaction events by <a href="https://github.com/sapthasurendran"><code>@​sapthasurendran</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/490">hyperledger/fabric-sdk-node#490</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.16...v2.2.17">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.16...v2.2.17</a></p>
<h2>v2.2.16</h2>
<h2>What's Changed</h2>
<ul>
<li>Downgrade nano dependency (used only for CouchDB wallets) to maintain compatibility with Node 10 and 12 by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/624">hyperledger/fabric-sdk-node#624</a></li>
<li>Add support for Node 18 LTS by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/625">hyperledger/fabric-sdk-node#625</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.15...v2.2.16">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.15...v2.2.16</a></p>
<h2>v2.2.15</h2>
<p>This is a maintenance release containing the following changes:</p>
<ul>
<li>Update dependencies to address a gRPC bug that could cause pings to be sent on destroyed HTTP sessions, resulting in an ERR_HTTP2_INVALID_SESSION error.</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.14...v2.2.15">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.14...v2.2.15</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/48c5b2d149a3619588ffca01f466717cbf097f1b"><code>48c5b2d</code></a> Release v2.2.18 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/676">#676</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/c91d5731d008489683febf6aab2b98d582f8c825"><code>c91d573</code></a> Fix ts-scenario TypeScript transpile failure (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/675">#675</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/ecbe99ca2619636aa2701816c9a8bd68589bdf27"><code>ecbe99c</code></a> Socket connection fix: destroy() used instead of abort() (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/674">#674</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/1ff998a72a74918bd799ee1e9bba005d1841b731"><code>1ff998a</code></a> Reduce scheduled build frequency to weekly (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/671">#671</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/1cd870daf103084a00c15a6c93e3d8ba029bacf9"><code>1cd870d</code></a> Document deprecation as of Fabric v2.5 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/668">#668</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/6565522a7638f1c15ca64b4187f07e6ac959667e"><code>6565522</code></a> Pull Fabric release images from DockerHub (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/666">#666</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/aaf1f354c31214aa8937b642a9000f289a506fd4"><code>aaf1f35</code></a> Update version and tag following release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/665">#665</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/933c10f9dee3691e92785373f59511037f0ab500"><code>933c10f</code></a> Release v2.2.17 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/664">#664</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/1f8d86c352b3f4e018663ba7a831f942dea2c763"><code>1f8d86c</code></a> Apply main branch changes following branch rename</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/dd6fff25695a0f4fc049519eec836dae4ae3d3a2"><code>dd6fff2</code></a> Update npm version used by Node</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.14...v2.2.18">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 22:33:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.10 to 1.8.17 in /chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.6.10 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/409418b103f35c6b89371731e2b1d5084b442318"><code>409418b</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a> from murgatroid99/grpc-js_prohibit_od_pick_first</li>
<li><a href="https://github.com/grpc/grpc-node/commit/ed70a0b381144b387698f2d57001f5a7bc82cbe9"><code>ed70a0b</code></a> Fix handling of OD policy with no child</li>
<li><a href="https://github.com/grpc/grpc-node/commit/073caf5b83387be8c1c7416477489646060e4942"><code>073caf5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2478">#2478</a> from murgatroid99/grpc-js-xds_docker_distroless_1.8.x</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d2d17b0b694d7c23e2448d9cde224b9427102fb4"><code>d2d17b0</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2482">#2482</a> from XuanWang-Amos/backport-1.8-file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a6aa7ea43e1458a578cf9ab81ed492a760c43a78"><code>a6aa7ea</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2475">#2475</a> from XuanWang-Amos/file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a62d2b027bf91e5084c9134305e88a645dc5f1c1"><code>a62d2b0</code></a> Use entrypoint /nodejs/bin/node</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9441de78f655ada34ada0dc1a8057122eb21f229"><code>9441de7</code></a> grpc-js-xds: Use distroless Node image for interop Dockerfile</li>
<li><a href="https://github.com/grpc/grpc-node/commit/b53f5882f13a5cb3c599804e96304bf5b8407ea6"><code>b53f588</code></a> grpc-js: Disallow pick_first as child of outlier_detection</li>
<li><a href="https://github.com/grpc/grpc-node/commit/09d74ca43d2fcb63c97405315bd01633322d9b34"><code>09d74ca</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a> from murgatroid99/grpc-js_transport_trace_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87b5466b1b5e6d269a9750305c5842c9e30e56e8"><code>87b5466</code></a> grpc-js: Implement trace function in Http2SubchannelConnector</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.6.10...@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.6.10&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 22:36:16 +0000 UTC
    </div>
</div>

