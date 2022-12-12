---
layout: default
title: anoncreds-spec
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-spec
---

# anoncreds-spec <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-spec){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/115" class=".btn">#115</a>
            </td>
            <td>
                <b>
                    *: Fix latex and update key def
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
        Created At 2022-12-12 07:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    chore(deps): bump minimatch and mocha
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimatch](https://github.com/isaacs/minimatch) to 3.1.2 and updates ancestor dependency [mocha](https://github.com/mochajs/mocha). These dependencies need to be updated together.

Updates `minimatch` from 3.0.4 to 3.1.2
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/isaacs/minimatch/commit/699c459443a6bd98f5b28197978f76e7f71467ac"><code>699c459</code></a> 3.1.2</li>
<li><a href="https://github.com/isaacs/minimatch/commit/2f2b5ff1bb1b6a01f4404f7e475f0a2cba578ab7"><code>2f2b5ff</code></a> fix: trim pattern</li>
<li><a href="https://github.com/isaacs/minimatch/commit/25d7c0d09c47063c9b0d2ace17ef8e951d90eccc"><code>25d7c0d</code></a> 3.1.1</li>
<li><a href="https://github.com/isaacs/minimatch/commit/55dda291dfb595bd11b4edb19b45dd98eda76de0"><code>55dda29</code></a> fix: treat nocase:true as always having magic</li>
<li><a href="https://github.com/isaacs/minimatch/commit/5e1fb8dd2bb78c0ae22101b9229fac4c76ef039e"><code>5e1fb8d</code></a> 3.1.0</li>
<li><a href="https://github.com/isaacs/minimatch/commit/f8145c54f34075069f4a23cb214d871da4cd4006"><code>f8145c5</code></a> Add 'allowWindowsEscape' option</li>
<li><a href="https://github.com/isaacs/minimatch/commit/570e8b1aef6c9e823a824aa0b9be10db43857cd7"><code>570e8b1</code></a> add publishConfig for v3 publishes</li>
<li><a href="https://github.com/isaacs/minimatch/commit/5b7cd3372be253759fb4d865eb3f38f189a5fcdf"><code>5b7cd33</code></a> 3.0.6</li>
<li><a href="https://github.com/isaacs/minimatch/commit/20b4b562830680867feb75f9c635aca08e5c86ff"><code>20b4b56</code></a> [fix] revert all breaking syntax changes</li>
<li><a href="https://github.com/isaacs/minimatch/commit/2ff038852ec03e85e60e0eb333005c680ac8a543"><code>2ff0388</code></a> document, expose, and test 'partial:true' option</li>
<li>Additional commits viewable in <a href="https://github.com/isaacs/minimatch/compare/v3.0.4...v3.1.2">compare view</a></li>
</ul>
</details>
<br />

Updates `mocha` from 8.4.0 to 10.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mochajs/mocha/releases">mocha's releases</a>.</em></p>
<blockquote>
<h2>v10.1.0</h2>
<h1>10.1.0 / 2022-10-16</h1>
<h2>:tada: Enhancements</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4896">#4896</a>: Browser: add support for <code>prefers-color-scheme: dark</code> (<a href="https://github.com/greggman"><strong><code>@​greggman</code></strong></a>)</li>
</ul>
<h2>:nut_and_bolt: Other</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4912">#4912</a>: Browser: increase contrast for replay buttons (<a href="https://github.com/JoshuaKGoldberg"><strong><code>@​JoshuaKGoldberg</code></strong></a>)</li>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4905">#4905</a>: Use standard <code>Promise.allSettled</code> instead of polyfill (<a href="https://github.com/outsideris"><strong><code>@​outsideris</code></strong></a>)</li>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4899">#4899</a>: Upgrade official GitHub actions to latest (<a href="https://github.com/ddzz"><strong><code>@​ddzz</code></strong></a>)</li>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4770">#4770</a>: Fix regex in function <code>clean</code>(<a href="https://github.com/yetingli"><strong><code>@​yetingli</code></strong></a>)</li>
</ul>
<h2>v10.0.0</h2>
<h1>10.0.0 / 2022-05-01</h1>
<h2>:boom: Breaking Changes</h2>
<ul>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4845">#4845</a>: <strong>Drop Node.js v12.x support</strong> (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4848">#4848</a>: Drop Internet-Explorer-11 support (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4857">#4857</a>: Drop AMD/RequireJS support (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4866">#4866</a>: Drop Growl notification support (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4863">#4863</a>: Rename executable <code>bin/mocha</code> to <code>bin/mocha.js</code> (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4865">#4865</a>: <code>--ignore</code> option in Windows: upgrade Minimatch (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4861">#4861</a>: Remove deprecated <code>Runner</code> signature (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
</ul>
<h2>:nut_and_bolt: Other</h2>
<ul>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4878">#4878</a>: Update production dependencies (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4876">#4876</a>: Add Node.js v18 to CI test matrix (<a href="https://github.com/outsideris"><strong><code>@​outsideris</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4852">#4852</a>: Replace deprecated <code>String.prototype.substr()</code> (<a href="https://github.com/CommanderRoot"><strong><code>@​CommanderRoot</code></strong></a>)</p>
</li>
</ul>
<p>Also thanks to <a href="https://github.com/ea2305"><strong><code>@​ea2305</code></strong></a> and <a href="https://github.com/SukkaW"><strong><code>@​SukkaW</code></strong></a> for improvements to our documentation.</p>
<h2>v9.2.2</h2>
<h1>9.2.2 / 2022-03-11</h1>
<p>Please also note our <a href="https://github.com/mochajs/mocha/discussions/categories/announcements">announcements</a>.</p>
<h2>:bug: Fixes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mochajs/mocha/blob/master/CHANGELOG.md">mocha's changelog</a>.</em></p>
<blockquote>
<h1>10.1.0 / 2022-10-16</h1>
<h2>:tada: Enhancements</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4896">#4896</a>: Browser: add support for <code>prefers-color-scheme: dark</code> (<a href="https://github.com/greggman"><strong><code>@​greggman</code></strong></a>)</li>
</ul>
<h2>:nut_and_bolt: Other</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4912">#4912</a>: Browser: increase contrast for replay buttons (<a href="https://github.com/JoshuaKGoldberg"><strong><code>@​JoshuaKGoldberg</code></strong></a>)</li>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4905">#4905</a>: Use standard <code>Promise.allSettled</code> instead of polyfill (<a href="https://github.com/outsideris"><strong><code>@​outsideris</code></strong></a>)</li>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4899">#4899</a>: Upgrade official GitHub actions to latest (<a href="https://github.com/ddzz"><strong><code>@​ddzz</code></strong></a>)</li>
<li><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4770">#4770</a>: Fix regex in function <code>clean</code>(<a href="https://github.com/yetingli"><strong><code>@​yetingli</code></strong></a>)</li>
</ul>
<h1>10.0.0 / 2022-05-01</h1>
<h2>:boom: Breaking Changes</h2>
<ul>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4845">#4845</a>: <strong>Drop Node.js v12.x support</strong> (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4848">#4848</a>: Drop Internet-Explorer-11 support (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4857">#4857</a>: Drop AMD/RequireJS support (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4866">#4866</a>: Drop Growl notification support (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4863">#4863</a>: Rename executable <code>bin/mocha</code> to <code>bin/mocha.js</code> (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4865">#4865</a>: <code>--ignore</code> option in Windows: upgrade Minimatch (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4861">#4861</a>: Remove deprecated <code>Runner</code> signature (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
</ul>
<h2>:nut_and_bolt: Other</h2>
<ul>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4878">#4878</a>: Update production dependencies (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4876">#4876</a>: Add Node.js v18 to CI test matrix (<a href="https://github.com/outsideris"><strong><code>@​outsideris</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4852">#4852</a>: Replace deprecated <code>String.prototype.substr()</code> (<a href="https://github.com/CommanderRoot"><strong><code>@​CommanderRoot</code></strong></a>)</p>
</li>
</ul>
<p>Also thanks to <a href="https://github.com/ea2305"><strong><code>@​ea2305</code></strong></a> and <a href="https://github.com/SukkaW"><strong><code>@​SukkaW</code></strong></a> for improvements to our documentation.</p>
<h1>9.2.2 / 2022-03-11</h1>
<h2>:bug: Fixes</h2>
<ul>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4842">#4842</a>: Loading of reporter throws wrong error (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
<li>
<p><a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4839">#4839</a>: <code>dry-run</code>: prevent potential call-stack crash (<a href="https://github.com/juergba"><strong><code>@​juergba</code></strong></a>)</p>
</li>
</ul>
<h2>:nut_and_bolt: Other</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mochajs/mocha/commit/5f96d511dbf913f135b92198aab721a27f6b44fe"><code>5f96d51</code></a> build(v10.1.0): release</li>
<li><a href="https://github.com/mochajs/mocha/commit/ed74f16878f6520411d9a391c5f184056be6da30"><code>ed74f16</code></a> build(v10.1.0): update CHANGELOG</li>
<li><a href="https://github.com/mochajs/mocha/commit/51d4746cf6ccefdcfcbc841c92f70efaa338e34f"><code>51d4746</code></a> chore(devDeps): update 'ESLint' to v8 (<a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4926">#4926</a>)</li>
<li><a href="https://github.com/mochajs/mocha/commit/4e06a6fd00537bcdb1b6fd98b4684875356193f9"><code>4e06a6f</code></a> fix(browser): increase contrast for replay buttons (<a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4912">#4912</a>)</li>
<li><a href="https://github.com/mochajs/mocha/commit/41567df1fa039875a043b54b0d4e26153b802893"><code>41567df</code></a> Support prefers-color-scheme: dark (<a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4896">#4896</a>)</li>
<li><a href="https://github.com/mochajs/mocha/commit/61b4b9209c2c64b32c8d48b1761c3b9384d411ea"><code>61b4b92</code></a> fix the regular expression for function <code>clean</code> in <code>utils.js</code> (<a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4770">#4770</a>)</li>
<li><a href="https://github.com/mochajs/mocha/commit/77c18d29c565e68a0d487e357765acb5ec776cc6"><code>77c18d2</code></a> chore: use standard 'Promise.allSettled' instead of polyfill (<a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4905">#4905</a>)</li>
<li><a href="https://github.com/mochajs/mocha/commit/84b2f846148b180d6e1af088f77358a85c81d1ba"><code>84b2f84</code></a> chore(ci): upgrade GH actions to latest versions (<a href="https://github-redirect.dependabot.com/mochajs/mocha/issues/4899">#4899</a>)</li>
<li><a href="https://github.com/mochajs/mocha/commit/023f548213e571031b41cabbcb8bb20e458b2725"><code>023f548</code></a> build(v10.0.0): release</li>
<li><a href="https://github.com/mochajs/mocha/commit/62b1566211a631b22f4bd7d888cd2c046efdd9e4"><code>62b1566</code></a> build(v10.0.0): update CHANGELOG</li>
<li>Additional commits viewable in <a href="https://github.com/mochajs/mocha/compare/v8.4.0...v10.1.0">compare view</a></li>
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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-spec/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 03:13:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    chore(deps): bump glob-parent from 5.1.0 to 5.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [glob-parent](https://github.com/gulpjs/glob-parent) from 5.1.0 to 5.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gulpjs/glob-parent/releases">glob-parent's releases</a>.</em></p>
<blockquote>
<h2>v5.1.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>eliminate ReDoS (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/36">#36</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/f9231168b0041fea3f8f954b3cceb56269fc6366">f923116</a>)</li>
</ul>
<h2>v5.1.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>unescape exclamation mark (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/26">#26</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/a98874f1a59e407f4fb1beb0db4efa8392da60bb">a98874f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/gulpjs/glob-parent/blob/main/CHANGELOG.md">glob-parent's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/gulpjs/glob-parent/compare/v5.1.1...v5.1.2">5.1.2</a> (2021-03-06)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>eliminate ReDoS (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/36">#36</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/f9231168b0041fea3f8f954b3cceb56269fc6366">f923116</a>)</li>
</ul>
<h3><a href="https://www.github.com/gulpjs/glob-parent/compare/v6.0.1...v6.0.2">6.0.2</a> (2021-09-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Improve performance (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/53">#53</a>) (<a href="https://www.github.com/gulpjs/glob-parent/commit/843f8de1c177e9a5c06c4cfd2349ca5207168e00">843f8de</a>)</li>
</ul>
<h3><a href="https://www.github.com/gulpjs/glob-parent/compare/v6.0.0...v6.0.1">6.0.1</a> (2021-07-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Resolve ReDoS vulnerability from CVE-2021-35065 (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/49">#49</a>) (<a href="https://www.github.com/gulpjs/glob-parent/commit/3e9f04a3b4349db7e1962d87c9a7398cda51f339">3e9f04a</a>)</li>
</ul>
<h2><a href="https://www.github.com/gulpjs/glob-parent/compare/v5.1.2...v6.0.0">6.0.0</a> (2021-05-03)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>Correct mishandled escaped path separators (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/34">#34</a>)</li>
<li>upgrade scaffold, dropping node &lt;10 support</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Correct mishandled escaped path separators (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/34">#34</a>) (<a href="https://www.github.com/gulpjs/glob-parent/commit/32f6d52663b7addac38d0dff570d8127edf03f47">32f6d52</a>), closes <a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/32">#32</a></li>
</ul>
<h3>Miscellaneous Chores</h3>
<ul>
<li>upgrade scaffold, dropping node &lt;10 support (<a href="https://www.github.com/gulpjs/glob-parent/commit/e83d0c5a411947cf69eb58f36349db80439c606f">e83d0c5</a>)</li>
</ul>
<h3><a href="https://github.com/gulpjs/glob-parent/compare/v5.1.0...v5.1.1">5.1.1</a> (2021-01-27)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>unescape exclamation mark (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/26">#26</a>) (<a href="https://github.com/gulpjs/glob-parent/commit/a98874f1a59e407f4fb1beb0db4efa8392da60bb">a98874f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gulpjs/glob-parent/commit/eb2c439de448c779b450472e591a2bc9e37e9668"><code>eb2c439</code></a> chore: update changelog</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/12bcb6c45c942e2d05fc1e6ff5402e72555b54b6"><code>12bcb6c</code></a> chore: release 5.1.2</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/f9231168b0041fea3f8f954b3cceb56269fc6366"><code>f923116</code></a> fix: eliminate ReDoS (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/36">#36</a>)</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/0b014a7962789b2d8f2cf0b6311f40667aecd62c"><code>0b014a7</code></a> chore: add JSDoc returns information (<a href="https://github-redirect.dependabot.com/gulpjs/glob-parent/issues/33">#33</a>)</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/2b24ebd64b2a045aa167c825376335555da139fd"><code>2b24ebd</code></a> chore: generate initial changelog</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/9b6e8747ddf664c9b1a36fbd2a23e43a35b8a52f"><code>9b6e874</code></a> chore: release 5.1.1</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/749c35ee084498ebb1ce8cc9cf655f6aa4d623c5"><code>749c35e</code></a> ci: try wrapping the JOB_ID in a string</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/5d39def48c9e9eaee0ca36dafdf7b6cdcd875b85"><code>5d39def</code></a> ci: attempt to switch to published coveralls</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/0b5b37f674a7e207457c99cb2f123299e5ab31c9"><code>0b5b37f</code></a> ci: put the npm step back in for only Windows</li>
<li><a href="https://github.com/gulpjs/glob-parent/commit/473f5d87644bf19f32c53de21d2420f03aa02e5a"><code>473f5d8</code></a> ci: update azure build images</li>
<li>Additional commits viewable in <a href="https://github.com/gulpjs/glob-parent/compare/v5.1.0...v5.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=glob-parent&package-manager=npm_and_yarn&previous-version=5.1.0&new-version=5.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-spec/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 03:13:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Another try to enable katex -- minimum change
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Enabling katex in the specification
- Temp change to use awhitehead spec-up until a fix is in spec-up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 23:18:55 +0000 UTC
    </div>
</div>

