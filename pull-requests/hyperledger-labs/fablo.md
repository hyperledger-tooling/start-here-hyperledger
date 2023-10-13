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
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Issue 340: connection-profile stuff
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
        Created At 2023-10-13 12:56:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Bump debug from 3.2.6 to 4.3.2 in /samples/chaincodes/chaincode-kv-node-1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [debug](https://github.com/debug-js/debug) from 3.2.6 to 4.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/debug-js/debug/releases">debug's releases</a>.</em></p>
<blockquote>
<h2>4.3.2</h2>
<h1>Patch release 4.3.2</h1>
<ul>
<li>Caches enabled statuses on a per-logger basis to speed up <code>.enabled</code> checks (<a href="https://redirect.github.com/debug-js/debug/issues/799">#799</a>)</li>
</ul>
<p>Thank you <a href="https://github.com/omg"><code>@​omg</code></a>!</p>
<h2>4.3.1</h2>
<h1>Patch release 4.3.1</h1>
<ul>
<li>Fixes a ReDOS regression (<a href="https://redirect.github.com/debug-js/debug/issues/458">#458</a>) - see <a href="https://redirect.github.com/debug-js/debug/issues/797">#797</a> for details.</li>
</ul>
<h2>4.3.0</h2>
<h1>Minor release</h1>
<ul>
<li><strong>Deprecated <code>debugInstance.destroy()</code></strong>. Future major versions will not have this method; please remove it from your codebases as it currently does nothing.</li>
<li>Fixed quoted percent sign</li>
<li>Fixed memory leak within debug instances that are created dynamically</li>
</ul>
<h2>4.2.0</h2>
<h1>Minor Release</h1>
<ul>
<li>Replaced phantomJS with chrome backend for browser tests</li>
<li>Deprecated and later removed Changelog.md in lieu of releases page</li>
<li>Removed bower.json (<a href="https://redirect.github.com/debug-js/debug/issues/602">#602</a>)</li>
<li>Removed .eslintrc (since we've switched to XO)</li>
<li>Removed .coveralls.yml</li>
<li>Removed the build system that was in place for various alternate package managers</li>
<li>Removed the examples folder (<a href="https://redirect.github.com/debug-js/debug/issues/650">#650</a>)</li>
<li>Switched to <code>console.debug</code> <strong>in the browser only</strong> when it is available (<a href="https://redirect.github.com/debug-js/debug/issues/600">#600</a>)</li>
<li>Copied custom logger to namespace extension (<a href="https://redirect.github.com/debug-js/debug/issues/646">#646</a>)</li>
<li>Added issue and pull request templates</li>
<li>Added <code>&quot;engines&quot;</code> key to package.json</li>
<li>Added ability to control <code>selectColor</code> (<a href="https://redirect.github.com/debug-js/debug/issues/747">#747</a>)</li>
<li>Updated dependencies</li>
<li>Marked <code>supports-color</code> as an optional peer dependency</li>
</ul>
<h2>4.1.1</h2>
<p>This  backport fixes a bug in coveralls configuration as well as the <code>.extend()</code> function.</p>
<h1>Patches</h1>
<ul>
<li>test: only run coveralls on travis (<a href="https://redirect.github.com/debug-js/debug/issues/663">#663</a>, <a href="https://redirect.github.com/debug-js/debug/issues/664">#664</a>, d0e498f159bd425b3403db38c98fe26a345d4dcd)</li>
<li>copy custom logger to namespace extension (<a href="https://redirect.github.com/debug-js/debug/issues/646">#646</a>, 57ef085703a0158679cc4a56a4980653b828ce51)</li>
</ul>
<h2>4.1.0</h2>
<h1>Minor Changes</h1>
<ul>
<li>migrate Makefile to npm scripts (4236585a40787fe60ed625452163299600df2ce6)</li>
<li>feat: Return namespaces string when invoking disable() (7ef8b417a86941372074f749019b9f439a1f6ef6)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/debug-js/debug/commit/e47f96de3de5921584364b4ac91e2769d22a3b1f"><code>e47f96d</code></a> 4.3.2</li>
<li><a href="https://github.com/debug-js/debug/commit/1e9d38c2e6e170abde6cfeaf7b2024d8b456f906"><code>1e9d38c</code></a> cache enabled status per-logger (<a href="https://redirect.github.com/debug-js/debug/issues/799">#799</a>)</li>
<li><a href="https://github.com/debug-js/debug/commit/0d3d66b0eb47c5d34e1a940e8a204446fdd832cd"><code>0d3d66b</code></a> 4.3.1</li>
<li><a href="https://github.com/debug-js/debug/commit/b6d12fdbc63b483e5c969da33ea6adc09946b5ac"><code>b6d12fd</code></a> fix regression</li>
<li><a href="https://github.com/debug-js/debug/commit/3f56313c1e4a0d59c1054fb9b10026b6903bfba7"><code>3f56313</code></a> 4.3.0</li>
<li><a href="https://github.com/debug-js/debug/commit/e2d3bc9e428bdd45adb8d6e7f8ab543bee54d9a6"><code>e2d3bc9</code></a> add deprecation notice for debug.destroy()</li>
<li><a href="https://github.com/debug-js/debug/commit/72e7f864bd75fc8353e4dd450de96d9104ba9f35"><code>72e7f86</code></a> fix memory leak within debug instance</li>
<li><a href="https://github.com/debug-js/debug/commit/27152cad248df54217a14c072e7be1cd16da5f6d"><code>27152ca</code></a> add test for enable/disable of existing instances</li>
<li><a href="https://github.com/debug-js/debug/commit/22e13fe07e21f32888201aa40833599fd10a4fbb"><code>22e13fe</code></a> fix quoted percent sign</li>
<li><a href="https://github.com/debug-js/debug/commit/80ef62a3af4df95250d77d64edfc3d0e1667e7e8"><code>80ef62a</code></a> 4.2.0</li>
<li>Additional commits viewable in <a href="https://github.com/debug-js/debug/compare/3.2.6...4.3.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~qix">qix</a>, a new releaser for debug since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=debug&package-manager=npm_and_yarn&previous-version=3.2.6&new-version=4.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 12:48:17 +0000 UTC
    </div>
</div>

