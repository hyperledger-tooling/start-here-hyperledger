---
layout: default
title: fabric-test
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-test
---

# fabric-test <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-test){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    Bump ajv from 6.12.2 to 6.12.3 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ajv](https://github.com/ajv-validator/ajv) from 6.12.2 to 6.12.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ajv-validator/ajv/releases">ajv's releases</a>.</em></p>
<blockquote>
<h2>v6.12.3</h2>
<p>Pass schema object to processCode function
Option for strictNumbers (<a href="https://github.com/issacgerges"><code>@​issacgerges</code></a>, <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1128">#1128</a>)
Fixed vulnerability related to untrusted schemas (<a href="https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=CVE-2020-15366">CVE-2020-15366</a>)</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ajv-validator/ajv/commit/521c3a53f15f5502fb4a734194932535d311267c"><code>521c3a5</code></a> 6.12.3</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/bd7107b54166a4ca67555ba37829375e31649bf8"><code>bd7107b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1229">#1229</a> from ajv-validator/dependabot/npm_and_yarn/mocha-8.0.1</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/9c26bb28f839a1cde853b64f7f6d035e4b3afd1e"><code>9c26bb2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1234">#1234</a> from ajv-validator/dependabot/npm_and_yarn/eslint-7.3.1</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/c6a6daaf9e2739f4e50a33c3aed647b7629d1fc4"><code>c6a6daa</code></a> Merge branch 'master' into dependabot/npm_and_yarn/mocha-8.0.1</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/15eda23010c8b2d1353ebf7afc8e27d818b149ac"><code>15eda23</code></a> Merge branch 'master' into dependabot/npm_and_yarn/eslint-7.3.1</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/d6aabb8e97029130cdb607dcd2e78a6d567e10d5"><code>d6aabb8</code></a> test: remove node 8 from travis test</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/c4801ca7771eef5cf7ad8c1adb7cce83c16f065f"><code>c4801ca</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1242">#1242</a> from ajv-validator/refactor</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/988982d3fde08e3ea074e8942442834e78c45587"><code>988982d</code></a> ignore proto properties</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/f2b1e3d2c89288561ee68d7459a41b7222cc520d"><code>f2b1e3d</code></a> whitespace</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/65e3678146e63b0c8ec80d66e05e146dff68a15d"><code>65e3678</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1239">#1239</a> from GrahamLea/patch-1</li>
<li>Additional commits viewable in <a href="https://github.com/ajv-validator/ajv/compare/v6.12.2...v6.12.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ajv&package-manager=npm_and_yarn&previous-version=6.12.2&new-version=6.12.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-test/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-12 23:14:31 +0000 UTC
    </div>
</div>

