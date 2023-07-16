---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    Bump semver from 5.7.1 to 5.7.2 in /samples/chaincodes/chaincode-kv-node-1.4
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 23:18:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    Bump semver from 5.7.1 to 5.7.2
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 15:36:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/395" class=".btn">#395</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie from 4.0.0 to 4.1.3 in /samples/chaincodes/chaincode-kv-node
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 10:26:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie from 4.0.0 to 4.1.3
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 10:24:16 +0000 UTC
    </div>
</div>

