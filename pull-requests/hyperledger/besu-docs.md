---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1633" class=".btn">#1633</a>
            </td>
            <td>
                <b>
                    Update minimum Java version.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Updated the documentation related to minimum Java version required to run Besu.
 

### Issue(s) fixed
#1622

### Preview
https://besu-docs-git-fork-bgravenorst-doc-1622-hyperledger.vercel.app/

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 23:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1632" class=".btn">#1632</a>
            </td>
            <td>
                <b>
                    1576(docs): documents config option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue https://github.com/hyperledger/besu-docs/issues/1576
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 12:11:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1631" class=".btn">#1631</a>
            </td>
            <td>
                <b>
                    1611(docs): improves clarity for profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Responds to [issue](https://github.com/hyperledger/besu-docs/issues/1611)

BUT raises Qs for me:

1. It sounds as if this feature was designed to allow users to create a set of configs to extend the config.toml BUT that it has been implemented to only support 3 pre-configured profiles.
> Is it really not possible to create your own custom profile?
2. I don't believe the pre-configured profiles are all doing what they say on the tin (!). Staker has 1 variable network=Mainnet >> I find it v. hard to believe that there would be a config file that does not provide network, relying on profile setting to do that. This profile claims to "maximize their hardware value and also want to serve full sets of data to their peers" -- but without putting this together with a boilerplate config.toml that helps achieve that, I suspect it!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 08:43:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1630" class=".btn">#1630</a>
            </td>
            <td>
                <b>
                    chore: fix typos in api index.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes some typos found in the api index.md
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-24 05:36:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1628" class=".btn">#1628</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group across 1 directory with 5 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 5 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [braces](https://github.com/micromatch/braces) | `3.0.2` | `3.0.3` |
| [tar](https://github.com/isaacs/node-tar) | `6.1.15` | `removed` |
| [semantic-release](https://github.com/semantic-release/semantic-release) | `21.1.2` | `24.0.0` |
| [@semantic-release/npm](https://github.com/semantic-release/npm) | `10.0.6` | `12.0.1` |
| [ws](https://github.com/websockets/ws) | `7.5.9` | `7.5.10` |


Updates `braces` from 3.0.2 to 3.0.3
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/micromatch/braces/commit/74b2db2938fad48a2ea54a9c8bf27a37a62c350d"><code>74b2db2</code></a> 3.0.3</li>
<li><a href="https://github.com/micromatch/braces/commit/88f1429a0f47e1dd3813de35211fc97ffda27f9e"><code>88f1429</code></a> update eslint. lint, fix unit tests.</li>
<li><a href="https://github.com/micromatch/braces/commit/415d660c3002d1ab7e63dbf490c9851da80596ff"><code>415d660</code></a> Snyk js braces 6838727 (<a href="https://redirect.github.com/micromatch/braces/issues/40">#40</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/190510f79db1adf21d92798b0bb6fccc1f72c9d6"><code>190510f</code></a> fix tests, skip 1 test in test/braces.expand</li>
<li><a href="https://github.com/micromatch/braces/commit/716eb9f12d820b145a831ad678618731927e8856"><code>716eb9f</code></a> readme bump</li>
<li><a href="https://github.com/micromatch/braces/commit/a5851e57f45c3431a94d83fc565754bc10f5bbc3"><code>a5851e5</code></a> Merge pull request <a href="https://redirect.github.com/micromatch/braces/issues/37">#37</a> from coderaiser/fix/vulnerability</li>
<li><a href="https://github.com/micromatch/braces/commit/2092bd1fb108d2c59bd62e243b70ad98db961538"><code>2092bd1</code></a> feature: braces: add maxSymbols (<a href="https://github.com/micromatch/braces/issues/">https://github.com/micromatch/braces/issues/</a>...</li>
<li><a href="https://github.com/micromatch/braces/commit/9f5b4cf47329351bcb64287223ffb6ecc9a5e6d3"><code>9f5b4cf</code></a> fix: vulnerability (<a href="https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727">https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/98414f9f1fabe021736e26836d8306d5de747e0d"><code>98414f9</code></a> remove funding file</li>
<li><a href="https://github.com/micromatch/braces/commit/665ab5d561c017a38ba7aafd92cc6655b91d8c14"><code>665ab5d</code></a> update keepEscaping doc (<a href="https://redirect.github.com/micromatch/braces/issues/27">#27</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/micromatch/braces/compare/3.0.2...3.0.3">compare view</a></li>
</ul>
</details>
<br />

Removes `tar`

Updates `semantic-release` from 21.1.2 to 24.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/semantic-release/semantic-release/releases">semantic-release's releases</a>.</em></p>
<blockquote>
<h2>v24.0.0</h2>
<h1><a href="https://github.com/semantic-release/semantic-release/compare/v23.1.1...v24.0.0">24.0.0</a> (2024-05-31)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> upgraded to the beta of the commit-analyzer plugin (<a href="https://github.com/semantic-release/semantic-release/commit/dfc3d9110ece8f4a1b72e209e3efce4c67a4902f">dfc3d91</a>)</li>
<li><strong>deps:</strong> upgraded to the beta of the release-notes-generator plugin (<a href="https://github.com/semantic-release/semantic-release/commit/4a4cd92097e73dc1defc514347c673d84e1b6a9e">4a4cd92</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li><strong>deps:</strong> the commit-analyzer plugin now expects to be used with the latest major versions of
conventional-changelog packages. if you are installing any of these packages in addition to
semantic-release, be sure to update them as well</li>
<li><strong>deps:</strong> the release-notes-generator plugin now expects to be used with the latest major
versions of conventional-changelog packages. if you are installing any of these packages in addition
to semantic-release, be sure to update them as well</li>
</ul>
<h2>v24.0.0-beta.2</h2>
<h1><a href="https://github.com/semantic-release/semantic-release/compare/v24.0.0-beta.1...v24.0.0-beta.2">24.0.0-beta.2</a> (2024-05-25)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> upgraded to the beta of the commit-analyzer plugin (<a href="https://github.com/semantic-release/semantic-release/commit/dfc3d9110ece8f4a1b72e209e3efce4c67a4902f">dfc3d91</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li><strong>deps:</strong> the commit-analyzer plugin now expects to be used with the latest major versions of
conventional-changelog packages. if you are installing any of these packages in addition to
semantic-release, be sure to update them as well</li>
</ul>
<h2>v24.0.0-beta.1</h2>
<h1><a href="https://github.com/semantic-release/semantic-release/compare/v23.1.1...v24.0.0-beta.1">24.0.0-beta.1</a> (2024-05-17)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> upgraded to the beta of the release-notes-generator plugin (<a href="https://github.com/semantic-release/semantic-release/commit/4a4cd92097e73dc1defc514347c673d84e1b6a9e">4a4cd92</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li><strong>deps:</strong> the release-notes-generator plugin now expects to be used with the latest major
versions of conventional-changelog packages. if you are installing any of these packages in addition
to semantic-release, be sure to update them as well</li>
</ul>
<h2>v23.1.1</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/semantic-release/semantic-release/commit/2b3e5f7c14727ed9052271b58f6a3daf3becf037"><code>2b3e5f7</code></a> Merge pull request <a href="https://redirect.github.com/semantic-release/semantic-release/issues/3327">#3327</a> from semantic-release/beta</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/c0e433dde68daca60aabfdd91bcf80e2a5383f36"><code>c0e433d</code></a> ci(action): update github/codeql-action action to v3.25.7 (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3326">#3326</a>)</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/2b770959d28a83e901c566f37a63c69f6e14ed6e"><code>2b77095</code></a> Merge branch 'master' of github.com:semantic-release/semantic-release into beta</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/5f05152fe642f29dda437ce78e1ce3bcb89f1dea"><code>5f05152</code></a> chore(deps): update npm to v10.8.1 (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3325">#3325</a>)</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/6d7dc855870291126472f0ea1a3cc1999f5d9b6d"><code>6d7dc85</code></a> chore(deps): update dependency got to v14.3.0 (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3311">#3311</a>)</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/20b2672d4005c21d9cabcbb91df79f72d32e3e1b"><code>20b2672</code></a> ci(action): update github/codeql-action action to v3.25.6 (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3316">#3316</a>)</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/2620c1078d844003322482ac96af7dde36cf7396"><code>2620c10</code></a> docs: update file extensions to include .mjs on configuration docs page (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3322">#3322</a>)</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/dfc3d9110ece8f4a1b72e209e3efce4c67a4902f"><code>dfc3d91</code></a> fix(deps): upgraded to the beta of the commit-analyzer plugin</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/e424297f2f97b712e83203c91d12220e9b4cae9f"><code>e424297</code></a> chore(deps): lock file maintenance (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3312">#3312</a>)</li>
<li><a href="https://github.com/semantic-release/semantic-release/commit/36809746f7a6c85eba681f0beca1ff33b0f0f0cc"><code>3680974</code></a> chore(deps): update dependency publint to v0.2.8 (<a href="https://redirect.github.com/semantic-release/semantic-release/issues/3310">#3310</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/semantic-release/semantic-release/compare/v21.1.2...v24.0.0">compare view</a></li>
</ul>
</details>
<br />

Updates `@semantic-release/npm` from 10.0.6 to 12.0.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/semantic-release/npm/releases"><code>@​semantic-release/npm</code>'s releases</a>.</em></p>
<blockquote>
<h2>v12.0.1</h2>
<h2><a href="https://github.com/semantic-release/npm/compare/v12.0.0...v12.0.1">12.0.1</a> (2024-05-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency execa to v9 (<a href="https://github.com/semantic-release/npm/commit/9ac5ed00021db4a7e2799b87ecf1b8f4fb7bede6">9ac5ed0</a>)</li>
</ul>
<h2>v12.0.0</h2>
<h1><a href="https://github.com/semantic-release/npm/compare/v11.0.3...v12.0.0">12.0.0</a> (2024-03-16)</h1>
<h3>Features</h3>
<ul>
<li><strong>exports:</strong> defined <code>exports</code> to point at ./index.js (<a href="https://github.com/semantic-release/npm/commit/9e193c2239ee651d5a1fddce499edb664140938f">9e193c2</a>)</li>
<li><strong>node-versions:</strong> dropped support for node v18 and v19 (<a href="https://github.com/semantic-release/npm/commit/2df962b6c7563a3a797ab6d54e0e071dd898f08c">2df962b</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li><strong>exports:</strong> <code>exports</code> has been defined, which prevents access to private apis (which arent
intended for consumption anyway)</li>
<li><strong>node-versions:</strong> node v18 and v19 are no longer supported</li>
</ul>
<h2>v11.0.3</h2>
<h2><a href="https://github.com/semantic-release/npm/compare/v11.0.2...v11.0.3">11.0.3</a> (2024-03-01)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> raised the minimum accepted range of npm to v10.5.0 (<a href="https://redirect.github.com/semantic-release/npm/issues/759">#759</a>) (<a href="https://github.com/semantic-release/npm/commit/a0313f82060ec344d77443a9b1b28e87178dcf78">a0313f8</a>), closes <a href="https://redirect.github.com/semantic-release/semantic-release/issues/3202">semantic-release/semantic-release#3202</a></li>
</ul>
<p>even though our existing range allowed anyone to update as soon as the new npm version was available, this will encourage being on a version that does not report the ip vulnerability a bit more forcefully</p>
<h2>v11.0.2</h2>
<h2><a href="https://github.com/semantic-release/npm/compare/v11.0.1...v11.0.2">11.0.2</a> (2023-12-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency npm to v10.2.5 (<a href="https://github.com/semantic-release/npm/commit/42b5dec34f4a894d30d1b8a944fb6ba86069c6a4">42b5dec</a>)</li>
</ul>
<h2>v11.0.1</h2>
<h2><a href="https://github.com/semantic-release/npm/compare/v11.0.0...v11.0.1">11.0.1</a> (2023-11-02)</h2>
<h3>Bug Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/semantic-release/npm/commit/9ac5ed00021db4a7e2799b87ecf1b8f4fb7bede6"><code>9ac5ed0</code></a> fix(deps): update dependency execa to v9</li>
<li><a href="https://github.com/semantic-release/npm/commit/63cbef1912ce4ffdc8f7689d188358698f69e23b"><code>63cbef1</code></a> ci(action): update actions/checkout action to v4.1.5 (<a href="https://redirect.github.com/semantic-release/npm/issues/796">#796</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/2e93b22c5eda014faa695268928f50ed8db28148"><code>2e93b22</code></a> chore(deps): update dependency sinon to v17.0.2 (<a href="https://redirect.github.com/semantic-release/npm/issues/795">#795</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/fbf77cfae64ac04c73e616655a99f3ddb5182a1d"><code>fbf77cf</code></a> chore(deps): lock file maintenance (<a href="https://redirect.github.com/semantic-release/npm/issues/794">#794</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/f93b63fee96d8e5fb29ff989cefec504c311d462"><code>f93b63f</code></a> chore(deps): update dependency ava to v6.1.3 (<a href="https://redirect.github.com/semantic-release/npm/issues/793">#793</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/86011db51801fedf17eec1e9611b1cbe8e46cafa"><code>86011db</code></a> chore(deps): update npm to v10.7.0 (<a href="https://redirect.github.com/semantic-release/npm/issues/788">#788</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/5850c2e96845f22ea0a6a2afd656ed1c1643e1c9"><code>5850c2e</code></a> chore(deps): update npm to v10.6.0</li>
<li><a href="https://github.com/semantic-release/npm/commit/8ae2364df5442920b1466981c71d7f7813311646"><code>8ae2364</code></a> chore(deps): lock file maintenance (<a href="https://redirect.github.com/semantic-release/npm/issues/787">#787</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/08859862a49c299e1551042b3e9822958c4d1af3"><code>0885986</code></a> chore(deps): lock file maintenance (<a href="https://redirect.github.com/semantic-release/npm/issues/786">#786</a>)</li>
<li><a href="https://github.com/semantic-release/npm/commit/f9c63abfbe92ec9629bae7ea70a61734272b307a"><code>f9c63ab</code></a> ci(action): update actions/checkout action to v4.1.4 (<a href="https://redirect.github.com/semantic-release/npm/issues/782">#782</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/semantic-release/npm/compare/v10.0.6...v12.0.1">compare view</a></li>
</ul>
</details>
<br />

Updates `ws` from 7.5.9 to 7.5.10
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>7.5.10</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 7.x release line (22c28763).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d962d70649e393841ee1ed726a8f7ffbe90d0c06"><code>d962d70</code></a> [dist] 7.5.10</li>
<li><a href="https://github.com/websockets/ws/commit/22c28763234aa75a7e1b76f5c01c181260d7917f"><code>22c2876</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/7.5.9...7.5.10">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/besu-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 12:07:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1627" class=".btn">#1627</a>
            </td>
            <td>
                <b>
                    Add bonsai-limit-trie-logs options and update how to page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu-docs/issues/1624
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 11:11:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1621" class=".btn">#1621</a>
            </td>
            <td>
                <b>
                    1618 docs adds eth_maxFeePG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1618 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 14:46:47 +0000 UTC
    </div>
</div>

