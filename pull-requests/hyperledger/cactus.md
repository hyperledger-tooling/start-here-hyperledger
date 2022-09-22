---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2162" class=".btn">#2162</a>
            </td>
            <td>
                <b>
                    feat(ubiquity): initial commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This plugin defines interfaces for developers to use a wrapped version of the Ubiquity SDK. Ubiquity is a high performance, multi-chain API for accessing blockchain data, i.e., provides one API to access multiple protocols. 
This API complements Cactus current connector offering by allowing to connect seamlessly to a multitude of public blockchains.


Signed-off-by: Rafael Belchior <rafael.belchior@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 15:40:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2160" class=".btn">#2160</a>
            </td>
            <td>
                <b>
                    build(deps): bump jose from 4.1.0 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jose](https://github.com/panva/jose) from 4.1.0 to 4.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v4.9.2</h2>
<h3>Fixes</h3>
<ul>
<li>limit default PBES2 alg's computational expense (<a href="https://github.com/panva/jose/commit/03d6d013bf6e070e85adfe5731f526978e3e8e4d">03d6d01</a>)</li>
</ul>
<h2>v4.9.1</h2>
<h3>Fixes</h3>
<ul>
<li><strong>deno:</strong> add a Deno package entrypoint (<a href="https://github.com/panva/jose/commit/9f3c459e30b71eec54163d500edb59f5c72bf7c9">9f3c459</a>)</li>
</ul>
<h2>v4.9.0</h2>
<h3>Features</h3>
<ul>
<li>add support for RFC 9278 - JWK Thumbprint URI (<a href="https://github.com/panva/jose/commit/d06ce654666c5f584716f39843534118407c14e0">d06ce65</a>)</li>
</ul>
<h3>Refactor</h3>
<ul>
<li>consume some base64url decode errors (<a href="https://github-redirect.dependabot.com/panva/jose/issues/436">#436</a>) (<a href="https://github.com/panva/jose/commit/caaf2c38dc51209d7adc493029f416c61759b1b1">caaf2c3</a>)</li>
<li>unify JOSENotSupported throw on key export (<a href="https://github.com/panva/jose/commit/fe5d093bf74b812ecd3ee92d40dd02619e88e06c">fe5d093</a>)</li>
</ul>
<h2>v4.8.3</h2>
<p>This release contains only code refactoring and documentation updates.</p>
<h2>v4.8.1</h2>
<h3>Fixes</h3>
<ul>
<li><strong>typescript:</strong> add types export for nodenext module resolution (<a href="https://github-redirect.dependabot.com/panva/jose/issues/406">#406</a>) (<a href="https://github.com/panva/jose/commit/5a6d8f0a2a3283bd1e832f1e71906d70f74c1262">5a6d8f0</a>)</li>
</ul>
<h2>v4.8.0</h2>
<h3>Features</h3>
<ul>
<li>add &quot;worker&quot; export in package.json (<a href="https://github-redirect.dependabot.com/panva/jose/issues/400">#400</a>) (<a href="https://github.com/panva/jose/commit/c58c80ae98b7a55b3b95e72438040983ae9a23de">c58c80a</a>)</li>
<li>optional headers options for createRemoteJWKSet (<a href="https://github-redirect.dependabot.com/panva/jose/issues/397">#397</a>) (<a href="https://github.com/panva/jose/commit/b4612f5d256b773ab7a1144ac839bdf0f8ccff53">b4612f5</a>)</li>
</ul>
<h2>v4.7.0</h2>
<h3>Features</h3>
<ul>
<li>add createRemoteJWKSet cacheMaxAge option (<a href="https://github.com/panva/jose/commit/5017d95764b3aca551631c1a2fbe7cc40cbb6055">5017d95</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/394">#394</a></li>
</ul>
<h2>v4.6.2</h2>
<h3>Fixes</h3>
<ul>
<li>dont check JWT iat is in the past unless maxTokenAge is used (<a href="https://github.com/panva/jose/commit/96d85c70033d2249de41ed07d97ed6843c15eb2a">96d85c7</a>)</li>
</ul>
<h2>v4.6.1</h2>
<p>This release contains only code refactoring and documentation updates.</p>
<h2>v4.6.0</h2>
<h3>Features</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/main/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/panva/jose/compare/v4.9.1...v4.9.2">4.9.2</a> (2022-09-01)</h2>
<h3>Fixes</h3>
<ul>
<li>limit default PBES2 alg's computational expense (<a href="https://github.com/panva/jose/commit/03d6d013bf6e070e85adfe5731f526978e3e8e4d">03d6d01</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.9.0...v4.9.1">4.9.1</a> (2022-08-29)</h2>
<h3>Fixes</h3>
<ul>
<li><strong>deno:</strong> add a Deno package entrypoint (<a href="https://github.com/panva/jose/commit/9f3c459e30b71eec54163d500edb59f5c72bf7c9">9f3c459</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.8.3...v4.9.0">4.9.0</a> (2022-08-17)</h2>
<h3>Features</h3>
<ul>
<li>add support for RFC 9278 - JWK Thumbprint URI (<a href="https://github.com/panva/jose/commit/d06ce654666c5f584716f39843534118407c14e0">d06ce65</a>)</li>
</ul>
<h3>Refactor</h3>
<ul>
<li>consume some base64url decode errors (<a href="https://github-redirect.dependabot.com/panva/jose/issues/436">#436</a>) (<a href="https://github.com/panva/jose/commit/caaf2c38dc51209d7adc493029f416c61759b1b1">caaf2c3</a>)</li>
<li>unify JOSENotSupported throw on key export (<a href="https://github.com/panva/jose/commit/fe5d093bf74b812ecd3ee92d40dd02619e88e06c">fe5d093</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.8.1...v4.8.3">4.8.3</a> (2022-06-29)</h2>
<h2><a href="https://github.com/panva/jose/compare/v4.8.0...v4.8.1">4.8.1</a> (2022-05-02)</h2>
<h3>Fixes</h3>
<ul>
<li><strong>typescript:</strong> add types export for nodenext module resolution (<a href="https://github-redirect.dependabot.com/panva/jose/issues/406">#406</a>) (<a href="https://github.com/panva/jose/commit/5a6d8f0a2a3283bd1e832f1e71906d70f74c1262">5a6d8f0</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.7.0...v4.8.0">4.8.0</a> (2022-04-26)</h2>
<h3>Features</h3>
<ul>
<li>add &quot;worker&quot; export in package.json (<a href="https://github-redirect.dependabot.com/panva/jose/issues/400">#400</a>) (<a href="https://github.com/panva/jose/commit/c58c80ae98b7a55b3b95e72438040983ae9a23de">c58c80a</a>)</li>
<li>optional headers options for createRemoteJWKSet (<a href="https://github-redirect.dependabot.com/panva/jose/issues/397">#397</a>) (<a href="https://github.com/panva/jose/commit/b4612f5d256b773ab7a1144ac839bdf0f8ccff53">b4612f5</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.6.2...v4.7.0">4.7.0</a> (2022-04-21)</h2>
<h3>Features</h3>
<ul>
<li>add createRemoteJWKSet cacheMaxAge option (<a href="https://github.com/panva/jose/commit/5017d95764b3aca551631c1a2fbe7cc40cbb6055">5017d95</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/394">#394</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/db71b3d15254b27666754fa2ec85b666b4cf1306"><code>db71b3d</code></a> chore(release): 4.9.2</li>
<li><a href="https://github.com/panva/jose/commit/03d6d013bf6e070e85adfe5731f526978e3e8e4d"><code>03d6d01</code></a> fix: limit default PBES2 alg's computational expense</li>
<li><a href="https://github.com/panva/jose/commit/8c5cc34eb558ce52b319107b4faeb26703994556"><code>8c5cc34</code></a> chore: cleanup after publish</li>
<li><a href="https://github.com/panva/jose/commit/8ed39d67cd1bb58c39641544758d905930a047d3"><code>8ed39d6</code></a> chore(release): 4.9.1</li>
<li><a href="https://github.com/panva/jose/commit/9f3c459e30b71eec54163d500edb59f5c72bf7c9"><code>9f3c459</code></a> fix(deno): add a Deno package entrypoint</li>
<li><a href="https://github.com/panva/jose/commit/d07c6e9abb0da94134cbd23e1de73e3a30069694"><code>d07c6e9</code></a> test: update expectations for P-384 ECDH</li>
<li><a href="https://github.com/panva/jose/commit/664279d468a508635c55c2c466a207790ce13ed7"><code>664279d</code></a> chore: cleanup after publish</li>
<li><a href="https://github.com/panva/jose/commit/24484d641500647fb5b2d07af57e868984cb7ee9"><code>24484d6</code></a> chore(release): 4.9.0</li>
<li><a href="https://github.com/panva/jose/commit/ebf277bedd4237d2382d13e2e3b5c786b99722b9"><code>ebf277b</code></a> chore: add refactors to version logs</li>
<li><a href="https://github.com/panva/jose/commit/d06ce654666c5f584716f39843534118407c14e0"><code>d06ce65</code></a> feat: add support for RFC 9278 - JWK Thumbprint URI</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v4.1.0...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=4.1.0&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 17:55:21 +0000 UTC
    </div>
</div>

