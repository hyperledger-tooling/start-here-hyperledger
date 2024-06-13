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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    build(deps): Bump the npm_and_yarn group across 1 directory with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 2 updates in the /common/policy-dsl directory: [braces](https://github.com/micromatch/braces) and [jest](https://github.com/jestjs/jest/tree/HEAD/packages/jest).

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-12 20:37:08 +0000 UTC
    </div>
</div>

