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
                PR <a href="https://github.com/hyperledger/fabric-test/pull/319" class=".btn">#319</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.1.7 to 1.3.1 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.1.7 to 1.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.3.1</h2>
<ul>
<li>Change a couple of <code>isFunction</code> checks to work in more contexts (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1761">#1761</a> contributed by <a href="https://github.com/zereraz"><code>@​zereraz</code></a>)</li>
<li>Eliminate some log spam in <code>subchannel</code> trace logs (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1770">#1770</a>)</li>
<li>Fix the check for outputting the &quot;read ECONNRESET&quot; error as <code>UNAVAILABLE</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1780">#1780</a>)</li>
<li>Make the <code>GRPC_VERBOSITY</code> environment variable accept lower-case values (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1781">#1781</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.3.0</h2>
<ul>
<li>Add support for <code>ipv4</code> and <code>ipv6</code> address schemes (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1752">#1752</a>)</li>
<li>Remove <code>google-auth-library</code> dependency (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1703">#1703</a>)</li>
<li>Add <code>grpc-node.max_session_memory</code> channel argument to configure maximum memory used per HTTP/2 session (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1666">#1666</a> contributed by dwrip)</li>
<li>Remove runtime Node version compatibility check (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1739">#1739</a>)</li>
<li>Experimental API changes: Add <code>ConfigSelector</code> type and add <code>configSelector</code> argument to <code>ResolverListener#onSuccessfulResolution</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1681">#1681</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js-xds</code> 1.3.0</h2>
<ul>
<li>Add <a href="https://github.com/grpc/proposal/blob/master/A28-xds-traffic-splitting-and-routing.md">xDS Traffic Splitting and Routing</a> feature (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1687">#1687</a>, <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1704">#1704</a>, <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1724">#1724</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.11</h2>
<ul>
<li>Fix a crash when using the library on Electron (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1709">#1709</a>)</li>
<li>Make <code>waitForReady</code> finish immediately if the client has been closed (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1714">#1714</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.10</h2>
<ul>
<li>Fixed an internal bug that caused trailer filters to be called twice for most calls (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1707">#1707</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.9</h2>
<ul>
<li>Speculative fix for ECONNRESET errors (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1705">#1705</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.8</h2>
<ul>
<li>Don't propagate non-numeric errors from auth plugins (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1690">#1690</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.7</h2>
<ul>
<li>Fix an issue holding the Node process open after the channel was closed in some cases (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1688">#1688</a>)</li>
<li>Improve error reporting when a stream fails to start (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1689">#1689</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.6</h2>
<ul>
<li>Loosen the dependency on <code>@types/node</code> to avoid conflicts with other packages' dependencies on the same types package (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1683">#1683</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.5</h2>
<ul>
<li>Fix a bug that caused some errors thrown in client response handling code to be incorrectly reported as response message parsing errors. (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1672">#1672</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.4</h2>
<ul>
<li>In the round robin load balancer, update name resolution when receiving a GOAWAY or similar disconnection (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1665">#1665</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js-xds</code> 1.2.4</h2>
<ul>
<li>Fix a crash when sending stats after reestablishing an LRS stream that has been dropped (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1710">#1710</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.2.3</h2>
<h2><code>@​grpc/grpc-js</code> 1.2.1</h2>
<ul>
<li>Fix handling of propagated and explicitly set deadlines when both are set (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1633">#1633</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/126961a7da23c0fd80496f506573890848292446"><code>126961a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1780">#1780</a> from murgatroid99/grpc-js_econnreset_error_parsing</li>
<li><a href="https://github.com/grpc/grpc-node/commit/21b5ba8d21141bb1910e2518963c0acc473b61ae"><code>21b5ba8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1770">#1770</a> from murgatroid99/grpc-js_connectivity_improvements</li>
<li><a href="https://github.com/grpc/grpc-node/commit/502becb9d2d1830317b04b1e6d406a48063f1b22"><code>502becb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1781">#1781</a> from murgatroid99/grpc-js_verbosity_case_insensitive</li>
<li><a href="https://github.com/grpc/grpc-node/commit/f009cd7b9fdbca41106078e2559669a24794390f"><code>f009cd7</code></a> grpc-js: Look for ECONNRESET errors by code instead of errno</li>
<li><a href="https://github.com/grpc/grpc-node/commit/cc0c8deea39ae3e9d744527104100a7ac39dc578"><code>cc0c8de</code></a> grpc-js: Make GRPC_VERBOSITY accept lower-case values</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9253b7f1043770f6a2fa465d996f4a41668d4e0a"><code>9253b7f</code></a> grpc-js: Don't transition out of idle when discarding subchannels</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d82b1a38033fea93e27fbd5107f47da968caf4c3"><code>d82b1a3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1761">#1761</a> from zereraz/master</li>
<li><a href="https://github.com/grpc/grpc-node/commit/923b44bb1c22bf4c4a7605eebb3f70a8df65ef98"><code>923b44b</code></a> grpc-js: Add type predicate to fix errors for isFunction</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d35fa3ab373783d5d044616ee893701ea309a43d"><code>d35fa3a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1749">#1749</a> from murgatroid99/grpc-js_v1.3.0_bump</li>
<li><a href="https://github.com/grpc/grpc-node/commit/7a8cd5a4bde13cde54b41847607fa6c83a4c906d"><code>7a8cd5a</code></a> grpc-js: Use helper isFunction</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.1.7...@grpc/grpc-js@1.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.1.7&new-version=1.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-12 00:53:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.15 to 4.17.21 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.15 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li><a href="https://github.com/lodash/lodash/commit/ded9bc66583ed0b4e3b7dc906206d40757b4a90a"><code>ded9bc6</code></a> Bump to v4.17.20.</li>
<li><a href="https://github.com/lodash/lodash/commit/63150ef7645ac07961b63a86490f419f356429aa"><code>63150ef</code></a> Documentation fixes.</li>
<li><a href="https://github.com/lodash/lodash/commit/00f0f62a979d2f5fa0287c06eae70cf9a62d8794"><code>00f0f62</code></a> test.js: Remove trailing comma.</li>
<li><a href="https://github.com/lodash/lodash/commit/846e434c7a5b5692c55ebf5715ed677b70a32389"><code>846e434</code></a> Temporarily use a custom fork of <code>lodash-cli</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/5d046f39cbd27f573914768e3b36eeefcc4f1229"><code>5d046f3</code></a> Re-enable Travis tests on <code>4.17</code> branch.</li>
<li><a href="https://github.com/lodash/lodash/commit/aa816b36d402a1ad9385142ce7188f17dae514fd"><code>aa816b3</code></a> Remove <code>/npm-package</code>.</li>
<li><a href="https://github.com/lodash/lodash/commit/d7fbc52ee0466a6d248f047b5d5c3e6d1e099056"><code>d7fbc52</code></a> Bump to v4.17.19</li>
<li>Additional commits viewable in <a href="https://github.com/lodash/lodash/compare/4.17.15...4.17.21">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bnjmnt4n">bnjmnt4n</a>, a new releaser for lodash since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.15&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-11 00:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Bump handlebars from 4.7.6 to 4.7.7 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [handlebars](https://github.com/wycats/handlebars.js) from 4.7.6 to 4.7.7.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/handlebars-lang/handlebars.js/blob/master/release-notes.md">handlebars's changelog</a>.</em></p>
<blockquote>
<h2>v4.7.7 - February 15th, 2021</h2>
<ul>
<li>fix weird error in integration tests - eb860c0</li>
<li>fix: check prototype property access in strict-mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>) - b6d3de7</li>
<li>fix: escape property names in compat mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>) - f058970</li>
<li>refactor: In spec tests, use expectTemplate over equals and shouldThrow (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1683">#1683</a>) - 77825f8</li>
<li>chore: start testing on Node.js 12 and 13 - 3789a30</li>
</ul>
<p>(POSSIBLY) BREAKING CHANGES:</p>
<ul>
<li>the changes from version <a href="https://github.com/handlebars-lang/handlebars.js/blob/master/release-notes.md#v460---january-8th-2020">4.6.0</a> now also apply
in when using the compile-option &quot;strict: true&quot;. Access to prototype properties is forbidden completely by default, specific properties or methods
can be allowed via runtime-options. See <a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1633">#1633</a> for details. If you are using Handlebars as documented, you should not be accessing prototype properties
from your template anyway, so the changes should not be a problem for you. Only the use of undocumented features can break your build.</li>
</ul>
<p>That is why we only bump the patch version despite mentioning breaking changes.</p>
<p><a href="https://github.com/wycats/handlebars.js/compare/v4.7.6...v4.7.7">Commits</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/a9a8e403213583ca90cb7c872d3a22796c37d961"><code>a9a8e40</code></a> v4.7.7</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/e66aed5b99c1b6c93564f37d627e34e5d60eb76e"><code>e66aed5</code></a> Update release notes</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/7d4d170ce46a53084a41920c5c7387c131357989"><code>7d4d170</code></a> disable IE in Saucelabs tests</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/eb860c08998f8f506360d305d89e1f4b40f72a0a"><code>eb860c0</code></a> fix weird error in integration tests</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/b6d3de7123eebba603e321f04afdbae608e8fea8"><code>b6d3de7</code></a> fix: check prototype property access in strict-mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/f0589701698268578199be25285b2ebea1c1e427"><code>f058970</code></a> fix: escape property names in compat mode (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1736">#1736</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/77825f8d3522356feb8e4160fac16344104d192b"><code>77825f8</code></a> refator: In spec tests, use expectTemplate over equals and shouldThrow (<a href="https://github-redirect.dependabot.com/wycats/handlebars.js/issues/1683">#1683</a>)</li>
<li><a href="https://github.com/handlebars-lang/handlebars.js/commit/3789a309554fd600caeae442f40881cf93eb3b54"><code>3789a30</code></a> chore: start testing on Node.js 12 and 13</li>
<li>See full diff in <a href="https://github.com/wycats/handlebars.js/compare/v4.7.6...v4.7.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=handlebars&package-manager=npm_and_yarn&previous-version=4.7.6&new-version=4.7.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-08 17:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Bump underscore from 1.9.2 to 1.13.1 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [underscore](https://github.com/jashkenas/underscore) from 1.9.2 to 1.13.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jashkenas/underscore/commit/943977e34e2279503528a71ddcc2dd5f96483945"><code>943977e</code></a> Merge branch 'umd-alias', tag 1.13.1 release</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5630f882932552ba23f34b57f91c0c6e2a38ad82"><code>5630f88</code></a> Add version 1.13.1 to the change log</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5aa5b526a94edf487ab1d4a4e3cde8f7749e6d2c"><code>5aa5b52</code></a> Update the bundle sizes</li>
<li><a href="https://github.com/jashkenas/underscore/commit/76c8d8a05db2d0f9ecfb193ba2ab7780c4a26441"><code>76c8d8a</code></a> Bump the version to 1.13.1</li>
<li><a href="https://github.com/jashkenas/underscore/commit/9cda0b09742c9ed6ae5e1bccb709b63f32a04f45"><code>9cda0b0</code></a> Add some build clarifications to the documentation (<a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2923">#2923</a>)</li>
<li><a href="https://github.com/jashkenas/underscore/commit/8b5928c04b9a61a99e2704740b80287247e9f47a"><code>8b5928c</code></a> Revert .gitignore underscore.js from 57a4a0e (fix <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2923">#2923</a>)</li>
<li><a href="https://github.com/jashkenas/underscore/commit/7054a54d63af2ed1c99eb3707836da709b5e625e"><code>7054a54</code></a> Update generated sources and tag 1.13.0 release</li>
<li><a href="https://github.com/jashkenas/underscore/commit/37dc52a61054674115be560ab9cbdd26b05031ed"><code>37dc52a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jashkenas/underscore/issues/2921">#2921</a> from jgonggrijp/prepare-1.13.0</li>
<li><a href="https://github.com/jashkenas/underscore/commit/5511d129881253807d728cc6a21fff55953ae4f9"><code>5511d12</code></a> Add version 1.13.0 to the change log</li>
<li><a href="https://github.com/jashkenas/underscore/commit/efe5fbf4a1d43c9a88c1646aa5ab53a4745655b8"><code>efe5fbf</code></a> Bump the version to 1.13.0</li>
<li>Additional commits viewable in <a href="https://github.com/jashkenas/underscore/compare/1.9.2...1.13.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jgonggrijp">jgonggrijp</a>, a new releaser for underscore since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=underscore&package-manager=npm_and_yarn&previous-version=1.9.2&new-version=1.13.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-07 02:25:02 +0000 UTC
    </div>
</div>

