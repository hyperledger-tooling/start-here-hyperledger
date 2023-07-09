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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie and jest in /samples/chaincodes/chaincode-kv-node-1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [tough-cookie](https://github.com/salesforce/tough-cookie). It's no longer used after updating ancestor dependency [jest](https://github.com/facebook/jest/tree/HEAD/packages/jest). These dependencies need to be updated together.

Removes `tough-cookie`

Updates `jest` from 25.5.4 to 29.6.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/jest/releases">jest's releases</a>.</em></p>
<blockquote>
<h2>v29.6.1</h2>
<h2>Fixes</h2>
<ul>
<li><code>[jest-circus]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/14110">#14110</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14304">#14304</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jestjs/jest/compare/v29.6.0...v29.6.1">https://github.com/jestjs/jest/compare/v29.6.0...v29.6.1</a></p>
<h2>v29.6.0</h2>
<h2>Features</h2>
<ul>
<li><code>[jest-circus, jest-snapshot]</code> Add support for snapshot matchers in concurrent tests (<a href="https://redirect.github.com/jestjs/jest/pull/14139">#14139</a>)</li>
<li><code>[jest-cli]</code> Include type definitions to generated config files (<a href="https://redirect.github.com/facebook/jest/pull/14078">#14078</a>)</li>
<li><code>[jest-snapshot]</code> Support arrays as property matchers (<a href="https://redirect.github.com/facebook/jest/pull/14025">#14025</a>)</li>
<li><code>[jest-core, jest-circus, jest-reporter, jest-runner]</code> Added support for reporting about start individual test cases using jest-circus (<a href="https://redirect.github.com/jestjs/jest/pull/14174">#14174</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li><code>[jest-circus]</code> Prevent false test failures caused by promise rejections handled asynchronously (<a href="https://redirect.github.com/jestjs/jest/pull/14110">#14110</a>)</li>
<li><code>[jest-config]</code> Handle frozen config object (<a href="https://redirect.github.com/facebook/jest/pull/14054">#14054</a>)</li>
<li><code>[jest-config]</code> Allow <code>coverageDirectory</code> and <code>collectCoverageFrom</code> in project config (<a href="https://redirect.github.com/jestjs/jest/pull/14180">#14180</a>)</li>
<li><code>[jest-core]</code> Always use workers in watch mode to avoid crashes (<a href="https://redirect.github.com/facebook/jest/pull/14059">#14059</a>).</li>
<li><code>[jest-environment-jsdom, jest-environment-node]</code> Fix assignment of <code>customExportConditions</code> via <code>testEnvironmentOptions</code> when custom env subclass defines a default value (<a href="https://redirect.github.com/facebook/jest/pull/13989">#13989</a>)</li>
<li><code>[jest-matcher-utils]</code> Fix copying value of inherited getters (<a href="https://redirect.github.com/facebook/jest/pull/14007">#14007</a>)</li>
<li><code>[jest-mock]</code> Tweak typings to allow <code>jest.replaceProperty()</code> replace methods (<a href="https://redirect.github.com/facebook/jest/pull/14008">#14008</a>)</li>
<li><code>[jest-mock]</code> Improve user input validation and error messages of <code>spyOn</code> and <code>replaceProperty</code> methods (<a href="https://redirect.github.com/facebook/jest/pull/14087">#14087</a>)</li>
<li><code>[jest-runtime]</code> Bind <code>jest.isolateModulesAsync</code> to <code>this</code> (<a href="https://redirect.github.com/facebook/jest/pull/14083">#14083</a>)</li>
<li><code>[jest-runtime]</code> Forward <code>wrapperLength</code> to the <code>Script</code> constructor as <code>columnOffset</code> for accurate debugging (<a href="https://redirect.github.com/facebook/jest/pull/14148">#14148</a>)</li>
<li><code>[jest-runtime]</code> Guard <code>_isMockFunction</code> access with <code>in</code> (<a href="https://redirect.github.com/facebook/jest/pull/14188">#14188</a>)</li>
<li><code>[jest-snapshot]</code> Fix a potential bug when not using prettier and improve performance (<a href="https://redirect.github.com/facebook/jest/pull/14036">#14036</a>)</li>
<li><code>[@jest/transform]</code> Do not instrument <code>.json</code> modules (<a href="https://redirect.github.com/facebook/jest/pull/14048">#14048</a>)</li>
<li><code>[jest-worker]</code> Restart a shut down worker before sending it a task (<a href="https://redirect.github.com/facebook/jest/pull/14015">#14015</a>)</li>
</ul>
<h2>Chore &amp; Maintenance</h2>
<ul>
<li><code>[*]</code> Update <code>semver</code> dependency to get vulnerability fix (<a href="https://redirect.github.com/jestjs/jest/pull/14262">#14262</a>)</li>
<li><code>[docs]</code> Updated documentation for the <code>--runTestsByPath</code> CLI command (<a href="https://redirect.github.com/facebook/jest/pull/14004">#14004</a>)</li>
<li><code>[docs]</code> Updated documentation regarding the synchronous fallback when asynchronous code transforms are unavailable (<a href="https://redirect.github.com/facebook/jest/pull/14056">#14056</a>)</li>
<li><code>[docs]</code> Update jest statistics of use and downloads in website Index.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/huntie"><code>@​huntie</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/13989">jestjs/jest#13989</a></li>
<li><a href="https://github.com/liammulh"><code>@​liammulh</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14001">jestjs/jest#14001</a></li>
<li><a href="https://github.com/BenceSzalai"><code>@​BenceSzalai</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14007">jestjs/jest#14007</a></li>
<li><a href="https://github.com/Mike-Dax"><code>@​Mike-Dax</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14056">jestjs/jest#14056</a></li>
<li><a href="https://github.com/bakasmarius"><code>@​bakasmarius</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14025">jestjs/jest#14025</a></li>
<li><a href="https://github.com/PeteTheHeat"><code>@​PeteTheHeat</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14015">jestjs/jest#14015</a></li>
<li><a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14083">jestjs/jest#14083</a></li>
<li><a href="https://github.com/soyjuanmacias"><code>@​soyjuanmacias</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14101">jestjs/jest#14101</a></li>
<li><a href="https://github.com/bharathkalyans"><code>@​bharathkalyans</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14154">jestjs/jest#14154</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jestjs/jest/blob/main/CHANGELOG.md">jest's changelog</a>.</em></p>
<blockquote>
<h2>29.6.1</h2>
<h3>Fixes</h3>
<ul>
<li><code>[jest-circus]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/14110">#14110</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14304">#14304</a>)</li>
</ul>
<h2>29.6.0</h2>
<h3>Features</h3>
<ul>
<li><code>[jest-circus, jest-snapshot]</code> Add support for snapshot matchers in concurrent tests (<a href="https://redirect.github.com/jestjs/jest/pull/14139">#14139</a>)</li>
<li><code>[jest-cli]</code> Include type definitions to generated config files (<a href="https://redirect.github.com/facebook/jest/pull/14078">#14078</a>)</li>
<li><code>[jest-snapshot]</code> Support arrays as property matchers (<a href="https://redirect.github.com/facebook/jest/pull/14025">#14025</a>)</li>
<li><code>[jest-core, jest-circus, jest-reporter, jest-runner]</code> Added support for reporting about start individual test cases using jest-circus (<a href="https://redirect.github.com/jestjs/jest/pull/14174">#14174</a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li><code>[jest-circus]</code> Prevent false test failures caused by promise rejections handled asynchronously (<a href="https://redirect.github.com/jestjs/jest/pull/14110">#14110</a>)</li>
<li><code>[jest-config]</code> Handle frozen config object (<a href="https://redirect.github.com/facebook/jest/pull/14054">#14054</a>)</li>
<li><code>[jest-config]</code> Allow <code>coverageDirectory</code> and <code>collectCoverageFrom</code> in project config (<a href="https://redirect.github.com/jestjs/jest/pull/14180">#14180</a>)</li>
<li><code>[jest-core]</code> Always use workers in watch mode to avoid crashes (<a href="https://redirect.github.com/facebook/jest/pull/14059">#14059</a>).</li>
<li><code>[jest-environment-jsdom, jest-environment-node]</code> Fix assignment of <code>customExportConditions</code> via <code>testEnvironmentOptions</code> when custom env subclass defines a default value (<a href="https://redirect.github.com/facebook/jest/pull/13989">#13989</a>)</li>
<li><code>[jest-matcher-utils]</code> Fix copying value of inherited getters (<a href="https://redirect.github.com/facebook/jest/pull/14007">#14007</a>)</li>
<li><code>[jest-mock]</code> Tweak typings to allow <code>jest.replaceProperty()</code> replace methods (<a href="https://redirect.github.com/facebook/jest/pull/14008">#14008</a>)</li>
<li><code>[jest-mock]</code> Improve user input validation and error messages of <code>spyOn</code> and <code>replaceProperty</code> methods (<a href="https://redirect.github.com/facebook/jest/pull/14087">#14087</a>)</li>
<li><code>[jest-runtime]</code> Bind <code>jest.isolateModulesAsync</code> to <code>this</code> (<a href="https://redirect.github.com/facebook/jest/pull/14083">#14083</a>)</li>
<li><code>[jest-runtime]</code> Forward <code>wrapperLength</code> to the <code>Script</code> constructor as <code>columnOffset</code> for accurate debugging (<a href="https://redirect.github.com/facebook/jest/pull/14148">#14148</a>)</li>
<li><code>[jest-runtime]</code> Guard <code>_isMockFunction</code> access with <code>in</code> (<a href="https://redirect.github.com/facebook/jest/pull/14188">#14188</a>)</li>
<li><code>[jest-snapshot]</code> Fix a potential bug when not using prettier and improve performance (<a href="https://redirect.github.com/facebook/jest/pull/14036">#14036</a>)</li>
<li><code>[@jest/transform]</code> Do not instrument <code>.json</code> modules (<a href="https://redirect.github.com/facebook/jest/pull/14048">#14048</a>)</li>
<li><code>[jest-worker]</code> Restart a shut down worker before sending it a task (<a href="https://redirect.github.com/facebook/jest/pull/14015">#14015</a>)</li>
</ul>
<h3>Chore &amp; Maintenance</h3>
<ul>
<li><code>[*]</code> Update <code>semver</code> dependency to get vulnerability fix (<a href="https://redirect.github.com/jestjs/jest/pull/14262">#14262</a>)</li>
<li><code>[docs]</code> Updated documentation for the <code>--runTestsByPath</code> CLI command (<a href="https://redirect.github.com/facebook/jest/pull/14004">#14004</a>)</li>
<li><code>[docs]</code> Updated documentation regarding the synchronous fallback when asynchronous code transforms are unavailable (<a href="https://redirect.github.com/facebook/jest/pull/14056">#14056</a>)</li>
<li><code>[docs]</code> Update jest statistics of use and downloads in website Index.</li>
</ul>
<h2>29.5.0</h2>
<h3>Features</h3>
<ul>
<li><code>[jest-changed-files]</code> Support Sapling (<a href="https://redirect.github.com/facebook/jest/pull/13941">#13941</a>)</li>
<li><code>[jest-circus, @jest/cli, jest-config]</code> Add feature to randomize order of tests via CLI flag or through the config file(<a href="https://redirect.github.com/facebook/jest/pull/12922">#12922</a>)</li>
<li><code>[jest-cli, jest-config, @jest/core, jest-haste-map, @jest/reporters, jest-runner, jest-runtime, @jest/types]</code> Add <code>workerThreads</code> configuration option to allow using <a href="https://nodejs.org/dist/latest/docs/api/worker_threads.html">worker threads</a> for parallelization (<a href="https://redirect.github.com/facebook/jest/pull/13939">#13939</a>)</li>
<li><code>[jest-cli]</code> Export <code>yargsOptions</code> (<a href="https://redirect.github.com/facebook/jest/pull/13970">#13970</a>)</li>
<li><code>[jest-config]</code> Add <code>openHandlesTimeout</code> option to configure possible open handles warning. (<a href="https://redirect.github.com/facebook/jest/pull/13875">#13875</a>)</li>
<li><code>[@jest/create-cache-key-function]</code> Allow passing <code>length</code> argument to <code>createCacheKey()</code> function and set its default value to <code>16</code> on Windows (<a href="https://redirect.github.com/facebook/jest/pull/13827">#13827</a>)</li>
<li><code>[jest-message-util]</code> Add support for <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/AggregateError">AggregateError</a> (<a href="https://redirect.github.com/facebook/jest/pull/13946">#13946</a> &amp; <a href="https://redirect.github.com/facebook/jest/pull/13947">#13947</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jestjs/jest/commit/1f019afdcdfc54a6664908bb45f343db4e3d0848"><code>1f019af</code></a> v29.6.1</li>
<li><a href="https://github.com/jestjs/jest/commit/c1e5b8a38ef54bb138409f89831942ebf6a7a67e"><code>c1e5b8a</code></a> v29.6.0</li>
<li><a href="https://github.com/jestjs/jest/commit/6ffa48d1cd7d85189f0dbc1e37fd0efafa5c221c"><code>6ffa48d</code></a> chore: upgrade TypeScript to v5 (<a href="https://github.com/facebook/jest/tree/HEAD/packages/jest/issues/14155">#14155</a>)</li>
<li><a href="https://github.com/jestjs/jest/commit/a95eeb6c2c8145a81190149a52a30fc177417ecc"><code>a95eeb6</code></a> chore: update tsd runner (<a href="https://github.com/facebook/jest/tree/HEAD/packages/jest/issues/14020">#14020</a>)</li>
<li><a href="https://github.com/jestjs/jest/commit/39f3beda6b396665bebffab94e8d7c45be30454c"><code>39f3bed</code></a> v29.5.0</li>
<li><a href="https://github.com/jestjs/jest/commit/a49c88610e49a3242576160740a32a2fe11161e1"><code>a49c886</code></a> v29.4.3</li>
<li><a href="https://github.com/jestjs/jest/commit/6d2632adae0f0fa1fe116d3b475fd9783d0de1b5"><code>6d2632a</code></a> Update copyrights with Meta Platforms, restore original license in Jasmine fo...</li>
<li><a href="https://github.com/jestjs/jest/commit/f0fc92e8443f09546c7ec0472bf9bce44fe5898f"><code>f0fc92e</code></a> v29.4.2</li>
<li><a href="https://github.com/jestjs/jest/commit/bc7b20c9d4f6c399477b5a2b955dc0e1b736cd9b"><code>bc7b20c</code></a> chore: make sure to exclude .eslintcache from published module (<a href="https://github.com/facebook/jest/tree/HEAD/packages/jest/issues/13832">#13832</a>)</li>
<li><a href="https://github.com/jestjs/jest/commit/bc84c8a15649aaaefdd624dc83824518c17467ed"><code>bc84c8a</code></a> v29.4.1</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/jest/commits/v29.6.1/packages/jest">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 23:40:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.7 to 1.8.17 in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.6.7 to 1.8.17.
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
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.6.7...@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.6.7&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-07-05 23:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                     Fix NPM issues causing errors 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes some issues caused by npm by:

- Removing unsupported test library for fabric that depends on packages that fail to compile 
- Bumps nodejs version from 12 to 16 at `samples/chaincodes/chaincode-kv-node/.nvmrc`
- Removing non-crucial tests from the sample chaincode 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 22:16:38 +0000 UTC
    </div>
</div>

