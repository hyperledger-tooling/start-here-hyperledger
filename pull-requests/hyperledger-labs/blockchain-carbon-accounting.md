---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    feat(data loader): add script to load emissions data and identifiers into OrbitDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a directory that contains a script to load emissions factors and identifiers from different XLSX and CSV files into OrbitDB. This is meant to be a drop-in replacement for the existing `egrid-data-loader.js` script. This is the first step towards migrating all the emissions records from CouchDB to OrbitDB. The following changes have been made:
- Imports data into OrbitDB instead of invoking the chaincode to add an emission factor/identifier
- Uses the IPFS HTTP API, so it can be connected to a public IPFS node that we run remotely
- Upgraded the code to TypeScript (some type definitions and interfaces will be added in later as the refactoring is done)
- Added in progress bars to improve the UX

Here are some instructions on how to test the data loader:
- Install `go-ipfs` on your computer [using these instructions](https://github.com/ipfs/go-ipfs#install-prebuilt-binaries)
- Initialize IPFS's config files by running `ipfs init`
- Start up an IPFS daemon with the following command
`ipfs daemon --enable-pubsub-experiment --writable`
- Ensure that you have Node >= v16 installed on your computer (the project will not work on a lower version of Node)
- Install `yarn` if you haven't already with `npm install -g yarn`
- Install `ts-node` globally with `npm install -g ts-node`
- Install the project's dependencies with
```sh
cd utility-emissions-channel/docker-compose-setup/data
yarn
```
- Download all the data files using the [instructions in the README](https://github.com/hyperledger-labs/blockchain-carbon-accounting/tree/main/utility-emissions-channel#seeding-the-fabric-database)
- For loading the files, simply replace `node egrid-data-loader.js` with `ts-node src/dataLoader.ts`. The other arguments can remain the same.

After loading the data, you may want to view all the inserted data. This can be done by running `ts-node src/getData.ts`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 16:57:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    build(deps): bump node-fetch from 2.6.1 to 2.6.7 in /net-emissions-token-network/interface/packages/subgraph
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.1 to 2.6.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v2.6.7</h2>
<h1>Security patch release</h1>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>fix: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1453">node-fetch/node-fetch#1453</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7</a></p>
<h2>v2.6.6</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(URL): prefer built in URL version when available and fallback to whatwg by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1352">node-fetch/node-fetch#1352</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6">https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6</a></p>
<h2>v2.6.2</h2>
<p>fixed main path in package.json</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f56b0c66d3dd2ef185436de1f2fd40f66bfea8f4"><code>f56b0c6</code></a> fix(URL): prefer built in URL version when available and fallback to whatwg (...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5417aea6a3275932283a200214522e6ab53f1ea"><code>b5417ae</code></a> fix: import whatwg-url in a way compatible with ESM Node (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1303">#1303</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/18193c5922c64046b922e18faf41821290535f06"><code>18193c5</code></a> fix v2.6.3 that did not sending query params (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1301">#1301</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/ace7536c955556be742d9910566738630cc3c2a6"><code>ace7536</code></a> fix: properly encode url with unicode characters (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1291">#1291</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/152214ca2f6e2a5a17d71e4638114625d3be30c6"><code>152214c</code></a> Fix(package.json): Corrected main file path in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1274">#1274</a>)</li>
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.1...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.1&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 23:00:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/395" class=".btn">#395</a>
            </td>
            <td>
                <b>
                    build(deps): bump node-fetch from 2.6.1 to 3.1.1 in /open-offsets-directory/node-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.1 to 3.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v3.1.1</h2>
<h2>Security patch release</h2>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>core: update fetch-blob by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1371">node-fetch/node-fetch#1371</a></li>
<li>docs: Fix typo around sending a file by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1381">node-fetch/node-fetch#1381</a></li>
<li>core: (http.request): Cast URL to string before sending it to NodeJS core by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1378">node-fetch/node-fetch#1378</a></li>
<li>core: handle errors from the request body stream by <a href="https://github.com/mdmitry01"><code>@​mdmitry01</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1392">node-fetch/node-fetch#1392</a></li>
<li>core: Better handle wrong redirect header in a response by <a href="https://github.com/tasinet"><code>@​tasinet</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1387">node-fetch/node-fetch#1387</a></li>
<li>core: Don't use buffer to make a blob by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1402">node-fetch/node-fetch#1402</a></li>
<li>docs: update readme for TS <code>@​types/node-fetch</code> by <a href="https://github.com/adamellsworth"><code>@​adamellsworth</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1405">node-fetch/node-fetch#1405</a></li>
<li>core: Fix logical operator priority to disallow GET/HEAD with non-empty body by <a href="https://github.com/maxshirshin"><code>@​maxshirshin</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1369">node-fetch/node-fetch#1369</a></li>
<li>core: Don't use global buffer by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1422">node-fetch/node-fetch#1422</a></li>
<li>ci: fix main branch by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1429">node-fetch/node-fetch#1429</a></li>
<li>core: use more node: protocol imports by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1428">node-fetch/node-fetch#1428</a></li>
<li>core: Warn when using data by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1421">node-fetch/node-fetch#1421</a></li>
<li>docs: Create SECURITY.md by <a href="https://github.com/JamieSlome"><code>@​JamieSlome</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1445">node-fetch/node-fetch#1445</a></li>
<li>core: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1449">node-fetch/node-fetch#1449</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mdmitry01"><code>@​mdmitry01</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1392">node-fetch/node-fetch#1392</a></li>
<li><a href="https://github.com/tasinet"><code>@​tasinet</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1387">node-fetch/node-fetch#1387</a></li>
<li><a href="https://github.com/adamellsworth"><code>@​adamellsworth</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1405">node-fetch/node-fetch#1405</a></li>
<li><a href="https://github.com/maxshirshin"><code>@​maxshirshin</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1369">node-fetch/node-fetch#1369</a></li>
<li><a href="https://github.com/JamieSlome"><code>@​JamieSlome</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1445">node-fetch/node-fetch#1445</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v3.1.0...v3.1.1">https://github.com/node-fetch/node-fetch/compare/v3.1.0...v3.1.1</a></p>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(Body): Discourage form-data and buffer() by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1212">node-fetch/node-fetch#1212</a></li>
<li>fix: Pass url string to http.request by <a href="https://github.com/serverwentdown"><code>@​serverwentdown</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1268">node-fetch/node-fetch#1268</a></li>
<li>Fix octocat image link by <a href="https://github.com/lakuapik"><code>@​lakuapik</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1281">node-fetch/node-fetch#1281</a></li>
<li>fix(Body.body): Normalize <code>Body.body</code> into a <code>node:stream</code> by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/924">node-fetch/node-fetch#924</a></li>
<li>docs(Headers): Add default Host request header to README.md file by <a href="https://github.com/robertoaceves"><code>@​robertoaceves</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1316">node-fetch/node-fetch#1316</a></li>
<li>Update CHANGELOG.md by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1292">node-fetch/node-fetch#1292</a></li>
<li>Add highWaterMark to cloned properties by <a href="https://github.com/davesidious"><code>@​davesidious</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1162">node-fetch/node-fetch#1162</a></li>
<li>Update README.md to fix HTTPResponseError by <a href="https://github.com/thedanfernandez"><code>@​thedanfernandez</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1135">node-fetch/node-fetch#1135</a></li>
<li>docs: switch <code>url</code> to <code>URL</code> by <a href="https://github.com/dhritzkiv"><code>@​dhritzkiv</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1318">node-fetch/node-fetch#1318</a></li>
<li>fix(types): declare buffer() deprecated by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1345">node-fetch/node-fetch#1345</a></li>
<li>chore: fix lint by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1348">node-fetch/node-fetch#1348</a></li>
<li>refactor: use node: prefix for imports by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1346">node-fetch/node-fetch#1346</a></li>
<li>Bump data-uri-to-buffer from 3.0.1 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1319">node-fetch/node-fetch#1319</a></li>
<li>Bump mocha from 8.4.0 to 9.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1339">node-fetch/node-fetch#1339</a></li>
<li>Referrer and Referrer Policy by <a href="https://github.com/tekwiz"><code>@​tekwiz</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1057">node-fetch/node-fetch#1057</a></li>
<li>Add typing for Response.redirect(url, status) by <a href="https://github.com/c-w"><code>@​c-w</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1169">node-fetch/node-fetch#1169</a></li>
<li>chore: Correct stuff in README.md by <a href="https://github.com/Jiralite"><code>@​Jiralite</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1361">node-fetch/node-fetch#1361</a></li>
<li>docs: Improve clarity of &quot;Loading and configuring&quot; by <a href="https://github.com/serverwentdown"><code>@​serverwentdown</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1323">node-fetch/node-fetch#1323</a></li>
<li>feat(Body): Added support for <code>BodyMixin.formData()</code> and constructing bodies with FormData by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1314">node-fetch/node-fetch#1314</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/blob/main/docs/CHANGELOG.md">node-fetch's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>All notable changes will be recorded here.</p>
<p>The format is based on <a href="https://keepachangelog.com/en/1.0.0/">Keep a Changelog</a>,
and this project adheres to <a href="https://semver.org/spec/v2.0.0.html">Semantic Versioning</a>.</p>
<h2>What's Changed</h2>
<ul>
<li>core: update fetch-blob by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1371">node-fetch/node-fetch#1371</a></li>
<li>docs: Fix typo around sending a file by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1381">node-fetch/node-fetch#1381</a></li>
<li>core: (http.request): Cast URL to string before sending it to NodeJS core by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1378">node-fetch/node-fetch#1378</a></li>
<li>core: handle errors from the request body stream by <a href="https://github.com/mdmitry01"><code>@​mdmitry01</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1392">node-fetch/node-fetch#1392</a></li>
<li>core: Better handle wrong redirect header in a response by <a href="https://github.com/tasinet"><code>@​tasinet</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1387">node-fetch/node-fetch#1387</a></li>
<li>core: Don't use buffer to make a blob by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1402">node-fetch/node-fetch#1402</a></li>
<li>docs: update readme for TS <code>@​types/node-fetch</code> by <a href="https://github.com/adamellsworth"><code>@​adamellsworth</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1405">node-fetch/node-fetch#1405</a></li>
<li>core: Fix logical operator priority to disallow GET/HEAD with non-empty body by <a href="https://github.com/maxshirshin"><code>@​maxshirshin</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1369">node-fetch/node-fetch#1369</a></li>
<li>core: Don't use global buffer by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1422">node-fetch/node-fetch#1422</a></li>
<li>ci: fix main branch by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1429">node-fetch/node-fetch#1429</a></li>
<li>core: use more node: protocol imports by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1428">node-fetch/node-fetch#1428</a></li>
<li>core: Warn when using data by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1421">node-fetch/node-fetch#1421</a></li>
<li>docs: Create SECURITY.md by <a href="https://github.com/JamieSlome"><code>@​JamieSlome</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1445">node-fetch/node-fetch#1445</a></li>
<li>core: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1449">node-fetch/node-fetch#1449</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mdmitry01"><code>@​mdmitry01</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1392">node-fetch/node-fetch#1392</a></li>
<li><a href="https://github.com/tasinet"><code>@​tasinet</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1387">node-fetch/node-fetch#1387</a></li>
<li><a href="https://github.com/adamellsworth"><code>@​adamellsworth</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1405">node-fetch/node-fetch#1405</a></li>
<li><a href="https://github.com/maxshirshin"><code>@​maxshirshin</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1369">node-fetch/node-fetch#1369</a></li>
<li><a href="https://github.com/JamieSlome"><code>@​JamieSlome</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1445">node-fetch/node-fetch#1445</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v3.1.0...v3.1.2">https://github.com/node-fetch/node-fetch/compare/v3.1.0...v3.1.2</a></p>
<h2>3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(Body): Discourage form-data and buffer() by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1212">node-fetch/node-fetch#1212</a></li>
<li>fix: Pass url string to http.request by <a href="https://github.com/serverwentdown"><code>@​serverwentdown</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1268">node-fetch/node-fetch#1268</a></li>
<li>Fix octocat image link by <a href="https://github.com/lakuapik"><code>@​lakuapik</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1281">node-fetch/node-fetch#1281</a></li>
<li>fix(Body.body): Normalize <code>Body.body</code> into a <code>node:stream</code> by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/924">node-fetch/node-fetch#924</a></li>
<li>docs(Headers): Add default Host request header to README.md file by <a href="https://github.com/robertoaceves"><code>@​robertoaceves</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1316">node-fetch/node-fetch#1316</a></li>
<li>Update CHANGELOG.md by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1292">node-fetch/node-fetch#1292</a></li>
<li>Add highWaterMark to cloned properties by <a href="https://github.com/davesidious"><code>@​davesidious</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1162">node-fetch/node-fetch#1162</a></li>
<li>Update README.md to fix HTTPResponseError by <a href="https://github.com/thedanfernandez"><code>@​thedanfernandez</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1135">node-fetch/node-fetch#1135</a></li>
<li>docs: switch <code>url</code> to <code>URL</code> by <a href="https://github.com/dhritzkiv"><code>@​dhritzkiv</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1318">node-fetch/node-fetch#1318</a></li>
<li>fix(types): declare buffer() deprecated by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1345">node-fetch/node-fetch#1345</a></li>
<li>chore: fix lint by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1348">node-fetch/node-fetch#1348</a></li>
<li>refactor: use node: prefix for imports by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1346">node-fetch/node-fetch#1346</a></li>
<li>Bump data-uri-to-buffer from 3.0.1 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1319">node-fetch/node-fetch#1319</a></li>
<li>Bump mocha from 8.4.0 to 9.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1339">node-fetch/node-fetch#1339</a></li>
<li>Referrer and Referrer Policy by <a href="https://github.com/tekwiz"><code>@​tekwiz</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1057">node-fetch/node-fetch#1057</a></li>
<li>Add typing for Response.redirect(url, status) by <a href="https://github.com/c-w"><code>@​c-w</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1169">node-fetch/node-fetch#1169</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/36e47e8a6406185921e4985dcbeff140d73eaa10"><code>36e47e8</code></a> 3.1.1 release (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1451">#1451</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/5304f3f7f7778f1011b622bedcb0e4d3c04dba31"><code>5304f3f</code></a> Don't change relative location header on manual redirect (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1105">#1105</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f5d3cf5e2579cb8f4c76c291871e69696aef8f80"><code>f5d3cf5</code></a> fix(Headers): don't forward secure headers to 3th party (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f2c3d563755d4d357df987fe871607e296463cef"><code>f2c3d56</code></a> Create SECURITY.md (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1445">#1445</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/4ae35388b078bddda238277142bf091898ce6fda"><code>4ae3538</code></a> core: Warn when using data (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1421">#1421</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/41f53b9065a00bc73d24215d42aacdcd284b199c"><code>41f53b9</code></a> fix: use more node: protocol imports (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1428">#1428</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f674875f98c4ef2970a9acf02324f520b1b77967"><code>f674875</code></a> ci: fix main branch (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1429">#1429</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1493d046bc0944886277b0b82dfdf78a7b9f7799"><code>1493d04</code></a> core: Don't use global buffer (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1422">#1422</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/eb33090b81442bc6af9f714a5158160856a1e2f2"><code>eb33090</code></a> Chore: Fix logical operator priority (regression) to disallow GET/HEAD with n...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/7ba5bc9e0aff386ae0e00792d1ea2e2f7a4fd7d6"><code>7ba5bc9</code></a> update readme for TS <code>@​type/node-fetch</code> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1405">#1405</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.1...v3.1.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.1&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-22 21:56:48 +0000 UTC
    </div>
</div>

