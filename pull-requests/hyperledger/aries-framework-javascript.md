---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1603" class=".btn">#1603</a>
            </td>
            <td>
                <b>
                    fix: save AnonCredsCredentialRecord createdAt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For some unfortunate reason, we are not saving `createdAt` at AnonCredsCredentialRecord creation. This is useful to do things like sorting credentials by their issuance date (something available with W3C Credential Reacords)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 02:02:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1601" class=".btn">#1601</a>
            </td>
            <td>
                <b>
                    build(deps): bump @mattrglobal/bbs-signatures from 1.1.0 to 1.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@mattrglobal/bbs-signatures](https://github.com/mattrglobal/bbs-signatures) from 1.1.0 to 1.3.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mattrglobal/bbs-signatures/blob/master/CHANGELOG.md"><code>@​mattrglobal/bbs-signatures</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/mattrglobal/bbs-signatures/compare/v1.3.0...v1.3.1">1.3.1</a> (2023-10-04)</h2>
<h3>Features</h3>
<ul>
<li>update <code>debug</code> from 4.1.1 to 4.3.4 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/a7e7aad830ddcaef588a27ff53c4104868800b4b">a7e7aad</a>)</li>
</ul>
<h1><a href="https://github.com/mattrglobal/bbs-signatures/compare/v1.2.0...v1.3.0">1.3.0</a> (2023-09-29)</h1>
<h3>Features</h3>
<ul>
<li>update <code>@mattrglobal/node-bbs-signatures</code> to 0.18.1 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update <code>@wasm-tool/wasm-pack-plugin</code> to 1.7.0 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update rust edition to 2021 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update <code>console_error_panic_hook</code> to 0.1.7 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update <code>serde-wasm-bindgen</code> to 0.6.0 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update <code>wasm-bindgen</code> to 0.2.87 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update <code>wasm-bindgen-future</code> to 0.4.37 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
<li>update <code>web-sys</code> to 0.3.64 (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>remove support for <code>wee_alloc</code> (<a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314">b929d7d</a>)</li>
</ul>
<h1><a href="https://github.com/mattrglobal/bbs-signatures/compare/1.0.0...1.2.0">1.2.0</a> (2023-09-18)</h1>
<h3>Features</h3>
<ul>
<li>add node 18.x support (<a href="https://github.com/mattrglobal/bbs-signatures/commit/5726e4c71637b1b7149698a671fa0cd7663170bb">5726e4c</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/1df8e1e38f56c0a89f43a34409a3f6ea3d6bd151"><code>1df8e1e</code></a> chore(release): publish</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/a7e7aad830ddcaef588a27ff53c4104868800b4b"><code>a7e7aad</code></a> build(deps): bump debug from 4.1.1 to 4.3.4 (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/162">#162</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/531f4cdd1956c75742a9a37937ed76df25872ce7"><code>531f4cd</code></a> chore(release): publish (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/159">#159</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/b929d7dadc35e6cc52d27227b990d825717c7314"><code>b929d7d</code></a> build(deps): remove wee_alloc (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/158">#158</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/a9e2e56153bee6df9ef4001b55097e0a1d5925ac"><code>a9e2e56</code></a> build(deps): bump bumpalo from 3.6.1 to 3.12.0 (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/148">#148</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/14ada23abce58faca258b06aef4fb0f0d4c1fb13"><code>14ada23</code></a> build(deps): bump <code>@​commitlint/cli</code> and <code>@​commitlint/config-conventional</code> version...</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/307153d2e43cf32c0cb8369c6928a74773fc95ba"><code>307153d</code></a> build(deps): bump semver from 6.3.0 to 6.3.1 in /sample/browser (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/151">#151</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/e99a9a4237d33b34914d7254f9efec4b2d045a1a"><code>e99a9a4</code></a> build(deps): bump semver from 6.3.0 to 6.3.1 in /sample/ts-node (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/152">#152</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/69c9edca4875a3075a39f47aae9ac5974be5ed2f"><code>69c9edc</code></a> build(deps-dev): bump webpack from 5.73.0 to 5.76.0 in /sample/browser (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/149">#149</a>)</li>
<li><a href="https://github.com/mattrglobal/bbs-signatures/commit/b19d7f20b8e041cafcdf735ad266b52f3628dca9"><code>b19d7f2</code></a> build(deps): bump json5 from 2.2.1 to 2.2.3 (<a href="https://redirect.github.com/mattrglobal/bbs-signatures/issues/147">#147</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/mattrglobal/bbs-signatures/compare/1.1.0...v1.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@mattrglobal/bbs-signatures&package-manager=npm_and_yarn&previous-version=1.1.0&new-version=1.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-05 13:40:15 +0000 UTC
    </div>
</div>

