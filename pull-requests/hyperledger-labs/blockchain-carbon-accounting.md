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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    build(deps): bump nanoid from 3.1.20 to 3.2.0 in /net-emissions-token-network/interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [nanoid](https://github.com/ai/nanoid) from 3.1.20 to 3.2.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ai/nanoid/blob/main/CHANGELOG.md">nanoid's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>This project adheres to <a href="http://semver.org/">Semantic Versioning</a>.</p>
<h2>3.2</h2>
<ul>
<li>Added <code>--size</code> and <code>--alphabet</code> arguments to binary (by Vitaly Baev).</li>
</ul>
<h2>3.1.32</h2>
<ul>
<li>Reduced <code>async</code> exports size (by Artyom Arutyunyan).</li>
<li>Moved from Jest to uvu (by Vitaly Baev).</li>
</ul>
<h2>3.1.31</h2>
<ul>
<li>Fixed collision vulnerability on object in <code>size</code> (by Artyom Arutyunyan).</li>
</ul>
<h2>3.1.30</h2>
<ul>
<li>Reduced size for project with <code>brotli</code> compression (by Anton Khlynovskiy).</li>
</ul>
<h2>3.1.29</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.28</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.27</h2>
<ul>
<li>Cleaned <code>dependencies</code> from development tools.</li>
</ul>
<h2>3.1.26</h2>
<ul>
<li>Improved performance (by Eitan Har-Shoshanim).</li>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.25</h2>
<ul>
<li>Fixed <code>browserify</code> support.</li>
</ul>
<h2>3.1.24</h2>
<ul>
<li>Fixed <code>browserify</code> support (by Artur Paikin).</li>
</ul>
<h2>3.1.23</h2>
<ul>
<li>Fixed <code>esbuild</code> support.</li>
</ul>
<h2>3.1.22</h2>
<ul>
<li>Added <code>default</code> and <code>browser.default</code> to <code>package.exports</code>.</li>
</ul>
<h2>3.1.21</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ai/nanoid/commit/23b136929a6d58f32e31b269534a3ce3f680a086"><code>23b1369</code></a> Release 3.2 version</li>
<li><a href="https://github.com/ai/nanoid/commit/967788efce880960512f969a56f8f22f3fc20bae"><code>967788e</code></a> Remove TS test tools</li>
<li><a href="https://github.com/ai/nanoid/commit/27eaa90cd207a7782bbcf17343092ae87dd62164"><code>27eaa90</code></a> Simplify new binary tool</li>
<li><a href="https://github.com/ai/nanoid/commit/a9d91239931dc77506381874826d297aee71d6ef"><code>a9d9123</code></a> Update dependencies</li>
<li><a href="https://github.com/ai/nanoid/commit/32b9bdaab1fbc28576b17de8516164ce0360f292"><code>32b9bda</code></a> Allows passing size or custom alphabet via cli as args (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/334">#334</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/246d5f87b6b34e23b5e401bdf3da1f80c810ac4c"><code>246d5f8</code></a> Update vite</li>
<li><a href="https://github.com/ai/nanoid/commit/afdf9c92b41427f35476fbe14b5af5d73dd7fbdb"><code>afdf9c9</code></a> doc: Fixed Typo (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/335">#335</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/90a446fef3ecaac78e5af2ea01025c4f40182e2b"><code>90a446f</code></a> Update benchmark results</li>
<li><a href="https://github.com/ai/nanoid/commit/8ba2319b579895cc1f9060b9946a44852f97c509"><code>8ba2319</code></a> bench: add <code>@​napi-rs/uuid</code> v4 (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/333">#333</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/f4257780ece488734a65c176e80c2fd8ab6aab8e"><code>f425778</code></a> Release 3.1.32 version</li>
<li>Additional commits viewable in <a href="https://github.com/ai/nanoid/compare/3.1.20...3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nanoid&package-manager=npm_and_yarn&previous-version=3.1.20&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-22 08:04:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    build(deps): bump nanoid from 3.1.23 to 3.2.0 in /open-offsets-directory/react
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [nanoid](https://github.com/ai/nanoid) from 3.1.23 to 3.2.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ai/nanoid/blob/main/CHANGELOG.md">nanoid's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>This project adheres to <a href="http://semver.org/">Semantic Versioning</a>.</p>
<h2>3.2</h2>
<ul>
<li>Added <code>--size</code> and <code>--alphabet</code> arguments to binary (by Vitaly Baev).</li>
</ul>
<h2>3.1.32</h2>
<ul>
<li>Reduced <code>async</code> exports size (by Artyom Arutyunyan).</li>
<li>Moved from Jest to uvu (by Vitaly Baev).</li>
</ul>
<h2>3.1.31</h2>
<ul>
<li>Fixed collision vulnerability on object in <code>size</code> (by Artyom Arutyunyan).</li>
</ul>
<h2>3.1.30</h2>
<ul>
<li>Reduced size for project with <code>brotli</code> compression (by Anton Khlynovskiy).</li>
</ul>
<h2>3.1.29</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.28</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.27</h2>
<ul>
<li>Cleaned <code>dependencies</code> from development tools.</li>
</ul>
<h2>3.1.26</h2>
<ul>
<li>Improved performance (by Eitan Har-Shoshanim).</li>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.25</h2>
<ul>
<li>Fixed <code>browserify</code> support.</li>
</ul>
<h2>3.1.24</h2>
<ul>
<li>Fixed <code>browserify</code> support (by Artur Paikin).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ai/nanoid/commit/23b136929a6d58f32e31b269534a3ce3f680a086"><code>23b1369</code></a> Release 3.2 version</li>
<li><a href="https://github.com/ai/nanoid/commit/967788efce880960512f969a56f8f22f3fc20bae"><code>967788e</code></a> Remove TS test tools</li>
<li><a href="https://github.com/ai/nanoid/commit/27eaa90cd207a7782bbcf17343092ae87dd62164"><code>27eaa90</code></a> Simplify new binary tool</li>
<li><a href="https://github.com/ai/nanoid/commit/a9d91239931dc77506381874826d297aee71d6ef"><code>a9d9123</code></a> Update dependencies</li>
<li><a href="https://github.com/ai/nanoid/commit/32b9bdaab1fbc28576b17de8516164ce0360f292"><code>32b9bda</code></a> Allows passing size or custom alphabet via cli as args (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/334">#334</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/246d5f87b6b34e23b5e401bdf3da1f80c810ac4c"><code>246d5f8</code></a> Update vite</li>
<li><a href="https://github.com/ai/nanoid/commit/afdf9c92b41427f35476fbe14b5af5d73dd7fbdb"><code>afdf9c9</code></a> doc: Fixed Typo (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/335">#335</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/90a446fef3ecaac78e5af2ea01025c4f40182e2b"><code>90a446f</code></a> Update benchmark results</li>
<li><a href="https://github.com/ai/nanoid/commit/8ba2319b579895cc1f9060b9946a44852f97c509"><code>8ba2319</code></a> bench: add <code>@​napi-rs/uuid</code> v4 (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/333">#333</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/f4257780ece488734a65c176e80c2fd8ab6aab8e"><code>f425778</code></a> Release 3.1.32 version</li>
<li>Additional commits viewable in <a href="https://github.com/ai/nanoid/compare/3.1.23...3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nanoid&package-manager=npm_and_yarn&previous-version=3.1.23&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-22 08:04:35 +0000 UTC
    </div>
</div>

