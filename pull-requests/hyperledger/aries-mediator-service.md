---
layout: default
title: aries-mediator-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mediator-service
---

# aries-mediator-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mediator-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    build(deps): bump tough-cookie from 4.0.0 to 4.1.3 in /acapy/controller
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 20:35:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    build(deps): bump semver from 7.3.8 to 7.5.4 in /load-testing/load-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 20:35:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    build(deps): bump semver from 5.7.1 to 5.7.2 in /afj
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 20:35:17 +0000 UTC
    </div>
</div>

