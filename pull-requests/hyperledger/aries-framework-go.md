---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3180" class=".btn">#3180</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<p>In scope of this release we changed version of the runtime Node.js for the setup-node action and updated package-lock.json file to  v2.</p>
<h3>Breaking Changes</h3>
<ul>
<li>With the update to Node 16 in <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/414">actions/setup-node#414</a>, all scripts will now be run with Node 16 rather than Node 12.</li>
<li>We removed deprecated <code>version</code> input (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/424">actions/setup-node#424</a>). Please use <code>node-version</code> input instead.</li>
</ul>
<h2>Fix logic of error handling for npm warning and uncaught exception</h2>
<p>In scope of this release we fix logic of error handling related to caching (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/358">actions/setup-node#358</a>) and (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/359">actions/setup-node#359</a>).</p>
<p>In the previous behaviour we relied on <code>stderr</code> output to throw error. The warning messages from package managers can be written to the stderr's output. For now the action will throw an error only if exit code differs from zero. Besides, we add logic to сatch and log unhandled exceptions.</p>
<h2>Adding Node.js version file support</h2>
<p>In scope of this release we add the <code>node-version-file</code> input and update <code>actions/cache</code> dependency to the latest version.</p>
<h2>Adding Node.js version file support</h2>
<p>The new input (<code>node-version-file</code>) provides functionality to specify the path to the file containing Node.js's version with such behaviour:</p>
<ul>
<li>If the file does not exist the action will throw an error.</li>
<li>If you specify both <code>node-version</code> and <code>node-version-file</code> inputs, the action will use value from the <code>node-version</code> input and throw the following warning: <code>Both node-version and node-version-file inputs are specified, only node-version will be used</code>.</li>
<li>For now the action does not support all of the variety of values for Node.js version files. The action can handle values according to the <a href="https://github.com/actions/setup-node#supported-version-syntax">documentation</a> and values with <code>v</code> prefix (<code>v14</code>)</li>
</ul>
<pre lang="yaml"><code>steps:
  - uses: actions/checkout@v2
  - name: Setup node from node version file
    uses: actions/setup-node@v2
    with:
      node-version-file: '.nvmrc'
  - run: npm install
  - run: npm test
</code></pre>
<h2>Update actions/cache dependency to 1.0.8 version.</h2>
<p>We updated actions/cache dependency to the latest version (1.0.8). For more information please refer to the <a href="https://github.com/actions/toolkit/blob/main/packages/cache/RELEASES.md">toolkit/cache</a>.</p>
<h2>Add &quot;cache-hit&quot; output</h2>
<p>This release introduces a new output: <code>cache-hit</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a>).</p>
<p>The <code>cache-hit</code> output contains boolean value indicating that an exact match was found for the key. It shows that the action uses already existing cache or not. The output is available only if cache is enabled.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/9ced9a43a244f3ac94f13bfd896db8c8f30da67a"><code>9ced9a4</code></a> remove version input (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/424">#424</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/3e90744edfed8715c51c59ca546063d5d3035443"><code>3e90744</code></a> Update lockfileVersion (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/422">#422</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/28df918a562341c61f4849bb5b0cae0da42e9ff8"><code>28df918</code></a> Update default runtime to node16 (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/414">#414</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/f099707f6e7a91b89cdebdeca599fc76cc8bf088"><code>f099707</code></a> fix tsc build error for <code>@​actions/http-client</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/402">#402</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/f658dc5bd7deff7ab8a4bfa9ccb65a6540175be2"><code>f658dc5</code></a> ci: use NPM cache in check-dist (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/393">#393</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/5e2e06871487f1c1f2806100f6ad85acf4bce48d"><code>5e2e068</code></a> ci(workflow): add cache to workflows using actions/setup-node (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/287">#287</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/7a0f7a99626ad9d2e3bcc28dce6c379216703cc3"><code>7a0f7a9</code></a> Fix grammar in the README (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/331">#331</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/7b558676dd6f955a469559a6f9db9e0447fe8749"><code>7b55867</code></a> chore: Remove strategy for non-matrix builds (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/186">#186</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/1f8c6b94b26d0feae1e387ca63ccbdc44d27b561"><code>1f8c6b9</code></a> Pass to warning uncaught exceptions (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/359">#359</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/9a74eb4e6473f91fbde564f97c2662fd1dc4875c"><code>9a74eb4</code></a> Throw error only if exit code is note zero.  (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/358">#358</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 08:18:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3179" class=".btn">#3179</a>
            </td>
            <td>
                <b>
                    feat: credential manifest - include style in resolved results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 22:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3178" class=".btn">#3178</a>
            </td>
            <td>
                <b>
                    feat: websocket read limit support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for setting read limit for outbound web socket transport (in addition to inbound that was already supported).

Closes #3155

Signed-off-by: Andrii Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 10:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3177" class=".btn">#3177</a>
            </td>
            <td>
                <b>
                    feat: credential application - validate presentation submission
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                also added support for "image" schema types

Closes #3176

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 03:10:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3174" class=".btn">#3174</a>
            </td>
            <td>
                <b>
                    feat: Added RequestCredential argument for Accept Offer endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Accept Offer endpoint in the REST API can now accept an optional RequestCredential object. This object will get passed to the underlying client instead of just assuming a blank RequestCredential. This is a required feature for the WACI issuance flow.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 19:47:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3172" class=".btn">#3172</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.23.0 to 0.26.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.23.0 to 0.26.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>v0.26.0</h2>
<h3>0.26.0 (February 13, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed The timeoutErrorMessage property in config not work with Node.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3581">#3581</a>)</li>
<li>Added errors to be displayed when the query parsing process itself fails (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3961">#3961</a>)</li>
<li>Fix/remove url required (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4426">#4426</a>)</li>
<li>Update follow-redirects dependency due to Vulnerability (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4462">#4462</a>)</li>
<li>Bump karma from 6.3.11 to 6.3.14 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4461">#4461</a>)</li>
<li>Bump follow-redirects from 1.14.7 to 1.14.8 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4473">#4473</a>)</li>
</ul>
<h2>v0.25.0</h2>
<h3>0.25.0 (January 18, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>Fixing maxBodyLength enforcement (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Don't rely on strict mode behaviour for arguments (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3470">#3470</a>)</li>
<li>Adding error handling when missing url (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3791">#3791</a>)</li>
<li>Update isAbsoluteURL.js removing escaping of non-special characters (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3809">#3809</a>)</li>
<li>Use native Array.isArray() in utils.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3836">#3836</a>)</li>
<li>Adding error handling inside stream end callback (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3967">#3967</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Added aborted even handler (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3916">#3916</a>)</li>
<li>Header types expanded allowing <code>boolean</code> and <code>number</code> types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4144">#4144</a>)</li>
<li>Fix cancel signature allowing cancel message to be <code>undefined</code> (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3153">#3153</a>)</li>
<li>Updated type checks to be formulated better (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3342">#3342</a>)</li>
<li>Avoid unnecessary buffer allocations (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3321">#3321</a>)</li>
<li>Adding a socket handler to keep TCP connection live when processing long living requests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3422">#3422</a>)</li>
<li>Added toFormData helper function (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3757">#3757</a>)</li>
<li>Adding responseEncoding prop type in AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3918">#3918</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Adding axios-test-instance to ecosystem (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Optimize the logic of isAxiosError (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3546">#3546</a>)</li>
<li>Add tests and documentation to display how multiple inceptors work (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3564">#3564</a>)</li>
<li>Updating follow-redirects to version 1.14.7 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4379">#4379</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Fixing changelog to show corrext pull request (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4219">#4219</a>)</li>
<li>Update upgrade guide for https proxy setting (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3604">#3604</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/HEAD/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/rijkvanzanten">Rijk van Zanten</a></li>
<li><a href="https://github.com/koh110">Kohta Ito</a></li>
<li><a href="https://github.com/bfaulk96">Brandon Faulkner</a></li>
<li><a href="https://github.com/NoriSte">Stefano Magni</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h3>0.26.0 (February 13, 2022)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed The timeoutErrorMessage property in config not work with Node.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3581">#3581</a>)</li>
<li>Added errors to be displayed when the query parsing process itself fails (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3961">#3961</a>)</li>
<li>Fix/remove url required (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4426">#4426</a>)</li>
<li>Update follow-redirects dependency due to Vurnerbility (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4462">#4462</a>)</li>
<li>Bump karma from 6.3.11 to 6.3.14 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4461">#4461</a>)</li>
<li>Bump follow-redirects from 1.14.7 to 1.14.8 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4473">#4473</a>)</li>
</ul>
<h3>0.25.0 (January 18, 2022)</h3>
<p>Breaking changes:</p>
<ul>
<li>Fixing maxBodyLength enforcement (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Don't rely on strict mode behaviour for arguments (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3470">#3470</a>)</li>
<li>Adding error handling when missing url (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3791">#3791</a>)</li>
<li>Update isAbsoluteURL.js removing escaping of non-special characters (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3809">#3809</a>)</li>
<li>Use native Array.isArray() in utils.js (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3836">#3836</a>)</li>
<li>Adding error handling inside stream end callback (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3967">#3967</a>)</li>
</ul>
<p>Fixes and Functionality:</p>
<ul>
<li>Added aborted even handler (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3916">#3916</a>)</li>
<li>Header types expanded allowing <code>boolean</code> and <code>number</code> types (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4144">#4144</a>)</li>
<li>Fix cancel signature allowing cancel message to be <code>undefined</code> (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3153">#3153</a>)</li>
<li>Updated type checks to be formulated better (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3342">#3342</a>)</li>
<li>Avoid unnecessary buffer allocations (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3321">#3321</a>)</li>
<li>Adding a socket handler to keep TCP connection live when processing long living requests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3422">#3422</a>)</li>
<li>Added toFormData helper function (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3757">#3757</a>)</li>
<li>Adding responseEncoding prop type in AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3918">#3918</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Adding axios-test-instance to ecosystem (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3786">#3786</a>)</li>
<li>Optimize the logic of isAxiosError (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3546">#3546</a>)</li>
<li>Add tests and documentation to display how multiple inceptors work (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3564">#3564</a>)</li>
<li>Updating follow-redirects to version 1.14.7 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4379">#4379</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Fixing changelog to show corrext pull request (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4219">#4219</a>)</li>
<li>Update upgrade guide for https proxy setting (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3604">#3604</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/rijkvanzanten">Rijk van Zanten</a></li>
<li><a href="https://github.com/koh110">Kohta Ito</a></li>
<li><a href="https://github.com/bfaulk96">Brandon Faulkner</a></li>
<li><a href="https://github.com/NoriSte">Stefano Magni</a></li>
<li><a href="https://github.com/fanguangyi">enofan</a></li>
<li><a href="https://github.com/puzpuzpuz">Andrey Pechkurov</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/c9aca7525703ab600eacd9e95fd7f6ecc9942616"><code>c9aca75</code></a> Releasing v0.26.0</li>
<li><a href="https://github.com/axios/axios/commit/3f842e034ec45c6b48247a48160620dfdf9336e4"><code>3f842e0</code></a> Merge branch 'master' of github.com:axios/axios</li>
<li><a href="https://github.com/axios/axios/commit/2f1e8189f2cf2e97f525975a2a609ca5213b6b7a"><code>2f1e818</code></a> Merge branch 'cookieMr-master'</li>
<li><a href="https://github.com/axios/axios/commit/95295f6f291fc7e647e8d3c2960b5d26a2df707d"><code>95295f6</code></a> Fixed conflict in package lock</li>
<li><a href="https://github.com/axios/axios/commit/b3aa79e13818ab6027b43d9aaae491f1ffcec0fe"><code>b3aa79e</code></a> Bump follow-redirects from 1.14.7 to 1.14.8 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4473">#4473</a>)</li>
<li><a href="https://github.com/axios/axios/commit/d660e29c1a0f4af84e2050f1fcfa52eb9715b363"><code>d660e29</code></a> Revert &quot;Fixed isFormData predicate; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4413">#4413</a>)&quot; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4472">#4472</a>)</li>
<li><a href="https://github.com/axios/axios/commit/447a24dfc337f93d35b9a8bed7629a76f7aed6bf"><code>447a24d</code></a> Bump karma from 6.3.11 to 6.3.14 (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4461">#4461</a>)</li>
<li><a href="https://github.com/axios/axios/commit/c5bdbd436d7ac90d7bac26247cb60752d171e47c"><code>c5bdbd4</code></a> Update follow-redirects dependency due to Vurnerbility</li>
<li><a href="https://github.com/axios/axios/commit/73e3bdb8835ba942096b662e9441f1d85ce4d484"><code>73e3bdb</code></a> Fixed isFormData predicate; (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4413">#4413</a>)</li>
<li><a href="https://github.com/axios/axios/commit/cc86c6c49fdbfd8e2517b191b8833d2f2816ff91"><code>cc86c6c</code></a> Fix/remove url required (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4426">#4426</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.23.0...v0.26.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.23.0&new-version=0.26.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 08:16:24 +0000 UTC
    </div>
</div>

