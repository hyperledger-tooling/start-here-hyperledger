---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/510" class=".btn">#510</a>
            </td>
            <td>
                <b>
                    Added checks for few private data collection parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

Added missing parameter checks to copy sdk's field to fabric's for private data collection fields


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 13:39:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/509" class=".btn">#509</a>
            </td>
            <td>
                <b>
                    Bump protobufjs from 6.11.3 to 7.2.4 in /packages/stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.11.3 to 7.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>protobufjs: v7.2.4</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2>protobufjs: v7.2.3</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
<h2>protobufjs: v7.2.2</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.1...protobufjs-v7.2.2">7.2.2</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab">14f0536</a>)</li>
</ul>
<h2>protobufjs: v7.2.1</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.0...protobufjs-v7.2.1">7.2.1</a> (2023-02-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>cli:</strong> fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2">e42eea4</a>)</li>
<li>Revert &quot;fix: error should be thrown&quot; (<a href="https://github.com/protobufjs/protobuf.js/commit/4489fa771464bcb49b57149760e9cc4131e8077e">4489fa7</a>)</li>
<li>use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83">dce9a2e</a>)</li>
<li>use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745">64e8936</a>)</li>
</ul>
<h2>protobufjs: v7.2.0</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.2...protobufjs-v7.2.0">7.2.0</a> (2023-01-24)</h2>
<h3>Features</h3>
<ul>
<li><strong>cli:</strong> generate static files at the granularity of proto messages (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1840">#1840</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/32f2d6a68b27997bd0f7619998695a9fa7a4fd70">32f2d6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>error should be thrown (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1817">#1817</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e7a34897a122342485468999a507626f1ea91507">e7a3489</a>)</li>
</ul>
<h2>protobufjs: v7.1.2</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.1...protobufjs-v7.1.2">7.1.2</a> (2022-09-22)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/master/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.1...protobufjs-v7.2.2">7.2.2</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab">14f0536</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.0...protobufjs-v7.2.1">7.2.1</a> (2023-02-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>cli:</strong> fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2">e42eea4</a>)</li>
<li>Revert &quot;fix: error should be thrown&quot; (<a href="https://github.com/protobufjs/protobuf.js/commit/4489fa771464bcb49b57149760e9cc4131e8077e">4489fa7</a>)</li>
<li>use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83">dce9a2e</a>)</li>
<li>use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745">64e8936</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.2...protobufjs-v7.2.0">7.2.0</a> (2023-01-24)</h2>
<h3>Features</h3>
<ul>
<li><strong>cli:</strong> generate static files at the granularity of proto messages (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1840">#1840</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/32f2d6a68b27997bd0f7619998695a9fa7a4fd70">32f2d6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>error should be thrown (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1817">#1817</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e7a34897a122342485468999a507626f1ea91507">e7a3489</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.1...protobufjs-v7.1.2">7.1.2</a> (2022-09-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>types:</strong> nested object can be a oneof (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1812">#1812</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/119d90aa1ce14d7bff20bb1dcc1ddc4544a80c23">119d90a</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/42e5a9ca85044800b16e193020e1d4d2e6b4010c"><code>42e5a9c</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1900">#1900</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d"><code>e66379f</code></a> fix: do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/56b1e64979dae757b67a21d326e16acee39f2267"><code>56b1e64</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1879">#1879</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8"><code>8817ee6</code></a> fix: type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e721d04dad42603e2f7f262b03cb9bd01f8adaa1"><code>e721d04</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1867">#1867</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab"><code>14f0536</code></a> fix: do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/644d588c0495da6a570344248e1b5af901bc3b0c"><code>644d588</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1865">#1865</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2"><code>e42eea4</code></a> fix(cli): fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83"><code>dce9a2e</code></a> fix: use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745"><code>64e8936</code></a> fix: use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.3...protobufjs-v7.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.11.3&new-version=7.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 22:32:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    Bump protobufjs from 6.11.3 to 7.2.4 in /packages/athena
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.11.3 to 7.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>protobufjs: v7.2.4</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2>protobufjs: v7.2.3</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
<h2>protobufjs: v7.2.2</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.1...protobufjs-v7.2.2">7.2.2</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab">14f0536</a>)</li>
</ul>
<h2>protobufjs: v7.2.1</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.0...protobufjs-v7.2.1">7.2.1</a> (2023-02-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>cli:</strong> fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2">e42eea4</a>)</li>
<li>Revert &quot;fix: error should be thrown&quot; (<a href="https://github.com/protobufjs/protobuf.js/commit/4489fa771464bcb49b57149760e9cc4131e8077e">4489fa7</a>)</li>
<li>use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83">dce9a2e</a>)</li>
<li>use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745">64e8936</a>)</li>
</ul>
<h2>protobufjs: v7.2.0</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.2...protobufjs-v7.2.0">7.2.0</a> (2023-01-24)</h2>
<h3>Features</h3>
<ul>
<li><strong>cli:</strong> generate static files at the granularity of proto messages (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1840">#1840</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/32f2d6a68b27997bd0f7619998695a9fa7a4fd70">32f2d6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>error should be thrown (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1817">#1817</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e7a34897a122342485468999a507626f1ea91507">e7a3489</a>)</li>
</ul>
<h2>protobufjs: v7.1.2</h2>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.1...protobufjs-v7.1.2">7.1.2</a> (2022-09-22)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/master/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.3...protobufjs-v7.2.4">7.2.4</a> (2023-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d">e66379f</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.2...protobufjs-v7.2.3">7.2.3</a> (2023-03-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8">8817ee6</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.1...protobufjs-v7.2.2">7.2.2</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab">14f0536</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.2.0...protobufjs-v7.2.1">7.2.1</a> (2023-02-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>cli:</strong> fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2">e42eea4</a>)</li>
<li>Revert &quot;fix: error should be thrown&quot; (<a href="https://github.com/protobufjs/protobuf.js/commit/4489fa771464bcb49b57149760e9cc4131e8077e">4489fa7</a>)</li>
<li>use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83">dce9a2e</a>)</li>
<li>use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745">64e8936</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.2...protobufjs-v7.2.0">7.2.0</a> (2023-01-24)</h2>
<h3>Features</h3>
<ul>
<li><strong>cli:</strong> generate static files at the granularity of proto messages (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1840">#1840</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/32f2d6a68b27997bd0f7619998695a9fa7a4fd70">32f2d6a</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>error should be thrown (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1817">#1817</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/e7a34897a122342485468999a507626f1ea91507">e7a3489</a>)</li>
</ul>
<h2><a href="https://github.com/protobufjs/protobuf.js/compare/protobufjs-v7.1.1...protobufjs-v7.1.2">7.1.2</a> (2022-09-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>types:</strong> nested object can be a oneof (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1812">#1812</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/119d90aa1ce14d7bff20bb1dcc1ddc4544a80c23">119d90a</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/42e5a9ca85044800b16e193020e1d4d2e6b4010c"><code>42e5a9c</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1900">#1900</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e66379f451b0393c27d87b37fa7d271619e16b0d"><code>e66379f</code></a> fix: do not let setProperty change the prototype (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1899">#1899</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/56b1e64979dae757b67a21d326e16acee39f2267"><code>56b1e64</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1879">#1879</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/8817ee613dfcf55f7f6fa8704f3fdd3e68c0e1d8"><code>8817ee6</code></a> fix: type names can be split into multiple tokens (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1877">#1877</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e721d04dad42603e2f7f262b03cb9bd01f8adaa1"><code>e721d04</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1867">#1867</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/14f05364a04fe1ca0bfb278b3407e058c6b5a1ab"><code>14f0536</code></a> fix: do not allow to extend same field twice to prevent the error (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1784">#1784</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/644d588c0495da6a570344248e1b5af901bc3b0c"><code>644d588</code></a> chore: release master (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1865">#1865</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/e42eea4868b11f4a07934804a56683321ed191e2"><code>e42eea4</code></a> fix(cli): fix relative path to Google pb files (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1859">#1859</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/dce9a2ef92d363752e40b295b0da9bd178f82e83"><code>dce9a2e</code></a> fix: use bundled filename to fix common pb includes (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1860">#1860</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/64e8936ad9f73c68b3fa1e57857dd38323b5a745"><code>64e8936</code></a> fix: use ES5 style function syntax (<a href="https://redirect.github.com/protobufjs/protobuf.js/issues/1830">#1830</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.3...protobufjs-v7.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.11.3&new-version=7.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 22:31:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    Updated login text to work with both IBP and HFL Support console
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
Updated login text to work with both IBP and HFL Support console

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 06:37:41 +0000 UTC
    </div>
</div>

