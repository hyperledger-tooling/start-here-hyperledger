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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie from 4.0.0 to 4.1.3 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 01:50:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1069" class=".btn">#1069</a>
            </td>
            <td>
                <b>
                    Bump protobufjs and fabric-network in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) to 7.2.4 and updates ancestor dependency [fabric-network](https://github.com/hyperledger/fabric-sdk-node). These dependencies need to be updated together.

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

Updates `fabric-network` from 2.2.10 to 2.2.18
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
<h2>v2.2.14</h2>
<p>This is a maintenance release containing the following changes:</p>
<ul>
<li>Dependency updates to address security vulnerability CVE-2022-25898.</li>
<li>Resolve an issue that could cause partial discovery results to be obtained under high load, and subsequent transaction failures.</li>
<li>Resolve an issue that could cause an unhandled promise rejection with exceptionally short commit timeouts.</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.13...v2.2.14">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.13...v2.2.14</a></p>
<h2>v2.2.13</h2>
<p>This is a maintenance release containing dependency updates to address security vulnerability CVE-2021-43138.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.12...v2.2.13">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.12...v2.2.13</a></p>
<h2>v2.2.12</h2>
<p>This is a maintenance release containing big fixes and the following enhancements:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.10...v2.2.18">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hyperledger-ghci">hyperledger-ghci</a>, a new releaser for fabric-network since your current version.</p>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 22:32:55 +0000 UTC
    </div>
</div>

