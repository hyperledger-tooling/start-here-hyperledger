---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/319" class=".btn">#319</a>
            </td>
            <td>
                <b>
                    Package version upgrades and RFC updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated proto and dependent packages to `1.5.1`. Fixed several RFC pages.

Signed-off-by: VRamakrishna <vramakr2@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 15:30:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Bump got and ava in /common/policy-dsl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [got](https://github.com/sindresorhus/got). It's no longer used after updating ancestor dependency [ava](https://github.com/avajs/ava). These dependencies need to be updated together.

Removes `got`

Updates `ava` from 3.15.0 to 4.3.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/avajs/ava/releases">ava's releases</a>.</em></p>
<blockquote>
<h2>v4.3.3</h2>
<p>Add compatibility with Node.js 18.8, thanks <a href="https://github.com/Brooooooklyn"><code>@​Brooooooklyn</code></a> <a href="https://github-redirect.dependabot.com/avajs/ava/issues/3091">#3091</a>.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/avajs/ava/compare/v4.3.1...v4.3.3">https://github.com/avajs/ava/compare/v4.3.1...v4.3.3</a></p>
<h2>v4.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>When translating line numbers, check whether the source map entry has original values in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3061">avajs/ava#3061</a></li>
<li>Report error when parsing for line number selection in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3062">avajs/ava#3062</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ericcornelissen"><code>@​ericcornelissen</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3048">avajs/ava#3048</a></li>
<li><a href="https://github.com/AlencarGabriel"><code>@​AlencarGabriel</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3051">avajs/ava#3051</a></li>
<li><a href="https://github.com/binyamin"><code>@​binyamin</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3028">avajs/ava#3028</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/avajs/ava/compare/v4.3.0...v4.3.1">https://github.com/avajs/ava/compare/v4.3.0...v4.3.1</a></p>
<h2>v4.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>We're now shipping type definitions compatible with TypeScript 4.7, by <a href="https://github.com/RebeccaStevens"><code>@​RebeccaStevens</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3024">avajs/ava#3024</a></li>
<li><code>throws</code> and <code>throwsAsync</code> assertions now take a function to test error messages, by <a href="https://github.com/il3ven"><code>@​il3ven</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/2995">avajs/ava#2995</a></li>
<li>Test failure summaries no longer duplicate <code>t.log()</code> messages, by <a href="https://github.com/il3ven"><code>@​il3ven</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3013">avajs/ava#3013</a></li>
<li>The number of timed-out tests is printed at the end of a run, by <a href="https://github.com/il3ven"><code>@​il3ven</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3021">avajs/ava#3021</a></li>
<li>We've documented how to load multiple instances of the same &quot;shared&quot; worker, by <a href="https://github.com/codetheweb"><code>@​codetheweb</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3009">avajs/ava#3009</a></li>
<li>Links to translated documentation have been updated, by <a href="https://github.com/forresst"><code>@​forresst</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3037">avajs/ava#3037</a></li>
<li>Node.js 17 has been removed from the test matrix, and Node.js 18 added in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3039">avajs/ava#3039</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/avajs/ava/compare/v4.2.0...v4.3.0">https://github.com/avajs/ava/compare/v4.2.0...v4.3.0</a></p>
<h2>v4.2.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update Babel recipe for AVA 4 by <a href="https://github.com/il3ven"><code>@​il3ven</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3000">avajs/ava#3000</a></li>
<li>Document how GitHub Actions can be configured for parallel builds by <a href="https://github.com/codetheweb"><code>@​codetheweb</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3007">avajs/ava#3007</a></li>
<li>Allow parallel builds to be disabled by <a href="https://github.com/il3ven"><code>@​il3ven</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3001">avajs/ava#3001</a></li>
<li>Improve typing of teardown methods by <a href="https://github.com/novemberborn"><code>@​novemberborn</code></a> in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3003">avajs/ava#3003</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mefengl"><code>@​mefengl</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/2999">avajs/ava#2999</a></li>
<li><a href="https://github.com/il3ven"><code>@​il3ven</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3000">avajs/ava#3000</a></li>
<li><a href="https://github.com/codetheweb"><code>@​codetheweb</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/avajs/ava/pull/3007">avajs/ava#3007</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/avajs/ava/compare/v4.1.0...v4.2.0">https://github.com/avajs/ava/compare/v4.1.0...v4.2.0</a></p>
<h2>v4.1.0</h2>
<h2>New features</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/avajs/ava/commit/a1347a58f3b9ab4faf595b86e65790e6b6ec127b"><code>a1347a5</code></a> 4.3.3</li>
<li><a href="https://github.com/avajs/ava/commit/6b78f4938ed04e5e3012eb28d8cbecdf10bbc293"><code>6b78f49</code></a> Handle <code>null</code> source maps during line number selection</li>
<li><a href="https://github.com/avajs/ava/commit/c37ea84449d504735637592e4335fb7909ebb6e4"><code>c37ea84</code></a> Test with AVA 4.3.2</li>
<li><a href="https://github.com/avajs/ava/commit/6d93de52854df88d8ab82ec574b313017f2c8bf2"><code>6d93de5</code></a> 4.3.2</li>
<li><a href="https://github.com/avajs/ava/commit/e81f5bdf7a176180d50755853ebcc6d1b6293025"><code>e81f5bd</code></a> Handle findSourceMap returning null since Node.js 18.8.0</li>
<li><a href="https://github.com/avajs/ava/commit/53e570998bcbee584701c271aa7478825895c35b"><code>53e5709</code></a> 4.3.1</li>
<li><a href="https://github.com/avajs/ava/commit/d57c76c47687e61c38e059ea6442d92b4a9404fa"><code>d57c76c</code></a> Report error when parsing for line number selection</li>
<li><a href="https://github.com/avajs/ava/commit/357234260afc49646cddc2e9253f2740dd25d8e6"><code>3572342</code></a> When translating line numbers, check whether the source map entry has origina...</li>
<li><a href="https://github.com/avajs/ava/commit/ac0d75d05d28e511b1b3654b09d11d602e360179"><code>ac0d75d</code></a> Document that AVA 4 cannot be run globally</li>
<li><a href="https://github.com/avajs/ava/commit/26a2e5d56a21e014edba382191d6c0a16444d880"><code>26a2e5d</code></a> Remove mentions of &quot;callback mode&quot; from docs</li>
<li>Additional commits viewable in <a href="https://github.com/avajs/ava/compare/v3.15.0...v4.3.3">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 07:17:03 +0000 UTC
    </div>
</div>

