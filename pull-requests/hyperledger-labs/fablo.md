---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    Simple K8 test and improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 12:18:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    Bump got and nodemon in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [got](https://github.com/sindresorhus/got). It's no longer used after updating ancestor dependency [nodemon](https://github.com/remy/nodemon). These dependencies need to be updated together.

Removes `got`

Updates `nodemon` from 2.0.18 to 2.0.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remy/nodemon/releases">nodemon's releases</a>.</em></p>
<blockquote>
<h2>v2.0.20</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.19...v2.0.20">2.0.20</a> (2022-09-16)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove postinstall script (<a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0">e099e91</a>)</li>
</ul>
<h2>v2.0.19</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.19">2.0.19</a> (2022-07-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Replace update notifier with simplified deps (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2033">#2033</a>) (<a href="https://github.com/remy/nodemon/commit/176c4a6bed989fe94f103c905e5eee341d26794d">176c4a6</a>), closes <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1961">#1961</a> <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2028">#2028</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0"><code>e099e91</code></a> fix: remove postinstall script</li>
<li><a href="https://github.com/remy/nodemon/commit/05de353d4de1a7e1f2aa2c9bf641c3fe2d652122"><code>05de353</code></a> chore: supports</li>
<li><a href="https://github.com/remy/nodemon/commit/876d60c8a241f13376f1b32f853d48ae77ec69a4"><code>876d60c</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/188f2d3cdc960fce5d7413e1326da76bd5be780c"><code>188f2d3</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/a1ad44a876df74be742c64af5640b300c302b977"><code>a1ad44a</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/8abd3fc9daff813199042c26a1e8aa5691a5ab37"><code>8abd3fc</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/30c80f8a4eee379fa2ebad95b81c42ef11670829"><code>30c80f8</code></a> chore: add unused files to .npmignore (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2055">#2055</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/3dd38deb4a97a52608aac148200b48d844df0a66"><code>3dd38de</code></a> docs: added link on banner (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1944">#1944</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/fb51359dde4b4ad6081f6c2690d1052fc8f5fcaf"><code>fb51359</code></a> docs: add important note about ignore rules</li>
<li><a href="https://github.com/remy/nodemon/commit/8fe7d770d06305e5e7a4aa4ab4783d4b2c5eaac8"><code>8fe7d77</code></a> chore: supporters</li>
<li>Additional commits viewable in <a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.20">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 06:20:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/354" class=".btn">#354</a>
            </td>
            <td>
                <b>
                    Bump async from 3.2.0 to 3.2.4 in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) from 3.2.0 to 3.2.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/master/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v3.2.4</h1>
<ul>
<li>Fix a bug in <code>priorityQueue</code> where it didn't wait for the result. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1725">#1725</a>)</li>
<li>Fix a bug where <code>unshiftAsync</code> was included in <code>priorityQueue</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1790">#1790</a>)</li>
</ul>
<h1>v3.2.3</h1>
<ul>
<li>Fix bugs in comment parsing in <code>autoInject</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1767">#1767</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1780">#1780</a>)</li>
</ul>
<h1>v3.2.2</h1>
<ul>
<li>Fix potential prototype pollution exploit</li>
</ul>
<h1>v3.2.1</h1>
<ul>
<li>Use <code>queueMicrotask</code> if available to the environment (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1761">#1761</a>)</li>
<li>Minor perf improvement in <code>priorityQueue</code> (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1727">#1727</a>)</li>
<li>More examples in documentation (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1726">#1726</a>)</li>
<li>Various doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1708">#1708</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1712">#1712</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1717">#1717</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1740">#1740</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1739">#1739</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1749">#1749</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1756">#1756</a>)</li>
<li>Improved test coverage (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1754">#1754</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/f3ab51af76ca87ebe3ec67b3dd6dec4959e04816"><code>f3ab51a</code></a> Version 3.2.4</li>
<li><a href="https://github.com/caolan/async/commit/7ea2cec7398b33a15daf5c3bd9bda6ae78caf297"><code>7ea2cec</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/bef7befc734e4b712ab6ffc82463cc40c1037056"><code>bef7bef</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/03eeab36ae5a0454bbf67b881f087692e0b7c7e4"><code>03eeab3</code></a> Bump yargs from 17.4.1 to 17.5.1 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1843">#1843</a>)</li>
<li><a href="https://github.com/caolan/async/commit/387efcf80f5b2c454effd2a64c75ff3c634ec3bd"><code>387efcf</code></a> Bump eslint from 8.14.0 to 8.17.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1849">#1849</a>)</li>
<li><a href="https://github.com/caolan/async/commit/131225a8c82fda93010b8b82da46e9a23b6b1816"><code>131225a</code></a> Bump karma from 6.3.19 to 6.3.20 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1844">#1844</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4cfa89cb240d9748d5bfee0656fbed08cf80cc10"><code>4cfa89c</code></a> Bump eslint from 8.14.0 to 8.16.0 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1845">#1845</a>)</li>
<li><a href="https://github.com/caolan/async/commit/90e940cbb5a051db7c2a28169769f97eef99fdd6"><code>90e940c</code></a> Bump rollup from 2.71.1 to 2.75.5 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1846">#1846</a>)</li>
<li><a href="https://github.com/caolan/async/commit/dd72cf5f614bcf2b08ae2678f6e8ffbd28136804"><code>dd72cf5</code></a> Bump <code>@​babel/eslint-parser</code> from 7.17.0 to 7.18.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1847">#1847</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4ae026e8da11f817f274f264dd3a9ec7ef3307c5"><code>4ae026e</code></a> Bump babel-minify from 0.5.1 to 0.5.2 (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1848">#1848</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/caolan/async/compare/v3.2.0...v3.2.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async&package-manager=npm_and_yarn&previous-version=3.2.0&new-version=3.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 06:19:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/353" class=".btn">#353</a>
            </td>
            <td>
                <b>
                    Bump jsdom and jest in /samples/chaincodes/chaincode-kv-node-1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [jsdom](https://github.com/jsdom/jsdom). It's no longer used after updating ancestor dependency [jest](https://github.com/facebook/jest/tree/HEAD/packages/jest). These dependencies need to be updated together.

Removes `jsdom`

Updates `jest` from 25.5.4 to 29.2.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/jest/releases">jest's releases</a>.</em></p>
<blockquote>
<h2>v29.2.2</h2>
<h2>Fixes</h2>
<ul>
<li><code>[@jest/test-sequencer]</code> Make sure sharding does not produce empty groups (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13476">#13476</a>)</li>
<li><code>[jest-circus]</code> Test marked as <code>todo</code> are shown as todo when inside a focussed describe (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13504">#13504</a>)</li>
<li><code>[jest-mock]</code> Ensure mock resolved and rejected values are promises from correct realm (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13503">#13503</a>)</li>
<li><code>[jest-snapshot]</code> Don't highlight passing asymmetric property matchers in snapshot diff (<a href="https://github-redirect.dependabot.com/facebook/jest/issues/13480">#13480</a>)</li>
</ul>
<h2>Chore &amp; Maintenance</h2>
<ul>
<li><code>[docs]</code> Update link to Jest 28 upgrade guide in error message (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13483">#13483</a>)</li>
<li><code>[jest-runner, jest-watcher]</code> Update <code>emittery</code> (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13490">#13490</a>)</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/moonrailgun"><code>@​moonrailgun</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/facebook/jest/pull/13483">facebook/jest#13483</a></li>
<li><a href="https://github.com/halldorbjarni"><code>@​halldorbjarni</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/facebook/jest/pull/13491">facebook/jest#13491</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/facebook/jest/compare/v29.2.1...v29.2.2">https://github.com/facebook/jest/compare/v29.2.1...v29.2.2</a></p>
<h2>v29.2.1</h2>
<h2>Features</h2>
<ul>
<li><code>[@jest/globals, jest-mock]</code> Add <code>jest.Spied*</code> utility types (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13440">#13440</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li><code>[jest-environment-node]</code> make <code>globalThis.performance</code> writable for Node 19 and fake timers (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13467">#13467</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://github-redirect.dependabot.com/facebook/jest/pull/13398">#13398</a> to restore mocking of setters (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13472">#13472</a>)</li>
</ul>
<h2>Performance</h2>
<ul>
<li><code>[*]</code> Use sha1 instead of sha256 for hashing (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13421">#13421</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/facebook/jest/compare/v29.2.0...v29.2.1">https://github.com/facebook/jest/compare/v29.2.0...v29.2.1</a></p>
<h2>v29.2.0</h2>
<h2>Features</h2>
<ul>
<li><code>[@jest/cli, jest-config]</code> A seed for the test run will be randomly generated, or set by a CLI option (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13400">#13400</a>)</li>
<li><code>[@jest/cli, jest-config]</code> <code>--show-seed</code> will display the seed value in the report, and can be set via a CLI flag or through the config file (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13400">#13400</a>)</li>
<li><code>[jest-config]</code> Add <code>readInitialConfig</code> utility function (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13356">#13356</a>)</li>
<li><code>[jest-core]</code> Allow <code>testResultsProcessor</code> to be async (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13343">#13343</a>)</li>
<li><code>[@jest/environment, jest-environment-node, jest-environment-jsdom, jest-runtime]</code> Add <code>getSeed()</code> to the <code>jest</code> object (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13400">#13400</a>)</li>
<li><code>[expect, @jest/expect-utils]</code> Allow <code>isA</code> utility to take a type argument (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13355">#13355</a>)</li>
<li><code>[expect]</code> Expose <code>AsyncExpectationResult</code> and <code>SyncExpectationResult</code> types (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13411">#13411</a>)</li>
</ul>
<h2>Fixes</h2>
<ul>
<li><code>[babel-plugin-jest-hoist]</code> Ignore <code>TSTypeQuery</code> when checking for hoisted references (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13367">#13367</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/jest/blob/main/CHANGELOG.md">jest's changelog</a>.</em></p>
<blockquote>
<h2>29.2.2</h2>
<h3>Fixes</h3>
<ul>
<li><code>[@jest/test-sequencer]</code> Make sure sharding does not produce empty groups (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13476">#13476</a>)</li>
<li><code>[jest-circus]</code> Test marked as <code>todo</code> are shown as todo when inside a focussed describe (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13504">#13504</a>)</li>
<li><code>[jest-mock]</code> Ensure mock resolved and rejected values are promises from correct realm (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13503">#13503</a>)</li>
<li><code>[jest-snapshot]</code> Don't highlight passing asymmetric property matchers in snapshot diff (<a href="https://github-redirect.dependabot.com/facebook/jest/issues/13480">#13480</a>)</li>
</ul>
<h3>Chore &amp; Maintenance</h3>
<ul>
<li><code>[docs]</code> Update link to Jest 28 upgrade guide in error message (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13483">#13483</a>)</li>
<li><code>[jest-runner, jest-watcher]</code> Update <code>emittery</code> (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13490">#13490</a>)</li>
</ul>
<h2>29.2.1</h2>
<h3>Features</h3>
<ul>
<li><code>[@jest/globals, jest-mock]</code> Add <code>jest.Spied*</code> utility types (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13440">#13440</a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li><code>[jest-environment-node]</code> make <code>globalThis.performance</code> writable for Node 19 and fake timers (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13467">#13467</a>)</li>
<li><code>[jest-mock]</code> Revert <a href="https://github-redirect.dependabot.com/facebook/jest/pull/13398">#13398</a> to restore mocking of setters (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13472">#13472</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li><code>[*]</code> Use sha1 instead of sha256 for hashing (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13421">#13421</a>)</li>
</ul>
<h2>29.2.0</h2>
<h3>Features</h3>
<ul>
<li><code>[@jest/cli, jest-config]</code> A seed for the test run will be randomly generated, or set by a CLI option (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13400">#13400</a>)</li>
<li><code>[@jest/cli, jest-config]</code> <code>--show-seed</code> will display the seed value in the report, and can be set via a CLI flag or through the config file (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13400">#13400</a>)</li>
<li><code>[jest-config]</code> Add <code>readInitialConfig</code> utility function (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13356">#13356</a>)</li>
<li><code>[jest-core]</code> Allow <code>testResultsProcessor</code> to be async (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13343">#13343</a>)</li>
<li><code>[@jest/environment, jest-environment-node, jest-environment-jsdom, jest-runtime]</code> Add <code>getSeed()</code> to the <code>jest</code> object (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13400">#13400</a>)</li>
<li><code>[expect, @jest/expect-utils]</code> Allow <code>isA</code> utility to take a type argument (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13355">#13355</a>)</li>
<li><code>[expect]</code> Expose <code>AsyncExpectationResult</code> and <code>SyncExpectationResult</code> types (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13411">#13411</a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li><code>[babel-plugin-jest-hoist]</code> Ignore <code>TSTypeQuery</code> when checking for hoisted references (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13367">#13367</a>)</li>
<li><code>[jest-core]</code> Fix <code>detectOpenHandles</code> false positives for some special objects such as <code>TLSWRAP</code> (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13414">#13414</a>)</li>
<li><code>[jest-mock]</code> Fix mocking of getters and setters on classes (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13398">#13398</a>)</li>
<li><code>[jest-reporters]</code> Revert: Transform file paths into hyperlinks (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13399">#13399</a>)</li>
<li><code>[@jest/types]</code> Infer type of <code>each</code> table correctly when the table is a tuple or array (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13381">#13381</a>)</li>
<li><code>[@jest/types]</code> Rework typings to allow the <code>*ReturnedWith</code> matchers to be called with no argument (<a href="https://github-redirect.dependabot.com/facebook/jest/pull/13385">#13385</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/jest/commit/0a8edbe0ac434394a16cc173a03ff54a9cc50e41"><code>0a8edbe</code></a> v29.2.2</li>
<li><a href="https://github.com/facebook/jest/commit/4551c0fdd4d25b7206824957c7bcc6baf61e63bf"><code>4551c0f</code></a> v29.2.1</li>
<li><a href="https://github.com/facebook/jest/commit/ee5b37a4f4433afcfffb0356cea47739d8092287"><code>ee5b37a</code></a> v29.2.0</li>
<li><a href="https://github.com/facebook/jest/commit/22322c9acc3197e43337b5415755823f09f410fe"><code>22322c9</code></a> refactor: use a single root tsconfig for type tests (<a href="https://github.com/facebook/jest/tree/HEAD/packages/jest/issues/13358">#13358</a>)</li>
<li><a href="https://github.com/facebook/jest/commit/3c31dd619e8c022cde53f40fa12ea2a67f4752ce"><code>3c31dd6</code></a> v29.1.2</li>
<li><a href="https://github.com/facebook/jest/commit/fd9cd900ad0904421a3d97661fdc3337194da1f9"><code>fd9cd90</code></a> v29.1.1</li>
<li><a href="https://github.com/facebook/jest/commit/51f10300daf90db003a1749ceaed1084c4f74811"><code>51f1030</code></a> v29.1.0</li>
<li><a href="https://github.com/facebook/jest/commit/77f865da39af5b3e1c114dc347e49257eb3dcfd1"><code>77f865d</code></a> v29.0.3</li>
<li><a href="https://github.com/facebook/jest/commit/616fcf56bb8481d29ba29cc34be32a92b1cf85e5"><code>616fcf5</code></a> v29.0.2</li>
<li><a href="https://github.com/facebook/jest/commit/132e815f95cad24b0ea28cd2f3aecaf8c87b047a"><code>132e815</code></a> chore: update to TypeScript 4.8 (<a href="https://github.com/facebook/jest/tree/HEAD/packages/jest/issues/13177">#13177</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/jest/commits/v29.2.2/packages/jest">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 06:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/352" class=".btn">#352</a>
            </td>
            <td>
                <b>
                    Minor fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jakub Dzikowski <jakub.t.dzikowski@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-28 12:38:10 +0000 UTC
    </div>
</div>

