---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    build(deps): bump react-router-dom from 6.24.0 to 6.25.1 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-router-dom](https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom) from 6.24.0 to 6.25.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remix-run/react-router/releases">react-router-dom's releases</a>.</em></p>
<blockquote>
<h2>react-router-dom-v5-compat@6.4.0-pre.15</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.15</li>
<li>react-router-dom@6.4.0-pre.15</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.11</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.11</li>
<li>react-router-dom@6.4.0-pre.11</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.10</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.10</li>
<li>react-router-dom@6.4.0-pre.10</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.9</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.9</li>
<li>react-router-dom@6.4.0-pre.9</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.8</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.8</li>
<li>react-router-dom@6.4.0-pre.8</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.7</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li><code>react-router@6.4.0-pre.7</code></li>
<li><code>react-router-dom@6.4.0-pre.7</code></li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.6</h2>
<h3>Patch Changes</h3>
<ul>
<li>44bce3c6: Fix <code>react-router-dom</code> peer dependency version
<ul>
<li>react-router@6.4.0-pre.6</li>
<li>react-router-dom@6.4.0-pre.6</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.5</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/remix-run/react-router/blob/main/packages/react-router-dom/CHANGELOG.md">react-router-dom's changelog</a>.</em></p>
<blockquote>
<h2>6.25.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>Memoize some <code>RouterProvider</code> internals to reduce unnecessary re-renders (<a href="https://redirect.github.com/remix-run/react-router/pull/11803">#11803</a>)</li>
<li>Updated dependencies:
<ul>
<li><code>react-router@6.25.1</code></li>
</ul>
</li>
</ul>
<h2>6.25.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>
<p>Stabilize <code>future.unstable_skipActionErrorRevalidation</code> as <code>future.v7_skipActionErrorRevalidation</code> (<a href="https://redirect.github.com/remix-run/react-router/pull/11769">#11769</a>)</p>
<ul>
<li>When this flag is enabled, actions will not automatically trigger a revalidation if they return/throw a <code>Response</code> with a <code>4xx</code>/<code>5xx</code> status code</li>
<li>You may still opt-into revalidation via <code>shouldRevalidate</code></li>
<li>This also changes <code>shouldRevalidate</code>'s <code>unstable_actionStatus</code> parameter to <code>actionStatus</code></li>
</ul>
</li>
</ul>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies:
<ul>
<li><code>react-router@6.25.0</code></li>
<li><code>@remix-run/router@1.18.0</code></li>
</ul>
</li>
</ul>
<h2>6.24.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>Remove <code>polyfill.io</code> reference from warning message because the domain was sold and has since been determined to serve malware (<a href="https://redirect.github.com/remix-run/react-router/pull/11741">#11741</a>)
<ul>
<li>See <a href="https://sansec.io/research/polyfill-supply-chain-attack">https://sansec.io/research/polyfill-supply-chain-attack</a></li>
</ul>
</li>
<li>Export <code>NavLinkRenderProps</code> type for easier typing of custom <code>NavLink</code> callback (<a href="https://redirect.github.com/remix-run/react-router/pull/11553">#11553</a>)</li>
<li>Updated dependencies:
<ul>
<li><code>@remix-run/router@1.17.1</code></li>
<li><code>react-router@6.24.1</code></li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remix-run/react-router/commit/98941f8886d0a2f08f36d17168e0b7e7400770b0"><code>98941f8</code></a> chore: Update version for release (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11815">#11815</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/db24ec9b2cd957c5cfcc8709556c23683c68c277"><code>db24ec9</code></a> chore: Update version for release (pre) (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11814">#11814</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/a252428492ddaa490bee4a399cf36e5dc85886dc"><code>a252428</code></a> Reduce RouterProvider re-renders when using View Transitions (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11803">#11803</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/6b8daf95d30c3816e52c51990310f6fcbd2506ed"><code>6b8daf9</code></a> Revert &quot;Temporary change to test release process off v6 branch&quot;</li>
<li><a href="https://github.com/remix-run/react-router/commit/b8a4cdb6a36821cd967c4a040a9325e9cc68a6f6"><code>b8a4cdb</code></a> Temporary change to test release process off v6 branch</li>
<li><a href="https://github.com/remix-run/react-router/commit/13dfa13e969f3a175637f9012ac568a70bbcae54"><code>13dfa13</code></a> chore: Update version for release (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11807">#11807</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/21b61c07c2fc66b1e51feeebdc5a6290344b699a"><code>21b61c0</code></a> chore: Update version for release (pre) (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11800">#11800</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/7b22365b9aa7ac230e8d544c24a8265dde107ee7"><code>7b22365</code></a> Stabilize future.unstable_skipActionErrorRevalidation (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11769">#11769</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/da65120ac550ee9a8b0a34e04e7bd4612357ff2a"><code>da65120</code></a> Fix useMatch undecoded params (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11789">#11789</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/0a876444b361d1320450c27f90e6ffd0740fc4d1"><code>0a87644</code></a> chore: Update version for release (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11767">#11767</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/remix-run/react-router/commits/react-router-dom@6.25.1/packages/react-router-dom">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-router-dom&package-manager=npm_and_yarn&previous-version=6.24.0&new-version=6.25.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 12:03:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:59:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:59:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:53:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:53:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:52:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    build(deps): bump uvicorn from 0.30.1 to 0.30.3 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [uvicorn](https://github.com/encode/uvicorn) from 0.30.1 to 0.30.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/releases">uvicorn's releases</a>.</em></p>
<blockquote>
<h2>Version 0.30.3</h2>
<h2>Fixed</h2>
<ul>
<li>Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/uvicorn/compare/0.30.2...0.30.3">https://github.com/encode/uvicorn/compare/0.30.2...0.30.3</a></p>
<h2>0.30.2</h2>
<h2>Added</h2>
<ul>
<li>Add <code>reason</code> support to <a href="https://asgi.readthedocs.io/en/latest/specs/www.html#disconnect-receive-event-ws"><code>websocket.disconnect</code></a> event (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>Iterate subprocesses in-place on the process manager (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/uvicorn/compare/0.30.1...0.30.2">https://github.com/encode/uvicorn/compare/0.30.1...0.30.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/blob/master/CHANGELOG.md">uvicorn's changelog</a>.</em></p>
<blockquote>
<h2>0.30.3 (2024-07-20)</h2>
<h3>Fixed</h3>
<ul>
<li>Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
</ul>
<h2>0.30.2 (2024-07-20)</h2>
<h3>Added</h3>
<ul>
<li>Add <code>reason</code> support to <a href="https://asgi.readthedocs.io/en/latest/specs/www.html#disconnect-receive-event-ws"><code>websocket.disconnect</code></a> event (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Iterate subprocesses in-place on the process manager (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/encode/uvicorn/commit/5bf788f0eb0fc771f5c4eed8f282c7ec256565d2"><code>5bf788f</code></a> Version 0.30.3 (<a href="https://redirect.github.com/encode/uvicorn/issues/2395">#2395</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/8f4c8a7f34914c16650ebd026127b96560425fde"><code>8f4c8a7</code></a> Add 100% clean coverage (<a href="https://redirect.github.com/encode/uvicorn/issues/2394">#2394</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/9baded3dcf1a59b2956a00e875be4bbb6bea162c"><code>9baded3</code></a> Bump the python-packages group with 9 updates (<a href="https://redirect.github.com/encode/uvicorn/issues/2376">#2376</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/92798254173f9c34a7cdc7817a06a99d0394af2a"><code>9279825</code></a> <code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/875f6c6a4d11407de0d46dc04f058eb8f6a244dc"><code>875f6c6</code></a> Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/ca24e1b52ca21e2dbe9c94824e042524fc06b831"><code>ca24e1b</code></a> Version 0.30.2 (<a href="https://redirect.github.com/encode/uvicorn/issues/2380">#2380</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/c23cd24e6676ee0638d014d7000af1e6e0996bd6"><code>c23cd24</code></a> Iterate subprocesses in-place (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/d79f285184404694c77f7ca649858e7488270cf7"><code>d79f285</code></a> docs(readme): add granian as an alternative (<a href="https://redirect.github.com/encode/uvicorn/issues/2359">#2359</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/4e9f48d249a7a3ffe6f48e185596ccd3caaf5915"><code>4e9f48d</code></a> Add <code>reason</code> support on WebSocketDisconnectEvent (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
<li>See full diff in <a href="https://github.com/encode/uvicorn/compare/0.30.1...0.30.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uvicorn&package-manager=pip&previous-version=0.30.1&new-version=0.30.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:51:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest from 8.2.2 to 8.3.1 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:51:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/815" class=".btn">#815</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:51:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/814" class=".btn">#814</a>
            </td>
            <td>
                <b>
                    build(deps): bump google-api-python-client from 2.136.0 to 2.137.0 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [google-api-python-client](https://github.com/googleapis/google-api-python-client) from 2.136.0 to 2.137.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/googleapis/google-api-python-client/releases">google-api-python-client's releases</a>.</em></p>
<blockquote>
<h2>v2.137.0</h2>
<h2><a href="https://github.com/googleapis/google-api-python-client/compare/v2.136.0...v2.137.0">2.137.0</a> (2024-07-09)</h2>
<h3>Features</h3>
<ul>
<li><strong>aiplatform:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/ce2fd6522497bed798011ff2e6bf404146ac4dda">https://togithub.com/googleapis/google-api-python-client/commit/ce2fd6522497bed798011ff2e6bf404146ac4dda</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>alloydb:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/97b5d4d916556ec1dd8010eba5cc9eb9d1e86eeb">https://togithub.com/googleapis/google-api-python-client/commit/97b5d4d916556ec1dd8010eba5cc9eb9d1e86eeb</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>analyticsadmin:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/ae5b795bdd3c073efb676f1bca7ef0f8e6922f8a">https://togithub.com/googleapis/google-api-python-client/commit/ae5b795bdd3c073efb676f1bca7ef0f8e6922f8a</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>assuredworkloads:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/e79f2d5fbb8c46a1ba9855d9ac44a92cad0bdb63">https://togithub.com/googleapis/google-api-python-client/commit/e79f2d5fbb8c46a1ba9855d9ac44a92cad0bdb63</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>backupdr:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/45ce2d1e232dd18d39c8386d088c185735749ae7">https://togithub.com/googleapis/google-api-python-client/commit/45ce2d1e232dd18d39c8386d088c185735749ae7</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>bigquery:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/9c9552326f1cbc523667b9f74bac454b0e383e85">https://togithub.com/googleapis/google-api-python-client/commit/9c9552326f1cbc523667b9f74bac454b0e383e85</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>bigtableadmin:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/b654a04a667bc7454b468d005d04e22a12f061e5">https://togithub.com/googleapis/google-api-python-client/commit/b654a04a667bc7454b468d005d04e22a12f061e5</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>cloudbuild:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/13199354b400eed00398316a41407f5bd3a4bc24">https://togithub.com/googleapis/google-api-python-client/commit/13199354b400eed00398316a41407f5bd3a4bc24</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>clouderrorreporting:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/c8565103936ebfa1cd55d93b25da6f9c3b3d1dcd">https://togithub.com/googleapis/google-api-python-client/commit/c8565103936ebfa1cd55d93b25da6f9c3b3d1dcd</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>contactcenterinsights:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/a41c7aafe9f6d5a6e5b8affd545389f6048aa3c2">https://togithub.com/googleapis/google-api-python-client/commit/a41c7aafe9f6d5a6e5b8affd545389f6048aa3c2</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>containeranalysis:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/8d07b6c7eb5328a30300651a0255ef89ede9a02d">https://togithub.com/googleapis/google-api-python-client/commit/8d07b6c7eb5328a30300651a0255ef89ede9a02d</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>container:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/bee9e2a8f3141163587bdaed02cd4d6d1a9b5dde">https://togithub.com/googleapis/google-api-python-client/commit/bee9e2a8f3141163587bdaed02cd4d6d1a9b5dde</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>dataform:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/0ec97e196743afcd5af48e7df22bc2002849f3af">https://togithub.com/googleapis/google-api-python-client/commit/0ec97e196743afcd5af48e7df22bc2002849f3af</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>datafusion:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/ac09a79a827c66caf0ee86b44b3e093a3c52d2ce">https://togithub.com/googleapis/google-api-python-client/commit/ac09a79a827c66caf0ee86b44b3e093a3c52d2ce</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>dataplex:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/a9c4b03d1e1b4f4f7b178304b89c55577aab59ce">https://togithub.com/googleapis/google-api-python-client/commit/a9c4b03d1e1b4f4f7b178304b89c55577aab59ce</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>discoveryengine:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/0c7f11bf9ad8bab304002383d950af51aaa480da">https://togithub.com/googleapis/google-api-python-client/commit/0c7f11bf9ad8bab304002383d950af51aaa480da</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>dlp:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/1662bdeb78dbcdf30d6b18979187c448bbf07972">https://togithub.com/googleapis/google-api-python-client/commit/1662bdeb78dbcdf30d6b18979187c448bbf07972</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>firebaseappcheck:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/44ba673ce94875eaaee141a681cb9f64d4590d2b">https://togithub.com/googleapis/google-api-python-client/commit/44ba673ce94875eaaee141a681cb9f64d4590d2b</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>firebaseml:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/2f05dafdb071b91e9ed41b050f34096ec7c9ca16">https://togithub.com/googleapis/google-api-python-client/commit/2f05dafdb071b91e9ed41b050f34096ec7c9ca16</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>games:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/b4c52c45b5415be44193de1639d2cd72d463fbce">https://togithub.com/googleapis/google-api-python-client/commit/b4c52c45b5415be44193de1639d2cd72d463fbce</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>integrations:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/43447c55cd301e96e09a580458e73221d13eb8be">https://togithub.com/googleapis/google-api-python-client/commit/43447c55cd301e96e09a580458e73221d13eb8be</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>pubsub:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/04affe4737b93ec400b2e1f7837015f0260ad353">https://togithub.com/googleapis/google-api-python-client/commit/04affe4737b93ec400b2e1f7837015f0260ad353</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>run:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/1969fbafafa34bbc4a041a5687b19a02575ca32f">https://togithub.com/googleapis/google-api-python-client/commit/1969fbafafa34bbc4a041a5687b19a02575ca32f</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>storage:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/fa6fb47da9bca59f3ff668b6a5d10651c9622d8a">https://togithub.com/googleapis/google-api-python-client/commit/fa6fb47da9bca59f3ff668b6a5d10651c9622d8a</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>tagmanager:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/861f77cb5acd7d7dd0f523206f0ce7c8eb12abf2">https://togithub.com/googleapis/google-api-python-client/commit/861f77cb5acd7d7dd0f523206f0ce7c8eb12abf2</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>vmmigration:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/d9305fc5c6bc6767c13668ac887c606b07a7c3a9">https://togithub.com/googleapis/google-api-python-client/commit/d9305fc5c6bc6767c13668ac887c606b07a7c3a9</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>vmwareengine:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/3d7665ddd712b2ead212b56e951c61ff47bdb559">https://togithub.com/googleapis/google-api-python-client/commit/3d7665ddd712b2ead212b56e951c61ff47bdb559</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
<li><strong>workloadmanager:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/4584750203673447ee60b602bcefea0eb658de49">https://togithub.com/googleapis/google-api-python-client/commit/4584750203673447ee60b602bcefea0eb658de49</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><strong>connectors:</strong> Update the api <a href="https://togithub.com/googleapis/google-api-python-client/commit/62aa538fbc0230137ff057766a0f10df98b24e2d">https://togithub.com/googleapis/google-api-python-client/commit/62aa538fbc0230137ff057766a0f10df98b24e2d</a> (<a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862">26e27a9</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/googleapis/google-api-python-client/commit/74de4f0c0d19d93e3a8313740cc9f4c61eab5aa6"><code>74de4f0</code></a> chore(main): release 2.137.0 (<a href="https://redirect.github.com/googleapis/google-api-python-client/issues/2436">#2436</a>)</li>
<li><a href="https://github.com/googleapis/google-api-python-client/commit/26e27a9d459e66efae363f6e968978521f19e862"><code>26e27a9</code></a> chore: Update discovery artifacts (<a href="https://redirect.github.com/googleapis/google-api-python-client/issues/2435">#2435</a>)</li>
<li><a href="https://github.com/googleapis/google-api-python-client/commit/9e30af7f5d9e487a6599142afbb18f651e4bd3fb"><code>9e30af7</code></a> chore: update templated files (<a href="https://redirect.github.com/googleapis/google-api-python-client/issues/2430">#2430</a>)</li>
<li>See full diff in <a href="https://github.com/googleapis/google-api-python-client/compare/v2.136.0...v2.137.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google-api-python-client&package-manager=pip&previous-version=2.136.0&new-version=2.137.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/813" class=".btn">#813</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/812" class=".btn">#812</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /connection_update/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:44:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/811" class=".btn">#811</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:43:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/810" class=".btn">#810</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /connection_update/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:43:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/809" class=".btn">#809</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:43:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/808" class=".btn">#808</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest from 8.2.2 to 8.3.1 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/807" class=".btn">#807</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /basicmessage_storage/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:42:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/806" class=".btn">#806</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /basicmessage_storage/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:42:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    build(deps): bump uvicorn from 0.30.1 to 0.30.3 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [uvicorn](https://github.com/encode/uvicorn) from 0.30.1 to 0.30.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/releases">uvicorn's releases</a>.</em></p>
<blockquote>
<h2>Version 0.30.3</h2>
<h2>Fixed</h2>
<ul>
<li>Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/uvicorn/compare/0.30.2...0.30.3">https://github.com/encode/uvicorn/compare/0.30.2...0.30.3</a></p>
<h2>0.30.2</h2>
<h2>Added</h2>
<ul>
<li>Add <code>reason</code> support to <a href="https://asgi.readthedocs.io/en/latest/specs/www.html#disconnect-receive-event-ws"><code>websocket.disconnect</code></a> event (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>Iterate subprocesses in-place on the process manager (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/uvicorn/compare/0.30.1...0.30.2">https://github.com/encode/uvicorn/compare/0.30.1...0.30.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/blob/master/CHANGELOG.md">uvicorn's changelog</a>.</em></p>
<blockquote>
<h2>0.30.3 (2024-07-20)</h2>
<h3>Fixed</h3>
<ul>
<li>Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
</ul>
<h2>0.30.2 (2024-07-20)</h2>
<h3>Added</h3>
<ul>
<li>Add <code>reason</code> support to <a href="https://asgi.readthedocs.io/en/latest/specs/www.html#disconnect-receive-event-ws"><code>websocket.disconnect</code></a> event (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Iterate subprocesses in-place on the process manager (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/encode/uvicorn/commit/5bf788f0eb0fc771f5c4eed8f282c7ec256565d2"><code>5bf788f</code></a> Version 0.30.3 (<a href="https://redirect.github.com/encode/uvicorn/issues/2395">#2395</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/8f4c8a7f34914c16650ebd026127b96560425fde"><code>8f4c8a7</code></a> Add 100% clean coverage (<a href="https://redirect.github.com/encode/uvicorn/issues/2394">#2394</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/9baded3dcf1a59b2956a00e875be4bbb6bea162c"><code>9baded3</code></a> Bump the python-packages group with 9 updates (<a href="https://redirect.github.com/encode/uvicorn/issues/2376">#2376</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/92798254173f9c34a7cdc7817a06a99d0394af2a"><code>9279825</code></a> <code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/875f6c6a4d11407de0d46dc04f058eb8f6a244dc"><code>875f6c6</code></a> Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/ca24e1b52ca21e2dbe9c94824e042524fc06b831"><code>ca24e1b</code></a> Version 0.30.2 (<a href="https://redirect.github.com/encode/uvicorn/issues/2380">#2380</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/c23cd24e6676ee0638d014d7000af1e6e0996bd6"><code>c23cd24</code></a> Iterate subprocesses in-place (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/d79f285184404694c77f7ca649858e7488270cf7"><code>d79f285</code></a> docs(readme): add granian as an alternative (<a href="https://redirect.github.com/encode/uvicorn/issues/2359">#2359</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/4e9f48d249a7a3ffe6f48e185596ccd3caaf5915"><code>4e9f48d</code></a> Add <code>reason</code> support on WebSocketDisconnectEvent (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
<li>See full diff in <a href="https://github.com/encode/uvicorn/compare/0.30.1...0.30.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uvicorn&package-manager=pip&previous-version=0.30.1&new-version=0.30.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:40:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:40:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/802" class=".btn">#802</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /firebase_push_notifications/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:36:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /firebase_push_notifications/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:36:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/800" class=".btn">#800</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:36:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/799" class=".btn">#799</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:35:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/798" class=".btn">#798</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest from 8.2.2 to 8.3.1 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    build(deps): bump uvicorn from 0.30.1 to 0.30.3 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [uvicorn](https://github.com/encode/uvicorn) from 0.30.1 to 0.30.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/releases">uvicorn's releases</a>.</em></p>
<blockquote>
<h2>Version 0.30.3</h2>
<h2>Fixed</h2>
<ul>
<li>Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/uvicorn/compare/0.30.2...0.30.3">https://github.com/encode/uvicorn/compare/0.30.2...0.30.3</a></p>
<h2>0.30.2</h2>
<h2>Added</h2>
<ul>
<li>Add <code>reason</code> support to <a href="https://asgi.readthedocs.io/en/latest/specs/www.html#disconnect-receive-event-ws"><code>websocket.disconnect</code></a> event (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>Iterate subprocesses in-place on the process manager (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
</ul>
<hr />
<p><strong>Full Changelog</strong>: <a href="https://github.com/encode/uvicorn/compare/0.30.1...0.30.2">https://github.com/encode/uvicorn/compare/0.30.1...0.30.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/blob/master/CHANGELOG.md">uvicorn's changelog</a>.</em></p>
<blockquote>
<h2>0.30.3 (2024-07-20)</h2>
<h3>Fixed</h3>
<ul>
<li>Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
</ul>
<h2>0.30.2 (2024-07-20)</h2>
<h3>Added</h3>
<ul>
<li>Add <code>reason</code> support to <a href="https://asgi.readthedocs.io/en/latest/specs/www.html#disconnect-receive-event-ws"><code>websocket.disconnect</code></a> event (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Iterate subprocesses in-place on the process manager (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/encode/uvicorn/commit/5bf788f0eb0fc771f5c4eed8f282c7ec256565d2"><code>5bf788f</code></a> Version 0.30.3 (<a href="https://redirect.github.com/encode/uvicorn/issues/2395">#2395</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/8f4c8a7f34914c16650ebd026127b96560425fde"><code>8f4c8a7</code></a> Add 100% clean coverage (<a href="https://redirect.github.com/encode/uvicorn/issues/2394">#2394</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/9baded3dcf1a59b2956a00e875be4bbb6bea162c"><code>9baded3</code></a> Bump the python-packages group with 9 updates (<a href="https://redirect.github.com/encode/uvicorn/issues/2376">#2376</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/92798254173f9c34a7cdc7817a06a99d0394af2a"><code>9279825</code></a> <code>ClientDisconnect</code> inherits from <code>OSError</code> instead of <code>IOError</code> (<a href="https://redirect.github.com/encode/uvicorn/issues/2393">#2393</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/875f6c6a4d11407de0d46dc04f058eb8f6a244dc"><code>875f6c6</code></a> Suppress <code>KeyboardInterrupt</code> from CLI and programmatic usage (<a href="https://redirect.github.com/encode/uvicorn/issues/2384">#2384</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/ca24e1b52ca21e2dbe9c94824e042524fc06b831"><code>ca24e1b</code></a> Version 0.30.2 (<a href="https://redirect.github.com/encode/uvicorn/issues/2380">#2380</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/c23cd24e6676ee0638d014d7000af1e6e0996bd6"><code>c23cd24</code></a> Iterate subprocesses in-place (<a href="https://redirect.github.com/encode/uvicorn/issues/2373">#2373</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/d79f285184404694c77f7ca649858e7488270cf7"><code>d79f285</code></a> docs(readme): add granian as an alternative (<a href="https://redirect.github.com/encode/uvicorn/issues/2359">#2359</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/4e9f48d249a7a3ffe6f48e185596ccd3caaf5915"><code>4e9f48d</code></a> Add <code>reason</code> support on WebSocketDisconnectEvent (<a href="https://redirect.github.com/encode/uvicorn/issues/2324">#2324</a>)</li>
<li>See full diff in <a href="https://github.com/encode/uvicorn/compare/0.30.1...0.30.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uvicorn&package-manager=pip&previous-version=0.30.1&new-version=0.30.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:34:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/795" class=".btn">#795</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:32:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:31:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/793" class=".btn">#793</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:23:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/792" class=".btn">#792</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:23:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/791" class=".btn">#791</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest from 8.2.2 to 8.3.1 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:22:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/789" class=".btn">#789</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest from 8.2.2 to 8.3.1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:19:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/788" class=".btn">#788</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:19:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/787" class=".btn">#787</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:19:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/786" class=".btn">#786</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:19:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/785" class=".btn">#785</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:19:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/784" class=".btn">#784</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /rpc/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:19:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/783" class=".btn">#783</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /rpc/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:18:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/780" class=".btn">#780</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-asyncio from 0.23.7 to 0.23.8 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:12:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/779" class=".btn">#779</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-ruff from 0.3.2 to 0.4.1 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:11:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/778" class=".btn">#778</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump ruff from 0.5.2 to 0.5.4 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:11:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/777" class=".btn">#777</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest from 8.2.2 to 8.3.1 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:11:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/776" class=".btn">#776</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest-asyncio from 0.23.7 to 0.23.8 in /multitenant_provider/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/775" class=".btn">#775</a>
            </td>
            <td>
                <b>
                    build(deps): bump pytest from 8.2.2 to 8.3.1 in /multitenant_provider/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:09:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/774" class=".btn">#774</a>
            </td>
            <td>
                <b>
                    Feat/773
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP for the lite plugin stuff
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 15:54:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/772" class=".btn">#772</a>
            </td>
            <td>
                <b>
                    Modular credential format support for oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR, we've restructured the OID4VCI plugin by extracting the JWT credential issuance logic and moving it to a new JWT_VC_JSON plugin. This adjustment enables the OID4VCI plugin to concentrate exclusively on the protocol, eliminating the need to process individual credential formats. This modular approach simplifies the addition of new credential formats in the future without requiring changes to the OID4VCI plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 22:21:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    Library upgrades
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Weekly group upgrades for the libraries reported by dependabot.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 19:51:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/770" class=".btn">#770</a>
            </td>
            <td>
                <b>
                    fix: debug value in cred id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a quick fix for a debug value mistakenly committed in #768.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:47:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/769" class=".btn">#769</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group across 1 directory with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 4 updates in the /oid4vci/integration/credo directory: [semver](https://github.com/npm/node-semver), [expo](https://github.com/expo/expo/tree/HEAD/packages/expo), [ws](https://github.com/websockets/ws) and [braces](https://github.com/micromatch/braces).

Updates `semver` from 5.7.2 to 7.6.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.6.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.4...v7.6.0">7.6.0</a> (2024-01-31)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/a7ab13a46201e342d34e84a989632b380f755baf"><code>a7ab13a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/671">#671</a> preserve pre-release and build parts of a version on coerce (<a href="https://redirect.github.com/npm/node-semver/issues/671">#671</a>) (<a href="https://github.com/madtisa"><code>@​madtisa</code></a>, madtisa, <a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
</ul>
<h3>Chores</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/816c7b2cbfcb1986958a290f941eddfd0441139e"><code>816c7b2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/0bd24d943cbd1a7f6a2b8d384590bfa98559e1de"><code>0bd24d9</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> bump <code>@​npmcli/template-oss</code> from 4.21.1 to 4.21.3 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/e521932f115a81030f4e7c34e8631cdd3c6a108b"><code>e521932</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/88739918080debeb239aae840b35c07436148e50"><code>8873991</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> chore: chore: postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/f317dc8689781bcfd98e2c32b46157276acdd47c"><code>f317dc8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> bump <code>@​npmcli/template-oss</code> from 4.19.0 to 4.21.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/7303db1fe54d6905b23ccb0162878e37d73535ef"><code>7303db1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/658">#658</a> add clean() test for build metadata (<a href="https://redirect.github.com/npm/node-semver/issues/658">#658</a>) (<a href="https://github.com/jethrodaniel"><code>@​jethrodaniel</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6240d75a7c620b0a222f05969a91fdc3dc2be0fb"><code>6240d75</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/656">#656</a> add missing quotes in README.md (<a href="https://redirect.github.com/npm/node-semver/issues/656">#656</a>) (<a href="https://github.com/zyxkad"><code>@​zyxkad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/14d263faa156e408a033b9b12a2f87735c2df42c"><code>14d263f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/7c34e1ac1bcc0bc6579b30745c96075c69bd0332"><code>7c34e1a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> bump <code>@​npmcli/template-oss</code> from 4.18.1 to 4.19.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/123e0b03287e1af295ef82d55f55c16805596f35"><code>123e0b0</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/737d5e1cf10e631bab8a28594aa2d5c9d4090814"><code>737d5e1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> bump <code>@​npmcli/template-oss</code> from 4.18.0 to 4.18.1 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/cce61804ba6f997225a1267135c06676fe0524d2"><code>cce6180</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/b914a3d0d26ca27d2685053d7d390af4e02eedd9"><code>b914a3d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> bump <code>@​npmcli/template-oss</code> from 4.17.0 to 4.18.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
</ul>
<h2>v7.5.4</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.4...v7.6.0">7.6.0</a> (2024-01-31)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/a7ab13a46201e342d34e84a989632b380f755baf"><code>a7ab13a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/671">#671</a> preserve pre-release and build parts of a version on coerce (<a href="https://redirect.github.com/npm/node-semver/issues/671">#671</a>) (<a href="https://github.com/madtisa"><code>@​madtisa</code></a>, madtisa, <a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
</ul>
<h3>Chores</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/816c7b2cbfcb1986958a290f941eddfd0441139e"><code>816c7b2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/0bd24d943cbd1a7f6a2b8d384590bfa98559e1de"><code>0bd24d9</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/667">#667</a> bump <code>@​npmcli/template-oss</code> from 4.21.1 to 4.21.3 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/e521932f115a81030f4e7c34e8631cdd3c6a108b"><code>e521932</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/88739918080debeb239aae840b35c07436148e50"><code>8873991</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> chore: chore: postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/f317dc8689781bcfd98e2c32b46157276acdd47c"><code>f317dc8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/652">#652</a> bump <code>@​npmcli/template-oss</code> from 4.19.0 to 4.21.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/7303db1fe54d6905b23ccb0162878e37d73535ef"><code>7303db1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/658">#658</a> add clean() test for build metadata (<a href="https://redirect.github.com/npm/node-semver/issues/658">#658</a>) (<a href="https://github.com/jethrodaniel"><code>@​jethrodaniel</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6240d75a7c620b0a222f05969a91fdc3dc2be0fb"><code>6240d75</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/656">#656</a> add missing quotes in README.md (<a href="https://redirect.github.com/npm/node-semver/issues/656">#656</a>) (<a href="https://github.com/zyxkad"><code>@​zyxkad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/14d263faa156e408a033b9b12a2f87735c2df42c"><code>14d263f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/7c34e1ac1bcc0bc6579b30745c96075c69bd0332"><code>7c34e1a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/625">#625</a> bump <code>@​npmcli/template-oss</code> from 4.18.1 to 4.19.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/123e0b03287e1af295ef82d55f55c16805596f35"><code>123e0b0</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/737d5e1cf10e631bab8a28594aa2d5c9d4090814"><code>737d5e1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/622">#622</a> bump <code>@​npmcli/template-oss</code> from 4.18.0 to 4.18.1 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
<li><a href="https://github.com/npm/node-semver/commit/cce61804ba6f997225a1267135c06676fe0524d2"><code>cce6180</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> postinstall for dependabot template-oss PR (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/b914a3d0d26ca27d2685053d7d390af4e02eedd9"><code>b914a3d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/598">#598</a> bump <code>@​npmcli/template-oss</code> from 4.17.0 to 4.18.0 (<a href="https://github.com/dependabot"><code>@​dependabot</code></a>[bot])</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.3...v7.5.4">7.5.4</a> (2023-07-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/cc6fde2d34b95cb600d126649d926901bd2a9703"><code>cc6fde2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/588">#588</a> trim each range set before parsing (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/99d8287516a1d2abf0286033e2e26eca6b69c09f"><code>99d8287</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/583">#583</a> correctly parse long build ids as valid (<a href="https://redirect.github.com/npm/node-semver/issues/583">#583</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/377f709718053a477ed717089c4403c4fec332a1"><code>377f709</code></a> chore: release 7.6.0 (<a href="https://redirect.github.com/npm/node-semver/issues/661">#661</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/a7ab13a46201e342d34e84a989632b380f755baf"><code>a7ab13a</code></a> feat: preserve pre-release and build parts of a version on coerce (<a href="https://redirect.github.com/npm/node-semver/issues/671">#671</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/816c7b2cbfcb1986958a290f941eddfd0441139e"><code>816c7b2</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/0bd24d943cbd1a7f6a2b8d384590bfa98559e1de"><code>0bd24d9</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.21.1 to 4.21.3</li>
<li><a href="https://github.com/npm/node-semver/commit/e521932f115a81030f4e7c34e8631cdd3c6a108b"><code>e521932</code></a> chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/88739918080debeb239aae840b35c07436148e50"><code>8873991</code></a> chore: chore: chore: postinstall for dependabot template-oss PR</li>
<li><a href="https://github.com/npm/node-semver/commit/f317dc8689781bcfd98e2c32b46157276acdd47c"><code>f317dc8</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.19.0 to 4.21.0</li>
<li><a href="https://github.com/npm/node-semver/commit/7303db1fe54d6905b23ccb0162878e37d73535ef"><code>7303db1</code></a> chore: add clean() test for build metadata (<a href="https://redirect.github.com/npm/node-semver/issues/658">#658</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/6240d75a7c620b0a222f05969a91fdc3dc2be0fb"><code>6240d75</code></a> chore: add missing quotes in README.md (<a href="https://redirect.github.com/npm/node-semver/issues/656">#656</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/14d263faa156e408a033b9b12a2f87735c2df42c"><code>14d263f</code></a> chore: postinstall for dependabot template-oss PR</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v5.7.2...v7.6.0">compare view</a></li>
</ul>
</details>
<br />

Updates `expo` from 50.0.17 to 51.0.20
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expo/expo/blob/main/CHANGELOG.md">expo's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>This is the log of notable changes to the Expo client that are developer-facing.
Package-specific changes not released in any SDK will be added here just before the release. Until then, you can find them in changelogs of the individual packages (see <a href="https://github.com/expo/expo/blob/main/packages">packages</a> directory).</p>
<h2>Unpublished</h2>
<h3>📚 3rd party library updates</h3>
<h3>🛠 Breaking changes</h3>
<h3>🎉 New features</h3>
<h3>🐛 Bug fixes</h3>
<h2>51.0.0 — 2024-05-07</h2>
<h3>🛠 Breaking changes</h3>
<ul>
<li><strong><code>expo-auth-session</code></strong>
<ul>
<li>Drop deprecated <code>expoClientId</code> field from auth proxy. (<a href="https://redirect.github.com/expo/expo/pull/28590">#28590</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-barcode-scanner</code></strong>
<ul>
<li><code>expo-barcode-scanner</code> is now deprecated. Please use <code>expo-camera</code> instead. (<a href="https://redirect.github.com/expo/expo/pull/26025">#26025</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-constants</code></strong>
<ul>
<li>Remove deprecated installationId, isDevice, nativeAppVersion, nativeBuildVersion, platform.platform, platform.systemVersion, platform.userInterfaceIdiom properties. (<a href="https://redirect.github.com/expo/expo/pull/26329">#26329</a> by <a href="https://github.com/aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-face-detector</code></strong>
<ul>
<li><code>expo-face-detector</code> is now deprecated. We recommed using <a href="https://github.com/mrousavy/react-native-vision-camera">react-native-vision-camera</a> instead. (<a href="https://redirect.github.com/expo/expo/pull/26026">#26026</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-location</code></strong>
<ul>
<li>[Web] <code>getPermissionsAsync</code> no longer prompts the user for permission instead we use the new browser API <code>navigator.permissions.query</code> to check the permission status. (<a href="https://redirect.github.com/expo/expo/pull/26837">#26836</a> by <a href="https://github.com/hems"><code>@​hems</code></a>) (<a href="https://redirect.github.com/expo/expo/pull/26837">#26837</a> by <a href="https://github.com/hems"><code>@​hems</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-local-authentication</code></strong>
<ul>
<li><code>SecurityLevel.BIOMETRIC</code> has been deprecated in favour of <code>SecurityLevel.BIOMETRIC_STRONG</code> and <code>SecurityLevel.BIOMETRIC_WEAK</code>. Using <code>SecurityLevel.BIOMETRIC</code> might lead to unexpected behaviour. (<a href="https://redirect.github.com/expo/expo/pull/26768">#26768</a> by <a href="https://github.com/behenate"><code>@​behenate</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-modules-core</code></strong>
<ul>
<li>Removed <code>ReactNativeHostHandler.onRegisterJSIModules</code> interface. (<a href="https://redirect.github.com/expo/expo/pull/26357">#26357</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
<li>Dropped supports for React Native 0.73 and lower. (<a href="https://redirect.github.com/expo/expo/pull/27601">#27601</a>, <a href="https://redirect.github.com/expo/expo/pull/27689">#27689</a>, <a href="https://redirect.github.com/expo/expo/pull/27629">#27629</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-sms</code></strong>
<ul>
<li>[web] <code>sendSMSAsync</code> now throws error code <code>ERR_UNAVAILABLE</code> instead of <code>E_SMS_UNAVAILABLE</code>. (<a href="https://redirect.github.com/expo/expo/pull/27437">#27437</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-sqlite</code></strong>
<ul>
<li>Refactor <code>expo-sqlite/next</code> API to be more React idiomatic. (<a href="https://redirect.github.com/expo/expo/pull/25657">#25657</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
<li>Moved the previous default export as <code>expo-sqlite/legacy</code> and promoted <code>expo-sqlite/next</code> as the default. <code>expo-sqlite/next</code> import is still as-is for backward compatibility. (<a href="https://redirect.github.com/expo/expo/pull/28278">#28278</a> by <a href="https://github.com/kudo"><code>@​kudo</code></a>)</li>
</ul>
</li>
</ul>
<h3>🎉 New features</h3>
<ul>
<li><strong><code>expo-barcode-scanner</code></strong>
<ul>
<li><code>BarCodeScannerResult</code> now returns an additional <code>raw</code> field corresponding to the barcode value as it was encoded in the barcode without parsing. Will always be undefined on iOS. (<a href="https://redirect.github.com/expo/expo/pull/25391">#25391</a> by <a href="https://github.com/ajacquierbret"><code>@​ajacquierbret</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-blur</code></strong>
<ul>
<li>Added support for Apple tvOS. (<a href="https://redirect.github.com/expo/expo/pull/26965">#26965</a> by <a href="https://github.com/douglowder"><code>@​douglowder</code></a>)</li>
<li>Mark React client components with &quot;use client&quot; directives. (<a href="https://redirect.github.com/expo/expo/pull/27300">#27300</a> by <a href="https://github.com/EvanBacon"><code>@​EvanBacon</code></a>)</li>
</ul>
</li>
<li><strong><code>expo-asset</code></strong>
<ul>
<li>Added config plugin to allow assets to be linked at build time. (<a href="https://redirect.github.com/expo/expo/pull/27052">#27052</a> by <a href="https://github.com/alanjhughes"><code>@​alanjhughes</code></a>)</li>
<li>Add Apple TV support to the new iOS native module. (<a href="https://redirect.github.com/expo/expo/pull/27823">#27823</a> by <a href="https://github.com/douglowder"><code>@​douglowder</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/expo/expo/commits/HEAD/packages/expo">compare view</a></li>
</ul>
</details>
<br />

Updates `ws` from 6.2.2 to 6.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>6.2.3</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 6.x release line (eeb76d31).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d87f3b6d3a00513af9bbb74f45ba9183af4e5f43"><code>d87f3b6</code></a> [dist] 6.2.3</li>
<li><a href="https://github.com/websockets/ws/commit/eeb76d313e2a00dd5247ca3597bba7877d064a63"><code>eeb76d3</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/6.2.2...6.2.3">compare view</a></li>
</ul>
</details>
<br />

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 17:09:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/768" class=".btn">#768</a>
            </td>
            <td>
                <b>
                    Fixes and interop testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds interop testing against Credo and Sphereon's OID4VCI client library. There were also some fixes to achieve interop:

- Issuer ID recorded in OID4VCI exchange record.
- Fill in the `iss` and `credentialSubject.issuer` fields using record Issuer ID instead of the verification method ID.

Heads up @timbl-ont @weiiv, there might be some minor conflicts with the work you've been doing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 21:25:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/767" class=".btn">#767</a>
            </td>
            <td>
                <b>
                    Bump the pip group in /kafka_events with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events with 2 updates: [setuptools](https://github.com/pypa/setuptools) and [zipp](https://github.com/jaraco/zipp).

Updates `setuptools` from 69.5.1 to 70.0.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pypa/setuptools/blob/main/NEWS.rst">setuptools's changelog</a>.</em></p>
<blockquote>
<h1>v70.0.0</h1>
<h2>Features</h2>
<ul>
<li>Emit a warning when <code>[tools.setuptools]</code> is present in <code>pyproject.toml</code> and will be ignored. -- by :user:<code>SnoopJ</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4150">#4150</a>)</li>
<li>Improved <code>AttributeError</code> error message if <code>pkg_resources.EntryPoint.require</code> is called without extras or distribution
Gracefully &quot;do nothing&quot; when trying to activate a <code>pkg_resources.Distribution</code> with a <code>None</code> location, rather than raising a <code>TypeError</code>
-- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4262">#4262</a>)</li>
<li>Typed the dynamically defined variables from <code>pkg_resources</code> -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4267">#4267</a>)</li>
<li>Modernized and refactored VCS handling in package_index. (<a href="https://redirect.github.com/pypa/setuptools/issues/4332">#4332</a>)</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>In install command, use super to call the superclass methods. Avoids race conditions when monkeypatching from _distutils_system_mod occurs late. (<a href="https://redirect.github.com/pypa/setuptools/issues/4136">#4136</a>)</li>
<li>Fix finder template for lenient editable installs of implicit nested namespaces
constructed by using <code>package_dir</code> to reorganise directory structure. (<a href="https://redirect.github.com/pypa/setuptools/issues/4278">#4278</a>)</li>
<li>Fix an error with <code>UnicodeDecodeError</code> handling in <code>pkg_resources</code> when trying to read files in UTF-8 with a fallback -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4348">#4348</a>)</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li>Uses RST substitution to put badges in 1 line. (<a href="https://redirect.github.com/pypa/setuptools/issues/4312">#4312</a>)</li>
</ul>
<h2>Deprecations and Removals</h2>
<ul>
<li>
<p>Further adoption of UTF-8 in <code>setuptools</code>.
This change regards mostly files produced and consumed during the build process
(e.g. metadata files, script wrappers, automatically updated config files, etc..)
Although precautions were taken to minimize disruptions, some edge cases might
be subject to backwards incompatibility.</p>
<p>Support for <code>&quot;locale&quot;</code> encoding is now <strong>deprecated</strong>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4309">#4309</a>)</p>
</li>
<li>
<p>Remove <code>setuptools.convert_path</code> after long deprecation period.
This function was never defined by <code>setuptools</code> itself, but rather a
side-effect of an import for internal usage. (<a href="https://redirect.github.com/pypa/setuptools/issues/4322">#4322</a>)</p>
</li>
<li>
<p>Remove fallback for customisations of <code>distutils</code>' <code>build.sub_command</code> after long
deprecated period.
Users are advised to import <code>build</code> directly from <code>setuptools.command.build</code>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4322">#4322</a>)</p>
</li>
<li>
<p>Removed <code>typing_extensions</code> from vendored dependencies -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4324">#4324</a>)</p>
</li>
<li>
<p>Remove deprecated <code>setuptools.dep_util</code>.
The provided alternative is <code>setuptools.modified</code>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4360">#4360</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pypa/setuptools/commit/5cbf12a9b63fd37985a4525617b46576b8ac3a7b"><code>5cbf12a</code></a> Workaround for release error in v70</li>
<li><a href="https://github.com/pypa/setuptools/commit/9c1bcc3417bd12668123f7e731e241d9e57bfc57"><code>9c1bcc3</code></a> Bump version: 69.5.1 → 70.0.0</li>
<li><a href="https://github.com/pypa/setuptools/commit/4dc0c31644b458ac43ce6148f6a9dc729a7e78b5"><code>4dc0c31</code></a> Remove deprecated <code>setuptools.dep_util</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4360">#4360</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/6c1ef5748dbd70c8c5423e12680345766ee101d9"><code>6c1ef57</code></a> Remove xfail now that test passes. Ref <a href="https://redirect.github.com/pypa/setuptools/issues/4371">#4371</a>.</li>
<li><a href="https://github.com/pypa/setuptools/commit/d14fa0162c95450898c11534caf26a0f03553176"><code>d14fa01</code></a> Add all site-packages dirs when creating simulated environment for test_edita...</li>
<li><a href="https://github.com/pypa/setuptools/commit/6b7f7a18afc90007544092c446dc0cd856d86b17"><code>6b7f7a1</code></a> Prevent <code>bin</code> folders to be taken as extern packages when vendoring (<a href="https://redirect.github.com/pypa/setuptools/issues/4370">#4370</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/69141f69f8bf38da34cbea552d6fdaa9c8619c53"><code>69141f6</code></a> Add doctest for vendorised bin folder</li>
<li><a href="https://github.com/pypa/setuptools/commit/2a53cc1200ec4b14e08e84be3c042f8983dfb7d7"><code>2a53cc1</code></a> Prevent 'bin' folders to be taken as extern packages</li>
<li><a href="https://github.com/pypa/setuptools/commit/720862807dea012f3a0e7061880691025f736f11"><code>7208628</code></a> Replace call to deprecated <code>validate_pyproject</code> command (<a href="https://redirect.github.com/pypa/setuptools/issues/4363">#4363</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/96d681aa405460f724c62c00ca125ae722ad810a"><code>96d681a</code></a> Remove call to deprecated validate_pyproject command</li>
<li>Additional commits viewable in <a href="https://github.com/pypa/setuptools/compare/v69.5.1...v70.0.0">compare view</a></li>
</ul>
</details>
<br />

Updates `zipp` from 3.18.2 to 3.19.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jaraco/zipp/blob/main/NEWS.rst">zipp's changelog</a>.</em></p>
<blockquote>
<h1>v3.19.1</h1>
<h2>Bugfixes</h2>
<ul>
<li>Improved handling of malformed zip files. (<a href="https://redirect.github.com/jaraco/zipp/issues/119">#119</a>)</li>
</ul>
<h1>v3.19.0</h1>
<h2>Features</h2>
<ul>
<li>Implement is_symlink. (<a href="https://redirect.github.com/jaraco/zipp/issues/117">#117</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jaraco/zipp/commit/6d1cb72aa55e0536f35d2af128994b5a61ca4c1a"><code>6d1cb72</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/fd604bd34f0343472521a36da1fbd22e793e14fd"><code>fd604bd</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/120">#120</a> from jaraco/bugfix/119-malformed-paths</li>
<li><a href="https://github.com/jaraco/zipp/commit/c18417ed2953e181728a7dac07bff88a2190abf7"><code>c18417e</code></a> Add news fragment.</li>
<li><a href="https://github.com/jaraco/zipp/commit/58115d2be968644ce71ce6bcc9b79826c82a1806"><code>58115d2</code></a> Employ SanitizedNames in CompleteDirs. Fixes broken test.</li>
<li><a href="https://github.com/jaraco/zipp/commit/564fcc10cdbfdaecdb33688e149827465931c9e0"><code>564fcc1</code></a> Add SanitizedNames mixin.</li>
<li><a href="https://github.com/jaraco/zipp/commit/79a309fe54dc6b7934fb72e9f31bcb58f2e9f547"><code>79a309f</code></a> Add some assertions about malformed paths.</li>
<li><a href="https://github.com/jaraco/zipp/commit/2d015c22348fab46ca765339f55f84fe9d6e8115"><code>2d015c2</code></a> Merge <a href="https://github.com/jaraco/skeleton">https://github.com/jaraco/skeleton</a></li>
<li><a href="https://github.com/jaraco/zipp/commit/a595a0fad054cd20b69d3e954c99174e3a548938"><code>a595a0f</code></a> Rename extras to align with core metadata spec.</li>
<li><a href="https://github.com/jaraco/zipp/commit/608f90a6e74919501577a1312dc5c7d8e1d391d7"><code>608f90a</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/3a22d724acf874111b43f87f7110225122ec3de5"><code>3a22d72</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/118">#118</a> from jaraco/feature/is-symlink</li>
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 19:35:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    Bump the pip group in /redis_events with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events with 2 updates: [setuptools](https://github.com/pypa/setuptools) and [zipp](https://github.com/jaraco/zipp).

Updates `setuptools` from 69.5.1 to 70.0.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pypa/setuptools/blob/main/NEWS.rst">setuptools's changelog</a>.</em></p>
<blockquote>
<h1>v70.0.0</h1>
<h2>Features</h2>
<ul>
<li>Emit a warning when <code>[tools.setuptools]</code> is present in <code>pyproject.toml</code> and will be ignored. -- by :user:<code>SnoopJ</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4150">#4150</a>)</li>
<li>Improved <code>AttributeError</code> error message if <code>pkg_resources.EntryPoint.require</code> is called without extras or distribution
Gracefully &quot;do nothing&quot; when trying to activate a <code>pkg_resources.Distribution</code> with a <code>None</code> location, rather than raising a <code>TypeError</code>
-- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4262">#4262</a>)</li>
<li>Typed the dynamically defined variables from <code>pkg_resources</code> -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4267">#4267</a>)</li>
<li>Modernized and refactored VCS handling in package_index. (<a href="https://redirect.github.com/pypa/setuptools/issues/4332">#4332</a>)</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>In install command, use super to call the superclass methods. Avoids race conditions when monkeypatching from _distutils_system_mod occurs late. (<a href="https://redirect.github.com/pypa/setuptools/issues/4136">#4136</a>)</li>
<li>Fix finder template for lenient editable installs of implicit nested namespaces
constructed by using <code>package_dir</code> to reorganise directory structure. (<a href="https://redirect.github.com/pypa/setuptools/issues/4278">#4278</a>)</li>
<li>Fix an error with <code>UnicodeDecodeError</code> handling in <code>pkg_resources</code> when trying to read files in UTF-8 with a fallback -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4348">#4348</a>)</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li>Uses RST substitution to put badges in 1 line. (<a href="https://redirect.github.com/pypa/setuptools/issues/4312">#4312</a>)</li>
</ul>
<h2>Deprecations and Removals</h2>
<ul>
<li>
<p>Further adoption of UTF-8 in <code>setuptools</code>.
This change regards mostly files produced and consumed during the build process
(e.g. metadata files, script wrappers, automatically updated config files, etc..)
Although precautions were taken to minimize disruptions, some edge cases might
be subject to backwards incompatibility.</p>
<p>Support for <code>&quot;locale&quot;</code> encoding is now <strong>deprecated</strong>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4309">#4309</a>)</p>
</li>
<li>
<p>Remove <code>setuptools.convert_path</code> after long deprecation period.
This function was never defined by <code>setuptools</code> itself, but rather a
side-effect of an import for internal usage. (<a href="https://redirect.github.com/pypa/setuptools/issues/4322">#4322</a>)</p>
</li>
<li>
<p>Remove fallback for customisations of <code>distutils</code>' <code>build.sub_command</code> after long
deprecated period.
Users are advised to import <code>build</code> directly from <code>setuptools.command.build</code>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4322">#4322</a>)</p>
</li>
<li>
<p>Removed <code>typing_extensions</code> from vendored dependencies -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4324">#4324</a>)</p>
</li>
<li>
<p>Remove deprecated <code>setuptools.dep_util</code>.
The provided alternative is <code>setuptools.modified</code>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4360">#4360</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pypa/setuptools/commit/5cbf12a9b63fd37985a4525617b46576b8ac3a7b"><code>5cbf12a</code></a> Workaround for release error in v70</li>
<li><a href="https://github.com/pypa/setuptools/commit/9c1bcc3417bd12668123f7e731e241d9e57bfc57"><code>9c1bcc3</code></a> Bump version: 69.5.1 → 70.0.0</li>
<li><a href="https://github.com/pypa/setuptools/commit/4dc0c31644b458ac43ce6148f6a9dc729a7e78b5"><code>4dc0c31</code></a> Remove deprecated <code>setuptools.dep_util</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4360">#4360</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/6c1ef5748dbd70c8c5423e12680345766ee101d9"><code>6c1ef57</code></a> Remove xfail now that test passes. Ref <a href="https://redirect.github.com/pypa/setuptools/issues/4371">#4371</a>.</li>
<li><a href="https://github.com/pypa/setuptools/commit/d14fa0162c95450898c11534caf26a0f03553176"><code>d14fa01</code></a> Add all site-packages dirs when creating simulated environment for test_edita...</li>
<li><a href="https://github.com/pypa/setuptools/commit/6b7f7a18afc90007544092c446dc0cd856d86b17"><code>6b7f7a1</code></a> Prevent <code>bin</code> folders to be taken as extern packages when vendoring (<a href="https://redirect.github.com/pypa/setuptools/issues/4370">#4370</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/69141f69f8bf38da34cbea552d6fdaa9c8619c53"><code>69141f6</code></a> Add doctest for vendorised bin folder</li>
<li><a href="https://github.com/pypa/setuptools/commit/2a53cc1200ec4b14e08e84be3c042f8983dfb7d7"><code>2a53cc1</code></a> Prevent 'bin' folders to be taken as extern packages</li>
<li><a href="https://github.com/pypa/setuptools/commit/720862807dea012f3a0e7061880691025f736f11"><code>7208628</code></a> Replace call to deprecated <code>validate_pyproject</code> command (<a href="https://redirect.github.com/pypa/setuptools/issues/4363">#4363</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/96d681aa405460f724c62c00ca125ae722ad810a"><code>96d681a</code></a> Remove call to deprecated validate_pyproject command</li>
<li>Additional commits viewable in <a href="https://github.com/pypa/setuptools/compare/v69.5.1...v70.0.0">compare view</a></li>
</ul>
</details>
<br />

Updates `zipp` from 3.18.2 to 3.19.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jaraco/zipp/blob/main/NEWS.rst">zipp's changelog</a>.</em></p>
<blockquote>
<h1>v3.19.1</h1>
<h2>Bugfixes</h2>
<ul>
<li>Improved handling of malformed zip files. (<a href="https://redirect.github.com/jaraco/zipp/issues/119">#119</a>)</li>
</ul>
<h1>v3.19.0</h1>
<h2>Features</h2>
<ul>
<li>Implement is_symlink. (<a href="https://redirect.github.com/jaraco/zipp/issues/117">#117</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jaraco/zipp/commit/6d1cb72aa55e0536f35d2af128994b5a61ca4c1a"><code>6d1cb72</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/fd604bd34f0343472521a36da1fbd22e793e14fd"><code>fd604bd</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/120">#120</a> from jaraco/bugfix/119-malformed-paths</li>
<li><a href="https://github.com/jaraco/zipp/commit/c18417ed2953e181728a7dac07bff88a2190abf7"><code>c18417e</code></a> Add news fragment.</li>
<li><a href="https://github.com/jaraco/zipp/commit/58115d2be968644ce71ce6bcc9b79826c82a1806"><code>58115d2</code></a> Employ SanitizedNames in CompleteDirs. Fixes broken test.</li>
<li><a href="https://github.com/jaraco/zipp/commit/564fcc10cdbfdaecdb33688e149827465931c9e0"><code>564fcc1</code></a> Add SanitizedNames mixin.</li>
<li><a href="https://github.com/jaraco/zipp/commit/79a309fe54dc6b7934fb72e9f31bcb58f2e9f547"><code>79a309f</code></a> Add some assertions about malformed paths.</li>
<li><a href="https://github.com/jaraco/zipp/commit/2d015c22348fab46ca765339f55f84fe9d6e8115"><code>2d015c2</code></a> Merge <a href="https://github.com/jaraco/skeleton">https://github.com/jaraco/skeleton</a></li>
<li><a href="https://github.com/jaraco/zipp/commit/a595a0fad054cd20b69d3e954c99174e3a548938"><code>a595a0f</code></a> Rename extras to align with core metadata spec.</li>
<li><a href="https://github.com/jaraco/zipp/commit/608f90a6e74919501577a1312dc5c7d8e1d391d7"><code>608f90a</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/3a22d724acf874111b43f87f7110225122ec3de5"><code>3a22d72</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/118">#118</a> from jaraco/feature/is-symlink</li>
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 19:35:38 +0000 UTC
    </div>
</div>

