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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3261" class=".btn">#3261</a>
            </td>
            <td>
                <b>
                    feat: validate data model of objects saved in a wallet.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
VC Wallet Data Model validation

**Description:**
https://github.com/trustbloc/wallet/issues/1714

**Summary:**
Data models are validated against their JSON LD context before being saved into the wallet content store.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 08:33:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3259" class=".btn">#3259</a>
            </td>
            <td>
                <b>
                    refactor: remote cryptobox URLs renamed to /wrap and /unwrap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this change updates the remote CryptoBox api URIs to point to remote KMS's key /wrap and /unwrap to match ECDH-ES and ECDH-1PU key wrapping.

This change requires the KMS server to udpate /easy to /wrap, /easyOpen and /sealOpen to /unwrap

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 17:38:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3257" class=".btn">#3257</a>
            </td>
            <td>
                <b>
                    feat: interop support for did service refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 20:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3256" class=".btn">#3256</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 3.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 3.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Add support for lts/-n aliases</h2>
<p>In scope of this release we added support for <code>lts/-n</code> aliases, improve logic for <code>current</code>, <code>latest</code> and <code>node</code> aliases to handle them from <code>toolcache</code>, update <code>ncc</code> package.</p>
<h3>Support of lts/-n aliases</h3>
<ul>
<li>Related pull request: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/481">actions/setup-node#481</a></li>
<li>Related issue: <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/26">actions/setup-node#26</a></li>
</ul>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v3
- uses: actions/setup-node@v3
  with:
    node-version: lts/-1
- run: npm ci
- run: npm test
</code></pre>
<h3>Minor improvements</h3>
<ul>
<li>Update zeit/ncc to vercel/ncc: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/476">actions/setup-node#476</a></li>
<li>Get latest version from cache if exists: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/496">actions/setup-node#496</a></li>
</ul>
<h2>Add current, node, latest aliases</h2>
<p>In scope of this release we added new aliases to install the latest Node.js version. <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/483">actions/setup-node#483</a></p>
<pre lang="yml"><code>steps:
- uses: actions/checkout@v3
- uses: actions/setup-node@v3
  with:
    node-version: current
- run: npm ci
- run: npm test
</code></pre>
<h2>Update actions/cache version to 2.0.2</h2>
<p>In scope of this release we updated <code>actions/cache</code> package as the new version contains fixes related to GHES 3.5 (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/460">actions/setup-node#460</a>)</p>
<h2>Add caching support on GHES 3.5</h2>
<p>In scope of this release we added <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/452">support for caching from GHES 3.5</a> and fixed download issue for files &gt; 2GB during restore. Besides, we updated <code>actions/cache</code> dependency to 2.0.0 version.</p>
<h2>v3.0.0</h2>
<p>In scope of this release we changed version of the runtime Node.js for the setup-node action and updated package-lock.json file to  v2.</p>
<h3>Breaking Changes</h3>
<ul>
<li>With the update to Node 16 in <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/414">actions/setup-node#414</a>, all scripts will now be run with Node 16 rather than Node 12.</li>
<li>We removed deprecated <code>version</code> input (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/424">actions/setup-node#424</a>). Please use <code>node-version</code> input instead.</li>
</ul>
<h2>Fix logic of error handling for npm warning and uncaught exception</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/eeb10cff27034e7acf239c5d29f62154018672fd"><code>eeb10cf</code></a> Support lts/-n aliases (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/481">#481</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/ed1a46e9f278c17e07705c4cc19a1d9a3fca12ac"><code>ed1a46e</code></a> Update zeit/ncc to vercel/ncc (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/476">#476</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/daff393d4372bf1c1f7bdda42b9a688053433967"><code>daff393</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/496">#496</a> from panticmilos/v-mpantic/get-latest-version-from-cache</li>
<li><a href="https://github.com/actions/setup-node/commit/b14573ddb960b7d615cb82f84704679a2ffbdf2c"><code>b14573d</code></a> remove installer import</li>
<li><a href="https://github.com/actions/setup-node/commit/7569de03e709e75afc4815ae1688120e2c5bc068"><code>7569de0</code></a> rename dist manifest to node versions</li>
<li><a href="https://github.com/actions/setup-node/commit/b20a2561b99d471cbfe1222b16de377c5ccc78dc"><code>b20a256</code></a> get manifest once</li>
<li><a href="https://github.com/actions/setup-node/commit/ea3459bb459f783f186dcfc5229793d2c6f40b25"><code>ea3459b</code></a> docs: Update advanced-usage.md (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/495">#495</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/141334fcd1248aba82bae2a0682d9f5a5e06cf84"><code>141334f</code></a> remove unnecessary dist call</li>
<li><a href="https://github.com/actions/setup-node/commit/808c8f917fea369038867811c092cb7843514fbb"><code>808c8f9</code></a> remove bumping deps</li>
<li><a href="https://github.com/actions/setup-node/commit/fd1b409bc3adb8a843e511763a0160bfa08e1aea"><code>fd1b409</code></a> unit tests</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v3.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=3.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-07 01:56:02 +0000 UTC
    </div>
</div>

