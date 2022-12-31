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

