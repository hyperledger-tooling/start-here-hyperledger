---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2797" class=".btn">#2797</a>
            </td>
            <td>
                <b>
                    build(deps): bump undici from 5.19.1 to 5.26.2 in /packages/cactus-plugin-ledger-connector-iroha2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                [skip ci]

Bumps [undici](https://github.com/nodejs/undici) from 5.19.1 to 5.26.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.26.2</h2>
<p>Security Release, CVE-2023-45143.</p>
<h2>v5.26.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix publish undici-types once and for all! by <a href="https://github.com/Ethan-Arrowood"><code>@​Ethan-Arrowood</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2338">nodejs/undici#2338</a></li>
<li>Fix node detection omfg by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2341">nodejs/undici#2341</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.26.0...v5.26.1">https://github.com/nodejs/undici/compare/v5.26.0...v5.26.1</a></p>
<h2>v5.26.0</h2>
<h2>What's Changed</h2>
<ul>
<li>use npm install instead of npm ci by <a href="https://github.com/Ethan-Arrowood"><code>@​Ethan-Arrowood</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2309">nodejs/undici#2309</a></li>
<li>change default header to <code>node</code> by <a href="https://github.com/Ethan-Arrowood"><code>@​Ethan-Arrowood</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2310">nodejs/undici#2310</a></li>
<li>chore: change order of the pseudo-headers by <a href="https://github.com/kyrylodolynskyi"><code>@​kyrylodolynskyi</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2308">nodejs/undici#2308</a></li>
<li>fix: Agent.Options.factory should accept URL object or string as parameter by <a href="https://github.com/nicole0707"><code>@​nicole0707</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2295">nodejs/undici#2295</a></li>
<li>build(deps-dev): bump sinon from 15.2.0 to 16.1.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2312">nodejs/undici#2312</a></li>
<li>test: handle npm ignore-scripts settings by <a href="https://github.com/panva"><code>@​panva</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2313">nodejs/undici#2313</a></li>
<li>feat: respect <code>--max-http-header-size</code> Node.js flag by <a href="https://github.com/balazsorban44"><code>@​balazsorban44</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2234">nodejs/undici#2234</a></li>
<li>fix(<a href="https://redirect.github.com/nodejs/undici/issues/2311">#2311</a>): End stream after body sent by <a href="https://github.com/metcoder95"><code>@​metcoder95</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2314">nodejs/undici#2314</a></li>
<li>disallow setting host header in fetch by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2322">nodejs/undici#2322</a></li>
<li>[StepSecurity] ci: Harden GitHub Actions by <a href="https://github.com/step-security-bot"><code>@​step-security-bot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2325">nodejs/undici#2325</a></li>
<li>fix fetch with coverage enabled by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2330">nodejs/undici#2330</a></li>
<li>Fix stuck when using http2 POST Buffer by <a href="https://github.com/binsee"><code>@​binsee</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2336">nodejs/undici#2336</a></li>
<li>fix: 🏷️ add allowH2 to BuildOptions by <a href="https://github.com/binsee"><code>@​binsee</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2334">nodejs/undici#2334</a></li>
<li>fix: 🐛 fix process http2 header by <a href="https://github.com/binsee"><code>@​binsee</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2332">nodejs/undici#2332</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/kyrylodolynskyi"><code>@​kyrylodolynskyi</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2308">nodejs/undici#2308</a></li>
<li><a href="https://github.com/nicole0707"><code>@​nicole0707</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2295">nodejs/undici#2295</a></li>
<li><a href="https://github.com/balazsorban44"><code>@​balazsorban44</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2234">nodejs/undici#2234</a></li>
<li><a href="https://github.com/binsee"><code>@​binsee</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2336">nodejs/undici#2336</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.23.4...v5.26.0">https://github.com/nodejs/undici/compare/v5.23.4...v5.26.0</a></p>
<h2>v5.25.3</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: improve parse-url implementation by <a href="https://github.com/anonrig"><code>@​anonrig</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2286">nodejs/undici#2286</a></li>
<li>test: enable websockets inclusion in WPTReport by <a href="https://github.com/panva"><code>@​panva</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2284">nodejs/undici#2284</a></li>
<li>remove npm run test from pre-commit hook by <a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2296">nodejs/undici#2296</a></li>
<li>perf: use <code>@​fastify/busboy</code> by <a href="https://github.com/gurgunday"><code>@​gurgunday</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2211">nodejs/undici#2211</a></li>
<li>Disable finalizationregistry if node code cov by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2298">nodejs/undici#2298</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/gurgunday"><code>@​gurgunday</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2211">nodejs/undici#2211</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.25.2...v5.25.3">https://github.com/nodejs/undici/compare/v5.25.2...v5.25.3</a></p>
<h2>v5.25.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/12a62187d45f332cf39dd405f7c52b759cf40cdd"><code>12a6218</code></a> Bumped v5.26.2</li>
<li><a href="https://github.com/nodejs/undici/commit/e041de359221ebeae04c469e8aff4145764e6d76"><code>e041de3</code></a> Merge pull request from GHSA-wqq4-5wpv-mx2g</li>
<li><a href="https://github.com/nodejs/undici/commit/c8c80b1115d668664d8cf3acec7535b0258c3079"><code>c8c80b1</code></a> 5.26.1</li>
<li><a href="https://github.com/nodejs/undici/commit/7bcb80c0a22509ceba1b786847faba5aded1bea0"><code>7bcb80c</code></a> Fix node detection omfg (<a href="https://redirect.github.com/nodejs/undici/issues/2341">#2341</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/69ea7b94434e2a3746e6ad1477d122a8d4075c76"><code>69ea7b9</code></a> hopefully this fixes it for good (<a href="https://redirect.github.com/nodejs/undici/issues/2338">#2338</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/4006aaf43ac8b30e16d6d3b89fa2e0df4b7eef33"><code>4006aaf</code></a> Bumped v5.26.0</li>
<li><a href="https://github.com/nodejs/undici/commit/df9795883fb75eb97d27f86ce97a491bf023717c"><code>df97958</code></a> fix: 🐛 fix process http2 header (<a href="https://redirect.github.com/nodejs/undici/issues/2332">#2332</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/b9d83681443405bcc4e77a4c196e559944f1dfa1"><code>b9d8368</code></a> fix: 🏷️ add allowH2 to BuildOptions (<a href="https://redirect.github.com/nodejs/undici/issues/2334">#2334</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/06380f6a10d25df963c06023c3190e3f9160ed8a"><code>06380f6</code></a> Fix stuck when using http2 POST Buffer (<a href="https://redirect.github.com/nodejs/undici/issues/2336">#2336</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/3a9f48171d7486a558ac6f62a7c521d46fdd208b"><code>3a9f481</code></a> fix fetch with coverage enabled (<a href="https://redirect.github.com/nodejs/undici/issues/2330">#2330</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.19.1...v5.26.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.19.1&new-version=5.26.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 16:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2796" class=".btn">#2796</a>
            </td>
            <td>
                <b>
                    build(deps): bump undici from 5.19.1 to 5.26.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                [skip ci]

Bumps [undici](https://github.com/nodejs/undici) from 5.19.1 to 5.26.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.26.2</h2>
<p>Security Release, CVE-2023-45143.</p>
<h2>v5.26.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix publish undici-types once and for all! by <a href="https://github.com/Ethan-Arrowood"><code>@​Ethan-Arrowood</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2338">nodejs/undici#2338</a></li>
<li>Fix node detection omfg by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2341">nodejs/undici#2341</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.26.0...v5.26.1">https://github.com/nodejs/undici/compare/v5.26.0...v5.26.1</a></p>
<h2>v5.26.0</h2>
<h2>What's Changed</h2>
<ul>
<li>use npm install instead of npm ci by <a href="https://github.com/Ethan-Arrowood"><code>@​Ethan-Arrowood</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2309">nodejs/undici#2309</a></li>
<li>change default header to <code>node</code> by <a href="https://github.com/Ethan-Arrowood"><code>@​Ethan-Arrowood</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2310">nodejs/undici#2310</a></li>
<li>chore: change order of the pseudo-headers by <a href="https://github.com/kyrylodolynskyi"><code>@​kyrylodolynskyi</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2308">nodejs/undici#2308</a></li>
<li>fix: Agent.Options.factory should accept URL object or string as parameter by <a href="https://github.com/nicole0707"><code>@​nicole0707</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2295">nodejs/undici#2295</a></li>
<li>build(deps-dev): bump sinon from 15.2.0 to 16.1.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2312">nodejs/undici#2312</a></li>
<li>test: handle npm ignore-scripts settings by <a href="https://github.com/panva"><code>@​panva</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2313">nodejs/undici#2313</a></li>
<li>feat: respect <code>--max-http-header-size</code> Node.js flag by <a href="https://github.com/balazsorban44"><code>@​balazsorban44</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2234">nodejs/undici#2234</a></li>
<li>fix(<a href="https://redirect.github.com/nodejs/undici/issues/2311">#2311</a>): End stream after body sent by <a href="https://github.com/metcoder95"><code>@​metcoder95</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2314">nodejs/undici#2314</a></li>
<li>disallow setting host header in fetch by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2322">nodejs/undici#2322</a></li>
<li>[StepSecurity] ci: Harden GitHub Actions by <a href="https://github.com/step-security-bot"><code>@​step-security-bot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2325">nodejs/undici#2325</a></li>
<li>fix fetch with coverage enabled by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2330">nodejs/undici#2330</a></li>
<li>Fix stuck when using http2 POST Buffer by <a href="https://github.com/binsee"><code>@​binsee</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2336">nodejs/undici#2336</a></li>
<li>fix: 🏷️ add allowH2 to BuildOptions by <a href="https://github.com/binsee"><code>@​binsee</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2334">nodejs/undici#2334</a></li>
<li>fix: 🐛 fix process http2 header by <a href="https://github.com/binsee"><code>@​binsee</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2332">nodejs/undici#2332</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/kyrylodolynskyi"><code>@​kyrylodolynskyi</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2308">nodejs/undici#2308</a></li>
<li><a href="https://github.com/nicole0707"><code>@​nicole0707</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2295">nodejs/undici#2295</a></li>
<li><a href="https://github.com/balazsorban44"><code>@​balazsorban44</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2234">nodejs/undici#2234</a></li>
<li><a href="https://github.com/binsee"><code>@​binsee</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2336">nodejs/undici#2336</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.23.4...v5.26.0">https://github.com/nodejs/undici/compare/v5.23.4...v5.26.0</a></p>
<h2>v5.25.3</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: improve parse-url implementation by <a href="https://github.com/anonrig"><code>@​anonrig</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2286">nodejs/undici#2286</a></li>
<li>test: enable websockets inclusion in WPTReport by <a href="https://github.com/panva"><code>@​panva</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2284">nodejs/undici#2284</a></li>
<li>remove npm run test from pre-commit hook by <a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2296">nodejs/undici#2296</a></li>
<li>perf: use <code>@​fastify/busboy</code> by <a href="https://github.com/gurgunday"><code>@​gurgunday</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2211">nodejs/undici#2211</a></li>
<li>Disable finalizationregistry if node code cov by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2298">nodejs/undici#2298</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/gurgunday"><code>@​gurgunday</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2211">nodejs/undici#2211</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.25.2...v5.25.3">https://github.com/nodejs/undici/compare/v5.25.2...v5.25.3</a></p>
<h2>v5.25.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/12a62187d45f332cf39dd405f7c52b759cf40cdd"><code>12a6218</code></a> Bumped v5.26.2</li>
<li><a href="https://github.com/nodejs/undici/commit/e041de359221ebeae04c469e8aff4145764e6d76"><code>e041de3</code></a> Merge pull request from GHSA-wqq4-5wpv-mx2g</li>
<li><a href="https://github.com/nodejs/undici/commit/c8c80b1115d668664d8cf3acec7535b0258c3079"><code>c8c80b1</code></a> 5.26.1</li>
<li><a href="https://github.com/nodejs/undici/commit/7bcb80c0a22509ceba1b786847faba5aded1bea0"><code>7bcb80c</code></a> Fix node detection omfg (<a href="https://redirect.github.com/nodejs/undici/issues/2341">#2341</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/69ea7b94434e2a3746e6ad1477d122a8d4075c76"><code>69ea7b9</code></a> hopefully this fixes it for good (<a href="https://redirect.github.com/nodejs/undici/issues/2338">#2338</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/4006aaf43ac8b30e16d6d3b89fa2e0df4b7eef33"><code>4006aaf</code></a> Bumped v5.26.0</li>
<li><a href="https://github.com/nodejs/undici/commit/df9795883fb75eb97d27f86ce97a491bf023717c"><code>df97958</code></a> fix: 🐛 fix process http2 header (<a href="https://redirect.github.com/nodejs/undici/issues/2332">#2332</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/b9d83681443405bcc4e77a4c196e559944f1dfa1"><code>b9d8368</code></a> fix: 🏷️ add allowH2 to BuildOptions (<a href="https://redirect.github.com/nodejs/undici/issues/2334">#2334</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/06380f6a10d25df963c06023c3190e3f9160ed8a"><code>06380f6</code></a> Fix stuck when using http2 POST Buffer (<a href="https://redirect.github.com/nodejs/undici/issues/2336">#2336</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/3a9f48171d7486a558ac6f62a7c521d46fdd208b"><code>3a9f481</code></a> fix fetch with coverage enabled (<a href="https://redirect.github.com/nodejs/undici/issues/2330">#2330</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.19.1...v5.26.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.19.1&new-version=5.26.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 16:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2795" class=".btn">#2795</a>
            </td>
            <td>
                <b>
                    docs: fix typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
[skip ci]

Co-authored-by: Peter Somogyvari <peter.somogyvari@accenture.com>

Signed-off-by: GoodDaisy <90915921+GoodDaisy@users.noreply.github.com>
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 12:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2794" class=".btn">#2794</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-cdl-socketio): separate endpoint for subscription key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add separate configurations for endpoints supporting access token and subscription key separately.
- This is required by current public instance of CDL.

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
- [X] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [X] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 11:50:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2793" class=".btn">#2793</a>
            </td>
            <td>
                <b>
                    build(deps): explicit bump of http-cache-semantics to >=4.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Updated the yarn.lock file via yarn up -R and
2. Also added a forced resolution of the versions in the root
package.json for good measure.

[skip ci]

Fixes #2335

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[ x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 19:41:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2792" class=".btn">#2792</a>
            </td>
            <td>
                <b>
                    fix(security): address CVE-2021-3749 - axios >=0.22.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensured that axios is updated to >=0.22.0 in all packages that use it.

The only place where it was not possible to upgrade it through upgrading
transitive dependencies was the ubiquity connector package so for that one
I forced the issue through the resolutions section of the root package.json.

-----------------------------------------------

The GitHub Cacti security advisory: https://github.com/hyperledger/cacti/security/dependabot/361

The general GitHub security advisory: https://github.com/advisories/GHSA-cph5-m8f7-6c5x

Weaknesses
- [WeaknessCWE-400](https://cwe.mitre.org/data/definitions/400.html)
- [WeaknessCWE-1333](https://cwe.mitre.org/data/definitions/1333.html)

CVE ID: `CVE-2021-3749`
GHSA ID: `GHSA-cph5-m8f7-6c5x`

Fixes #2790

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 06:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2789" class=".btn">#2789</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): fix CVE-2023-36665 protobufjs try 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Upgraded fabric-network from 2.2.10 to 2.2.18 wherever it was still 2.2.10
2. Upgraded ipfs-http-client project-wide from 51.0.1 to 60.0.1
3. Upgraded @google-cloud/secret-manager from 3.9.0 to 5.0.1

This is the second try at fixing this issue. For some reason the first
PR didn't get it done. The most likely reason is that other commits
in the meantime added back the vulnerable versions of the packages, but
I'm not a 100% sure.

[skip ci]

Fixes #2682

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 05:18:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2788" class=".btn">#2788</a>
            </td>
            <td>
                <b>
                    fix(security): remediate qs vulnerability CVE-2022-24999
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Mass-upgraded the following dependencies throughout the project to get
rid of the vulnerability in qs' older versions:
1. `express`
2. `body-parser`

GitHub Cacti Security Advisories:
1. https://github.com/hyperledger/cacti/security/dependabot/279
2. https://github.com/hyperledger/cacti/security/dependabot/278
3. https://github.com/hyperledger/cacti/security/dependabot/274

CVE ID: CVE-2022-24999
GHSA ID: GHSA-hrpp-h998-j3pp

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 02:51:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2787" class=".btn">#2787</a>
            </td>
            <td>
                <b>
                    fix(ledger-browser): fix vulnerability CVE-2022-37601
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GitHub Security Advisory link to the vulnerability:
https://github.com/hyperledger/cacti/security/dependabot/260

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**

[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 02:09:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2786" class=".btn">#2786</a>
            </td>
            <td>
                <b>
                    docs(cactus-test-plugin-ledger-connector-besu): add README.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added missing readme file for the test package. It doesn't do much but
it does explain the core concept behind the package and that it is not
something that can/should be used for production deployments.

Fixes #834

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 23:37:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2785" class=".btn">#2785</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-cdl-socketio): support subscription key auth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add alternative auth method using subscriptionKey instead of accessToken.
- Both auth methods are supported but can't be used at the same time.
- Adjust manual test script to work with subscriptionKey.
- Build manual script as part of the main build.
- Update README.
- Remove default `api/v1/` URL prefix for compatibility with https://en-portal.research.global.fujitsu.com/

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 09:59:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2784" class=".btn">#2784</a>
            </td>
            <td>
                <b>
                    docs: add Pull Request Template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Checkbox is updated so it will reflect as expected.

fixes: #91
related to: #2708

Signed-off-by: ruzell22 <ruzell.vince.aquino@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 07:04:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.7.0 to 0.17.0 in /weaver/core/network/fabric-interop-cc/libs/testutils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.7.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.7.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.7.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:38:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2782" class=".btn">#2782</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/sdks/fabric/go-sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/core/network/fabric-interop-cc/libs/assetexchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:36:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2775" class=".btn">#2775</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/core/network/fabric-interop-cc/libs/utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:35:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2774" class=".btn">#2774</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/common/protos-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:35:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2773" class=".btn">#2773</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/samples/fabric/simplestatewithacl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2772" class=".btn">#2772</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/samples/fabric/go-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.7.0 to 0.17.0 in /packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/fixtures/go/asset-transfer-private-data/chaincode-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.7.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.7.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.7.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 21:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2761" class=".btn">#2761</a>
            </td>
            <td>
                <b>
                    docs(README): updated README files to reflect recent documentation upgrades
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated README files to add current info and update links to point to the newly published integrated documentation (https://hyperledger.github.io/cacti/)
- Added a blog entries section to the documentation website.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 21:11:23 +0000 UTC
    </div>
</div>

