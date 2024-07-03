---
layout: default
title: indy-besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-besu
---

# indy-besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    Bump chai and @types/chai in /smart_contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [chai](https://github.com/chaijs/chai) and [@types/chai](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/HEAD/types/chai). These dependencies needed to be updated together.
Updates `chai` from 4.3.8 to 4.3.10
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/chaijs/chai/releases">chai's releases</a>.</em></p>
<blockquote>
<h2>v4.3.10</h2>
<p>This release simply bumps all dependencies to their latest non-breaking versions.</p>
<h2>What's Changed</h2>
<ul>
<li>upgrade all dependencies by <a href="https://github.com/keithamus"><code>@​keithamus</code></a> in <a href="https://redirect.github.com/chaijs/chai/pull/1540">chaijs/chai#1540</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/chaijs/chai/compare/v4.3.9...v4.3.10">https://github.com/chaijs/chai/compare/v4.3.9...v4.3.10</a></p>
<h2>v4.3.9</h2>
<p>Upgrade dependencies.</p>
<p>This release upgrades dependencies to address <strong><a href="https://www.cve.org/CVERecord?id=CVE-2023-43646">CVE-2023-43646</a></strong> where a large function name can cause &quot;catastrophic backtracking&quot; (aka ReDOS attack) which can cause the test suite to hang.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/chaijs/chai/compare/v4.3.8...v4.3.9">https://github.com/chaijs/chai/compare/v4.3.8...v4.3.9</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/chaijs/chai/commit/744a16e1cc4e8a9c6d4499e1e520a0bc4c80ec18"><code>744a16e</code></a> 4.3.10</li>
<li><a href="https://github.com/chaijs/chai/commit/0ccd823cb3ee6a433156c4e23cc67de79d4f368d"><code>0ccd823</code></a> upgrade all dependencies (<a href="https://redirect.github.com/chaijs/chai/issues/1540">#1540</a>)</li>
<li><a href="https://github.com/chaijs/chai/commit/923d0a48fc59a910ecee37c85535379520a3e1b6"><code>923d0a4</code></a> 4.3.9</li>
<li><a href="https://github.com/chaijs/chai/commit/1a0f8872711f64b8353c30ebcfdf0ceeab404bab"><code>1a0f887</code></a> make</li>
<li><a href="https://github.com/chaijs/chai/commit/a141e5739ab32ae579cd2df2eb745dbf1375ac27"><code>a141e57</code></a> upgrade deps</li>
<li>See full diff in <a href="https://github.com/chaijs/chai/compare/v4.3.8...v4.3.10">compare view</a></li>
</ul>
</details>
<br />

Updates `@types/chai` from 4.3.6 to 4.3.16
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/DefinitelyTyped/DefinitelyTyped/commits/HEAD/types/chai">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:42:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Bump @nomicfoundation/hardhat-network-helpers from 1.0.9 to 1.0.11 in /smart_contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@nomicfoundation/hardhat-network-helpers](https://github.com/nomicfoundation/hardhat) from 1.0.9 to 1.0.11.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nomicfoundation/hardhat/releases"><code>@​nomicfoundation/hardhat-network-helpers</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​nomicfoundation/hardhat-network-helpers</code><a href="https://github.com/1"><code>@​1</code></a>.0.11</h2>
<p>This release adds support for using network helpers on anvil network (thanks <a href="https://github.com/tmigone"><code>@​tmigone</code></a>!)</p>
<hr />
<blockquote>
<p>💡 <strong>The Nomic Foundation is hiring! Check <a href="https://www.nomic.foundation/jobs">our open positions</a>.</strong></p>
</blockquote>
<hr />
<h2><code>@​nomicfoundation/hardhat-network-helpers</code><a href="https://github.com/1"><code>@​1</code></a>.0.10</h2>
<p>This version adds support for using the Hardhat network helpers on the Anvil network (thanks <a href="https://github.com/tmigone"><code>@​tmigone</code></a>!)</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/f579adca83f0a4c47bf29cd5df9ebc9347443039"><code>f579adc</code></a> Version Packages</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/0c7b68ee4136f5df99ce391a28714e7550eefee1"><code>0c7b68e</code></a> Merge pull request <a href="https://redirect.github.com/nomicfoundation/hardhat/issues/5195">#5195</a> from NomicFoundation/hardhat-tracer-support</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/b45eb94db46380409ed46f8f93e20e1b53bae1ba"><code>b45eb94</code></a> Fix pnpm wrongly handling deep peer deps</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/3c27724779a7ab20f8962b10bb75ed95ff6a35e5"><code>3c27724</code></a> Update pnpm-lock.yaml</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/0b8e781efaac4e956226a3148830ff436a7054fc"><code>0b8e781</code></a> Merge branch 'main' into hardhat-tracer-support</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/001b948f161f7d32307b60b8b934a135df4bd4ce"><code>001b948</code></a> Bump EDR dependency to ^0.4.0</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/d2ce0243d1da6c54ac2bc1d07cf4157f18c2c62d"><code>d2ce024</code></a> Merge pull request <a href="https://redirect.github.com/nomicfoundation/hardhat/issues/5290">#5290</a> from NomicFoundation/main-pnpm-9</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/5fcf38eb11f96616a3a2797f943d144c041b7758"><code>5fcf38e</code></a> Migrate to pnpm 9</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/389f9fe225d0516dd76d3b4e91ce37d8b887568d"><code>389f9fe</code></a> Merge remote-tracking branch 'refs/remotes/origin/hardhat-tracer-support' int...</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/06171bdfb67a6d7bc5fc289a22a3c0328414f5a2"><code>06171bd</code></a> Merge branch 'main' into hardhat-tracer-support</li>
<li>Additional commits viewable in <a href="https://github.com/nomicfoundation/hardhat/compare/@nomicfoundation/hardhat-network-helpers@1.0.9...@nomicfoundation/hardhat-network-helpers@1.0.11">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~kanej">kanej</a>, a new releaser for <code>@​nomicfoundation/hardhat-network-helpers</code> since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@nomicfoundation/hardhat-network-helpers&package-manager=npm_and_yarn&previous-version=1.0.9&new-version=1.0.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:42:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Bump ethers from 6.8.0 to 6.8.1 in /smart_contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ethers](https://github.com/ethers-io/ethers.js) from 6.8.0 to 6.8.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethers-io/ethers.js/releases">ethers's releases</a>.</em></p>
<blockquote>
<h2>ethers/v6.8.1 (2023-11-01 16:08)</h2>
<ul>
<li>Fixed typo in error description when converting values to arrays (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4427">#4427</a>, <a href="https://redirect.github.com/ethers-io/ethers.js/issues/4446">#4446</a>; <a href="https://github.com/ethers-io/ethers.js/commit/8fed2f84768ace4bf3e5742c931a74841da7c637">8fed2f8</a>).</li>
<li>Fix invalid token nonpayable being included in formatted constructor (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4412">#4412</a>; <a href="https://github.com/ethers-io/ethers.js/commit/2e0bd90744b8e76fcf03f75a66cb0061d50f7bd9">2e0bd90</a>).</li>
<li>Add ENS support for Sepolia (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4422">#4422</a>; <a href="https://github.com/ethers-io/ethers.js/commit/1da50ae286da01e58a70bb8df8aa5cc5d260e33e">1da50ae</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ethers-io/ethers.js/blob/main/CHANGELOG.md">ethers's changelog</a>.</em></p>
<blockquote>
<h2>ethers/v6.8.1 (2023-11-01 16:08)</h2>
<ul>
<li>Fixed typo in error description when converting values to arrays (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4427">#4427</a>, <a href="https://redirect.github.com/ethers-io/ethers.js/issues/4446">#4446</a>; <a href="https://github.com/ethers-io/ethers.js/commit/8fed2f84768ace4bf3e5742c931a74841da7c637">8fed2f8</a>).</li>
<li>Fix invalid token nonpayable being included in formatted constructor (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4412">#4412</a>; <a href="https://github.com/ethers-io/ethers.js/commit/2e0bd90744b8e76fcf03f75a66cb0061d50f7bd9">2e0bd90</a>).</li>
<li>Add ENS support for Sepolia (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4422">#4422</a>; <a href="https://github.com/ethers-io/ethers.js/commit/1da50ae286da01e58a70bb8df8aa5cc5d260e33e">1da50ae</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethers-io/ethers.js/commit/5431723ec38bff131feb15322598f4e4f049825c"><code>5431723</code></a> admin: updated dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/8fed2f84768ace4bf3e5742c931a74841da7c637"><code>8fed2f8</code></a> Fixed typo in error description when converting values to arrays (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4427">#4427</a>, <a href="https://redirect.github.com/ethers-io/ethers.js/issues/4446">#4446</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/73adb393e838fdeee3f97285d8fbd30b41198c78"><code>73adb39</code></a> docs: fixed typo in jsdocs (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4391">#4391</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/2e0bd90744b8e76fcf03f75a66cb0061d50f7bd9"><code>2e0bd90</code></a> Fix invalid token nonpayable being included in formatted constructor (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4412">#4412</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/1da50ae286da01e58a70bb8df8aa5cc5d260e33e"><code>1da50ae</code></a> Add ENS support for Sepolia (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4422">#4422</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/e0c1d976b28820be5182cc5c793f361869cdb31a"><code>e0c1d97</code></a> tests: only trigger browser testing when relevant code changed</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/e454afb2fa3612c273a09b154c36b35fafab17b1"><code>e454afb</code></a> tests: fix typo in env prepare scripts</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/4772915f0cd915585b83cc3c796d6d9fda196325"><code>4772915</code></a> tests: updated env tests for TypeScript 5.2</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/3a73c56ee36cc5039637883a7cb3e52483bc75ec"><code>3a73c56</code></a> admin: updated dist files</li>
<li>See full diff in <a href="https://github.com/ethers-io/ethers.js/compare/v6.8.0...v6.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ethers&package-manager=npm_and_yarn&previous-version=6.8.0&new-version=6.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Bump chrono from 0.4.33 to 0.4.38 in /vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [chrono](https://github.com/chronotope/chrono) from 0.4.33 to 0.4.38.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/chronotope/chrono/releases">chrono's releases</a>.</em></p>
<blockquote>
<h2>v0.4.38</h2>
<p>This release bring a ca. 20% improvement to the performance of the formatting code, and a convenient <code>days_since</code> method for the <code>Weekday</code> type.</p>
<p>Chrono 0.4.38 also removes the long deprecated <code>rustc-serialize</code> feature. Support for <code>rustc-serialize</code> will be <a href="https://redirect.github.com/rust-lang/rust/pull/116016">soft-destabilized in the next Rust edition</a>. Removing the feature will not break existing users of the feature; Cargo will just not update dependents that rely on it to newer versions of chrono.</p>
<p>In chrono 0.4.36 we made an accidental breaking change by switching to <code>derive(Copy)</code> for <code>DateTime</code> instead of a manual implementation. It is reverted in this release.</p>
<h1>Removals</h1>
<ul>
<li>Remove <code>rustc-serialize</code> feature (<a href="https://redirect.github.com/chronotope/chrono/issues/1548">#1548</a>, thanks <a href="https://github.com/workingjubilee"><code>@​workingjubilee</code></a>)</li>
</ul>
<h1>Additions</h1>
<ul>
<li>Add <code>Weekday::days_since</code> (<a href="https://redirect.github.com/chronotope/chrono/issues/1249">#1249</a>, based on <a href="https://redirect.github.com/chronotope/chrono/issues/216">#216</a> by <a href="https://github.com/clarfonthey"><code>@​clarfonthey</code></a>)</li>
<li>Add <code>TimeDelta::checked_mul</code> and <code>TimeDelta::checked_div</code> (<a href="https://redirect.github.com/chronotope/chrono/issues/1565">#1565</a>, thanks <a href="https://github.com/Zomtir"><code>@​Zomtir</code></a>)</li>
</ul>
<h1>Fixes</h1>
<ul>
<li>Return error when rounding with a zero duration (<a href="https://redirect.github.com/chronotope/chrono/issues/1474">#1474</a>, thanks <a href="https://github.com/Dav1dde"><code>@​Dav1dde</code></a>)</li>
<li>Manually implement <code>Copy</code> for <code>DateTime</code> if offset is <code>Copy</code> (<a href="https://redirect.github.com/chronotope/chrono/issues/1573">#1573</a>)</li>
</ul>
<h1>Internal</h1>
<ul>
<li>Inline <code>test_encodable_json</code> and <code>test_decodable_json</code> functions (<a href="https://redirect.github.com/chronotope/chrono/issues/1550">#1550</a>)</li>
<li>CI: Reduce combinations in <code>cargo hack check</code> (<a href="https://redirect.github.com/chronotope/chrono/issues/1553">#1553</a>)</li>
<li>Refactor formatting code (<a href="https://redirect.github.com/chronotope/chrono/issues/1335">#1335</a>)</li>
<li>Optimize number formatting (<a href="https://redirect.github.com/chronotope/chrono/issues/1558">#1558</a>)</li>
<li>Only package files needed for building and testing (<a href="https://redirect.github.com/chronotope/chrono/issues/1554">#1554</a>)</li>
</ul>
<p>Thanks to all contributors on behalf of the chrono team, <a href="https://github.com/djc"><code>@​djc</code></a> and <a href="https://github.com/pitdicker"><code>@​pitdicker</code></a>!</p>
<h2>v0.4.37</h2>
<p>Version 0.4.36 introduced an unexpected breaking change and was yanked. In it <code>LocalResult</code> was renamed to <code>MappedLocalTime</code> to avoid the impression that it is a <code>Result</code> type were some of the results are errors. For backwards compatibility a type alias with the old name was added.</p>
<p>As it turns out there is one case where a type alias behaves differently from the regular enum: you can't import enum variants from a type alias with <code>use chrono::LocalResult::*</code>. With 0.4.37 we make the new name <code>MappedLocalTime</code> the alias, but keep using it in function signatures and the documentation as much as possible.</p>
<p>See also the release notes of <a href="https://github.com/chronotope/chrono/releases/tag/v0.4.36">chrono 0.4.36</a> from yesterday for the yanked release.</p>
<h2>v0.4.36</h2>
<p>This release un-deprecates the methods on <code>TimeDelta</code> that were deprecated with the 0.4.35 release because of the churn they are causing for the ecosystem.</p>
<p>New is the <code>DateTime::with_time()</code> method. As an example of when it is useful:</p>
<pre lang="rust"><code>use chrono::{Local, NaiveTime};
// Today at 12:00:00
let today_noon = Local::now().with_time(NaiveTime::from_hms_opt(12, 0, 0).unwrap());
</code></pre>
<h1>Additions</h1>
<ul>
<li>Add <code>DateTime::with_time()</code> (<a href="https://redirect.github.com/chronotope/chrono/issues/1510">#1510</a>)</li>
</ul>
<h1>Deprecations</h1>
<ul>
<li>Revert <code>TimeDelta</code> deprecations (<a href="https://redirect.github.com/chronotope/chrono/issues/1543">#1543</a>)</li>
<li>Deprecate <code>TimeStamp::timestamp_subsec_nanos</code>, which was missed in the 0.4.35 release (<a href="https://redirect.github.com/chronotope/chrono/issues/1486">#1486</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/chronotope/chrono/commit/352a35203a140e2352e5a5be62ba8dfd03b616e1"><code>352a352</code></a> Prepare 0.4.38</li>
<li><a href="https://github.com/chronotope/chrono/commit/46d44d6074ebdfddc62778bff24551f8d7bf9695"><code>46d44d6</code></a> Manually implement <code>Copy</code> for <code>DateTime</code> if offset is <code>Copy</code></li>
<li><a href="https://github.com/chronotope/chrono/commit/760eb660d3b6ff9c5e0d34cfa1daa83d0a815e9e"><code>760eb66</code></a> Update windows-bindgen requirement from 0.55 to 0.56</li>
<li><a href="https://github.com/chronotope/chrono/commit/391187fff3be8ac345edb0fd859d36cb99c24316"><code>391187f</code></a> Return error when rounding with zero duration</li>
<li><a href="https://github.com/chronotope/chrono/commit/ffc75e57054182603436b56e67c284d9fb7dec78"><code>ffc75e5</code></a> Add <code>TimeDelta::checked_mul</code> and <code>TimeDelta::checked_div</code></li>
<li><a href="https://github.com/chronotope/chrono/commit/f8cecbe57ea6c2d7ce69c7e17ec989258a515ee0"><code>f8cecbe</code></a> Make <code>Weekday::num_days_from public</code>, rename to <code>days_since</code>.</li>
<li><a href="https://github.com/chronotope/chrono/commit/0cfc405d3e93b1f4e8c6fd37a51449b6be7edb2c"><code>0cfc405</code></a> Optimize number formatting</li>
<li><a href="https://github.com/chronotope/chrono/commit/74ba83ba27056e5bb610327d37c488f2b212af86"><code>74ba83b</code></a> Take <code>pad</code> by value</li>
<li><a href="https://github.com/chronotope/chrono/commit/78e79dbabf30ba6fcf59ff6cc439c2dd944b0da0"><code>78e79db</code></a> Match on tuples in <code>format_fixed</code></li>
<li><a href="https://github.com/chronotope/chrono/commit/f3d76c7bb0902e269b902cf1bc9d986501675c52"><code>f3d76c7</code></a> Match on tuples in <code>format_numeric</code></li>
<li>Additional commits viewable in <a href="https://github.com/chronotope/chrono/compare/v0.4.33...v0.4.38">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=chrono&package-manager=cargo&previous-version=0.4.33&new-version=0.4.38)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Bump ts-node from 10.9.1 to 10.9.2 in /smart_contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ts-node](https://github.com/TypeStrong/ts-node) from 10.9.1 to 10.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/TypeStrong/ts-node/releases">ts-node's releases</a>.</em></p>
<blockquote>
<h2>Fix <code>tsconfig.json</code> file not found</h2>
<p><strong>Fixed</strong></p>
<ul>
<li>Fixed <code>tsconfig.json</code> file not found on latest TypeScript version (<a href="https://redirect.github.com/TypeStrong/ts-node/pull/2091">TypeStrong/ts-node#2091</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TypeStrong/ts-node/commit/057ac1beb118f9c42d21e876a17320ad73ea6be2"><code>057ac1b</code></a> 10.9.2</li>
<li><a href="https://github.com/TypeStrong/ts-node/commit/c8805d5d4bcdfa564fdcc0ff6630381c9f54ee5a"><code>c8805d5</code></a> Update package lock</li>
<li><a href="https://github.com/TypeStrong/ts-node/commit/99862f7ec663927045ecb5703230c368816d0857"><code>99862f7</code></a> Bump swc dependency</li>
<li><a href="https://github.com/TypeStrong/ts-node/commit/cdc4e883ab7072865abc4070f651374503cc88a9"><code>cdc4e88</code></a> Ignore test files in build schema</li>
<li><a href="https://github.com/TypeStrong/ts-node/commit/08cdfb0c70fbe3cadd658ef025d7947a0a59c920"><code>08cdfb0</code></a> Backport swc fixes on main</li>
<li><a href="https://github.com/TypeStrong/ts-node/commit/9639daa83c2122dd3d5ac4520f2d990d997fe8ba"><code>9639daa</code></a> Ignore test files in build</li>
<li><a href="https://github.com/TypeStrong/ts-node/commit/cc1a503e5faae87b034b76a3f5ddd53e5e7a6b3b"><code>cc1a503</code></a> Fix <code>tsconfig.json</code> not found with TS &gt;= 5.3 (<a href="https://redirect.github.com/TypeStrong/ts-node/issues/2091">#2091</a>)</li>
<li>See full diff in <a href="https://github.com/TypeStrong/ts-node/compare/v10.9.1...v10.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ts-node&package-manager=npm_and_yarn&previous-version=10.9.1&new-version=10.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Bump log from 0.4.20 to 0.4.22 in /vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [log](https://github.com/rust-lang/log) from 0.4.20 to 0.4.22.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/log/blob/master/CHANGELOG.md">log's changelog</a>.</em></p>
<blockquote>
<h2>[0.4.22] - 2024-06-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Add some clarifications to the library docs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/620">rust-lang/log#620</a></li>
<li>Add links to <code>colog</code> crate by <a href="https://github.com/chrivers"><code>@​chrivers</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/621">rust-lang/log#621</a></li>
<li>adding line_number test + updating some testing infrastructure by <a href="https://github.com/DIvkov575"><code>@​DIvkov575</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/619">rust-lang/log#619</a></li>
<li>Clarify the actual set of functions that can race in _racy variants by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/623">rust-lang/log#623</a></li>
<li>Replace deprecated std::sync::atomic::spin_loop_hint() by <a href="https://github.com/Catamantaloedis"><code>@​Catamantaloedis</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/625">rust-lang/log#625</a></li>
<li>Check usage of max_level features by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/627">rust-lang/log#627</a></li>
<li>Remove unneeded import by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/628">rust-lang/log#628</a></li>
<li>Loosen orderings for logger initialization in <a href="https://redirect.github.com/rust-lang/log/pull/632">rust-lang/log#632</a>. Originally by <a href="https://github.com/pwoolcoc"><code>@​pwoolcoc</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/599">rust-lang/log#599</a></li>
<li>Use Location::caller() for file and line info in <a href="https://redirect.github.com/rust-lang/log/pull/633">rust-lang/log#633</a>. Originally by <a href="https://github.com/Cassy343"><code>@​Cassy343</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/520">rust-lang/log#520</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/chrivers"><code>@​chrivers</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/621">rust-lang/log#621</a></li>
<li><a href="https://github.com/DIvkov575"><code>@​DIvkov575</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/619">rust-lang/log#619</a></li>
<li><a href="https://github.com/Catamantaloedis"><code>@​Catamantaloedis</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/625">rust-lang/log#625</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/rust-lang/log/compare/0.4.21...0.4.22">https://github.com/rust-lang/log/compare/0.4.21...0.4.22</a></p>
<h2>[0.4.21] - 2024-02-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Minor clippy nits by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/578">rust-lang/log#578</a></li>
<li>Simplify Display impl by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/579">rust-lang/log#579</a></li>
<li>Set all crates to 2021 edition by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/580">rust-lang/log#580</a></li>
<li>Various changes based on review by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/583">rust-lang/log#583</a></li>
<li>Fix typo in file_static() method doc by <a href="https://github.com/dimo414"><code>@​dimo414</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/590">rust-lang/log#590</a></li>
<li>Specialize empty key value pairs by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/576">rust-lang/log#576</a></li>
<li>Fix incorrect lifetime in Value::to_str() by <a href="https://github.com/peterjoel"><code>@​peterjoel</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/587">rust-lang/log#587</a></li>
<li>Remove some API of the key-value feature by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/585">rust-lang/log#585</a></li>
<li>Add logcontrol-log and log-reload by <a href="https://github.com/swsnr"><code>@​swsnr</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/595">rust-lang/log#595</a></li>
<li>Add Serialization section to kv::Value docs by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/593">rust-lang/log#593</a></li>
<li>Rename Value::to_str to to_cow_str by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/592">rust-lang/log#592</a></li>
<li>Clarify documentation and simplify initialization of <code>STATIC_MAX_LEVEL</code> by <a href="https://github.com/ptosi"><code>@​ptosi</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/594">rust-lang/log#594</a></li>
<li>Update docs to 2021 edition, test by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/577">rust-lang/log#577</a></li>
<li>Add &quot;alterable_logger&quot; link to README.md by <a href="https://github.com/brummer-simon"><code>@​brummer-simon</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/589">rust-lang/log#589</a></li>
<li>Normalize line ending by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/602">rust-lang/log#602</a></li>
<li>Remove <code>ok_or</code> in favor of <code>Option::ok_or</code> by <a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/607">rust-lang/log#607</a></li>
<li>Use <code>Acquire</code> ordering for initialization check by <a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/610">rust-lang/log#610</a></li>
<li>Get structured logging API ready for stabilization by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/613">rust-lang/log#613</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/nyurik"><code>@​nyurik</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/578">rust-lang/log#578</a></li>
<li><a href="https://github.com/dimo414"><code>@​dimo414</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/590">rust-lang/log#590</a></li>
<li><a href="https://github.com/peterjoel"><code>@​peterjoel</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/587">rust-lang/log#587</a></li>
<li><a href="https://github.com/ptosi"><code>@​ptosi</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/594">rust-lang/log#594</a></li>
<li><a href="https://github.com/brummer-simon"><code>@​brummer-simon</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/589">rust-lang/log#589</a></li>
<li><a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/607">rust-lang/log#607</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/log/commit/d5ba2cfee9b3b4ca1fcad911b7f59dc79eeee022"><code>d5ba2cf</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/634">#634</a> from rust-lang/cargo/0.4.22</li>
<li><a href="https://github.com/rust-lang/log/commit/d1a8306aadb88d56b74c73cdce4ef0153fb549cb"><code>d1a8306</code></a> prepare for 0.4.22 release</li>
<li><a href="https://github.com/rust-lang/log/commit/46894ef229483bbabd30a806c474417fc034559c"><code>46894ef</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/633">#633</a> from rust-lang/feat/panic-info</li>
<li><a href="https://github.com/rust-lang/log/commit/e0d389c9cadd91363f2fec52bd30f9585168a89f"><code>e0d389c</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/632">#632</a> from rust-lang/feat/loosen-atomics</li>
<li><a href="https://github.com/rust-lang/log/commit/c9e5e13e9b02ec80e784c6fe4deacdc8f3194fca"><code>c9e5e13</code></a> use Location::caller() for file and line info</li>
<li><a href="https://github.com/rust-lang/log/commit/507b672660288f0223edb6353d34f8733fa0a2f4"><code>507b672</code></a> loosen orderings for logger initialization</li>
<li><a href="https://github.com/rust-lang/log/commit/c879b011a8ac662545adf9484d9a668ebcf9b814"><code>c879b01</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/628">#628</a> from Thomasdezeeuw/fix-warnings</li>
<li><a href="https://github.com/rust-lang/log/commit/405fdb4d9f847c93c0133469ea808f09320714ba"><code>405fdb4</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/627">#627</a> from Thomasdezeeuw/check-features</li>
<li><a href="https://github.com/rust-lang/log/commit/1307ade1122549badf2b8fdd10c11e519eaa029a"><code>1307ade</code></a> Remove unneeded import</li>
<li><a href="https://github.com/rust-lang/log/commit/710560ecb7035a6baf1fd9d97d7f09d0cc075006"><code>710560e</code></a> Don't use --all-features in CI</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/log/compare/0.4.20...0.4.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log&package-manager=cargo&previous-version=0.4.20&new-version=0.4.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Bump solidity-coverage from 0.8.6 to 0.8.12 in /smart_contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [solidity-coverage](https://github.com/sc-forks/solidity-coverage) from 0.8.6 to 0.8.12.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/releases">solidity-coverage's releases</a>.</em></p>
<blockquote>
<h2>v0.8.12</h2>
<h2>What's Changed</h2>
<ul>
<li>Adds &quot;work-around&quot; support for the <code>hardhat-viem</code> plugin. If you're using viem, run the coverage task with:
<pre><code>SOLIDITY_COVERAGE=true npx hardhat coverage
</code></pre>
</li>
<li>Adds support for solc v0.4.x</li>
<li>Fixes a bug where plugin crashed if the contract sources directory name contained a period.</li>
<li>Fixes a bug where instrumentation failed if there was whitespace between <code>require</code> statement and the terminating semi-colon</li>
</ul>
<h4>PRs</h4>
<ul>
<li>Add extendConfig logic for hardhat-viem plugin by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/883">sc-forks/solidity-coverage#883</a></li>
<li>Support solc v0.4.x by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/877">sc-forks/solidity-coverage#877</a></li>
<li>Use fs.stat to check directory status by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/880">sc-forks/solidity-coverage#880</a></li>
<li>Update hardhat dev dep to 2.22.2 (EDR) by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/881">sc-forks/solidity-coverage#881</a></li>
<li>Tolerate whitespace between <code>require</code> and terminating <code>;</code> by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/884">sc-forks/solidity-coverage#884</a></li>
<li>Document <code>extendConfig</code> changes in README by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/885">sc-forks/solidity-coverage#885</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.11...v0.8.12">https://github.com/sc-forks/solidity-coverage/compare/v0.8.11...v0.8.12</a></p>
<h2>v0.8.11</h2>
<h2>Summary</h2>
<p>0.8.11 fixes a(nother) bug that resulted in some line hits remaining undetected when compiling with viaIR=true</p>
<h2>What's Changed</h2>
<ul>
<li>Check all SWAP opcodes for inst. hashes when viaIR is true by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/873">sc-forks/solidity-coverage#873</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.10...v0.8.11">https://github.com/sc-forks/solidity-coverage/compare/v0.8.10...v0.8.11</a></p>
<h2>0.8.10</h2>
<h2>Summary</h2>
<p>0.8.10 fixes a bug that resulted in some line hits remaining undetected when compiling with <code>viaIR=true</code></p>
<h2>What's Changed</h2>
<ul>
<li>Check all PUSH opcodes for instr. hashes when viaIR is true by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/871">sc-forks/solidity-coverage#871</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.9...v0.8.10">https://github.com/sc-forks/solidity-coverage/compare/v0.8.9...v0.8.10</a></p>
<h2>0.8.9</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix regression introduced in 0.8.7 where modifier branch coverage for modifiers inherited from a dependency was not measured correctly in some cases <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/868">sc-forks/solidity-coverage#868</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.8...v0.8.9">https://github.com/sc-forks/solidity-coverage/compare/v0.8.8...v0.8.9</a></p>
<h2>0.8.8</h2>
<h2>What's Changed</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/blob/master/CHANGELOG.md">solidity-coverage's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1>0.8.11 / 2024-03-07</h1>
<ul>
<li>Check all SWAP opcodes for inst. hashes when viaIR is true (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/873">sc-forks/solidity-coverage#873</a>)</li>
</ul>
<h1>0.8.10 / 2024-02-29</h1>
<ul>
<li>Check all PUSH opcodes for instr. hashes when viaIR is true (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/871">sc-forks/solidity-coverage#871</a>)</li>
</ul>
<h1>0.8.9 / 2024-02-27</h1>
<ul>
<li>Fix duplicate hash logic (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/868">sc-forks/solidity-coverage#868</a>)</li>
<li>Improve organization of edge case code in collector (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/869">sc-forks/solidity-coverage#869</a>)</li>
</ul>
<h1>0.8.8 / 2024-02-21</h1>
<ul>
<li>Coerce sources path to absolute path if necessary (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/866">sc-forks/solidity-coverage#866</a>)</li>
<li>Only inject file-level instr. for first pragma in file (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/865">sc-forks/solidity-coverage#865</a>)</li>
</ul>
<h1>0.8.7 / 2024-02-09</h1>
<ul>
<li>Documentation Cleanup &amp; Improvements for 0.8.7 release
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/859">sc-forks/solidity-coverage#859</a>)</li>
<li>Add tests for file-level function declarations
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/858">sc-forks/solidity-coverage#858</a>)</li>
<li>Add try / catch unit tests (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/857">sc-forks/solidity-coverage#857</a>)</li>
<li>Fix test project configs for viaIR detection in overrides
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/856">sc-forks/solidity-coverage#856</a>)</li>
<li>Enable coverage when viaIR compiler flag is true
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/854">sc-forks/solidity-coverage#854</a>)</li>
<li>Add missing onPreCompile hook
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/851">sc-forks/solidity-coverage#851</a>)</li>
<li>Remove ganache-cli related code from API &amp; tests
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/849">sc-forks/solidity-coverage#849</a>)</li>
<li>Add command option to specify the source files to run the coverage on
(<a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/838">sc-forks/solidity-coverage#838</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/f550eaeed9c05922bdb059030d86c27a0c22c142"><code>f550eae</code></a> 0.8.12</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/a1158f5ec64f8c33438edcfbb383d87cb8ab8a3b"><code>a1158f5</code></a> Document <code>extendConfig</code> changes in README (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/885">#885</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/4f5626d6543ecc72bde8f0646a16494ff2f7ca93"><code>4f5626d</code></a> Tolerate whitespace between <code>require</code> and terminating <code>;</code> (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/884">#884</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/09a7c833ae289791a9037babd4bc2e106c291845"><code>09a7c83</code></a> Add extendConfig logic for hardhat-viem plugin (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/883">#883</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/011ee40ecf1494b23c069750c17dfe6006d295e1"><code>011ee40</code></a> Update hardhat dev dep to 2.22.2 (EDR) (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/881">#881</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/66fda89e69421ba1def9bbb7dd292487cc3c375f"><code>66fda89</code></a> Use fs.stat to check directory status (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/880">#880</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/a20fbf7b1130d62d1c686d0401a9da537fd35e7b"><code>a20fbf7</code></a> Support solc v0.4.x (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/877">#877</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/12436cc14da96f6808a8e1e45e88f91699d9739d"><code>12436cc</code></a> Update changelog: 0.8.11</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/ba32cd32dcff95b381f75fd0b28b2118383e8019"><code>ba32cd3</code></a> 0.8.11</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/6236a8fe9ddc074adb63c71e8cd45aeda09f755d"><code>6236a8f</code></a> Check all SWAP opcodes for inst. hashes when viaIR is true (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/873">#873</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.6...v0.8.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=solidity-coverage&package-manager=npm_and_yarn&previous-version=0.8.6&new-version=0.8.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Bump rstest from 0.18.2 to 0.21.0 in /vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rstest](https://github.com/la10736/rstest) from 0.18.2 to 0.21.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/la10736/rstest/releases">rstest's releases</a>.</em></p>
<blockquote>
<h2>0.21.0</h2>
<p>Use <code>crate-name</code> feature to enable the crate rename support (enabled by default)</p>
<h2>0.20.0</h2>
<p>Introduce #[by_ref] and add support for import rstest with another name.</p>
<p>Introduce MSRV and minor fixes</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/la10736/rstest/blob/master/CHANGELOG.md">rstest's changelog</a>.</em></p>
<blockquote>
<h2>[0.21.0] 2024/6/1</h2>
<h3>Changed</h3>
<ul>
<li>Add feature <code>crate-name</code> enabled by default to opt-in crate rename
support. See <a href="https://redirect.github.com/la10736/rstest/issues/258">#258</a></li>
</ul>
<h2>[0.20.0] 2024/5/30</h2>
<h3>Add</h3>
<ul>
<li>Implemented <code>#[by_ref]</code> attribute to take get a local lifetime for test arguments.
See <a href="https://redirect.github.com/la10736/rstest/issues/241">#241</a> for more details. Thanks to
<a href="https://github.com/narpfel"><code>@​narpfel</code></a> for suggesting it and useful discussions.</li>
<li>Support for import <code>rstest</code> with another name. See <a href="https://redirect.github.com/la10736/rstest/issues/221">#221</a></li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Don't remove Lifetimes from test function if any. See <a href="https://redirect.github.com/la10736/rstest/issues/230">#230</a>
<a href="https://redirect.github.com/la10736/rstest/issues/241">#241</a> for more details.</li>
<li><a href="https://doc.rust-lang.org/std/path/struct.PathBuf.html"><code>PathBuf</code></a> does no longer need to be
in scope when using <code>#[files]</code> (see <a href="https://redirect.github.com/la10736/rstest/pull/242">#242</a>)</li>
<li><code>#[from(now::accept::also::path::for::fixture)]</code> See <a href="https://redirect.github.com/la10736/rstest/issues/246">#246</a>
for more details</li>
</ul>
<h2>[0.19.0] 2024/4/9</h2>
<h3>Changed</h3>
<ul>
<li>Defined <code>rust-version</code> for each crate (see <a href="https://redirect.github.com/la10736/rstest/issues/227">#227</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>
<p><code>#[once]</code> fixtures now require the returned type to be
<a href="https://doc.rust-lang.org/std/marker/trait.Sync.html"><code>Sync</code></a> to prevent UB
when tests are executed in parallel. (see <a href="https://redirect.github.com/la10736/rstest/issues/235">#235</a>
for more details)</p>
</li>
<li>
<p><code>#[future(awt)]</code> and <code>#[awt]</code> now properly handle mutable (<code>mut</code>) parameters by treating futures as immutable and
treating the awaited rebinding as mutable.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/la10736/rstest/commit/38da6bfb9640763727778c07225228ebf405500e"><code>38da6bf</code></a> Prepare 0.21.0 Release</li>
<li><a href="https://github.com/la10736/rstest/commit/ca69788392e8b45f371939525d949b97e5b93673"><code>ca69788</code></a> bump version rstest_test to 0.13.0</li>
<li><a href="https://github.com/la10736/rstest/commit/b6b43c6740381ddbda6bf88276a3946c8e02f049"><code>b6b43c6</code></a> Clean chackoutlist</li>
<li><a href="https://github.com/la10736/rstest/commit/fef4f7b4f4eb1e0eb1c40b8554bdcb32b96e4a1e"><code>fef4f7b</code></a> Implemented Opt-in crate-name support Fix <a href="https://redirect.github.com/la10736/rstest/issues/258">#258</a></li>
<li><a href="https://github.com/la10736/rstest/commit/236be92a8a7b376669c7e5c18e29cc2e4e85f84c"><code>236be92</code></a> Build should use build tests target</li>
<li><a href="https://github.com/la10736/rstest/commit/8fde5be94fb6918492189c3f55528bd1e7962d01"><code>8fde5be</code></a> Prepare next changelog</li>
<li><a href="https://github.com/la10736/rstest/commit/f29e6346fee09a8854e20aa4c13a50da094fde30"><code>f29e634</code></a> Dependency should have a n explicit version to be published</li>
<li><a href="https://github.com/la10736/rstest/commit/e27ad2a4db085c714b9a98012683721f0fd5cb3d"><code>e27ad2a</code></a> Removed empty section</li>
<li><a href="https://github.com/la10736/rstest/commit/386779448365f5bb8620f404ad485b5a82a261be"><code>3867794</code></a> Fixed docs</li>
<li><a href="https://github.com/la10736/rstest/commit/b90fb8e0923b394223b72ab1ef63367959abfcba"><code>b90fb8e</code></a> Fix checkout list</li>
<li>Additional commits viewable in <a href="https://github.com/la10736/rstest/compare/v0.18.2...v0.21.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rstest&package-manager=cargo&previous-version=0.18.2&new-version=0.21.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Bump base64 from 0.21.7 to 0.22.1 in /vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [base64](https://github.com/marshallpierce/rust-base64) from 0.21.7 to 0.22.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/marshallpierce/rust-base64/blob/master/RELEASE-NOTES.md">base64's changelog</a>.</em></p>
<blockquote>
<h1>0.22.1</h1>
<ul>
<li>Correct the symbols used for the predefined <code>alphabet::BIN_HEX</code>.</li>
</ul>
<h1>0.22.0</h1>
<ul>
<li><code>DecodeSliceError::OutputSliceTooSmall</code> is now conservative rather than precise. That is, the error will only occur if the decoded output <em>cannot</em> fit, meaning that <code>Engine::decode_slice</code> can now be used with exactly-sized output slices. As part of this, <code>Engine::internal_decode</code> now returns <code>DecodeSliceError</code> instead of <code>DecodeError</code>, but that is not expected to affect any external callers.</li>
<li><code>DecodeError::InvalidLength</code> now refers specifically to the <em>number of valid symbols</em> being invalid (i.e. <code>len % 4 == 1</code>), rather than just the number of input bytes. This avoids confusing scenarios when based on interpretation you could make a case for either <code>InvalidLength</code> or <code>InvalidByte</code> being appropriate.</li>
<li>Decoding is somewhat faster (5-10%)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/e14400697453bcc85997119b874bc03d9601d0af"><code>e144006</code></a> v0.22.1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/64cca59ddbb4c43244a8f38629b59960ffe36bc0"><code>64cca59</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/271">#271</a> from JobanSD/patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/838355e0ac5fb8237ec9b96be5edb011bff00275"><code>838355e</code></a> Correct BinHex 4.0 alphabet according to specifications</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/bf15ccf30af8bb6b1f326fffa025d7b0aaa3342f"><code>bf15ccf</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/270">#270</a> from marshallpierce/mp/clippy</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/fc6aabee8afaf8b2f4cfb12df4cf461bcf9b003d"><code>fc6aabe</code></a> Appease clippy</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/9a518a2d5d028068d4bf83ebf437f7a3575e640e"><code>9a518a2</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/267">#267</a> from bdura/patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/d96c80f242e3080a03fd1c079730e17373ef0eb6"><code>d96c80f</code></a> Merge branch 'marshallpierce:master' into patch-1</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/5d70ba7576f9aafcbf02bd8acfcb9973411fb95f"><code>5d70ba7</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/269">#269</a> from marshallpierce/mp/decode-precisely</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/efb6c006c75ddbe60c084c2e3e0e084cd18b0122"><code>efb6c00</code></a> Release notes</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/2b91084a31ad11624acd81e06455ba0cbd21d4a8"><code>2b91084</code></a> Add some tests to boost coverage</li>
<li>Additional commits viewable in <a href="https://github.com/marshallpierce/rust-base64/compare/v0.21.7...v0.22.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=base64&package-manager=cargo&previous-version=0.21.7&new-version=0.22.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Bump @types/node from 16.18.101 to 20.14.9 in /vdr/wasm/demo/node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@types/node](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/HEAD/types/node) from 16.18.101 to 20.14.9.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/DefinitelyTyped/DefinitelyTyped/commits/HEAD/types/node">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@types/node&package-manager=npm_and_yarn&previous-version=16.18.101&new-version=20.14.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Bump typescript from 4.9.5 to 5.5.2 in /vdr/wasm/demo/node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [typescript](https://github.com/Microsoft/TypeScript) from 4.9.5 to 5.5.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Microsoft/TypeScript/releases">typescript's releases</a>.</em></p>
<blockquote>
<h2>TypeScript 5.5</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-5/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=is%3Aissue+milestone%3A%22TypeScript+5.5.2%22+is%3Aclosed+">fixed issues query for TypeScript v5.5.2 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=is%3Aissue+milestone%3A%22TypeScript+5.5.1%22+is%3Aclosed+">fixed issues query for TypeScript v5.5.1 (RC)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=is%3Aissue+milestone%3A%22TypeScript+5.5.0%22+is%3Aclosed+">fixed issues query for TypeScript v5.5.0 (Beta)</a>.</li>
</ul>
<p>Downloads are available on:</p>
<ul>
<li><a href="https://www.npmjs.com/package/typescript">npm</a></li>
<li><a href="https://www.nuget.org/packages/Microsoft.TypeScript.MSBuild">NuGet package</a></li>
</ul>
<h2>TypeScript 5.5 RC</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-5-rc/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.5.0%22+is%3Aclosed+">fixed issues query for Typescript 5.5.0 (Beta)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.5.1%22+is%3Aclosed+">fixed issues query for Typescript 5.5.1 (RC)</a>.</li>
</ul>
<p>Downloads are available on:</p>
<ul>
<li><a href="https://www.nuget.org/packages/Microsoft.TypeScript.MSBuild">NuGet package</a></li>
</ul>
<h2>TypeScript 5.5 Beta</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-5-beta/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.5.0%22+is%3Aclosed+">fixed issues query for Typescript 5.5.0 (Beta)</a>.</li>
</ul>
<p>Downloads are available on:</p>
<ul>
<li><a href="https://www.npmjs.com/package/typescript">npm</a></li>
<li><a href="https://www.nuget.org/packages/Microsoft.TypeScript.MSBuild">NuGet package</a></li>
</ul>
<h2>TypeScript 5.4.5</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-4/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.0%22+is%3Aclosed+">fixed issues query for Typescript 5.4.0 (Beta)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.1%22+is%3Aclosed+">fixed issues query for Typescript 5.4.1 (RC)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.2%22+is%3Aclosed+">fixed issues query for Typescript 5.4.2 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.3%22+is%3Aclosed+">fixed issues query for Typescript 5.4.3 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.4%22+is%3Aclosed+">fixed issues query for Typescript 5.4.4 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.5%22+is%3Aclosed+">fixed issues query for Typescript 5.4.5 (Stable)</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/microsoft/TypeScript/commit/ce2e60e4ea15a65992e54a9e8877d16be9d42abb"><code>ce2e60e</code></a> Update LKG</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/f3b21a2033206e585b2b7b18622104f09eb87f2e"><code>f3b21a2</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58931">#58931</a> (Defer creation of barebonesLibSourc...) into release-5.5 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/7b1620bea227ea47f8944a2b02a7ed91691c3046"><code>7b1620b</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58811">#58811</a> (fix(58801): &quot;Move to file&quot; on globa...) into release-5.5 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/5367ae10f58edfacd6d3b1e77bd05576036b8ca2"><code>5367ae1</code></a> Bump version to 5.5.2 and LKG</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/02132e5b8183b0ee73e52d75ff6e28ff0c9fe3d2"><code>02132e5</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58895">#58895</a> (Fix global when typescript.js loade...) into release-5.5 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/45b1e3c25444c4193cefb4ca97dfd1064f75a561"><code>45b1e3c</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58872">#58872</a> (Fix declaration emit crash) into release-5.5 (<a href="https://redirect.github.com/Microsoft/TypeScript/issues/58874">#58874</a>)</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/17933ee33af4a3c44233820abf8bdb0ad2bf143a"><code>17933ee</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58810">#58810</a> (Fixed declaration emit issue relate...) into release-5.5 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/552b07e795ec5db98c37fd4ace730133bbf0e781"><code>552b07e</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58786">#58786</a> (Fixed declaration emit crash relate...) into release-5.5 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/39c9eebf1707b194b525a4c471b8b6bfe3f52642"><code>39c9eeb</code></a> Pick <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58857">#58857</a> to release-5.5 (<a href="https://redirect.github.com/Microsoft/TypeScript/issues/58858">#58858</a>)</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/2b0009c6790d66bbc943fc3975eb8bc9e8dec83f"><code>2b0009c</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58846">#58846</a> (Ensure the updates with crashes rev...) into release-5.5 (#...</li>
<li>Additional commits viewable in <a href="https://github.com/Microsoft/TypeScript/compare/v4.9.5...v5.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=typescript&package-manager=npm_and_yarn&previous-version=4.9.5&new-version=5.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    Bump serde_json from 1.0.113 to 1.0.119 in /vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.113 to 1.0.119.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.119</h2>
<ul>
<li>Add <code>serde_json::Map::shift_insert</code> (<a href="https://redirect.github.com/serde-rs/json/issues/1149">#1149</a>, thanks <a href="https://github.com/joshka"><code>@​joshka</code></a>)</li>
</ul>
<h2>v1.0.118</h2>
<ul>
<li>Implement Hash for serde_json::Value (<a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a>, thanks <a href="https://github.com/edwardycl"><code>@​edwardycl</code></a>)</li>
</ul>
<h2>v1.0.117</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/serde-rs/json/issues/1130">#1130</a>)</li>
</ul>
<h2>v1.0.116</h2>
<ul>
<li>Make module structure comprehensible to static analysis (<a href="https://redirect.github.com/serde-rs/json/issues/1124">#1124</a>, thanks <a href="https://github.com/mleonhard"><code>@​mleonhard</code></a>)</li>
</ul>
<h2>v1.0.115</h2>
<ul>
<li>Documentation improvements</li>
</ul>
<h2>v1.0.114</h2>
<ul>
<li>Fix unused_imports warnings when compiled by rustc 1.78</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/b48b9a3a0c09952579e98c8940fe0d1ee4aae588"><code>b48b9a3</code></a> Release 1.0.119</li>
<li><a href="https://github.com/serde-rs/json/commit/8878cd7c042a5f94ae4ee9889cbcbd12cc5ce334"><code>8878cd7</code></a> Make shift_insert available for inlining like other Map methods</li>
<li><a href="https://github.com/serde-rs/json/commit/352b7abf007cf3b9b063b01e0b1e8f6af62a4e39"><code>352b7ab</code></a> Document the cfg required for Map::shift_insert to exist</li>
<li><a href="https://github.com/serde-rs/json/commit/c17e63f6eff6cb40594beb1bddd4562c4cc81442"><code>c17e63f</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1149">#1149</a> from joshka/master</li>
<li><a href="https://github.com/serde-rs/json/commit/309ef6b8870e47622a283061cbda3f5514bfaf0d"><code>309ef6b</code></a> Add Map::shift_insert()</li>
<li><a href="https://github.com/serde-rs/json/commit/a9e089a2ce245bc223b56fbb6c525e2fe7b1f0ef"><code>a9e089a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1146">#1146</a> from haouvw/master</li>
<li><a href="https://github.com/serde-rs/json/commit/a83fe96ae2a202925f1caa7abc51991f321d7c22"><code>a83fe96</code></a> chore: remove repeat words</li>
<li><a href="https://github.com/serde-rs/json/commit/c4f24f3be29a3d096d3ac7b1d5594777a613ec0d"><code>c4f24f3</code></a> Release 1.0.118</li>
<li><a href="https://github.com/serde-rs/json/commit/51d94ebdc07127de22fb655bdcf6a01d119492d5"><code>51d94eb</code></a> Combine Map's Hash into one impl</li>
<li><a href="https://github.com/serde-rs/json/commit/5e7bedc0a0e19ecda1c15a412ab7c69569f4aa84"><code>5e7bedc</code></a> Touch up PR 1127</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.113...v1.0.119">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.113&new-version=1.0.119)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:41:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Bump bs58 from 5.0.0 to 6.0.0 in /vdr/wasm/demo/node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [bs58](https://github.com/cryptocoinjs/bs58) from 5.0.0 to 6.0.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/e23aea1ef3fd572169db3cbbfabfd51f72202ac4"><code>e23aea1</code></a> 6.0.0</li>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/f20339e401cc1ff38aea516bc1901ddd236610b1"><code>f20339e</code></a> Merge pull request <a href="https://redirect.github.com/cryptocoinjs/bs58/issues/48">#48</a> from Nesopie/feat/hybrid</li>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/0fd6d481cc0d8ad7b7a6d463bf6141f7e68316f3"><code>0fd6d48</code></a> chore: rm lockfile from .gitignore</li>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/f2d5c7d519f61459be088a373c812c7b28a65d5b"><code>f2d5c7d</code></a> fix: included files for publishing</li>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/7ef8ae8d0b27cb96950bd2bdebf32b99be42f256"><code>7ef8ae8</code></a> feat: hybrid cjs and esm support</li>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/3ebc63d1254c6472a0fd1f6d416d49d8b588e380"><code>3ebc63d</code></a> Fix npm publish bug</li>
<li><a href="https://github.com/cryptocoinjs/bs58/commit/d77eedfe19f3cc419e25628bc9bc44bea2df5fdd"><code>d77eedf</code></a> Merge pull request <a href="https://redirect.github.com/cryptocoinjs/bs58/issues/44">#44</a> from cryptocoinjs/feature/uint8array</li>
<li>See full diff in <a href="https://github.com/cryptocoinjs/bs58/compare/v5.0.0...v6.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=bs58&package-manager=npm_and_yarn&previous-version=5.0.0&new-version=6.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:40:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Bump secp256k1 from 4.0.3 to 5.0.0 in /network/tools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [secp256k1](https://github.com/cryptocoinjs/secp256k1-node) from 4.0.3 to 5.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cryptocoinjs/secp256k1-node/releases">secp256k1's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>3482be9 Fix segfaults when used with worker_threads (<a href="https://redirect.github.com/cryptocoinjs/secp256k1-node/issues/195">#195</a>)</li>
<li>4afabb4 docs: fix example of unrelated public/private pair (<a href="https://redirect.github.com/cryptocoinjs/secp256k1-node/issues/192">#192</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cryptocoinjs/secp256k1-node/commit/6d3474b81d073cc9c8cc8cfadb580c84f8df5248"><code>6d3474b</code></a> 5.0.0</li>
<li><a href="https://github.com/cryptocoinjs/secp256k1-node/commit/3482be91bafc766680be6de2d4da07dc5705e9bb"><code>3482be9</code></a> Fix segfaults when used with worker_threads (<a href="https://redirect.github.com/cryptocoinjs/secp256k1-node/issues/195">#195</a>)</li>
<li><a href="https://github.com/cryptocoinjs/secp256k1-node/commit/4afabb44e6de6c0164d1e7c0ecfbbea181d304a8"><code>4afabb4</code></a> docs: fix example of unrelated public/private pair (<a href="https://redirect.github.com/cryptocoinjs/secp256k1-node/issues/192">#192</a>)</li>
<li>See full diff in <a href="https://github.com/cryptocoinjs/secp256k1-node/compare/v4.0.3...v5.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=secp256k1&package-manager=npm_and_yarn&previous-version=4.0.3&new-version=5.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 11:40:53 +0000 UTC
    </div>
</div>

