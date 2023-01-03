---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    Bump json5 and react-scripts in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies need to be updated together.

Updates `json5` from 2.2.0 to 2.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `react-scripts` from 4.0.3 to 5.0.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/create-react-app/commit/19fa58d527ae74f2b6baa0867463eea1d290f9a5"><code>19fa58d</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/9802941ff049a28da2682801bc182a29761b71f4"><code>9802941</code></a> fix: webpack noise printed only if error or warning (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12245">#12245</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/2eef1d0a1db2e84cdcd6e7ca941c85a48cc7cc65"><code>2eef1d0</code></a> Update templates to use React 18 <code>createRoot</code> (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12220">#12220</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/221e511730ca51c036c6954a9d2ee7659ff860f9"><code>221e511</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/5614c87bfbaae0ce52ac15aedd2cd0f91ffd420d"><code>5614c87</code></a> Add support for Tailwind (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11717">#11717</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/20edab4894b301f6b90dad0f90a2f82c52a7ac66"><code>20edab4</code></a> fix(webpackDevServer): disable overlay for warnings (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11413">#11413</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/3afbbc0ab922fb982bb275ccb3fe5beecdf5f889"><code>3afbbc0</code></a> Update all dependencies (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11624">#11624</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/f5467d5e77d51a3f23dd5fa70697dbab79832489"><code>f5467d5</code></a> feat(eslint-config-react-app): support ESLint 8.x (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11375">#11375</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/c7627ce96c4674f327081f101dd0e2771be4d045"><code>c7627ce</code></a> Update webpack and dev server (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11646">#11646</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/544befeb536a89b0ff95792df70bb037b17f55b9"><code>544befe</code></a> Update package.json (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11597">#11597</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/create-react-app/commits/react-scripts@5.0.1/packages/react-scripts">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 08:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) and [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies needed to be updated together.
Updates `json5` from 2.2.0 to 2.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.9.0 to 3.10.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[3.10.1] - 2021-07-06</h2>
<h3>Fixed</h3>
<ul>
<li>Add register.js to published files</li>
</ul>
<h2>[3.10.0] - 2021-07-06</h2>
<h3>Added</h3>
<ul>
<li>feat(tsconfig-loader): extends config from node_modules (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/106">#106</a>). Thanks to <a href="https://github.com/zorji"><code>@​zorji</code></a> for this PR!</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Update CHANGELOG.md (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/96">#96</a>). Thanks to <a href="https://github.com/OliverJAsh"><code>@​OliverJAsh</code></a> for this PR!</li>
<li>Fix &quot;bootstraping&quot; typo (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/111">#111</a>). Thanks to <a href="https://github.com/KRMisha"><code>@​KRMisha</code></a> for this PR!</li>
<li>Update Readme fixes <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/116">#116</a> (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/123">#123</a>). Thanks to <a href="https://github.com/benwinding"><code>@​benwinding</code></a> for this PR!</li>
<li>Fixed typo (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/144">#144</a>). Thanks to <a href="https://github.com/mprinc"><code>@​mprinc</code></a> for this PR!</li>
<li>[TYPO] src/mapping-entry.ts (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/145">#145</a>). Thanks to <a href="https://github.com/mprinc"><code>@​mprinc</code></a> for this PR!</li>
<li>docs(README): fix typos (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/156">#156</a>). Thanks to <a href="https://github.com/PiDelport"><code>@​PiDelport</code></a> for this PR!</li>
<li>deps: bump json5 to use type definition provided officially (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/158">#158</a>). Thanks to <a href="https://github.com/koba04"><code>@​koba04</code></a> for this PR!</li>
<li>Update tsconfig-loader.ts (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/161">#161</a>). Thanks to <a href="https://github.com/fecqs"><code>@​fecqs</code></a> for this PR!</li>
<li>fix typo (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/165">#165</a>). Thanks to <a href="https://github.com/wonda-tea-coffee"><code>@​wonda-tea-coffee</code></a> for this PR!</li>
<li>Add file extenstion to typings property value (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/151">#151</a>). Thanks to <a href="https://github.com/dangrussell"><code>@​dangrussell</code></a> for this PR!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/80bc8106ee580dea5d379e462fdd4cbeb43ecfcf"><code>80bc810</code></a> v3.10.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/beb9a47268bc7cc7f1979b537a68e23d6d53738e"><code>beb9a47</code></a> Add changelog for 3.10.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/893b76df7ec945b13c6a34fccdcb152cded39717"><code>893b76d</code></a> Add register.js to published files</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9327fa1cafa6a7b4ac20eaaad2c83a694617152c"><code>9327fa1</code></a> v3.10.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/766a0e872117b0ad28ab872095b64e6c6e419776"><code>766a0e8</code></a> Update changelog for 3.10.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/2cf8b21b2b406da68b81edf5ef6fc0563a9fe329"><code>2cf8b21</code></a> Categorize changelog</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/fb67ba26eaec10fdbdac26763e6994fc304a80ec"><code>fb67ba2</code></a> Update changelog with unreleased PRs</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/079285a9f254977a0d10d98b4836866ee53e2a9c"><code>079285a</code></a> Add file extenstion to typings property value (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/151">#151</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/c49386cb979c220019749334697ffb2c79e69a98"><code>c49386c</code></a> feat(tsconfig-loader): extends config from node_modules without './node_modul...</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f289c99cf65392652da7eee855831afab62e36a5"><code>f289c99</code></a> fix typo (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/165">#165</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.9.0...v3.10.1">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 08:04:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/322" class=".btn">#322</a>
            </td>
            <td>
                <b>
                    Bump flat and @wdio/mocha-framework in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [flat](https://github.com/hughsk/flat) to 5.0.2 and updates ancestor dependency [@wdio/mocha-framework](https://github.com/webdriverio/webdriverio/tree/HEAD/packages/wdio-mocha-framework). These dependencies need to be updated together.

Updates `flat` from 4.1.1 to 5.0.2
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hughsk/flat/commit/e5ffd664df8a1fcc05adc22dd0ac6a2b32a0955d"><code>e5ffd66</code></a> Release 5.0.2</li>
<li><a href="https://github.com/hughsk/flat/commit/fdb79d537748c827e8b886f897d8e1eb3c1acd17"><code>fdb79d5</code></a> Update dependencies, refresh lockfile, format with standard.</li>
<li><a href="https://github.com/hughsk/flat/commit/e52185dded05768a1036327c5e79a399778d9191"><code>e52185d</code></a> Test against node 14 in CI.</li>
<li><a href="https://github.com/hughsk/flat/commit/0189cb11dbc942447af78930bcb0ebc132b88384"><code>0189cb1</code></a> Avoid arrow function syntax.</li>
<li><a href="https://github.com/hughsk/flat/commit/f25d3a11306bc460e43a14affa64d44a1d3cf8ed"><code>f25d3a1</code></a> Release 5.0.1</li>
<li><a href="https://github.com/hughsk/flat/commit/54cc7ad380ebfbdf22e6654934dde5a34fdf3104"><code>54cc7ad</code></a> use standard formatting</li>
<li><a href="https://github.com/hughsk/flat/commit/779816e81b6546da12280ee529d78dc57a7a5e1c"><code>779816e</code></a> drop dependencies</li>
<li><a href="https://github.com/hughsk/flat/commit/2eea6d3a556feb1bdb02dc2f376c935da59a66e4"><code>2eea6d3</code></a> Bump lodash from 4.17.15 to 4.17.19</li>
<li><a href="https://github.com/hughsk/flat/commit/a61a554952cfb550f276acc02ceea403afe01700"><code>a61a554</code></a> Bump acorn from 7.1.0 to 7.4.0</li>
<li><a href="https://github.com/hughsk/flat/commit/20ef0ef55dfa028caddaedbcb33efbdb04d18e13"><code>20ef0ef</code></a> Fix prototype pollution on unflatten</li>
<li>Additional commits viewable in <a href="https://github.com/hughsk/flat/compare/4.1.1...5.0.2">compare view</a></li>
</ul>
</details>
<br />

Updates `@wdio/mocha-framework` from 5.23.0 to 8.0.14
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webdriverio/webdriverio/releases"><code>@​wdio/mocha-framework</code>'s releases</a>.</em></p>
<blockquote>
<h2>v8.0.14 (2022-12-28)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>wdio-allure-reporter</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9472">#9472</a> Create CJS export for Allure Reporter (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li><code>webdriverio</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9435">#9435</a> Have fallback for <code>scrollIntoView</code> if actions command fails (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>wdio-browserstack-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9437">#9437</a> update: mark session as failed if no specs ran (<a href="https://github.com/Ankit098"><code>@​Ankit098</code></a>)</li>
</ul>
</li>
<li><code>wdio-types</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9441">#9441</a> Add missing noProxy typing for Capabilities ProxyObject (<a href="https://github.com/taina0407"><code>@​taina0407</code></a>)</li>
</ul>
</li>
<li><code>wdio-cucumber-framework</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9438">#9438</a> <code>@​wdio/cucumber-framework</code>: add missing Promise.all in registerRequired… (<a href="https://github.com/SCG82"><code>@​SCG82</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9448">#9448</a> docs: Fix a few typos (<a href="https://github.com/timgates42"><code>@​timgates42</code></a>)</li>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9403">#9403</a> fix: updated wdio execution command in proxy setup (<a href="https://github.com/vjuturu"><code>@​vjuturu</code></a>)</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li><code>wdio-types</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9444">#9444</a> <code>@​wdio/types</code>: node16 module resolution compatibility (<a href="https://github.com/SCG82"><code>@​SCG82</code></a>)</li>
</ul>
</li>
<li><code>devtools</code>, <code>eslint-plugin-wdio</code>, <code>wdio-allure-reporter</code>, <code>wdio-appium-service</code>, <code>wdio-browser-runner</code>, <code>wdio-browserstack-service</code>, <code>wdio-cli</code>, <code>wdio-concise-reporter</code>, <code>wdio-config</code>, <code>wdio-crossbrowsertesting-service</code>, <code>wdio-cucumber-framework</code>, <code>wdio-devtools-service</code>, <code>wdio-globals</code>, <code>wdio-jasmine-framework</code>, <code>wdio-junit-reporter</code>, <code>wdio-local-runner</code>, <code>wdio-logger</code>, <code>wdio-mocha-framework</code>, <code>wdio-repl</code>, <code>wdio-reporter</code>, <code>wdio-runner</code>, <code>wdio-sauce-service</code>, <code>wdio-selenium-standalone-service</code>, <code>wdio-shared-store-service</code>, <code>wdio-spec-reporter</code>, <code>wdio-sumologic-reporter</code>, <code>wdio-testingbot-service</code>, <code>wdio-types</code>, <code>wdio-utils</code>, <code>wdio-webdriver-mock-service</code>, <code>webdriver</code>, <code>webdriverio</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9445">#9445</a> Adding new EsLint rules (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li>Other
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9429">#9429</a> Update reference link to eslint governance file (<a href="https://github.com/Relequestual"><code>@​Relequestual</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 7</h4>
<ul>
<li>Ankit Singh (<a href="https://github.com/Ankit098"><code>@​Ankit098</code></a>)</li>
<li>Ben Hutton (<a href="https://github.com/Relequestual"><code>@​Relequestual</code></a>)</li>
<li>Christian Bromann (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
<li>Tim Gates (<a href="https://github.com/timgates42"><code>@​timgates42</code></a>)</li>
<li>Vampire (<a href="https://github.com/taina0407"><code>@​taina0407</code></a>)</li>
<li><a href="https://github.com/SCG82"><code>@​SCG82</code></a></li>
<li><a href="https://github.com/vjuturu"><code>@​vjuturu</code></a></li>
</ul>
<h2>v8.0.13 (2022-12-14)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>wdio-cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9399">#9399</a> Kill worker process if parent shuts down (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li><code>wdio-local-runner</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9398">#9398</a> Fix watch mode by better resolving worker readiness (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li><code>wdio-utils</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9397">#9397</a> Fix async iterators (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9392">#9392</a> Add docs for Accessibility Testing (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webdriverio/webdriverio/blob/main/CHANGELOG.md"><code>@​wdio/mocha-framework</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v8.0.14 (2022-12-28)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>wdio-allure-reporter</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9472">#9472</a> Create CJS export for Allure Reporter (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li><code>webdriverio</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9435">#9435</a> Have fallback for <code>scrollIntoView</code> if actions command fails (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>wdio-browserstack-service</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9437">#9437</a> update: mark session as failed if no specs ran (<a href="https://github.com/Ankit098"><code>@​Ankit098</code></a>)</li>
</ul>
</li>
<li><code>wdio-types</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9441">#9441</a> Add missing noProxy typing for Capabilities ProxyObject (<a href="https://github.com/taina0407"><code>@​taina0407</code></a>)</li>
</ul>
</li>
<li><code>wdio-cucumber-framework</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9438">#9438</a> <code>@​wdio/cucumber-framework</code>: add missing Promise.all in registerRequired… (<a href="https://github.com/SCG82"><code>@​SCG82</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9448">#9448</a> docs: Fix a few typos (<a href="https://github.com/timgates42"><code>@​timgates42</code></a>)</li>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9403">#9403</a> fix: updated wdio execution command in proxy setup (<a href="https://github.com/vjuturu"><code>@​vjuturu</code></a>)</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li><code>wdio-types</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9444">#9444</a> <code>@​wdio/types</code>: node16 module resolution compatibility (<a href="https://github.com/SCG82"><code>@​SCG82</code></a>)</li>
</ul>
</li>
<li><code>devtools</code>, <code>eslint-plugin-wdio</code>, <code>wdio-allure-reporter</code>, <code>wdio-appium-service</code>, <code>wdio-browser-runner</code>, <code>wdio-browserstack-service</code>, <code>wdio-cli</code>, <code>wdio-concise-reporter</code>, <code>wdio-config</code>, <code>wdio-crossbrowsertesting-service</code>, <code>wdio-cucumber-framework</code>, <code>wdio-devtools-service</code>, <code>wdio-globals</code>, <code>wdio-jasmine-framework</code>, <code>wdio-junit-reporter</code>, <code>wdio-local-runner</code>, <code>wdio-logger</code>, <code>wdio-mocha-framework</code>, <code>wdio-repl</code>, <code>wdio-reporter</code>, <code>wdio-runner</code>, <code>wdio-sauce-service</code>, <code>wdio-selenium-standalone-service</code>, <code>wdio-shared-store-service</code>, <code>wdio-spec-reporter</code>, <code>wdio-sumologic-reporter</code>, <code>wdio-testingbot-service</code>, <code>wdio-types</code>, <code>wdio-utils</code>, <code>wdio-webdriver-mock-service</code>, <code>webdriver</code>, <code>webdriverio</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9445">#9445</a> Adding new EsLint rules (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li>Other
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9429">#9429</a> Update reference link to eslint governance file (<a href="https://github.com/Relequestual"><code>@​Relequestual</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 7</h4>
<ul>
<li>Ankit Singh (<a href="https://github.com/Ankit098"><code>@​Ankit098</code></a>)</li>
<li>Ben Hutton (<a href="https://github.com/Relequestual"><code>@​Relequestual</code></a>)</li>
<li>Christian Bromann (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
<li>Tim Gates (<a href="https://github.com/timgates42"><code>@​timgates42</code></a>)</li>
<li>Vampire (<a href="https://github.com/taina0407"><code>@​taina0407</code></a>)</li>
<li><a href="https://github.com/SCG82"><code>@​SCG82</code></a></li>
<li><a href="https://github.com/vjuturu"><code>@​vjuturu</code></a></li>
</ul>
<h2>v8.0.13 (2022-12-14)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>wdio-cli</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9399">#9399</a> Kill worker process if parent shuts down (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li><code>wdio-local-runner</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9398">#9398</a> Fix watch mode by better resolving worker readiness (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
<li><code>wdio-utils</code>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9397">#9397</a> Fix async iterators (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://github-redirect.dependabot.com/webdriverio/webdriverio/pull/9392">#9392</a> Add docs for Accessibility Testing (<a href="https://github.com/christian-bromann"><code>@​christian-bromann</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webdriverio/webdriverio/commit/ab58bc79c1df2e146d02a68ee444766ec371e6d2"><code>ab58bc7</code></a> v8.0.14</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/e233109633c5576e1edbf25adfb4ad6cdfd39b19"><code>e233109</code></a> enforce curly brackets</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/62e24d4dd9d58f3b4168866189d60e7e8da09a9b"><code>62e24d4</code></a> Adding new EsLint rules (<a href="https://github.com/webdriverio/webdriverio/tree/HEAD/packages/wdio-mocha-framework/issues/9445">#9445</a>)</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/912db21d2cd4552a02b776ba74cae05440b076de"><code>912db21</code></a> v8.0.13</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/22627575a41d9dc7415a2441bd894c0419725334"><code>2262757</code></a> v8.0.11</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/1c350a14144ecc5f1ebc598c385bae6aa80739c3"><code>1c350a1</code></a> v8.0.10</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/f92405a6bab7d0409d3b2777e8d65aaa493a4899"><code>f92405a</code></a> v8.0.9</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/c07255fefc67137fd27f23da5f0792c10157f8c0"><code>c07255f</code></a> v8.0.8</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/a874a82a727634d1323fff05c17455ba0907a020"><code>a874a82</code></a> v8.0.7</li>
<li><a href="https://github.com/webdriverio/webdriverio/commit/4f63a94a3af029401d652ff1d0fa36e9057f553c"><code>4f63a94</code></a> v8.0.6</li>
<li>Additional commits viewable in <a href="https://github.com/webdriverio/webdriverio/commits/v8.0.14/packages/wdio-mocha-framework">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~wdio-user">wdio-user</a>, a new releaser for <code>@​wdio/mocha-framework</code> since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-30 23:37:51 +0000 UTC
    </div>
</div>

