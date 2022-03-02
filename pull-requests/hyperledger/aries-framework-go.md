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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3190" class=".btn">#3190</a>
            </td>
            <td>
                <b>
                    feat: add version id and version time to resolve DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 16:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3189" class=".btn">#3189</a>
            </td>
            <td>
                <b>
                    feat: add BatchCrypto support in EDV
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change includes EDV batch Crypto computation to help support combining all MAC/Encryption/KW operations in one 1 call

Part of #3175

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 16:12:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3188" class=".btn">#3188</a>
            </td>
            <td>
                <b>
                    feat: /kms/import supports importing ecdhkw private keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 00:09:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3187" class=".btn">#3187</a>
            </td>
            <td>
                <b>
                    fix: allow didcomm v1 messages to use didcomm v2 from-did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 15:46:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3186" class=".btn">#3186</a>
            </td>
            <td>
                <b>
                    update test-suite.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                chore(deps): bump actions/setup-node from 2.4.0 to 3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 07:52:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3185" class=".btn">#3185</a>
            </td>
            <td>
                <b>
                    update build.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                chore(deps): bump actions/setup-node from 2.4.0 to 3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 07:51:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3184" class=".btn">#3184</a>
            </td>
            <td>
                <b>
                    Update bbs-interop.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                chore(deps): bump actions/setup-node from 2.4.0 to 3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 07:49:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3183" class=".btn">#3183</a>
            </td>
            <td>
                <b>
                    Size computation for allocation may overflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performing calculations involving the size of potentially large strings or slices can result in an overflow (for signed integer types) or a wraparound (for unsigned types). An overflow causes the result of the calculation to become negative, while a wraparound results in a small (positive) number.

This can cause further issues. If, for example, the result is then used in an allocation, it will cause a runtime panic if it is negative, and allocate an unexpectedly small buffer otherwise.

Recommendation:
Always guard against overflow in arithmetic operations involving potentially large numbers by doing one of the following:

Validate the size of the data from which the numbers are computed.
Define a guard on the arithmetic expression, so that the operation is performed only if the result can be known to be less than, or equal to, the maximum value for the type.
Use a wider type (such as uint64 instead of int), so that larger input values do not cause overflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 07:24:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3182" class=".btn">#3182</a>
            </td>
            <td>
                <b>
                    Update go.sum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GJSON before 1.9.3 allows a ReDoS (regular expression denial of service) attack.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-26 07:44:26 +0000 UTC
    </div>
</div>

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

