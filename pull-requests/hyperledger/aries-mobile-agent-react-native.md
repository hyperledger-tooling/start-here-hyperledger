---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    chore(deps): bump shell-quote and @react-native-community/cli-tools in /core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/ljharb/shell-quote) and [@react-native-community/cli-tools](https://github.com/react-native-community/cli/tree/HEAD/packages/tools). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/shell-quote/blob/main/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.7.3...v1.7.4">v1.7.4</a> - 2022-10-12</h2>
<h3>Merged</h3>
<ul>
<li>Add node_modules to .gitignore <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/48"><code>[#48](https://github.com/ljharb/shell-quote/issues/48)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a></li>
<li>[eslint] additional cleanup <a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a></li>
<li>[eslint] add eslint <a href="https://github.com/ljharb/shell-quote/commit/6ee1437df1b10a79bdf2aaa04f2bacc9f420dc15"><code>6ee1437</code></a></li>
<li>[readme] rename, add badges <a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a></li>
<li>[meta] update URLs <a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/ljharb/shell-quote/commit/f97411ef4d2f183200fc8a28beca9faf9b08a640"><code>f97411e</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/ljharb/shell-quote/commit/051f60857ad5035280208abdc348bf5ba42a6254"><code>051f608</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/ljharb/shell-quote/commit/dc1cc12b956ccd93d58aaaad263bee7d50576d27"><code>dc1cc12</code></a></li>
</ul>
<!-- raw HTML omitted -->
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
<h2>1.7.2</h2>
<ul>
<li>Fix a regression introduced in 1.6.3. This reverts the Windows path quoting fix. (<a href="https://github.com/ljharb/shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c">144e1c2</a>)</li>
</ul>
<h2>1.7.1</h2>
<ul>
<li>Fix <code>$</code> being removed when not part of an environment variable name. (<a href="https://github.com/Admin"><code>@​Adman</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/32">#32</a>)</li>
</ul>
<h2>1.7.0</h2>
<ul>
<li>Add support for parsing <code>&gt;&gt;</code> and <code>&gt;&amp;</code> redirection operators. (<a href="https://github.com/forivall"><code>@​forivall</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/16">#16</a>)</li>
<li>Add support for parsing <code>&lt;(</code> process substitution operator. (<a href="https://github.com/cuonglm"><code>@​cuonglm</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/15">#15</a>)</li>
</ul>
<h2>1.6.3</h2>
<ul>
<li>Fix Windows path quoting problems. (<a href="https://github.com/dy"><code>@​dy</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/34">#34</a>)</li>
</ul>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.6.2">v1.6.2</a> - 2019-08-13</h2>
<h3>Merged</h3>
<ul>
<li>Use native JSON and Array methods <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/21"><code>[#21](https://github.com/ljharb/shell-quote/issues/21)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>fix whitespace <a href="https://github.com/ljharb/shell-quote/commit/72fb5a8ce29b4f67f28302af33c217b58f92e260"><code>72fb5a8</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/shell-quote/commit/5409e72ef6c905c4d1637883cd394f6f07abd934"><code>5409e72</code></a> v1.7.4</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a> [actions] add reusable workflows</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a> [meta] create FUNDING.yml; add <code>funding</code> in package.json</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a> [meta] add <code>auto-changelog</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a> [readme] rename, add badges</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a> [meta] update URLs</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a> [eslint] additional cleanup</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a> [eslint] fix indentation and whitespace</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.7.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for shell-quote since your current version.</p>
</details>
<br />

Updates `@react-native-community/cli-tools` from 6.1.0 to 6.2.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/react-native-community/cli/releases"><code>@​react-native-community/cli-tools</code>'s releases</a>.</em></p>
<blockquote>
<h2>v6.2.0</h2>
<h2>Features</h2>
<ul>
<li>support renamed <code>-PreactNativeArchitectures</code> (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1496">#1496</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li>better Handle EPERM on Windows (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1495">#1495</a>)</li>
<li>use <code>simclt</code> instead of deprecated <code>instruments</code> (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1484">#1484</a>)</li>
<li>platform-ios: add missing <code>ora</code> dependency (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1483">#1483</a>)</li>
</ul>
<h2>Chore &amp; Maintenance</h2>
<ul>
<li>bump lerna to 4 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1504">#1504</a>)</li>
<li>bump chalk to 4.x (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1505">#1505</a>)</li>
<li>GH Actions: lint &amp; unit tests (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1499">#1499</a>)</li>
<li>remove mkdirp (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1500">#1500</a>)</li>
<li>add 6.1.0 release to compatibility table (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1501">#1501</a>)</li>
<li>replace azure with github actions (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1494">#1494</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-native-community/cli/commit/7a10b39160d53caf43f36ae9e62d4bed942003ea"><code>7a10b39</code></a> Publish</li>
<li><a href="https://github.com/react-native-community/cli/commit/a327ac86983d8b1dc8020f4d10c27d0764695a25"><code>a327ac8</code></a> chore(deps): bump shell-quote to 1.7.3 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1642">#1642</a>)</li>
<li><a href="https://github.com/react-native-community/cli/commit/908eac093d84ef0a5786e3de0f480519ddcc3ecb"><code>908eac0</code></a> v6.2.0</li>
<li><a href="https://github.com/react-native-community/cli/commit/1ac43cce3df75bff069558ac13e8314a17d892e4"><code>1ac43cc</code></a> bump chalk to 4.x (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1505">#1505</a>)</li>
<li><a href="https://github.com/react-native-community/cli/commit/ad0883d8e9b20e30e85adacbfc0b525df5d72840"><code>ad0883d</code></a> chore(deps): remove mkdirp (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1500">#1500</a>)</li>
<li>See full diff in <a href="https://github.com/react-native-community/cli/commits/@react-native-community/cli-tools@6.2.1/packages/tools">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 21:08:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    chore(deps): bump shell-quote and @react-native-community/cli-tools in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shell-quote](https://github.com/ljharb/shell-quote) and [@react-native-community/cli-tools](https://github.com/react-native-community/cli/tree/HEAD/packages/tools). These dependencies needed to be updated together.
Updates `shell-quote` from 1.6.1 to 1.7.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/shell-quote/blob/main/CHANGELOG.md">shell-quote's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.7.3...v1.7.4">v1.7.4</a> - 2022-10-12</h2>
<h3>Merged</h3>
<ul>
<li>Add node_modules to .gitignore <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/48"><code>[#48](https://github.com/ljharb/shell-quote/issues/48)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>[eslint] fix indentation and whitespace <a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a></li>
<li>[eslint] additional cleanup <a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a></li>
<li>[meta] add <code>auto-changelog</code> <a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a></li>
<li>[actions] add reusable workflows <a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a></li>
<li>[eslint] add eslint <a href="https://github.com/ljharb/shell-quote/commit/6ee1437df1b10a79bdf2aaa04f2bacc9f420dc15"><code>6ee1437</code></a></li>
<li>[readme] rename, add badges <a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a></li>
<li>[meta] update URLs <a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a></li>
<li>[meta] create FUNDING.yml; add <code>funding</code> in package.json <a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a></li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file <a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a></li>
<li>Only apps should have lockfiles <a href="https://github.com/ljharb/shell-quote/commit/f97411ef4d2f183200fc8a28beca9faf9b08a640"><code>f97411e</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/ljharb/shell-quote/commit/051f60857ad5035280208abdc348bf5ba42a6254"><code>051f608</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a></li>
<li>[Tests] add <code>aud</code> in <code>posttest</code> <a href="https://github.com/ljharb/shell-quote/commit/dc1cc12b956ccd93d58aaaad263bee7d50576d27"><code>dc1cc12</code></a></li>
</ul>
<!-- raw HTML omitted -->
<h2>1.7.3</h2>
<ul>
<li>Fix a security issue where the regex for windows drive letters allowed some shell meta-characters
to escape the quoting rules. (CVE-2021-42740)</li>
</ul>
<h2>1.7.2</h2>
<ul>
<li>Fix a regression introduced in 1.6.3. This reverts the Windows path quoting fix. (<a href="https://github.com/ljharb/shell-quote/commit/144e1c20cd57549a414c827fb3032e60b7b8721c">144e1c2</a>)</li>
</ul>
<h2>1.7.1</h2>
<ul>
<li>Fix <code>$</code> being removed when not part of an environment variable name. (<a href="https://github.com/Admin"><code>@​Adman</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/32">#32</a>)</li>
</ul>
<h2>1.7.0</h2>
<ul>
<li>Add support for parsing <code>&gt;&gt;</code> and <code>&gt;&amp;</code> redirection operators. (<a href="https://github.com/forivall"><code>@​forivall</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/16">#16</a>)</li>
<li>Add support for parsing <code>&lt;(</code> process substitution operator. (<a href="https://github.com/cuonglm"><code>@​cuonglm</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/15">#15</a>)</li>
</ul>
<h2>1.6.3</h2>
<ul>
<li>Fix Windows path quoting problems. (<a href="https://github.com/dy"><code>@​dy</code></a> in <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/34">#34</a>)</li>
</ul>
<h2><a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.6.2">v1.6.2</a> - 2019-08-13</h2>
<h3>Merged</h3>
<ul>
<li>Use native JSON and Array methods <a href="https://github-redirect.dependabot.com/ljharb/shell-quote/pull/21"><code>[#21](https://github.com/ljharb/shell-quote/issues/21)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>fix whitespace <a href="https://github.com/ljharb/shell-quote/commit/72fb5a8ce29b4f67f28302af33c217b58f92e260"><code>72fb5a8</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/shell-quote/commit/5409e72ef6c905c4d1637883cd394f6f07abd934"><code>5409e72</code></a> v1.7.4</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/4763c36274c5881a2d141ce9f2b17b7d1d95e8cd"><code>4763c36</code></a> [actions] add reusable workflows</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/86415722d875578adf1f95f9e649ba42c805bc32"><code>8641572</code></a> [meta] create FUNDING.yml; add <code>funding</code> in package.json</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/497fca509af3b7d6daaba459bad1f45ac0af3ff1"><code>497fca5</code></a> [meta] add <code>auto-changelog</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/7eb513483d931602452ec572ed456714148acd2b"><code>7eb5134</code></a> [readme] rename, add badges</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/67381b61fa95e57819333463f491428747893186"><code>67381b6</code></a> [meta] update URLs</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/2e2007a393f90bf079fc556a921120b3508c4fc3"><code>2e2007a</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/18cadf95357392fcd78ea8619956fd41eed62649"><code>18cadf9</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/ljharb/shell-quote/commit/397cb628f3d96e4e47763147c0d6074997a13880"><code>397cb62</code></a> [eslint] additional cleanup</li>
<li><a href="https://github.com/ljharb/shell-quote/commit/aaa9d1f65bf3445e6af1efaa4a8f8c13a21aa593"><code>aaa9d1f</code></a> [eslint] fix indentation and whitespace</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/shell-quote/compare/1.6.1...v1.7.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for shell-quote since your current version.</p>
</details>
<br />

Updates `@react-native-community/cli-tools` from 6.2.0 to 6.2.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-native-community/cli/commit/7a10b39160d53caf43f36ae9e62d4bed942003ea"><code>7a10b39</code></a> Publish</li>
<li><a href="https://github.com/react-native-community/cli/commit/a327ac86983d8b1dc8020f4d10c27d0764695a25"><code>a327ac8</code></a> chore(deps): bump shell-quote to 1.7.3 (<a href="https://github.com/react-native-community/cli/tree/HEAD/packages/tools/issues/1642">#1642</a>)</li>
<li>See full diff in <a href="https://github.com/react-native-community/cli/commits/@react-native-community/cli-tools@6.2.1/packages/tools">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 21:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    chore: update core AFJ to 0.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

Updates core AFJ module to 0.2.2 to align with app.

# Related Issues

#491 

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [ ] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 20:30:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    feat: card rendering using flexbox layout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This new simplified rendering strat relies on [Flexbox Layout](https://reactnative.dev/docs/flexbox) and automatically image scaling. As part of this automatic scaling the logo images MUST be provided in a predefined aspect ratio: 1:1  (width:height) for logos that shows issuer name, or `4:1` (width:height) for when the issuer name is hidden.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 01:11:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    changed core/App folder to core/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

# Summary of Changes

Changed outdated core/App folder to core/src folder. This makes the file structure easier to understand

# Related Issues

Resolves: #408 

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 22:19:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    chore(deps): bump @xmldom/xmldom from 0.7.5 to 0.7.6 in /app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@xmldom/xmldom](https://github.com/xmldom/xmldom) from 0.7.5 to 0.7.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/releases"><code>@​xmldom/xmldom</code>'s releases</a>.</em></p>
<blockquote>
<h2>0.7.6</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/441"><code>[#441](https://github.com/xmldom/xmldom/issues/441)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/jftanner"><code>@​jftanner</code></a>, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/blob/master/CHANGELOG.md"><code>@​xmldom/xmldom</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">0.7.6</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/441"><code>[#441](https://github.com/xmldom/xmldom/issues/441)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/jftanner"><code>@​jftanner</code></a>, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.3...0.8.2">0.8.3</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.1...0.9.0-beta.2">0.9.0-beta.2</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.3...0.8.2">0.8.3</a></h2>
<h3>Fixed</h3>
<ul>
<li>Avoid iterating over prototype properties <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/437"><code>[#437](https://github.com/xmldom/xmldom/issues/437)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/436"><code>[#436](https://github.com/xmldom/xmldom/issues/436)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/Supraja9726"><code>@​Supraja9726</code></a> for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.2...0.9.0-beta.1">0.9.0-beta.1</a></h2>
<h3>Fixed</h3>
<p><strong>Only use HTML rules if mimeType matches</strong> <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/338"><code>[#338](https://github.com/xmldom/xmldom/issues/338)</code></a>, fixes <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/203"><code>[#203](https://github.com/xmldom/xmldom/issues/203)</code></a></p>
<p>In the living specs for parsing XML and HTML, that this library is trying to implement,
there is a distinction between the different types of documents being parsed:
There are quite some rules that are different for parsing, constructing and serializing XML vs HTML documents.</p>
<p>So far xmldom was always &quot;detecting&quot; whether &quot;the HTML rules should be applied&quot; by looking at the current namespace. So from the first time an the HTML default namespace (<code>http://www.w3.org/1999/xhtml</code>) was found, every node was treated as being part of an HTML document. This misconception is the root cause for quite some reported bugs.</p>
<p>BREAKING CHANGE: HTML rules are no longer applied just because of the namespace, but require the <code>mimeType</code> argument passed to <code>DOMParser.parseFromString(source, mimeType)</code> to match <code>'text/html'</code>. Doing so implies all rules for handling casing for tag and attribute names when parsing, creation of nodes and searching nodes.</p>
<p>BREAKING CHANGE: Correct the return type of <code>DOMParser.parseFromString</code> to <code>Document | undefined</code>. In case of parsing errors it was always possible that &quot;the returned <code>Document</code>&quot; has not been created. In case you are using Typescript you now need to handle those cases.</p>
<p>BREAKING CHANGE: The instance property <code>DOMParser.options</code> is no longer available, instead use the individual <code>readonly</code> property per option (<code>assign</code>, <code>domHandler</code>, <code>errorHandler</code>, <code>normalizeLineEndings</code>, <code>locator</code>, <code>xmlns</code>). Those also provides the default value if the option was not passed. The 'locator' option is now just a boolean (default remains <code>true</code>).</p>
<p>BREAKING CHANGE: The following methods no longer allow a (non spec compliant) boolean argument to toggle &quot;HTML rules&quot;:</p>
<ul>
<li><code>XMLSerializer.serializeToString</code></li>
<li><code>Node.toString</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/xmldom/xmldom/commit/3ca016d7da634686dbcadd076dda07d28a8ffd45"><code>3ca016d</code></a> 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/b28e631b8bc42edca9df6eb68e5b84f78529b3cb"><code>b28e631</code></a> docs: Prepare CHANGELOG for 0.7.6</li>
<li><a href="https://github.com/xmldom/xmldom/commit/1f20aee8ef1a8f3964add1a188f723bbc54862a0"><code>1f20aee</code></a> fix: Backport PR-437 to 0.7.x branch</li>
<li>See full diff in <a href="https://github.com/xmldom/xmldom/compare/0.7.5...0.7.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@xmldom/xmldom&package-manager=npm_and_yarn&previous-version=0.7.5&new-version=0.7.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 21:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    feat: oca image display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR let us use OCA format overlay to display images in the credential details.

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 13:07:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    fix: OCA fix credential logo display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes
Fixing display of credential logo

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 22:58:31 +0000 UTC
    </div>
</div>

