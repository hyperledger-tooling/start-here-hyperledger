---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    fix: now decrypt work properly for rotated keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Fix tinkcrypto.Decrypt to work properly for rotated keys.

**Summary:**

Iterate through all key prefixes in the keyset to try to decrypt data.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 11:00:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3031" class=".btn">#3031</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.61.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.61.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.61.0</h2>
<h1>Bugfixes</h1>
<ul>
<li>use a wasm md4 implementation for node 17 support</li>
<li>include the <code>path</code> submodules in the node.js default externals</li>
</ul>
<h1>Performance</h1>
<ul>
<li>improve string to binary conversion performance for hashing</li>
</ul>
<h1>Contribution</h1>
<ul>
<li>CI runs on node.js 17</li>
</ul>
<h2>v5.60.0</h2>
<h1>Features</h1>
<ul>
<li>Allow to pass more options to <code>experiments.lazyCompilation</code>. e. g. port, https stuff</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>output.hashFunction</code> used to persistent caching too</li>
<li>Initialize <code>buildDependencies</code> Set correctly when loaders are added in <code>beforeLoaders</code> hook</li>
</ul>
<h2>v5.59.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix regexp in managedPaths</li>
<li>fix hanging when trying to write lockfile for <code>experiments.buildHttp</code></li>
</ul>
<h2>v5.59.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>/*#__PURE__*/</code> for <code>Object()</code> in generated code</li>
<li>add RegExp and function support for <code>managed/immutablePaths</code></li>
<li>add hooks for multiple phases in module build</li>
<li>improvements to <code>experiments.buildHttp</code>
<ul>
<li>allow to share cache</li>
<li>add allowlist</li>
</ul>
</li>
<li>add <code>splitChunks.minSizeReduction</code> option</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix memory caching for Data URLs</li>
<li>fix crash in <code>waitFor</code> when modules are unsafe cached</li>
<li>fix bug in build cycle detection</li>
</ul>
<h2>v5.58.2</h2>
<h1>Bugfixes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/0306510f7d1b9b13900f1dcf78a767c2ed390a61"><code>0306510</code></a> 5.61.0</li>
<li><a href="https://github.com/webpack/webpack/commit/42b4ffb01aa91abc48db16603976cae2009adb58"><code>42b4ffb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14594">#14594</a> from webpack/ci/node-17</li>
<li><a href="https://github.com/webpack/webpack/commit/c2b6f7866e33c63288261c012b05e00aa6bacca2"><code>c2b6f78</code></a> fix test cases for node 17</li>
<li><a href="https://github.com/webpack/webpack/commit/1d7f6da4162f23995c8a5baf88ba9f5f73b33c76"><code>1d7f6da</code></a> run CI on node 17</li>
<li><a href="https://github.com/webpack/webpack/commit/1992e9ce2b739ec2864856f29a7cdf6134ab0de7"><code>1992e9c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14583">#14583</a> from juanrgm/fix/path-submodules-14582</li>
<li><a href="https://github.com/webpack/webpack/commit/0f6c78cca174a73184fdc0d9c9c2bd376b48557c"><code>0f6c78c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14584">#14584</a> from webpack/hash/md4</li>
<li><a href="https://github.com/webpack/webpack/commit/a6bb3e58ecba1d0468d65364ba629d5a04805d14"><code>a6bb3e5</code></a> default to the default hash function</li>
<li><a href="https://github.com/webpack/webpack/commit/205d3a05ee2a1cce4a4b8d7c270beaee784cfe78"><code>205d3a0</code></a> add support for additional digest types</li>
<li><a href="https://github.com/webpack/webpack/commit/d806cf5294a010f5c3280a38ab7500c681ca7c11"><code>d806cf5</code></a> use correct batch size for BatchedHash</li>
<li><a href="https://github.com/webpack/webpack/commit/7afc8330921f2c112d015e462910950c55aa9863"><code>7afc833</code></a> improve micro benchmarks</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.61.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.61.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 08:16:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3026" class=".btn">#3026</a>
            </td>
            <td>
                <b>
                    fix: wallet present proof fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixed issue where wallet is only relying parent thread id of present
proof V2

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 15:50:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3024" class=".btn">#3024</a>
            </td>
            <td>
                <b>
                    DIDComm v2 Messaging without DIDExchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Outbound Dispatcher SendToDID can now create a default connection, if a connection doesn't yet exist, allowing didcomm V2 protocols to operate without DIDExchange, as long as the recipient DID can be resolved (ie, public or otherwise previously provided to the agent).

Also fixes connection Recorder/Lookup so it makes only one database read instead of two, when fetching a record by DIDs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 18:55:10 +0000 UTC
    </div>
</div>

