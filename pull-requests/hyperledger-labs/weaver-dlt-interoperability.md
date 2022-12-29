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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    Bump json5 from 2.2.1 to 2.2.2 in /common/policy-dsl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 2.2.1 to 2.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li><a href="https://github.com/json5/json5/commit/d720b4fe4ad800b726da6b0f43c8454c4310fe8d"><code>d720b4f</code></a> Improve readme (e.g. explain JSON5 better!) (<a href="https://github-redirect.dependabot.com/json5/json5/issues/291">#291</a>)</li>
<li><a href="https://github.com/json5/json5/commit/910ce25914ed366a39a610b17bcd581b5da02d32"><code>910ce25</code></a> docs: fix spelling of Aseem</li>
<li><a href="https://github.com/json5/json5/commit/2aab4dd2a7c212dd4af7b91f29aa315c20251b92"><code>2aab4dd</code></a> test: require tap as t in cli tests</li>
<li><a href="https://github.com/json5/json5/commit/6d426865cec0ba7e20d4a98341e61cf26176b8fb"><code>6d42686</code></a> test: remove mocha syntax from tests</li>
<li><a href="https://github.com/json5/json5/commit/4798b9dbde850c8e84e59ac58ba2894ef184434d"><code>4798b9d</code></a> docs: update installation and usage for modules</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=2.2.1&new-version=2.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-29 08:08:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/354" class=".btn">#354</a>
            </td>
            <td>
                <b>
                    Data Sharing Protocol Bug Fixes and RFC Specification Improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixed the Fabric view structure and the associated proof collection and validation logic to take into account the fact that different proof-generating peers may produce and sign different blobs representing the same underlying data (because protobuf serialization and data encryption are typically non-deterministic). This required changes to the common protobufs, the Fabric Driver, the Fabric Interoperation Chaincode, and the Fabric Interoperation Node SDK. (The Fabric Interoperation Go SDK will be updated at a later date along with various other feature upgrades.) This fixes #350 and #351 .

Images were fixed to be rendered properly on dark backgrounds as required by #260 .

Asset transfer RFC specifications were completed as required by #237 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 06:53:17 +0000 UTC
    </div>
</div>

