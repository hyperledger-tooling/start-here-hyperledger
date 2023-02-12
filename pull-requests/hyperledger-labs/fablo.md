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
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Bump cacheable-request and got
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [cacheable-request](https://github.com/jaredwray/cacheable-request) to 10.2.7 and updates ancestor dependency [got](https://github.com/sindresorhus/got). These dependencies need to be updated together.

Updates `cacheable-request` from 7.0.2 to 10.2.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jaredwray/cacheable-request/releases">cacheable-request's releases</a>.</em></p>
<blockquote>
<h2>v10.2.6</h2>
<h1>Fix for memory leak on Listeners</h1>
<p>The listener was not being removed on <code>response</code> and just error but new handlers were being added causing a memory leak.</p>
<p><a href="https://github.com/jaredwray/cacheable-request/blob/c4815689be40854a3d748a3927959354c09b0ebb/src/index.ts#L220-L225">line 220 in src/index.ts was modified to remove the listener on response also </a></p>
<pre><code>			if (this.cache instanceof Keyv) {
				const cachek = this.cache;
				cachek.once('error', errorHandler);
				ee.on('error', () =&gt; cachek.removeListener('error', errorHandler));
				ee.on('response', () =&gt; cachek.removeListener('error', errorHandler));
			}
</code></pre>
<h2>What's Changed</h2>
<ul>
<li>upgrading jest and components to latest by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/220">jaredwray/cacheable-request#220</a></li>
<li>upgrading <code>@​types/jest</code> to 29.2.6 by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/221">jaredwray/cacheable-request#221</a></li>
<li>fixing listener memory leak - issue <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/issues/222">#222</a> by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/223">jaredwray/cacheable-request#223</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jaredwray/cacheable-request/compare/v10.2.5...v10.2.6">https://github.com/jaredwray/cacheable-request/compare/v10.2.5...v10.2.6</a></p>
<h2>v10.2.5</h2>
<p>Types definition issue with http-cache-sematics as that type definition needs to be in dependencies. Thanks <a href="https://github.com/Maxim-Mazurok"><code>@​Maxim-Mazurok</code></a></p>
<h2>What's Changed</h2>
<ul>
<li>Move <code>@​types/http-cache-semantics</code> from dev to deps by <a href="https://github.com/Maxim-Mazurok"><code>@​Maxim-Mazurok</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/219">jaredwray/cacheable-request#219</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jaredwray/cacheable-request/compare/v10.2.4...v10.2.5">https://github.com/jaredwray/cacheable-request/compare/v10.2.4...v10.2.5</a></p>
<h1>v10.2.4</h1>
<p>Minor updates with one exception is that we removed <code>@types/http-cache-semantics</code> from the main dependencies as it does not look to be needed.</p>
<h2>What's Changed</h2>
<ul>
<li>upgrading typescript to 4.9.4 by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/214">jaredwray/cacheable-request#214</a></li>
<li>upgrading jest types and eslint for jest to latest by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/215">jaredwray/cacheable-request#215</a></li>
<li>upgrading sqlite3 to 5.1.4 by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/216">jaredwray/cacheable-request#216</a></li>
<li>removing <code>@​types/http-cache-semantics</code> from the dependencies and moving… by <a href="https://github.com/jaredwray"><code>@​jaredwray</code></a> in <a href="https://github-redirect.dependabot.com/jaredwray/cacheable-request/pull/217">jaredwray/cacheable-request#217</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jaredwray/cacheable-request/compare/v10.2.3...v10.2.4">https://github.com/jaredwray/cacheable-request/compare/v10.2.3...v10.2.4</a></p>
<h1>v10.2.3 Maintenance Release</h1>
<p>Upgrading core modules in the system such as keyv and also a minor fix to an uncaught exception that we were seeing referenced here: <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1925">sindresorhus/got#1925</a></p>
<p>Additional update is moving <code>normalize-url</code> to <code>8.0.0</code> which after testing it looks to not affect anything but will post the release notes here: <a href="https://github.com/sindresorhus/normalize-url/releases/tag/v8.0.0">https://github.com/sindresorhus/normalize-url/releases/tag/v8.0.0</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/jaredwray/cacheable-request/commits">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jaredwray">jaredwray</a>, a new releaser for cacheable-request since your current version.</p>
</details>
<br />

Updates `got` from 11.8.5 to 12.5.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v12.5.3</h2>
<ul>
<li>Fix abort event listeners not always being cleaned up (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2162">#2162</a>)  3cc40b5</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.2...v12.5.3">https://github.com/sindresorhus/got/compare/v12.5.2...v12.5.3</a></p>
<h2>v12.5.2</h2>
<ul>
<li>Improve TypeScript 4.9 compatibility (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2163">#2163</a>)  39f83b6</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.1...v12.5.2">https://github.com/sindresorhus/got/compare/v12.5.1...v12.5.2</a></p>
<h2>v12.5.1</h2>
<ul>
<li>Fix compatibility with TypeScript and ESM  3b3ea67</li>
<li>Fix request body not being properly cached (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2150">#2150</a>)  3e9d3af</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.0...v12.5.1">https://github.com/sindresorhus/got/compare/v12.5.0...v12.5.1</a></p>
<h2>v12.5.0</h2>
<ul>
<li>Disable method rewriting on 307 and 308 status codes (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2145">#2145</a>)  e049e94</li>
<li>Upgrade dependencies  8630815 f0ac0b3 4c3762a</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.4.1...v12.5.0">https://github.com/sindresorhus/got/compare/v12.4.1...v12.5.0</a></p>
<h2>v12.4.1</h2>
<h3>Fixes</h3>
<ul>
<li>Fix <code>options.context</code> being not extensible b671480715dbbff908e9a385f5e714570c663cd7</li>
<li>Don't emit <code>uploadProgress</code> after promise cancelation 693de217b030816f574d6e4cb505ee2e77b21c29</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.4.0...v12.4.1">https://github.com/sindresorhus/got/compare/v12.4.0...v12.4.1</a></p>
<h2>v12.4.0</h2>
<h3>Improvements</h3>
<ul>
<li>Support FormData without known length (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2120">#2120</a>)  850773c</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Don&amp;<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/39">#39</a>;t call <code>beforeError</code> hooks with <code>HTTPError</code> if the <code>throwHttpErrors</code> option is <code>false</code> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2104">#2104</a>)  3927348</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.3.1...v12.4.0">https://github.com/sindresorhus/got/compare/v12.3.1...v12.4.0</a></p>
<h2>v12.3.1</h2>
<ul>
<li>Don&amp;<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/39">#39</a>;t freeze signal when freezing Options (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2100">#2100</a>)  43b1467</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.3.0...v12.3.1">https://github.com/sindresorhus/got/compare/v12.3.0...v12.3.1</a></p>
<h2>v12.3.0</h2>
<ul>
<li>Add <code>.off()</code> method for events (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2092">#2092</a>)  88056be</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.2.0...v12.3.0">https://github.com/sindresorhus/got/compare/v12.2.0...v12.3.0</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/2a4b4e7b272dba6abb36cb9ed63fbc24d3ebacf6"><code>2a4b4e7</code></a> 12.5.3</li>
<li><a href="https://github.com/sindresorhus/got/commit/3cc40b549c4af3617e8f6793d07533f7d4123f90"><code>3cc40b5</code></a> Fix abort event listeners not always being cleaned up (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2162">#2162</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/5f278d74125608b7abe75941cb6a71e21e0fb892"><code>5f278d7</code></a> 12.5.2</li>
<li><a href="https://github.com/sindresorhus/got/commit/39f83b6dad77acf9814df6d482a1a0b76732b0a4"><code>39f83b6</code></a> Improve TypeScript 4.9 compatibility (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2163">#2163</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/623229fad64b89a58c68c9f47fc36a4883cc994a"><code>623229f</code></a> Simplify <code>CookieJar</code> docs (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2155">#2155</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/07afa3c4807ca83be909995c4347cf1029439ece"><code>07afa3c</code></a> Make GitHub Actions workflow more secure (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2154">#2154</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/a4482a54eb67bce79552f9f1ea0a3dcef7585991"><code>a4482a5</code></a> 12.5.1</li>
<li><a href="https://github.com/sindresorhus/got/commit/3b3ea6776b4f15d69d1b4dde87f32173a3a6fdb2"><code>3b3ea67</code></a> Fix compatibility with TypeScript and ESM</li>
<li><a href="https://github.com/sindresorhus/got/commit/3e9d3af606c38f60e6225f8e009aacd6962fef71"><code>3e9d3af</code></a> Fix request body not being properly cached (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2150">#2150</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/6c7ebab3674fbf8a21275cfe9e06f71740219c05"><code>6c7ebab</code></a> Minor tweaks for ESM strict mode</li>
<li>Additional commits viewable in <a href="https://github.com/sindresorhus/got/compare/v11.8.5...v12.5.3">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 14:28:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/376" class=".btn">#376</a>
            </td>
            <td>
                <b>
                    Bump cacheable-request and nodemon in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [cacheable-request](https://github.com/jaredwray/cacheable-request). It's no longer used after updating ancestor dependency [nodemon](https://github.com/remy/nodemon). These dependencies need to be updated together.

Removes `cacheable-request`

Updates `nodemon` from 2.0.18 to 2.0.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remy/nodemon/releases">nodemon's releases</a>.</em></p>
<blockquote>
<h2>v2.0.20</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.19...v2.0.20">2.0.20</a> (2022-09-16)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove postinstall script (<a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0">e099e91</a>)</li>
</ul>
<h2>v2.0.19</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.19">2.0.19</a> (2022-07-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Replace update notifier with simplified deps (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2033">#2033</a>) (<a href="https://github.com/remy/nodemon/commit/176c4a6bed989fe94f103c905e5eee341d26794d">176c4a6</a>), closes <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1961">#1961</a> <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2028">#2028</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0"><code>e099e91</code></a> fix: remove postinstall script</li>
<li><a href="https://github.com/remy/nodemon/commit/05de353d4de1a7e1f2aa2c9bf641c3fe2d652122"><code>05de353</code></a> chore: supports</li>
<li><a href="https://github.com/remy/nodemon/commit/876d60c8a241f13376f1b32f853d48ae77ec69a4"><code>876d60c</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/188f2d3cdc960fce5d7413e1326da76bd5be780c"><code>188f2d3</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/a1ad44a876df74be742c64af5640b300c302b977"><code>a1ad44a</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/8abd3fc9daff813199042c26a1e8aa5691a5ab37"><code>8abd3fc</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/30c80f8a4eee379fa2ebad95b81c42ef11670829"><code>30c80f8</code></a> chore: add unused files to .npmignore (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2055">#2055</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/3dd38deb4a97a52608aac148200b48d844df0a66"><code>3dd38de</code></a> docs: added link on banner (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1944">#1944</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/fb51359dde4b4ad6081f6c2690d1052fc8f5fcaf"><code>fb51359</code></a> docs: add important note about ignore rules</li>
<li><a href="https://github.com/remy/nodemon/commit/8fe7d770d06305e5e7a4aa4ab4783d4b2c5eaac8"><code>8fe7d77</code></a> chore: supporters</li>
<li>Additional commits viewable in <a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.20">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 06:07:31 +0000 UTC
    </div>
</div>

