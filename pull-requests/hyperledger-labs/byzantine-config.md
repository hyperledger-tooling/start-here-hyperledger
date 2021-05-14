---
layout: default
title: byzantine-config
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/byzantine-config
---

# byzantine-config <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/byzantine-config){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/byzantine-config/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Bump grpc from 1.24.2 to 1.24.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [grpc](https://github.com/grpc/grpc-node) from 1.24.2 to 1.24.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases">grpc's releases</a>.</em></p>
<blockquote>
<h2>Node gRPC v1.24.7</h2>
<ul>
<li>Log just serialization and deserialization errors on the server, instead of logging all errors with the code <code>INTERNAL</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1750">#1750</a>)</li>
<li>Replace the <code>instanceof Function</code> check to make it work properly in certain environments (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1759">#1759</a> contributed by <a href="https://github.com/zereraz"><code>@​zereraz</code></a>)</li>
</ul>
<h2>Node gRPC v1.24.6</h2>
<ul>
<li>Fix prototype pollution possibility in loadPackageDefinition (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1701">#1701</a>)</li>
</ul>
<h2>Node gRPC v1.24.5</h2>
<ul>
<li>Add support for Electron 11 and newer versions of Electron 10 (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1684">#1684</a>)</li>
</ul>
<h2>Node gRPC v1.24.4</h2>
<ul>
<li>Add support for Electron 10 and newer minor versions of Electron 8 and 9 (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1615">#1615</a>)</li>
<li>Add a note in the README stating the latest supported versions of Node and Electron (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1615">#1615</a>)</li>
<li>Prevent prototype pollution in <code>loadPackageDefinition</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1606">#1606</a>)</li>
<li>Add <code>ResponseType</code> to <code>ServerWritableStream</code> type definition for compatibility with <code>@grpc/grpc-js</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1590">#1590</a> contributed by <a href="https://github.com/badsyntax"><code>@​badsyntax</code></a>)</li>
<li>Add <code>methodTypes</code> enum to type definition (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1496">#1496</a> contributed by <a href="https://github.com/jncr"><code>@​jncr</code></a>)</li>
</ul>
<h2>grpc 1.24.3</h2>
<ul>
<li>Add support for S390x (originally <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1230">#1230</a> contributed by <a href="https://github.com/shahidhs-ibm"><code>@​shahidhs-ibm</code></a>)</li>
<li>Add support for Node 14, and Electron 7, 8, and 9</li>
<li>Unbundle the dependency on <code>node-pre-gyp</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1371">#1371</a> contributed by <a href="https://github.com/Naktibalda"><code>@​Naktibalda</code></a>)</li>
</ul>
<p><strong>Known Issues</strong>:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1407">#1407</a> may cause errors when running on Node 14</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/grpc/grpc-node/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=grpc&package-manager=npm_and_yarn&previous-version=1.24.2&new-version=1.24.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/byzantine-config/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 00:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/byzantine-config/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Bump hosted-git-info from 2.8.5 to 2.8.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [hosted-git-info](https://github.com/npm/hosted-git-info) from 2.8.5 to 2.8.9.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/hosted-git-info/blob/v2.8.9/CHANGELOG.md">hosted-git-info's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/hosted-git-info/compare/v2.8.8...v2.8.9">2.8.9</a> (2021-04-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>backport regex fix from <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/76">#76</a> (<a href="https://github.com/npm/hosted-git-info/commit/29adfe5">29adfe5</a>), closes <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/84">#84</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2><a href="https://github.com/npm/hosted-git-info/compare/v2.8.7...v2.8.8">2.8.8</a> (2020-02-29)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/61">#61</a> &amp; <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/65">#65</a> addressing issues w/ url.URL implmentation which regressed node 6 support (<a href="https://github.com/npm/hosted-git-info/commit/5038b18">5038b18</a>), closes <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/66">#66</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2><a href="https://github.com/npm/hosted-git-info/compare/v2.8.6...v2.8.7">2.8.7</a> (2020-02-26)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Do not attempt to use url.URL when unavailable (<a href="https://github.com/npm/hosted-git-info/commit/2d0bb66">2d0bb66</a>), closes <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/61">#61</a> <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/62">#62</a></li>
<li>Do not pass scp-style URLs to the WhatWG url.URL (<a href="https://github.com/npm/hosted-git-info/commit/f2cdfcf">f2cdfcf</a>), closes <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/60">#60</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2><a href="https://github.com/npm/hosted-git-info/compare/v2.8.5...v2.8.6">2.8.6</a> (2020-02-25)</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/hosted-git-info/commit/8d4b3697d79bcd89cdb36d1db165e3696c783a01"><code>8d4b369</code></a> chore(release): 2.8.9</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/29adfe5ef789784c861b2cdeb15051ec2ba651a7"><code>29adfe5</code></a> fix: backport regex fix from <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/76">#76</a></li>
<li><a href="https://github.com/npm/hosted-git-info/commit/afeaefdd86ba9bb5044be3c1554a666d007cf19a"><code>afeaefd</code></a> chore(release): 2.8.8</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/5038b1891a61ca3cd7453acbf85d7011fe0086bb"><code>5038b18</code></a> fix: <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/61">#61</a> &amp; <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/65">#65</a> addressing issues w/ url.URL implmentation which regressed nod...</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/7440afa859162051c191e55d8ecfaf69a193b026"><code>7440afa</code></a> chore(release): 2.8.7</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/2d0bb6615ecb8f9ef1019bc0737aab7f6449641f"><code>2d0bb66</code></a> fix: Do not attempt to use url.URL when unavailable</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/f2cdfcf33ad2bd3bd1acdba0326281089f53c5b1"><code>f2cdfcf</code></a> fix: Do not pass scp-style URLs to the WhatWG url.URL</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/e1b83df5d9cb1f8bb220352e20565560548d2292"><code>e1b83df</code></a> chore(release): 2.8.6</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/ff259a6117c62df488e927820e30bec2f7ee453f"><code>ff259a6</code></a> Ensure passwords in hosted Git URLs are correctly escaped</li>
<li>See full diff in <a href="https://github.com/npm/hosted-git-info/compare/v2.8.5...v2.8.9">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~nlf">nlf</a>, a new releaser for hosted-git-info since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hosted-git-info&package-manager=npm_and_yarn&previous-version=2.8.5&new-version=2.8.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/byzantine-config/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 08:12:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/byzantine-config/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Bump url-parse from 1.4.7 to 1.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [url-parse](https://github.com/unshiftio/url-parse) from 1.4.7 to 1.5.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/unshiftio/url-parse/commit/eb6d9f51e395b7e47bf2594e457d541db21c713b"><code>eb6d9f5</code></a> [dist] 1.5.1</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/750d8e8a9d45dbce9ff09759f0fe4564cdd47d74"><code>750d8e8</code></a> [fix] Fixes relative path resolving <a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/199">#199</a> <a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/200">#200</a> (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/201">#201</a>)</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/3ac777474ba5dc48a7e33771cbb311fc6f69bef8"><code>3ac7774</code></a> [test] Make test consistent for browser testing</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/267a0c6f7ef1a58271be61611c5103daace602c9"><code>267a0c6</code></a> [dist] 1.5.0</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d1e7e8822f26e8a49794b757123b51386325b2b0"><code>d1e7e88</code></a> [security] More backslash fixes (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/197">#197</a>)</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d99bf4cf259b7378c855f786edc253e70405ffdc"><code>d99bf4c</code></a> [ignore] Remove npm-debug.log from .gitignore</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/422c8b5e4cac6a79cd35b4e86731476dcbeec7e4"><code>422c8b5</code></a> [pkg] Replace nyc with c8</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/933809d630c7b21399b4e5df59fccccd80033b21"><code>933809d</code></a> [pkg] Move coveralls to dev dependencies</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/190b2168035899a2a88f2dc2625963bf7e2f338f"><code>190b216</code></a> [pkg] Add .npmrc</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ce3783f4ea25753cfa36376769c14e4e2fe6ea80"><code>ce3783f</code></a> [test] Do not test on all available versions of Edge and Safari</li>
<li>Additional commits viewable in <a href="https://github.com/unshiftio/url-parse/compare/1.4.7...1.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url-parse&package-manager=npm_and_yarn&previous-version=1.4.7&new-version=1.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/byzantine-config/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 14:20:58 +0000 UTC
    </div>
</div>

