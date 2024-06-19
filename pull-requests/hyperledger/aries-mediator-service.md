---
layout: default
title: aries-mediator-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mediator-service
---

# aries-mediator-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mediator-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    build(deps): bump the npm_and_yarn group in /afj with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group in /afj with 2 updates: [ws](https://github.com/websockets/ws) and [tar](https://github.com/isaacs/node-tar).

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

Updates `tar` from 6.1.13 to 6.2.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/isaacs/node-tar/blob/main/CHANGELOG.md">tar's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>7.4</h2>
<ul>
<li>Deprecate <code>onentry</code> in favor of <code>onReadEntry</code> for clarity.</li>
</ul>
<h2>7.3</h2>
<ul>
<li>Add <code>onWriteEntry</code> option</li>
</ul>
<h2>7.2</h2>
<ul>
<li>DRY the command definitions into a single <code>makeCommand</code> method,
and update the type signatures to more appropriately infer the
return type from the options and arguments provided.</li>
</ul>
<h2>7.1</h2>
<ul>
<li>Update minipass to v7.1.0</li>
<li>Update the type definitions of <code>write()</code> and <code>end()</code> methods on
<code>Unpack</code> and <code>Parser</code> classes to be compatible with the
NodeJS.WritableStream type in the latest versions of
<code>@types/node</code>.</li>
</ul>
<h2>7.0</h2>
<ul>
<li>Rewrite in TypeScript, provide ESM and CommonJS hybrid
interface</li>
<li>Add tree-shake friendly exports, like <code>import('tar/create')</code>
and <code>import('tar/read-entry')</code> to get individual functions or
classes.</li>
<li>Add <code>chmod</code> option that defaults to false, and deprecate
<code>noChmod</code>. That is, reverse the default option regarding
explicitly setting file system modes to match tar entry
settings.</li>
<li>Add <code>processUmask</code> option to avoid having to call
<code>process.umask()</code> when <code>chmod: true</code> (or <code>noChmod: false</code>) is
set.</li>
</ul>
<h2>6.2</h2>
<ul>
<li>Add support for brotli compression</li>
<li>Add <code>maxDepth</code> option to prevent extraction into excessively
deep folders.</li>
</ul>
<h2>6.1</h2>
<ul>
<li>remove dead link to benchmarks (<a href="https://redirect.github.com/isaacs/node-tar/issues/313">#313</a>) (<a href="https://github.com/yetzt"><code>@​yetzt</code></a>)</li>
<li>add examples/explanation of using tar.t (<a href="https://github.com/isaacs"><code>@​isaacs</code></a>)</li>
<li>ensure close event is emited after stream has ended (<a href="https://github.com/webark"><code>@​webark</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/isaacs/node-tar/commit/bef7b1e4ffab822681fea2a9b22187192ed14717"><code>bef7b1e</code></a> 6.2.1</li>
<li><a href="https://github.com/isaacs/node-tar/commit/fe8cd57da5686f8695415414bda49206a545f7f7"><code>fe8cd57</code></a> prevent extraction in excessively deep subfolders</li>
<li><a href="https://github.com/isaacs/node-tar/commit/fe7ebfdcede1f8a2e65db12e19ecc4b3a9934648"><code>fe7ebfd</code></a> remove security.md</li>
<li><a href="https://github.com/isaacs/node-tar/commit/5bc9d404e88c39870e0fbb55655a53de6fbf0a04"><code>5bc9d40</code></a> 6.2.0</li>
<li><a href="https://github.com/isaacs/node-tar/commit/fe1ef5ec87156ddadcec8b70cdec201f26665681"><code>fe1ef5e</code></a> changelog 6.2</li>
<li><a href="https://github.com/isaacs/node-tar/commit/e483220935d931cf6b09292aba62170e68f36205"><code>e483220</code></a> get rid of npm lint stuff</li>
<li><a href="https://github.com/isaacs/node-tar/commit/689928a0ba7d9b9014d88a5fa35261f9ae4ef2f3"><code>689928a</code></a> ci that works outside of npm org</li>
<li><a href="https://github.com/isaacs/node-tar/commit/db6f53928650a04b340ecdc01db2d49937e5d63c"><code>db6f539</code></a> file inference improvements for .tbr and .tgz</li>
<li><a href="https://github.com/isaacs/node-tar/commit/336fa8f27c44bec70d46a6482096af24c668ee16"><code>336fa8f</code></a> refactor: dry and other pr comments</li>
<li><a href="https://github.com/isaacs/node-tar/commit/eeba22238736ed0832488efb3c515ada98073424"><code>eeba222</code></a> chore: lint fixes</li>
<li>Additional commits viewable in <a href="https://github.com/isaacs/node-tar/compare/v6.1.13...v6.2.1">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 07:46:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    build(deps): bump the npm_and_yarn group in /acapy/controller with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group in /acapy/controller with 3 updates: [ws](https://github.com/websockets/ws), [braces](https://github.com/micromatch/braces) and [jest](https://github.com/jestjs/jest/tree/HEAD/packages/jest).

Updates `ws` from 7.5.6 to 7.5.10
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>7.5.10</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 7.x release line (22c28763).</li>
</ul>
<h2>7.5.9</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported bc8bd34e to the 7.x release line (0435e6e1).</li>
</ul>
<h2>7.5.8</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported 0fdcc0af to the 7.x release line (2758ed35).</li>
<li>Backported d68ba9e1 to the 7.x release line (dc1781bc).</li>
</ul>
<h2>7.5.7</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported 6946f5fe to the 7.x release line (1f72e2e1).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d962d70649e393841ee1ed726a8f7ffbe90d0c06"><code>d962d70</code></a> [dist] 7.5.10</li>
<li><a href="https://github.com/websockets/ws/commit/22c28763234aa75a7e1b76f5c01c181260d7917f"><code>22c2876</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/8a78f8770618cc5a1ade485a7445cb6d6f46e2f2"><code>8a78f87</code></a> [dist] 7.5.9</li>
<li><a href="https://github.com/websockets/ws/commit/0435e6e12b8d38992cf0651cb8605dde2294bd25"><code>0435e6e</code></a> [security] Fix same host check for ws+unix: redirects</li>
<li><a href="https://github.com/websockets/ws/commit/4271f07cfc95cf7e1936388fb69e22a3731fa260"><code>4271f07</code></a> [dist] 7.5.8</li>
<li><a href="https://github.com/websockets/ws/commit/dc1781bc319cb347878d11cf730947d0bef69a51"><code>dc1781b</code></a> [security] Drop sensitive headers when following insecure redirects</li>
<li><a href="https://github.com/websockets/ws/commit/2758ed355073105a60b8b836b25265b8cdcb3b42"><code>2758ed3</code></a> [fix] Abort the handshake if the Upgrade header is invalid</li>
<li><a href="https://github.com/websockets/ws/commit/a370613fab74b82990582fa7728e130c5e87ee4c"><code>a370613</code></a> [dist] 7.5.7</li>
<li><a href="https://github.com/websockets/ws/commit/1f72e2e14f4fbb20265c228a43bb64ab915d8046"><code>1f72e2e</code></a> [security] Drop sensitive headers when following redirects (<a href="https://redirect.github.com/websockets/ws/issues/2013">#2013</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/7.5.6...7.5.10">compare view</a></li>
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

Updates `jest` from 26.6.3 to 29.7.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jestjs/jest/releases">jest's releases</a>.</em></p>
<blockquote>
<h2>v29.7.0</h2>
<h2>Features</h2>
<ul>
<li><code>[create-jest]</code> Add <code>npm init</code> / <code>yarn create</code> initialiser for Jest projects (<a href="https://redirect.github.com/jestjs/jest/pull/14453">#14465</a>)</li>
<li><code>[jest-validate]</code> Allow deprecation warnings for unknown options (<a href="https://redirect.github.com/jestjs/jest/pull/14499">#14499</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li><code>[jest-resolver]</code> Replace unmatched capture groups in <code>moduleNameMapper</code> with empty string instead of <code>undefined</code> (<a href="https://redirect.github.com/jestjs/jest/pull/14507">#14507</a>)</li>
<li><code>[jest-snapshot]</code> Allow for strings as well as template literals in inline snapshots (<a href="https://redirect.github.com/jestjs/jest/pull/14465">#14465</a>)</li>
<li><code>[@jest/test-sequencer]</code> Calculate test runtime if <code>perStats.duration</code> is missing (<a href="https://redirect.github.com/jestjs/jest/pull/14473">#14473</a>)</li>
</ul>
<h2>Performance</h2>
<ul>
<li><code>[@jest/create-cache-key-function]</code> Cache access of <code>NODE_ENV</code> and <code>BABEL_ENV</code> (<a href="https://redirect.github.com/jestjs/jest/pull/14455">#14455</a>)</li>
</ul>
<h2>Chore &amp; Maintenance</h2>
<ul>
<li><code>[jest-cli]</code> Move internal config initialisation logic to the <code>create-jest</code> package (<a href="https://redirect.github.com/jestjs/jest/pull/14453">#14465</a>)</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/bawjensen"><code>@​bawjensen</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14465">jestjs/jest#14465</a></li>
<li><a href="https://github.com/malaviya-parth"><code>@​malaviya-parth</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14467">jestjs/jest#14467</a></li>
<li><a href="https://github.com/niklasholm"><code>@​niklasholm</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14507">jestjs/jest#14507</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jestjs/jest/compare/v29.6.4...v29.7.0">https://github.com/jestjs/jest/compare/v29.6.4...v29.7.0</a></p>
<h2>v29.6.4</h2>
<h2>Fixes</h2>
<ul>
<li><code>[jest-core]</code> Fix typo in <code>scheduleAndRun</code> performance marker (<a href="https://redirect.github.com/jestjs/jest/pull/14434">#14434</a>)</li>
<li><code>[jest-environment-node]</code> Make sure <code>atob</code> and <code>btoa</code> are writeable in Node 20 (<a href="https://redirect.github.com/jestjs/jest/pull/14446">#14446</a>)</li>
<li><code>[jest-worker]</code> Additional error wrapper for <code>parentPort.postMessage</code> to fix unhandled <code>DataCloneError</code>. (<a href="https://redirect.github.com/jestjs/jest/pull/14437">#14437</a>)</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/stanleyume"><code>@​stanleyume</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14424">jestjs/jest#14424</a></li>
<li><a href="https://github.com/dj-stormtrooper"><code>@​dj-stormtrooper</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14437">jestjs/jest#14437</a></li>
<li><a href="https://github.com/thw0rted"><code>@​thw0rted</code></a> made their first contribution in <a href="https://redirect.github.com/jestjs/jest/pull/14444">jestjs/jest#14444</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jestjs/jest/compare/v29.6.3...v29.6.4">https://github.com/jestjs/jest/compare/v29.6.3...v29.6.4</a></p>
<h2>v29.6.3</h2>
<h2>Fixes</h2>
<ul>
<li><code>[expect, @jest/expect-utils]</code> <code>ObjectContaining</code> support <code>symbol</code> as key (<a href="https://redirect.github.com/jestjs/jest/pull/14414">#14414</a>)</li>
<li><code>[expect]</code> Remove <code>@types/node</code> from dependencies (<a href="https://redirect.github.com/jestjs/jest/pull/14385">#14385</a>)</li>
<li><code>[jest-core]</code> Use workers in watch mode by default to avoid crashes (<a href="https://redirect.github.com/facebook/jest/pull/14059">#14059</a> &amp; <a href="https://redirect.github.com/facebook/jest/pull/14085">#14085</a>).</li>
<li><code>[jest-reporters]</code> Update <code>istanbul-lib-instrument</code> dependency to v6. (<a href="https://redirect.github.com/jestjs/jest/pull/14401">#14401</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/13692">#13692</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14429">#14429</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/13866">#13866</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14429">#14429</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jestjs/jest/blob/main/CHANGELOG.md">jest's changelog</a>.</em></p>
<blockquote>
<h2>29.7.0</h2>
<h3>Features</h3>
<ul>
<li><code>[create-jest]</code> Add <code>npm init</code> / <code>yarn create</code> initialiser for Jest projects (<a href="https://redirect.github.com/jestjs/jest/pull/14453">#14465</a>)</li>
<li><code>[jest-validate]</code> Allow deprecation warnings for unknown options (<a href="https://redirect.github.com/jestjs/jest/pull/14499">#14499</a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li><code>[jest-resolver]</code> Replace unmatched capture groups in <code>moduleNameMapper</code> with empty string instead of <code>undefined</code> (<a href="https://redirect.github.com/jestjs/jest/pull/14507">#14507</a>)</li>
<li><code>[jest-snapshot]</code> Allow for strings as well as template literals in inline snapshots (<a href="https://redirect.github.com/jestjs/jest/pull/14465">#14465</a>)</li>
<li><code>[@jest/test-sequencer]</code> Calculate test runtime if <code>perStats.duration</code> is missing (<a href="https://redirect.github.com/jestjs/jest/pull/14473">#14473</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li><code>[@jest/create-cache-key-function]</code> Cache access of <code>NODE_ENV</code> and <code>BABEL_ENV</code> (<a href="https://redirect.github.com/jestjs/jest/pull/14455">#14455</a>)</li>
</ul>
<h3>Chore &amp; Maintenance</h3>
<ul>
<li><code>[jest-cli]</code> Move internal config initialisation logic to the <code>create-jest</code> package (<a href="https://redirect.github.com/jestjs/jest/pull/14453">#14465</a>)</li>
</ul>
<h2>29.6.4</h2>
<h3>Fixes</h3>
<ul>
<li><code>[jest-core]</code> Fix typo in <code>scheduleAndRun</code> performance marker (<a href="https://redirect.github.com/jestjs/jest/pull/14434">#14434</a>)</li>
<li><code>[jest-environment-node]</code> Make sure <code>atob</code> and <code>btoa</code> are writeable in Node 20 (<a href="https://redirect.github.com/jestjs/jest/pull/14446">#14446</a>)</li>
<li><code>[jest-worker]</code> Additional error wrapper for <code>parentPort.postMessage</code> to fix unhandled <code>DataCloneError</code>. (<a href="https://redirect.github.com/jestjs/jest/pull/14437">#14437</a>)</li>
</ul>
<h2>29.6.3</h2>
<h3>Fixes</h3>
<ul>
<li><code>[expect, @jest/expect-utils]</code> <code>ObjectContaining</code> support <code>sumbol</code> as key (<a href="https://redirect.github.com/jestjs/jest/pull/14414">#14414</a>)</li>
<li><code>[expect]</code> Remove <code>@types/node</code> from dependencies (<a href="https://redirect.github.com/jestjs/jest/pull/14385">#14385</a>)</li>
<li><code>[jest-core]</code> Use workers in watch mode by default to avoid crashes (<a href="https://redirect.github.com/facebook/jest/pull/14059">#14059</a> &amp; <a href="https://redirect.github.com/facebook/jest/pull/14085">#14085</a>).</li>
<li><code>[jest-reporters]</code> Update <code>istanbul-lib-instrument</code> dependency to v6. (<a href="https://redirect.github.com/jestjs/jest/pull/14401">#14401</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/13692">#13692</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14429">#14429</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/13866">#13866</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14429">#14429</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://redirect.github.com/jestjs/jest/pull/13867">#13867</a> as it was a breaking change (<a href="https://redirect.github.com/jestjs/jest/pull/14429">#14429</a>)</li>
<li><code>[@jest/reporters]</code> Marks Reporter's hooks as optional (<a href="https://redirect.github.com/jestjs/jest/pull/14433">#14433</a>)</li>
<li><code>[jest-runtime]</code> Fix dynamic ESM import module bug when loaded module through <code>jest.isolateModulesAsync</code> (<a href="https://redirect.github.com/jestjs/jest/pull/14397">#14397</a>)</li>
</ul>
<h3>Chore &amp; Maintenance</h3>
<ul>
<li><code>[jest-changed-files, jest-circus, jest-console, @jest/core, @jest/runtime, @jest/transform]</code> Use <code>invariant</code> and <code>notEmpty</code> from <code>jest-util</code> rather than own internal (<a href="https://redirect.github.com/jestjs/jest/pull/14366">#14366</a>)</li>
</ul>
<h2>29.6.2</h2>
<h3>Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jestjs/jest/commit/4e56991693da7cd4c3730dc3579a1dd1403ee630"><code>4e56991</code></a> v29.7.0</li>
<li><a href="https://github.com/jestjs/jest/commit/55cd6a0aaf6f9178199dfa7af7a00fcaa7c421fd"><code>55cd6a0</code></a> v29.6.4</li>
<li><a href="https://github.com/jestjs/jest/commit/fb7d95c8af6e0d65a8b65348433d8a0ea0725b5b"><code>fb7d95c</code></a> v29.6.3</li>
<li><a href="https://github.com/jestjs/jest/commit/49bacb9620b87c476bd5ba1b30e26ca2c4f42a70"><code>49bacb9</code></a> chore: update jest repo organisation in urls (<a href="https://github.com/jestjs/jest/tree/HEAD/packages/jest/issues/14413">#14413</a>)</li>
<li><a href="https://github.com/jestjs/jest/commit/0fd5b1c37555f485c56a6ad2d6b010a72204f9f6"><code>0fd5b1c</code></a> v29.6.2</li>
<li><a href="https://github.com/jestjs/jest/commit/1f019afdcdfc54a6664908bb45f343db4e3d0848"><code>1f019af</code></a> v29.6.1</li>
<li><a href="https://github.com/jestjs/jest/commit/c1e5b8a38ef54bb138409f89831942ebf6a7a67e"><code>c1e5b8a</code></a> v29.6.0</li>
<li><a href="https://github.com/jestjs/jest/commit/6ffa48d1cd7d85189f0dbc1e37fd0efafa5c221c"><code>6ffa48d</code></a> chore: upgrade TypeScript to v5 (<a href="https://github.com/jestjs/jest/tree/HEAD/packages/jest/issues/14155">#14155</a>)</li>
<li><a href="https://github.com/jestjs/jest/commit/a95eeb6c2c8145a81190149a52a30fc177417ecc"><code>a95eeb6</code></a> chore: update tsd runner (<a href="https://github.com/jestjs/jest/tree/HEAD/packages/jest/issues/14020">#14020</a>)</li>
<li><a href="https://github.com/jestjs/jest/commit/39f3beda6b396665bebffab94e8d7c45be30454c"><code>39f3bed</code></a> v29.5.0</li>
<li>Additional commits viewable in <a href="https://github.com/jestjs/jest/commits/v29.7.0/packages/jest">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 09:07:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    build(deps): bump hyperledger/aries-cloudagent-python from py3.9-0.10.4 to py3.9-0.12.1 in /acapy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps [hyperledger/aries-cloudagent-python](https://github.com/hyperledger/aries-cloudagent-python) from py3.9-0.10.4 to py3.9-0.12.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/hyperledger/aries-cloudagent-python/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyperledger/aries-cloudagent-python&package-manager=docker&previous-version=py3.9-0.10.4&new-version=py3.9-0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 12:04:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    build(deps): bump hyperledger/aries-cloudagent-python from py3.9-0.10.4 to py3.9-0.12.1 in /redis-pq-demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps [hyperledger/aries-cloudagent-python](https://github.com/hyperledger/aries-cloudagent-python) from py3.9-0.10.4 to py3.9-0.12.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/hyperledger/aries-cloudagent-python/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyperledger/aries-cloudagent-python&package-manager=docker&previous-version=py3.9-0.10.4&new-version=py3.9-0.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:57:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    build(deps): update requests requirement from ~=2.31.0 to ~=2.32.3 in /acapy/plugins/firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [requests](https://github.com/psf/requests) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.3</h2>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/0e322af87745eff34caffe4df68456ebc20d9068"><code>0e322af</code></a> v2.32.3</li>
<li><a href="https://github.com/psf/requests/commit/e18879932287c2bf4bcee4ddf6ccb8a69b6fc656"><code>e188799</code></a> Don't create default SSLContext if ssl module isn't present (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
<li><a href="https://github.com/psf/requests/commit/145b5399486b56e00250204f033441f3fdf2f3c9"><code>145b539</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a> from sigmavirus24/bug/6715</li>
<li><a href="https://github.com/psf/requests/commit/b1d73ddb509a3a2d3e10744e85f9cdebdbde90f0"><code>b1d73dd</code></a> Don't use default SSLContext with custom poolmanager kwargs</li>
<li><a href="https://github.com/psf/requests/commit/6badbac6e0d6b5a53872f26401761ad37a9002b8"><code>6badbac</code></a> Update HISTORY.md</li>
<li><a href="https://github.com/psf/requests/commit/a62a2d35d918baa8e793f7aa4fb41527644dfca5"><code>a62a2d3</code></a> Allow for overriding of specific pool key params</li>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.31.0...v2.32.3">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 11:55:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump pytest-cov from 2.10.1 to 2.12.1 in /acapy/plugins/firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-cov](https://github.com/pytest-dev/pytest-cov) from 2.10.1 to 2.12.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-cov/blob/master/CHANGELOG.rst">pytest-cov's changelog</a>.</em></p>
<blockquote>
<h2>2.12.1 (2021-06-01)</h2>
<ul>
<li>Changed the <code>toml</code> requirement to be always be directly required (instead of being required through a coverage extra).
This fixes issues with pip-compile (<code>pip-tools#1300 &lt;https://github.com/jazzband/pip-tools/issues/1300&gt;</code><em>).
Contributed by Sorin Sbarnea in <code>[#472](https://github.com/pytest-dev/pytest-cov/issues/472) &lt;https://github.com/pytest-dev/pytest-cov/pull/472&gt;</code></em>.</li>
<li>Documented <code>show_contexts</code>.
Contributed by Brian Rutledge in <code>[#473](https://github.com/pytest-dev/pytest-cov/issues/473) &lt;https://github.com/pytest-dev/pytest-cov/pull/473&gt;</code>_.</li>
</ul>
<h2>2.12.0 (2021-05-14)</h2>
<ul>
<li>Added coverage's <code>toml</code> extra to install requirements in setup.py.
Contributed by Christian Riedel in <code>[#410](https://github.com/pytest-dev/pytest-cov/issues/410) &lt;https://github.com/pytest-dev/pytest-cov/pull/410&gt;</code>_.</li>
<li>Fixed <code>pytest_cov.__version__</code> to have the right value (string with version instead of a string
including <code>__version__ =</code>).</li>
<li>Fixed license classifier in <code>setup.py</code>.
Contributed by Chris Sreesangkom in <code>[#467](https://github.com/pytest-dev/pytest-cov/issues/467) &lt;https://github.com/pytest-dev/pytest-cov/pull/467&gt;</code>_.</li>
<li>Fixed <em>commits since</em> badge.
Contributed by Terence Honles in <code>[#470](https://github.com/pytest-dev/pytest-cov/issues/470) &lt;https://github.com/pytest-dev/pytest-cov/pull/470&gt;</code>_.</li>
</ul>
<h2>2.11.1 (2021-01-20)</h2>
<ul>
<li>Fixed support for newer setuptools (v42+).
Contributed by Michał Górny in <code>[#451](https://github.com/pytest-dev/pytest-cov/issues/451) &lt;https://github.com/pytest-dev/pytest-cov/pull/451&gt;</code>_.</li>
</ul>
<h2>2.11.0 (2021-01-18)</h2>
<ul>
<li>Bumped minimum coverage requirement to 5.2.1. This prevents reporting issues.
Contributed by Mateus Berardo de Souza Terra in <code>[#433](https://github.com/pytest-dev/pytest-cov/issues/433) &lt;https://github.com/pytest-dev/pytest-cov/pull/433&gt;</code>_.</li>
<li>Improved sample projects (from the <code>examples &lt;https://github.com/pytest-dev/pytest-cov/tree/master/examples&gt;</code>_
directory) to support running <code>tox -e pyXY</code>. Now the example configures a suffixed coverage data file,
and that makes the cleanup environment unnecessary.
Contributed by Ganden Schaffner in <code>[#435](https://github.com/pytest-dev/pytest-cov/issues/435) &lt;https://github.com/pytest-dev/pytest-cov/pull/435&gt;</code>_.</li>
<li>Removed the empty <code>console_scripts</code> entrypoint that confused some Gentoo build script.
I didn't ask why it was so broken cause I didn't want to ruin my day.
Contributed by Michał Górny in <code>[#434](https://github.com/pytest-dev/pytest-cov/issues/434) &lt;https://github.com/pytest-dev/pytest-cov/pull/434&gt;</code>_.</li>
<li>Fixed the missing <code>coverage context &lt;https://coverage.readthedocs.io/en/latest/contexts.html&gt;</code>_
when using subprocesses.
Contributed by Bernát Gábor in <code>[#443](https://github.com/pytest-dev/pytest-cov/issues/443) &lt;https://github.com/pytest-dev/pytest-cov/pull/443&gt;</code>_.</li>
<li>Updated the config section in the docs.
Contributed by Pamela McA'Nulty in <code>[#429](https://github.com/pytest-dev/pytest-cov/issues/429) &lt;https://github.com/pytest-dev/pytest-cov/pull/429&gt;</code>_.</li>
<li>Migrated CI to travis-ci.com (from .org).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/67d49b9e06cbc1cace3fc2cdfe70b09f55d1726f"><code>67d49b9</code></a> Bump version: 2.12.0 → 2.12.1</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/3685acbd61df9135e41b188374347d04d2d689db"><code>3685acb</code></a> Use 2019 image for pypy.</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/df20c973a5a34c4e085362dcf41df88fc3ee6297"><code>df20c97</code></a> Looks like I got the images wrong.</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/17252e0896ac18d7b15284d8dc4e2ecb16b050c9"><code>17252e0</code></a> Remove unnecessary pin.</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/ac7cc916268266807d43e9d7f0bcb1ae4277010c"><code>ac7cc91</code></a> Update changelog.</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/34edfa1cf80f8d722dec4f587b10d2783f89a0f0"><code>34edfa1</code></a> Avoid using toml as extra (<a href="https://redirect.github.com/pytest-dev/pytest-cov/issues/472">#472</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/edc60bb9e560d7ea53056590a64a4e5c81b5e62c"><code>edc60bb</code></a> Document <code>show_contexts</code> (<a href="https://redirect.github.com/pytest-dev/pytest-cov/issues/473">#473</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/297965e05a7712e50c2f8a4dc26cd189132aba22"><code>297965e</code></a> Update appveyor envs. Workaround pypy install problem.</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/9692bad8c3501b77cf950d0732ae9cb5c8bb0bd4"><code>9692bad</code></a> Bump version: 2.11.1 → 2.12.0</li>
<li><a href="https://github.com/pytest-dev/pytest-cov/commit/f533121b78d479ee4bf0c3c09b48d9513523ffb1"><code>f533121</code></a> Update changelog.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-cov/compare/v2.10.1...v2.12.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-cov&package-manager=pip&previous-version=2.10.1&new-version=2.12.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:55:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    build(deps-dev): update pytest requirement from ~=6.2 to ~=8.2 in /acapy/plugins/firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest](https://github.com/pytest-dev/pytest) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.2</h2>
<h1>pytest 8.2.2 (2024-06-04)</h1>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12355">#12355</a>: Fix possible catastrophic performance slowdown on a certain parametrization pattern involving many higher-scoped parameters.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12367">#12367</a>: Fix a regression in pytest 8.2.0 where unittest class instances (a fresh one is created for each test) were not released promptly on test teardown but only on session teardown.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12381">#12381</a>: Fix possible &quot;Directory not empty&quot; crashes arising from concurent cache dir (<code>.pytest_cache</code>) creation. Regressed in pytest 8.2.0.</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12290">#12290</a>: Updated Sphinx theme to use Furo instead of Flask, enabling Dark mode theme.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12356">#12356</a>: Added a subsection to the documentation for debugging flaky tests to mention
lack of thread safety in pytest as a possible source of flakyness.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12363">#12363</a>: The documentation webpages now links to a canonical version to reduce outdated documentation in search engine results.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/329d3712146e69c471be3e30883d54bdde2f76cb"><code>329d371</code></a> Prepare release version 8.2.2</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/214d098fcce88940f5ce9353786b3cc8f0bd3938"><code>214d098</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12414">#12414</a> from bluetech/backport-12409</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/153a436bc40c9e89d90d62255ef5a89e9a762dca"><code>153a436</code></a> [8.2.x] fixtures: fix catastrophic performance problem in <code>reorder_items</code></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/b41d5a52bbb808780ab310456d71e5ce509fd402"><code>b41d5a5</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12412">#12412</a> from pytest-dev/backport-12408-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9bb73d734ff40f52d7bbebd708b5e3ab1ba20798"><code>9bb73d7</code></a> [8.2.x] cacheprovider: fix &quot;Directory not empty&quot; crash from cache directory c...</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4569a01e3d20d64811d48b0b09539596520ea5a6"><code>4569a01</code></a> [8.2.x] doc: Update trainings/events (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12402">#12402</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/1d103e5cdc1cb08f332e61a5b20fb205fa5228e7"><code>1d103e5</code></a> [8.2.x] Clarify pytest_ignore_collect docs (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12386">#12386</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/240a252d34fff26efad5b3a92e62be4c9af94b70"><code>240a252</code></a> [8.2.x] Add html_baseurl to sphinx conf.py (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12372">#12372</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a5ee3c41268199c2c0af59c33050326b1c4a342e"><code>a5ee3c4</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12370">#12370</a> from pytest-dev/backport-12368-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f7358aec2884720b4de4594ffd0811b46316514c"><code>f7358ae</code></a> [8.2.x] unittest: fix class instances no longer released on test teardown sin...</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/6.2.0...8.2.2">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 11:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    build(deps): update marshmallow requirement from ~=3.20.1 to ~=3.21.3 in /acapy/plugins/firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [marshmallow](https://github.com/marshmallow-code/marshmallow) to permit the latest version.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/marshmallow-code/marshmallow/blob/dev/CHANGELOG.rst">marshmallow's changelog</a>.</em></p>
<blockquote>
<p>3.21.3 (2024-06-05)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix memory leak that prevented schema instances from getting GC'd (:pr:<code>2277</code>).
Thanks :user:<code>mrcljx</code> for the PR.</li>
</ul>
<p>3.21.2 (2024-05-01)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Allow timestamp 0 in <code>fields.DateTime</code> (:issue:<code>2133</code>).
Thanks :user:<code>flydzen</code> for reporting.</li>
</ul>
<p>3.21.1 (2024-03-04)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix error message when field is declared as a class and not an instance (:issue:<code>2245</code>).
Thanks :user:<code>travnick</code> for reporting.</li>
</ul>
<p>3.21.0 (2024-02-26)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix validation of <code>URL</code> fields to allow missing user field,
per NWG RFC 3986 (:issue:<code>2232</code>). Thanks :user:<code>ddennerline3</code> for reporting
and :user:<code>deckar01</code> for the PR.</li>
</ul>
<p>Other changes:</p>
<ul>
<li><em>Backwards-incompatible</em>: <code>__version__</code>, <code>__parsed_version__</code>, and <code>__version_info__</code>
attributes are deprecated (:issue:<code>2227</code>). Use feature detection or
<code>importlib.metadata.version(&quot;marshmallow&quot;)</code> instead.</li>
</ul>
<p>3.20.2 (2024-01-09)</p>
<hr />
<p>Bug fixes:</p>
<ul>
<li>Fix <code>Nested</code> field type hint for lambda <code>Schema</code> types (:pr:<code>2164</code>).
Thanks :user:<code>somethingnew2-0</code> for the PR.</li>
</ul>
<p>Other changes:</p>
<ul>
<li>Officially support Python 3.12 (:pr:<code>2188</code>).</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/b9646e326c511c11fc07aef4aa0004c14a5d454c"><code>b9646e3</code></a> Bump version and update changelog</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/99103a675fa469c05ea93c4cbc91d47fd5556eee"><code>99103a6</code></a> Remove leaky lru_cache (<a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2277">#2277</a>)</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/47205b5c4f89794341eebbbbd0e39b765c4c8bbe"><code>47205b5</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2276">#2276</a>)</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/aaecd5b02dc46b068e30964edbfb8d91d1eab3db"><code>aaecd5b</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/c592536b649fab0bbfb4bc3f84b65577a13b8ca2"><code>c592536</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2269">#2269</a>)</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/ee0c903c3c1ea6ee4e00b9565ab2556da996b6de"><code>ee0c903</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/d4fd5a4abbb556e337afde6b46bf3a37ab7100f9"><code>d4fd5a4</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/511b8c5354929b78b63d57578556443e41f8293f"><code>511b8c5</code></a> Bump version and update changelog</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/03f56a4f0fae9e650028227be265b5786b0575a9"><code>03f56a4</code></a> Merge pull request <a href="https://redirect.github.com/marshmallow-code/marshmallow/issues/2264">#2264</a> from marshmallow-code/allow_timestamp_0</li>
<li><a href="https://github.com/marshmallow-code/marshmallow/commit/58fbbcd3446ade39ea3be83ce9ee9170acf0230b"><code>58fbbcd</code></a> Encapsulate timestamp boolean check in utils</li>
<li>Additional commits viewable in <a href="https://github.com/marshmallow-code/marshmallow/compare/3.20.1...3.21.3">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 11:55:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    build(deps-dev): update mock requirement from ~=4.0 to ~=5.1 in /acapy/plugins/firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [mock](https://github.com/testing-cabal/mock) to permit the latest version.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/testing-cabal/mock/blob/master/CHANGELOG.rst">mock's changelog</a>.</em></p>
<blockquote>
<h2>5.1.0</h2>
<ul>
<li>
<p>bpo-44185: :func:<code>unittest.mock.mock_open</code> will call the :func:<code>close</code>
method of the file handle mock when it is exiting from the context
manager. Patch by Samet Yaslan.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/94924">gh-94924</a>: :func:<code>unittest.mock.create_autospec</code> now properly returns
coroutine functions compatible with :func:<code>inspect.iscoroutinefunction</code></p>
</li>
<li>
<p>bpo-17013: Add <code>ThreadingMock</code> to :mod:<code>unittest.mock</code> that can be used
to create Mock objects that can wait until they are called. Patch by
Karthikeyan Singaravelan and Mario Corchero.</p>
</li>
<li>
<p>bpo-41768: :mod:<code>unittest.mock</code> speccing no longer calls class properties.
Patch by Melanie Witt.</p>
</li>
</ul>
<h2>5.0.2</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/102978">gh-102978</a>: Fixes :func:<code>unittest.mock.patch</code> not enforcing function
signatures for methods decorated with <code>@classmethod</code> or
<code>@staticmethod</code> when patch is called with <code>autospec=True</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/103329">gh-103329</a>: Regression tests for the behaviour of
<code>unittest.mock.PropertyMock</code> were added.</p>
</li>
</ul>
<h2>5.0.1</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/100740">gh-100740</a>: Fix <code>unittest.mock.Mock</code> not respecting the spec for
attribute names prefixed with <code>assert</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/100690">gh-100690</a>: <code>Mock</code> objects which are not unsafe will now raise an
<code>AttributeError</code> when accessing an attribute that matches the name of an
assertion but without the prefix <code>assert_</code>, e.g. accessing
<code>called_once</code> instead of <code>assert_called_once</code>. This is in addition to
this already happening for accessing attributes with prefixes <code>assert</code>,
<code>assret</code>, <code>asert</code>, <code>aseert</code>, and <code>assrt</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/96127">gh-96127</a>: <code>inspect.signature</code> was raising <code>TypeError</code> on call with
mock objects. Now it correctly returns <code>(*args, **kwargs)</code> as infered
signature.</p>
</li>
</ul>
<h2>5.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/testing-cabal/mock/issues/98624">gh-98624</a>: Add a mutex to unittest.mock.NonCallableMock to protect
concurrent access to mock attributes.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/testing-cabal/mock/commit/d344fa2794b3b1ae7e4a4dbf265fb040d6f41d1f"><code>d344fa2</code></a> Preparing for 5.1.0 release.</li>
<li><a href="https://github.com/testing-cabal/mock/commit/e53a01c315095bac1101fb3545c61382dc0d23fd"><code>e53a01c</code></a> latest sync point</li>
<li><a href="https://github.com/testing-cabal/mock/commit/73343195e09fd20b9a39187a71c138fa13e02f9d"><code>7334319</code></a> Remove unused branches from mock module (<a href="https://redirect.github.com/testing-cabal/mock/issues/106617">#106617</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/f0cc38503e2d91341ca4e263d5acf934b7c0d130"><code>f0cc385</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/61215">GH-61215</a>: threadingmock: Remove unused branch for <code>timeout</code> (<a href="https://redirect.github.com/testing-cabal/mock/issues/106591">#106591</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/acd5fc58e41cd866b4ceff262140bd3304fb127a"><code>acd5fc5</code></a> Python 3.6+ compat</li>
<li><a href="https://github.com/testing-cabal/mock/commit/8d36bf4cc5f86cb7cc0b60d7b9f2c9c5e53f7f37"><code>8d36bf4</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/106300">gh-106300</a>: Improve <code>assertRaises(Exception)</code> usages in tests (<a href="https://redirect.github.com/testing-cabal/mock/issues/106302">GH-106302</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/9cbc589905dbb0f415ab3a995eee48f4906c0418"><code>9cbc589</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/106458">gh-106458</a>: Mark <code>testthreadingmock.py</code> with <code>@requires_working_threading</code> (GH...</li>
<li><a href="https://github.com/testing-cabal/mock/commit/0dc15d43989f7563b442b82e2807819b50b9d726"><code>0dc15d4</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/61215">gh-61215</a>: Rename <code>wait_until_any_call</code> to <code>wait_until_any_call_with</code> (<a href="https://redirect.github.com/testing-cabal/mock/issues/106414">#106414</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/cb8b3c8c8a3f1661f93b989440853b9377a91303"><code>cb8b3c8</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/61215">gh-61215</a>: New mock to wait for multi-threaded events to happen (<a href="https://redirect.github.com/testing-cabal/mock/issues/16094">#16094</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/0bd94e622397bb2245a951086adb450731ee5d63"><code>0bd94e6</code></a> bpo-44185: Added close() to mock_open <strong>exit</strong> (<a href="https://redirect.github.com/testing-cabal/mock/issues/26902">#26902</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/testing-cabal/mock/compare/4.0.0...5.1.0">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 11:55:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    build(deps): bump ubuntu from 18.04 to 24.04 in /afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps ubuntu from 18.04 to 24.04.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ubuntu&package-manager=docker&previous-version=18.04&new-version=24.04)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:49:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    build(deps): bump findy-network/findy-base from indy-1.16.ubuntu-18.04 to indy-1.16.ubuntu-22.04 in /afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps [findy-network/findy-base](https://github.com/findy-network/findy-agent-infra) from indy-1.16.ubuntu-18.04 to indy-1.16.ubuntu-22.04.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/findy-network/findy-agent-infra/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=findy-network/findy-base&package-manager=docker&previous-version=indy-1.16.ubuntu-18.04&new-version=indy-1.16.ubuntu-22.04)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:49:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    build(deps): bump ubuntu from 20.04 to 24.04 in /load-testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps ubuntu from 20.04 to 24.04.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ubuntu&package-manager=docker&previous-version=20.04&new-version=24.04)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:47:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    build(deps): bump @aries-framework/core from 0.3.3 to 0.4.2 in /afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@aries-framework/core](https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core) from 0.3.3 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-framework-javascript/releases"><code>@​aries-framework/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<p>Release v0.4.2</p>
<p>You can find the changelog in the <a href="https://github.com/hyperledger/aries-framework-javascript/blob/main/CHANGELOG.md">CHANGELOG.md</a> file.</p>
<h2>v0.4.1</h2>
<p>Release v0.4.1</p>
<p>You can find the changelog in the <a href="https://github.com/hyperledger/aries-framework-javascript/blob/main/CHANGELOG.md">CHANGELOG.md</a> file.</p>
<h2>v0.4.0</h2>
<p>Release v0.4.0</p>
<p>You can find the changelog in the <a href="https://github.com/hyperledger/aries-framework-javascript/blob/main/CHANGELOG.md">CHANGELOG.md</a> file.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/openwallet-foundation/credo-ts/blob/main/packages/core/CHANGELOG.md"><code>@​aries-framework/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/hyperledger/aries-framework-javascript/compare/v0.4.1...v0.4.2">0.4.2</a> (2023-10-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>askar:</strong> throw error if imported wallet exists (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1593">#1593</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/c2bb2a52f10add35de883c9a27716db01b9028df">c2bb2a5</a>)</li>
<li><strong>core:</strong> remove node-fetch dependency (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1578">#1578</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/9ee2ce7f0913510fc5b36aef1b7eeffb259b4aed">9ee2ce7</a>)</li>
<li>do not send package via outdated session (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1559">#1559</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/de6a735a900b6d7444b17d79e63acaca19cb812a">de6a735</a>)</li>
<li>duplicate service ids in connections protocol (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1589">#1589</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/dd75be88c4e257b6ca76868ceaeb3a8b7d67c185">dd75be8</a>)</li>
<li>implicit invitation to specific service (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1592">#1592</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/4071dc97b8ca779e6def3711a538ae821e1e513c">4071dc9</a>)</li>
<li>log and throw on WebSocket sending errors (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1573">#1573</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/11050afc7965adfa9b00107ba34abfbe3afaf874">11050af</a>)</li>
<li><strong>oob:</strong> support oob with connection and messages (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1558">#1558</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/9732ce436a0ddee8760b02ac5182e216a75176c2">9732ce4</a>)</li>
<li>service validation in OOB invitation objects (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1575">#1575</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/91a9434efd53ccbaf80f5613cd908913ad3b806b">91a9434</a>)</li>
<li>update tsyringe for ts 5 support (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1588">#1588</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/296955b3a648416ac6b502da05a10001920af222">296955b</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>allow connection invitation encoded in oob url param (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1583">#1583</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/9d789fa4e9d159312872f45089d73609eb3d6835">9d789fa</a>)</li>
</ul>
<h2><a href="https://github.com/hyperledger/aries-framework-javascript/compare/v0.4.0...v0.4.1">0.4.1</a> (2023-08-28)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>create message subscription first (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1549">#1549</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/93276debeff1e56c9803e7700875c4254a48236b">93276de</a>)</li>
<li>force did:key resolver/registrar presence (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1535">#1535</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/aaa13dc77d6d5133cd02e768e4173462fa65064a">aaa13dc</a>)</li>
<li>listen to incoming messages on agent initialize not constructor (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1542">#1542</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/8f2d593bcda0bb2d7bea25ad06b9e37784961997">8f2d593</a>)</li>
<li>priority sorting for didcomm services (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1555">#1555</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/80c37b30eb9ac3b438288e14c252f79f619dd12f">80c37b3</a>)</li>
<li>race condition singleton records (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1495">#1495</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/6c2dda544bf5f5d3a972a778c389340da6df97c4">6c2dda5</a>)</li>
<li><strong>transport:</strong> Use connection in WebSocket ID (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1551">#1551</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/8d2057f3fe6f3ba236ba5a811b57a7256eae92bf">8d2057f</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li><strong>anoncreds:</strong> auto create link secret (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1521">#1521</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/c6f03e49d79a33b1c4b459cef11add93dee051d0">c6f03e4</a>)</li>
<li>oob without handhsake improvements and routing (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1511">#1511</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/9e69cf441a75bf7a3c5556cf59e730ee3fce8c28">9e69cf4</a>)</li>
<li>support askar profiles for multi-tenancy (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1538">#1538</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/e448a2a58dddff2cdf80c4549ea2d842a54b43d1">e448a2a</a>)</li>
<li><strong>w3c:</strong> add convenience methods to vc and vp (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1477">#1477</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/83cbfe38e788366b616dc244fe34cc49a5a4d331">83cbfe3</a>)</li>
</ul>
<h1><a href="https://github.com/hyperledger/aries-framework-javascript/compare/v0.3.3...v0.4.0">0.4.0</a> (2023-06-03)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>connection id in sessions for new connections (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1383">#1383</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/0351eec52a9f5e581508819df3005be7b995e59e">0351eec</a>)</li>
<li><strong>connections:</strong> store imageUrl when using DIDExchange (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1433">#1433</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/66afda2fe7311977047928e0b1c857ed2c5602c7">66afda2</a>)</li>
<li><strong>core:</strong> repository event when calling deleteById (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1356">#1356</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/953069a785f2a6b8d1e11123aab3a09aab1e65ff">953069a</a>)</li>
<li>create new socket if socket state is 'closing' (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1337">#1337</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/da8f2ad36c386497b16075790a364faae50fcd47">da8f2ad</a>)</li>
<li>Emit RoutingCreated event for mediator routing record (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1445">#1445</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/414595727d611ff774c4f404a4eeea509cf03a71">4145957</a>)</li>
<li>imports from core (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1303">#1303</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/3e02227a7b23677e9886eb1c03d1a3ec154947a9">3e02227</a>)</li>
<li>isNewSocket logic (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1355">#1355</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/18abb18316f155d0375af477dedef9cdfdada70e">18abb18</a>)</li>
<li>issuance with unqualified identifiers (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1431">#1431</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/de90cafb8d12b7a940f881184cd745c4b5043cbc">de90caf</a>)</li>
<li>jsonld credential format identifier version (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1412">#1412</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/c46a6b81b8a1e28e05013c27ffe2eeaee4724130">c46a6b8</a>)</li>
<li>loosen base64 validation (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1312">#1312</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/af384e8a92f877c647999f9356b72a8017308230">af384e8</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/a0458febe4902e823c81b8e394a39b6bdbff31bc"><code>a0458fe</code></a> chore(release): v0.4.2 (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1591">#1591</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/296955b3a648416ac6b502da05a10001920af222"><code>296955b</code></a> fix: update tsyringe for ts 5 support (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1588">#1588</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/91a9434efd53ccbaf80f5613cd908913ad3b806b"><code>91a9434</code></a> fix: service validation in OOB invitation objects (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1575">#1575</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/c2bb2a52f10add35de883c9a27716db01b9028df"><code>c2bb2a5</code></a> fix(askar): throw error if imported wallet exists (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1593">#1593</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/4071dc97b8ca779e6def3711a538ae821e1e513c"><code>4071dc9</code></a> fix: implicit invitation to specific service (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1592">#1592</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/dd75be88c4e257b6ca76868ceaeb3a8b7d67c185"><code>dd75be8</code></a> fix: duplicate service ids in connections protocol (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1589">#1589</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/9d789fa4e9d159312872f45089d73609eb3d6835"><code>9d789fa</code></a> feat: allow connection invitation encoded in oob url param (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1583">#1583</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/9732ce436a0ddee8760b02ac5182e216a75176c2"><code>9732ce4</code></a> fix(oob): support oob with connection and messages (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1558">#1558</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/11050afc7965adfa9b00107ba34abfbe3afaf874"><code>11050af</code></a> fix: log and throw on WebSocket sending errors (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1573">#1573</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/9ee2ce7f0913510fc5b36aef1b7eeffb259b4aed"><code>9ee2ce7</code></a> fix(core): remove node-fetch dependency (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/core/issues/1578">#1578</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-framework-javascript/commits/v0.4.2/packages/core">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@aries-framework/core&package-manager=npm_and_yarn&previous-version=0.3.3&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:42:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/146" class=".btn">#146</a>
            </td>
            <td>
                <b>
                    build(deps): bump @aries-framework/node from 0.3.3 to 0.4.2 in /afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@aries-framework/node](https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node) from 0.3.3 to 0.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-framework-javascript/releases"><code>@​aries-framework/node</code>'s releases</a>.</em></p>
<blockquote>
<h2>v0.4.2</h2>
<p>Release v0.4.2</p>
<p>You can find the changelog in the <a href="https://github.com/hyperledger/aries-framework-javascript/blob/main/CHANGELOG.md">CHANGELOG.md</a> file.</p>
<h2>v0.4.1</h2>
<p>Release v0.4.1</p>
<p>You can find the changelog in the <a href="https://github.com/hyperledger/aries-framework-javascript/blob/main/CHANGELOG.md">CHANGELOG.md</a> file.</p>
<h2>v0.4.0</h2>
<p>Release v0.4.0</p>
<p>You can find the changelog in the <a href="https://github.com/hyperledger/aries-framework-javascript/blob/main/CHANGELOG.md">CHANGELOG.md</a> file.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/openwallet-foundation/credo-ts/blob/main/packages/node/CHANGELOG.md"><code>@​aries-framework/node</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/hyperledger/aries-framework-javascript/compare/v0.4.1...v0.4.2">0.4.2</a> (2023-10-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>log and throw on WebSocket sending errors (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1573">#1573</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/11050afc7965adfa9b00107ba34abfbe3afaf874">11050af</a>)</li>
</ul>
<h2><a href="https://github.com/hyperledger/aries-framework-javascript/compare/v0.4.0...v0.4.1">0.4.1</a> (2023-08-28)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>samples:</strong> mediator wallet and http transport (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1508">#1508</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/04a80589b19725fb493e51e52a7345915b2c7341">04a8058</a>)</li>
</ul>
<h1><a href="https://github.com/hyperledger/aries-framework-javascript/compare/v0.3.3...v0.4.0">0.4.0</a> (2023-06-03)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>
<p>return HTTP 415 if unsupported content type (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1313">#1313</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/122cdde6982174a8e9cf70ef26a1393cb3912066">122cdde</a>)</p>
</li>
<li>
<p>feat!: add data, cache and temp dirs to FileSystem (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1306">#1306</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/ff5596d0631e93746494c017797d0191b6bdb0b1">ff5596d</a>), closes <a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1306">#1306</a></p>
</li>
</ul>
<h3>Features</h3>
<ul>
<li>add initial askar package (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1211">#1211</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/f18d1890546f7d66571fe80f2f3fc1fead1cd4c3">f18d189</a>)</li>
<li><strong>anoncreds:</strong> legacy indy proof format service (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1283">#1283</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/c72fd7416f2c1bc0497a84036e16adfa80585e49">c72fd74</a>)</li>
<li><strong>askar:</strong> import/export wallet support for SQLite (<a href="https://redirect.github.com/hyperledger/aries-framework-javascript/issues/1377">#1377</a>) (<a href="https://github.com/hyperledger/aries-framework-javascript/commit/19cefa54596a4e4848bdbe89306a884a5ce2e991">19cefa5</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li>Agent-produced files will now be divided in different system paths depending on their nature: data, temp and cache. Previously, they were located at a single location, defaulting to a temporary directory.</li>
</ul>
<p>If you specified a custom path in <code>FileSystem</code> object constructor, you now must provide an object containing <code>baseDataPath</code>, <code>baseTempPath</code> and <code>baseCachePath</code>. They can point to the same path, although it's recommended to specify different path to avoid future file clashes.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/a0458febe4902e823c81b8e394a39b6bdbff31bc"><code>a0458fe</code></a> chore(release): v0.4.2 (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1591">#1591</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/11050afc7965adfa9b00107ba34abfbe3afaf874"><code>11050af</code></a> fix: log and throw on WebSocket sending errors (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1573">#1573</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/c0d9304790e3fdee5dfb8791c73f4d18b788b9bb"><code>c0d9304</code></a> chore(release): v0.4.1 (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1548">#1548</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/04a80589b19725fb493e51e52a7345915b2c7341"><code>04a8058</code></a> fix(samples): mediator wallet and http transport (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1508">#1508</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/efc0ddfd23290f99bfde6a3e27c4f1e682630b2e"><code>efc0ddf</code></a> chore(release): v0.4.0 (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1475">#1475</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/11366e540421517ce21e8cca8781741fc482be8e"><code>11366e5</code></a> fix!: return didcomm mime-type in http response (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1456">#1456</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/d247b53d99629e4ba768a55b617a217936fcef89"><code>d247b53</code></a> feat(indy-vdr)!: did transaction endorsement (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1417">#1417</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/95582560cc071e088e4b23d962a13dfcd93e308f"><code>9558256</code></a> chore!: update dependencies (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1388">#1388</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/122cdde6982174a8e9cf70ef26a1393cb3912066"><code>122cdde</code></a> fix: return HTTP 415 if unsupported content type (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1313">#1313</a>)</li>
<li><a href="https://github.com/openwallet-foundation/credo-ts/commit/19cefa54596a4e4848bdbe89306a884a5ce2e991"><code>19cefa5</code></a> feat(askar): import/export wallet support for SQLite (<a href="https://github.com/hyperledger/aries-framework-javascript/tree/HEAD/packages/node/issues/1377">#1377</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-framework-javascript/commits/v0.4.2/packages/node">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@aries-framework/node&package-manager=npm_and_yarn&previous-version=0.3.3&new-version=0.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:42:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/145" class=".btn">#145</a>
            </td>
            <td>
                <b>
                    build(deps): bump tslog from 4.8.2 to 4.9.3 in /afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tslog](https://github.com/fullstack-build/tslog) from 4.8.2 to 4.9.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/fullstack-build/tslog/releases">tslog's releases</a>.</em></p>
<blockquote>
<h2>v4.9.3</h2>
<ul>
<li>Fix _extend fn - alter provided object  135ee61</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.9.2...v4.9.3">https://github.com/fullstack-build/tslog/compare/v4.9.2...v4.9.3</a></p>
<h2>v4.9.2</h2>
<ul>
<li>Add more tests for some types  1e93acc</li>
<li>Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/259">#259</a> from vktrl/master  3044fce</li>
<li>add null test for node  be1e549</li>
<li>fix undefined check, add null test for browser  d510305</li>
<li>Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/257">#257</a> from fullstack-build/development  6ab687e</li>
<li>Fix docs, fix <a href="https://redirect.github.com/fullstack-build/tslog/issues/256">#256</a>  c24f7e1</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.9.1...v4.9.2">https://github.com/fullstack-build/tslog/compare/v4.9.1...v4.9.2</a></p>
<h2>v4.9.1</h2>
<ul>
<li>Move runtime into BaseLogger, fix <a href="https://redirect.github.com/fullstack-build/tslog/issues/256">#256</a>  4bb3465</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.9.0...v4.9.1">https://github.com/fullstack-build/tslog/compare/v4.9.0...v4.9.1</a></p>
<h2>v4.9.0</h2>
<ul>
<li>Support errors with multiple properties, Fix <a href="https://redirect.github.com/fullstack-build/tslog/issues/227">#227</a>  7743ccb</li>
<li>Add URL support, fix <a href="https://redirect.github.com/fullstack-build/tslog/issues/247">#247</a>  ef3dd47</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.8.7...v4.9.0">https://github.com/fullstack-build/tslog/compare/v4.8.7...v4.9.0</a></p>
<h2>v4.8.7</h2>
<ul>
<li>Fix <a href="https://redirect.github.com/fullstack-build/tslog/issues/254">#254</a>  a7ed0e7</li>
<li>Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/255">#255</a> from sachaw/development-1  6fa3885</li>
<li>Update util.inspect.polyfil.ts  42fcbb4</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.8.6...v4.8.7">https://github.com/fullstack-build/tslog/compare/v4.8.6...v4.8.7</a></p>
<h2>v4.8.6</h2>
<ul>
<li>fix nodejs environment usage in browser environments for v4.8.5  dee37b0</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.8.5...v4.8.6">https://github.com/fullstack-build/tslog/compare/v4.8.5...v4.8.6</a></p>
<h2>v4.8.5</h2>
<ul>
<li>Add ESM file extensions, fix <a href="https://redirect.github.com/fullstack-build/tslog/issues/250">#250</a>  2ead365</li>
</ul>
<p><a href="https://github.com/fullstack-build/tslog/compare/v4.8.4...v4.8.5">https://github.com/fullstack-build/tslog/compare/v4.8.4...v4.8.5</a></p>
<h2>v4.8.4</h2>
<ul>
<li>Make Universal again  80ace78</li>
<li>allow for custom placeholders in the template string  2467191</li>
<li>Clone error with all constructor parameters  0e751a5</li>
<li>Add typings for helper methods  c643b10</li>
<li>Fix typing for settings  6f3b68e</li>
<li>Actually export my types  1929006</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/fullstack-build/tslog/commit/c4e6eadc85ed79763792fb8a3049e2d50c88b2dc"><code>c4e6ead</code></a> 4.9.3</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/f42d3fbd918551a3829c001249e6940175668ee8"><code>f42d3fb</code></a> Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/290">#290</a> from fullstack-build/development</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/c7fd9123c8be02e5794b7e867b4accc1b546d8d5"><code>c7fd912</code></a> Update README</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/21821bdb8fdbdcc287fe6f03f79b0d2adea0a051"><code>21821bd</code></a> Update README to reflect the lower test coverage</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/7e47b61207b99be26109b87e228f0a2cda6e2fb2"><code>7e47b61</code></a> Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/286">#286</a> from jakubhruby/master</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/8190017def691c739096fddad91c8a7b678212a5"><code>8190017</code></a> Format source</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/f9fc041f245959825bb68734d0e91eeb0e2ea43e"><code>f9fc041</code></a> Merge master into development</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/f7474a346ba4b0bd6a289b75b4618548059ccb21"><code>f7474a3</code></a> Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/281">#281</a> from fullstack-build/dependabot/npm_and_yarn/axios-an...</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/e1305b01e2c55ccaaf93c802ed3ff8ed65212b8a"><code>e1305b0</code></a> Merge branch 'master' into dependabot/npm_and_yarn/axios-and-jest-puppeteer-1...</li>
<li><a href="https://github.com/fullstack-build/tslog/commit/3cb27fc977b579eb9447700486a7c3f5453c6fad"><code>3cb27fc</code></a> Merge pull request <a href="https://redirect.github.com/fullstack-build/tslog/issues/288">#288</a> from fullstack-build/dependabot/npm_and_yarn/examples...</li>
<li>Additional commits viewable in <a href="https://github.com/fullstack-build/tslog/compare/v4.8.2...v4.9.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tslog&package-manager=npm_and_yarn&previous-version=4.8.2&new-version=4.9.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:41:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    build(deps): bump dotenv from 16.0.3 to 16.4.5 in /load-testing/load-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [dotenv](https://github.com/motdotla/dotenv) from 16.0.3 to 16.4.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/motdotla/dotenv/blob/master/CHANGELOG.md">dotenv's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.4.4...v16.4.5">16.4.5</a> (2024-02-19)</h2>
<h3>Changed</h3>
<ul>
<li>🐞 fix recent regression when using <code>path</code> option. return to historical behavior: do not attempt to auto find <code>.env</code> if <code>path</code> set. (regression was introduced in <code>16.4.3</code>) <a href="https://redirect.github.com/motdotla/dotenv/pull/814">#814</a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.4.3...v16.4.4">16.4.4</a> (2024-02-13)</h2>
<h3>Changed</h3>
<ul>
<li>🐞 Replaced chaining operator <code>?.</code> with old school <code>&amp;&amp;</code> (fixing node 12 failures) <a href="https://redirect.github.com/motdotla/dotenv/pull/812">#812</a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.4.2...v16.4.3">16.4.3</a> (2024-02-12)</h2>
<h3>Changed</h3>
<ul>
<li>Fixed processing of multiple files in <code>options.path</code> <a href="https://redirect.github.com/motdotla/dotenv/pull/805">#805</a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.4.1...v16.4.2">16.4.2</a> (2024-02-10)</h2>
<h3>Changed</h3>
<ul>
<li>Changed funding link in package.json to <a href="https://dotenvx.com"><code>dotenvx.com</code></a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.4.0...v16.4.1">16.4.1</a> (2024-01-24)</h2>
<ul>
<li>Patch support for array as <code>path</code> option <a href="https://redirect.github.com/motdotla/dotenv/pull/797">#797</a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.3.2...v16.4.0">16.4.0</a> (2024-01-23)</h2>
<ul>
<li>Add <code>error.code</code> to error messages around <code>.env.vault</code> decryption handling <a href="https://redirect.github.com/motdotla/dotenv/pull/795">#795</a></li>
<li>Add ability to find <code>.env.vault</code> file when filename(s) passed as an array <a href="https://redirect.github.com/motdotla/dotenv/pull/784">#784</a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.3.1...v16.3.2">16.3.2</a> (2024-01-18)</h2>
<h3>Added</h3>
<ul>
<li>Add debug message when no encoding set <a href="https://redirect.github.com/motdotla/dotenv/pull/735">#735</a></li>
</ul>
<h3>Changed</h3>
<ul>
<li>Fix output typing for <code>populate</code> <a href="https://redirect.github.com/motdotla/dotenv/pull/792">#792</a></li>
<li>Use subarray instead of slice <a href="https://redirect.github.com/motdotla/dotenv/pull/793">#793</a></li>
</ul>
<h2><a href="https://github.com/motdotla/dotenv/compare/v16.3.0...v16.3.1">16.3.1</a> (2023-06-17)</h2>
<h3>Added</h3>
<ul>
<li>Add missing type definitions for <code>processEnv</code> and <code>DOTENV_KEY</code> options. <a href="https://redirect.github.com/motdotla/dotenv/pull/756">#756</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/motdotla/dotenv/commit/9f3e83352ec6ba912161748a2fd15b07829430e2"><code>9f3e833</code></a> 16.4.5</li>
<li><a href="https://github.com/motdotla/dotenv/commit/69241772b6f37af8e388f61916334d84ec0deeb7"><code>6924177</code></a> Merge pull request <a href="https://redirect.github.com/motdotla/dotenv/issues/814">#814</a> from motdotla/dont-check-existance</li>
<li><a href="https://github.com/motdotla/dotenv/commit/353342048cae3621f8abb3a23e00af880ab2c69f"><code>3533420</code></a> changelog 🪵</li>
<li><a href="https://github.com/motdotla/dotenv/commit/249e5a64f612d59aaac74f594f951024490d9765"><code>249e5a6</code></a> adjust logic to support tests</li>
<li><a href="https://github.com/motdotla/dotenv/commit/87fd887e31b913d334ef820f27737d80b28389ee"><code>87fd887</code></a> do not check if exists</li>
<li><a href="https://github.com/motdotla/dotenv/commit/1146910932ed1dd19c2c6506f7fc6373047c1321"><code>1146910</code></a> rename .env-multiline to .env.multiline</li>
<li><a href="https://github.com/motdotla/dotenv/commit/d03e39794ac29aa7e7fde20492b0b8c51544d9d7"><code>d03e397</code></a> 16.4.4</li>
<li><a href="https://github.com/motdotla/dotenv/commit/3275a0a940a8560bc42e93b5a814cea23b3dae38"><code>3275a0a</code></a> changelog 🪵</li>
<li><a href="https://github.com/motdotla/dotenv/commit/f40a8c3e3519ba9dca3014ff47541f276f90420a"><code>f40a8c3</code></a> Merge pull request <a href="https://redirect.github.com/motdotla/dotenv/issues/812">#812</a> from motdotla/patch-12</li>
<li><a href="https://github.com/motdotla/dotenv/commit/1dc22d312fc641c9384fcec4b8181d089e37de8c"><code>1dc22d3</code></a> replace 14 chaining operator</li>
<li>Additional commits viewable in <a href="https://github.com/motdotla/dotenv/compare/v16.0.3...v16.4.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=dotenv&package-manager=npm_and_yarn&previous-version=16.0.3&new-version=16.4.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:17:59 +0000 UTC
    </div>
</div>

