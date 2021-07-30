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
                PR <a href="https://github.com/hyperledger-labs/byzantine-config/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Bump grpc from 1.24.2 to 1.24.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [grpc](https://github.com/grpc/grpc-node) from 1.24.2 to 1.24.11.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases">grpc's releases</a>.</em></p>
<blockquote>
<h2>Node gRPC 1.24.11</h2>
<ul>
<li><strong>SECURITY FIX</strong>: Fix a double free bug in server-side TCP error handling code (grpc/grpc#26750 picked up in <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1861">#1861</a>). This bug was discovered by Brad Buckingham and Alex Skwarczynski.</li>
<li>Update the <code>ServiceDefinition</code> TypeScript type for compatibility with <code>@grpc/grpc-js</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1860">#1860</a>)</li>
</ul>
<h2>Node gRPC 1.24.10</h2>
<ul>
<li>Make callback function check properly handle async functions (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1786">#1786</a> contributed by <a href="https://github.com/amje"><code>@​amje</code></a>)</li>
</ul>
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
<li><a href="https://github.com/grpc/grpc-node/commit/39680a5084f4c0c0b98370a5d61edda65dbfe026"><code>39680a5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1861">#1861</a> from murgatroid99/grpc-native_submodule_bump</li>
<li><a href="https://github.com/grpc/grpc-node/commit/bb518305751e577ef05abfc11362ebd2cc5de3b2"><code>bb51830</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1860">#1860</a> from murgatroid99/grpc-native_ServiceDefinition_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/cd825350128c5aed2a97845160df1d91e6fc0f26"><code>cd82535</code></a> grpc-native: Update submodule and version</li>
<li><a href="https://github.com/grpc/grpc-node/commit/913734dd588eda89c71f06cadc4f7066477a273b"><code>913734d</code></a> grpc: Make ServiceDefinition type argument optional</li>
<li><a href="https://github.com/grpc/grpc-node/commit/465f7a15c9ea9b330596aaaceeb7b75297afd9ab"><code>465f7a1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1788">#1788</a> from murgatroid99/grpc-native_v1.24.10</li>
<li><a href="https://github.com/grpc/grpc-node/commit/870523f68027cca35fb0f37083bee14538c5ceea"><code>870523f</code></a> native: Bump version to 1.24.10</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d85324db64037920f0aee5244c6b2a8c52f083d2"><code>d85324d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1786">#1786</a> from amje/fix-function-check</li>
<li><a href="https://github.com/grpc/grpc-node/commit/b1c1f964015b633acf1a5b5e59673fb9ae25c04a"><code>b1c1f96</code></a> fix(grpc-native-core): incomplete function check</li>
<li><a href="https://github.com/grpc/grpc-node/commit/ccaceae014c948c7b28ad3401b5271ac0db00b54"><code>ccaceae</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1775">#1775</a> from murgatroid99/grpc-native_node-pre-gyp_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/52d44f55d923c6c6d6f20eaa4afa209516ed0f7d"><code>52d44f5</code></a> native: Fix reference to node-pre-gyp</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/grpc@1.24.2...grpc@1.24.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=grpc&package-manager=npm_and_yarn&previous-version=1.24.2&new-version=1.24.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-29 19:52:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/byzantine-config/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Bump ws from 5.2.2 to 5.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [ws](https://github.com/websockets/ws) from 5.2.2 to 5.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>5.2.3</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported 00c425ec to the 5.x release line (76d47c14).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/6dd88e7e968ef2416445d8f8620c17d99b15c77c"><code>6dd88e7</code></a> [dist] 5.2.3</li>
<li><a href="https://github.com/websockets/ws/commit/76d47c1479002022a3e4357b3c9f0e23a68d4cd2"><code>76d47c1</code></a> [security] Fix ReDoS vulnerability</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/5.2.2...5.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ws&package-manager=npm_and_yarn&previous-version=5.2.2&new-version=5.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-29 19:49:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/byzantine-config/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Bump color-string from 1.5.3 to 1.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [color-string](https://github.com/Qix-/color-string) from 1.5.3 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Qix-/color-string/releases">color-string's releases</a>.</em></p>
<blockquote>
<h2>1.6.0</h2>
<h1>Minor release 1.6.0</h1>
<ul>
<li><a href="https://github.com/Qix-/color-string/issues/55">#55</a> - Add support for space-separated HSL</li>
</ul>
<p>Thanks <a href="https://github.com/htunnicliff"><code>@​htunnicliff</code></a> for the contribution :)</p>
<h2>1.5.5 (Patch/Security Release) - hwb() ReDos patch (low-severity)</h2>
<blockquote>
<p>Release notes copied verbatim from the commit message, which can be found here: 0789e21284c33d89ebc4ab4ca6f759b9375ac9d3</p>
</blockquote>
<pre><code>Discovered by Yeting Li, c/o Colin Ife via Snyk.io.
<p>A ReDos (Regular Expression Denial of Service) vulnerability
was responsibly disclosed to me via email by Colin on
Mar 5 2021 regarding an exponential time complexity for
linearly increasing input lengths for <code>hwb()</code> color strings.</p>
<p>Strings reaching more than 5000 characters would see several
milliseconds of processing time; strings reaching more than
50,000 characters began seeing 1500ms (1.5s) of processing time.</p>
<p>The cause was due to a the regular expression that parses
hwb() strings - specifically, the hue value - where
the integer portion of the hue value used a 0-or-more quantifier
shortly thereafter followed by a 1-or-more quantifier.</p>
<p>This caused excessive backtracking and a cartesian scan,
resulting in exponential time complexity given a linear
increase in input length.</p>
<p>Thank you Yeting Li and Colin Ife for bringing this to my
attention in a secure, responsible and professional manner.</p>
<p>A CVE will not be assigned for this vulnerability.
</code></pre></p>
<h2>1.5.4 (Patch Release)</h2>
<ul>
<li>Removes rounding of alpha values in RGBA hex (<code>#rrggbbaa</code>) and condensed-hex (<code>#rgba</code>) parsers, which caused certain unique inputs to result in identical outputs (see <a href="https://github.com/qix-/color/issues/174">https://github.com/qix-/color/issues/174</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/Qix-/color-string/commits/1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=color-string&package-manager=npm_and_yarn&previous-version=1.5.3&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-29 19:49:00 +0000 UTC
    </div>
</div>

