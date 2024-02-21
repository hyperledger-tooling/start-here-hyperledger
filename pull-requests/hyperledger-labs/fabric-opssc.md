---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump axios and fabric-network in /common/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) to 1.6.7 and updates ancestor dependency [fabric-network](https://github.com/hyperledger/fabric-sdk-node). These dependencies need to be updated together.

Updates `axios` from 0.21.4 to 1.6.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.7</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li>capture async stack only for rejections with native error objects; (<a href="https://redirect.github.com/axios/axios/issues/6203">#6203</a>) (<a href="https://github.com/axios/axios/commit/1a08f90f402336e4d00e9ee82f211c6adb1640b0">1a08f90</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+30/-26 ([#6203](https://github.com/axios/axios/issues/6203) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/zh-lx" title="+0/-3 ([#6186](https://github.com/axios/axios/issues/6186) )">zhoulixiang</a></li>
</ul>
<h2>Release v1.6.6</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fixed missed dispatchBeforeRedirect argument (<a href="https://redirect.github.com/axios/axios/issues/5778">#5778</a>) (<a href="https://github.com/axios/axios/commit/a1938ff073fcb0f89011f001dfbc1fa1dc995e39">a1938ff</a>)</li>
<li>wrap errors to improve async stack trace (<a href="https://redirect.github.com/axios/axios/issues/5987">#5987</a>) (<a href="https://github.com/axios/axios/commit/123f354b920f154a209ea99f76b7b2ef3d9ebbab">123f354</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/ikonst" title="+91/-8 ([#5987](https://github.com/axios/axios/issues/5987) )">Ilya Priven</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/zaosoula" title="+6/-6 ([#5778](https://github.com/axios/axios/issues/5778) )">Zao Soula</a></li>
</ul>
<h2>Release v1.6.5</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>ci:</strong> refactor notify action as a job of publish action; (<a href="https://redirect.github.com/axios/axios/issues/6176">#6176</a>) (<a href="https://github.com/axios/axios/commit/0736f95ce8776366dc9ca569f49ba505feb6373c">0736f95</a>)</li>
<li><strong>dns:</strong> fixed lookup error handling; (<a href="https://redirect.github.com/axios/axios/issues/6175">#6175</a>) (<a href="https://github.com/axios/axios/commit/f4f2b039dd38eb4829e8583caede4ed6d2dd59be">f4f2b03</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+41/-6 ([#6176](https://github.com/axios/axios/issues/6176) [#6175](https://github.com/axios/axios/issues/6175) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/jasonsaayman" title="+6/-1 ()">Jay</a></li>
</ul>
<h2>Release v1.6.4</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> fixed formToJSON prototype pollution vulnerability; (<a href="https://redirect.github.com/axios/axios/issues/6167">#6167</a>) (<a href="https://github.com/axios/axios/commit/3c0c11cade045c4412c242b5727308cff9897a0e">3c0c11c</a>)</li>
<li><strong>security:</strong> fixed security vulnerability in follow-redirects (<a href="https://redirect.github.com/axios/axios/issues/6163">#6163</a>) (<a href="https://github.com/axios/axios/commit/75af1cdff5b3a6ca3766d3d3afbc3115bb0811b8">75af1cd</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/jasonsaayman" title="+34/-6 ()">Jay</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+34/-3 ([#6172](https://github.com/axios/axios/issues/6172) [#6167](https://github.com/axios/axios/issues/6167) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/gnesher" title="+10/-10 ([#6163](https://github.com/axios/axios/issues/6163) )">Guy Nesher</a></li>
</ul>
<h2>Release v1.6.3</h2>
<h2>Release notes:</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/axios/axios/compare/v1.6.6...v1.6.7">1.6.7</a> (2024-01-25)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>capture async stack only for rejections with native error objects; (<a href="https://redirect.github.com/axios/axios/issues/6203">#6203</a>) (<a href="https://github.com/axios/axios/commit/1a08f90f402336e4d00e9ee82f211c6adb1640b0">1a08f90</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+30/-26 ([#6203](https://github.com/axios/axios/issues/6203) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/zh-lx" title="+0/-3 ([#6186](https://github.com/axios/axios/issues/6186) )">zhoulixiang</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.6.5...v1.6.6">1.6.6</a> (2024-01-24)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fixed missed dispatchBeforeRedirect argument (<a href="https://redirect.github.com/axios/axios/issues/5778">#5778</a>) (<a href="https://github.com/axios/axios/commit/a1938ff073fcb0f89011f001dfbc1fa1dc995e39">a1938ff</a>)</li>
<li>wrap errors to improve async stack trace (<a href="https://redirect.github.com/axios/axios/issues/5987">#5987</a>) (<a href="https://github.com/axios/axios/commit/123f354b920f154a209ea99f76b7b2ef3d9ebbab">123f354</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/ikonst" title="+91/-8 ([#5987](https://github.com/axios/axios/issues/5987) )">Ilya Priven</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/zaosoula" title="+6/-6 ([#5778](https://github.com/axios/axios/issues/5778) )">Zao Soula</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.6.4...v1.6.5">1.6.5</a> (2024-01-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>ci:</strong> refactor notify action as a job of publish action; (<a href="https://redirect.github.com/axios/axios/issues/6176">#6176</a>) (<a href="https://github.com/axios/axios/commit/0736f95ce8776366dc9ca569f49ba505feb6373c">0736f95</a>)</li>
<li><strong>dns:</strong> fixed lookup error handling; (<a href="https://redirect.github.com/axios/axios/issues/6175">#6175</a>) (<a href="https://github.com/axios/axios/commit/f4f2b039dd38eb4829e8583caede4ed6d2dd59be">f4f2b03</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+41/-6 ([#6176](https://github.com/axios/axios/issues/6176) [#6175](https://github.com/axios/axios/issues/6175) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/jasonsaayman" title="+6/-1 ()">Jay</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.6.3...v1.6.4">1.6.4</a> (2024-01-03)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> fixed formToJSON prototype pollution vulnerability; (<a href="https://redirect.github.com/axios/axios/issues/6167">#6167</a>) (<a href="https://github.com/axios/axios/commit/3c0c11cade045c4412c242b5727308cff9897a0e">3c0c11c</a>)</li>
<li><strong>security:</strong> fixed security vulnerability in follow-redirects (<a href="https://redirect.github.com/axios/axios/issues/6163">#6163</a>) (<a href="https://github.com/axios/axios/commit/75af1cdff5b3a6ca3766d3d3afbc3115bb0811b8">75af1cd</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/jasonsaayman" title="+34/-6 ()">Jay</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+34/-3 ([#6172](https://github.com/axios/axios/issues/6172) [#6167](https://github.com/axios/axios/issues/6167) )">Dmitriy Mozgovoy</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/a52e4d9af51205959ef924f87bcf90c605e08a1e"><code>a52e4d9</code></a> chore(release): v1.6.7 (<a href="https://redirect.github.com/axios/axios/issues/6204">#6204</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2b69888dd5601bbc872452ccd24010219fb6e41a"><code>2b69888</code></a> chore: remove unnecessary check (<a href="https://redirect.github.com/axios/axios/issues/6186">#6186</a>)</li>
<li><a href="https://github.com/axios/axios/commit/1a08f90f402336e4d00e9ee82f211c6adb1640b0"><code>1a08f90</code></a> fix: capture async stack only for rejections with native error objects; (<a href="https://redirect.github.com/axios/axios/issues/6203">#6203</a>)</li>
<li><a href="https://github.com/axios/axios/commit/104aa3f65dc30d70273798dff413fb44edd1c9e6"><code>104aa3f</code></a> chore(release): v1.6.6 (<a href="https://redirect.github.com/axios/axios/issues/6199">#6199</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1938ff073fcb0f89011f001dfbc1fa1dc995e39"><code>a1938ff</code></a> fix: fixed missed dispatchBeforeRedirect argument (<a href="https://redirect.github.com/axios/axios/issues/5778">#5778</a>)</li>
<li><a href="https://github.com/axios/axios/commit/123f354b920f154a209ea99f76b7b2ef3d9ebbab"><code>123f354</code></a> fix: wrap errors to improve async stack trace (<a href="https://redirect.github.com/axios/axios/issues/5987">#5987</a>)</li>
<li><a href="https://github.com/axios/axios/commit/6d4c421ee157d93b47f3f9082a7044b1da221461"><code>6d4c421</code></a> chore(release): v1.6.5 (<a href="https://redirect.github.com/axios/axios/issues/6177">#6177</a>)</li>
<li><a href="https://github.com/axios/axios/commit/0736f95ce8776366dc9ca569f49ba505feb6373c"><code>0736f95</code></a> fix(ci): refactor notify action as a job of publish action; (<a href="https://redirect.github.com/axios/axios/issues/6176">#6176</a>)</li>
<li><a href="https://github.com/axios/axios/commit/f4f2b039dd38eb4829e8583caede4ed6d2dd59be"><code>f4f2b03</code></a> fix(dns): fixed lookup error handling; (<a href="https://redirect.github.com/axios/axios/issues/6175">#6175</a>)</li>
<li><a href="https://github.com/axios/axios/commit/1f73dcbbe0bb37f9e9908abb46a3c252536655c8"><code>1f73dcb</code></a> docs: update sponsor links</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.21.4...v1.6.7">compare view</a></li>
</ul>
</details>
<br />

Updates `fabric-network` from 2.2.18 to 2.2.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/fabric-sdk-node/releases">fabric-network's releases</a>.</em></p>
<blockquote>
<h2>v2.2.20</h2>
<h2>What's Changed</h2>
<ul>
<li>Update dependencies to address CVE-2023-45857 by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/689">hyperledger/fabric-sdk-node#689</a></li>
</ul>
<h2>Supported Node versions</h2>
<p>The updated dependency to address CVE-2023-45857 is used only by the CouchDB wallet implementation, and requires Node 14 or later. Therefore Node 10 and 12 are no longer supported by the <strong>fabric-network</strong> package. If you need to continue running on one of these unsupported Node versions, you should continue to use <strong>fabric-network@2.2.19</strong>.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20</a></p>
<h2>v2.2.19</h2>
<h2>What's Changed</h2>
<ul>
<li>Explicitly import <a href="https://www.npmjs.com/package/long">long</a> to address changes to typing in dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/682">hyperledger/fabric-sdk-node#682</a></li>
<li>Use require to import <a href="https://www.npmjs.com/package/long">long</a> to improve compatibility with client application TypeScript configuration by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/683">hyperledger/fabric-sdk-node#683</a></li>
<li>Regenerate fabric-protos using current <a href="https://www.npmjs.com/package/protobufjs">protobufjs</a> to address typing issues introduced by new versions of dependencies by <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a> in <a href="https://redirect.github.com/hyperledger/fabric-sdk-node/pull/684">hyperledger/fabric-sdk-node#684</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19">https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.19</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/ea65b92719f6024168b55cd01631711634752d4b"><code>ea65b92</code></a> Release v2.2.20 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/690">#690</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/cd20a8443882509844a4ed656b8dbe1f076302fb"><code>cd20a84</code></a> Update dependencies to address CVE-2023-45857 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/689">#689</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/53b41aea00f15ef8afd69eedb3264380c8298d22"><code>53b41ae</code></a> Update version following v2.2.19 release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/686">#686</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/7d6752ec4d19c4c06150fadc25e8753e60fa6d61"><code>7d6752e</code></a> Release v2.2.19 (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/685">#685</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/80573efebb1883bd5bec86e268a6c6cd37ea1011"><code>80573ef</code></a> Regenerate fabric-protos using current protobufjs (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/684">#684</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/83729649113304a08cd1e7519613ab0bf7b3897d"><code>8372964</code></a> Use require to import long (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/683">#683</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/8743c2e75151f1ce9249039804f0127ebeb014fd"><code>8743c2e</code></a> Fixes required by changes to typing in dependencies (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/682">#682</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-sdk-node/commit/9bf4de090e02cf0f3a5595ae3b98c6dd45b92808"><code>9bf4de0</code></a> Update versions following release (<a href="https://redirect.github.com/hyperledger/fabric-sdk-node/issues/677">#677</a>)</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.18...v2.2.20">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 10:46:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump axios from 0.21.4 to 0.28.0 in /integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.21.4 to 0.28.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v0.28.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fix(security): fixed CVE-2023-45857 by backporting <code>withXSRFToken</code> option to v0.x (<a href="https://redirect.github.com/axios/axios/issues/6091">#6091</a>)</li>
</ul>
<h3>Backports from v1.x:</h3>
<ul>
<li>Allow null indexes on formSerializer and paramsSerializer v0.x (<a href="https://redirect.github.com/axios/axios/issues/4961">#4961</a>)</li>
<li>Fixing content-type header repeated <a href="https://redirect.github.com/axios/axios/issues/4745">#4745</a></li>
<li>Fixed timeout error message for HTTP 4738</li>
<li>Added <code>axios.formToJSON</code> method (<a href="https://redirect.github.com/axios/axios/issues/4735">#4735</a>)</li>
<li>URL params serializer (<a href="https://redirect.github.com/axios/axios/issues/4734">#4734</a>)</li>
<li>Fixed toFormData Blob issue on node&gt;v17 <a href="https://redirect.github.com/axios/axios/issues/4728">#4728</a></li>
<li>Adding types for progress event callbacks <a href="https://redirect.github.com/axios/axios/issues/4675">#4675</a></li>
<li>Fixed max body length defaults <a href="https://redirect.github.com/axios/axios/issues/4731">#4731</a></li>
<li>Added data URL support for node.js (<a href="https://redirect.github.com/axios/axios/issues/4725">#4725</a>)</li>
<li>Added isCancel type assert (<a href="https://redirect.github.com/axios/axios/issues/4293">#4293</a>)</li>
<li>Added the ability for the <code>url-encoded-form</code> serializer to respect the <code>formSerializer</code> config (<a href="https://redirect.github.com/axios/axios/issues/4721">#4721</a>)</li>
<li>Add <code>string[]</code> to <code>AxiosRequestHeaders</code> type (<a href="https://redirect.github.com/axios/axios/issues/4322">#4322</a>)</li>
<li>Allow type definition for axios instance methods (<a href="https://redirect.github.com/axios/axios/issues/4224">#4224</a>)</li>
<li>Fixed <code>AxiosError</code> stack capturing; (<a href="https://redirect.github.com/axios/axios/issues/4718">#4718</a>)</li>
<li>Fixed <code>AxiosError</code> status code type; (<a href="https://redirect.github.com/axios/axios/issues/4717">#4717</a>)</li>
<li>Adding Canceler parameters config and request (<a href="https://redirect.github.com/axios/axios/issues/4711">#4711</a>)</li>
<li>fix(types): allow to specify partial default headers for instance creation (<a href="https://redirect.github.com/axios/axios/issues/4185">#4185</a>)</li>
<li>Added <code>blob</code> to the list of protocols supported by the browser (<a href="https://redirect.github.com/axios/axios/issues/4678">#4678</a>)</li>
<li>Fixing Z_BUF_ERROR when no content (<a href="https://redirect.github.com/axios/axios/issues/4701">#4701</a>)</li>
<li>Fixed race condition on immediate requests cancellation (<a href="https://redirect.github.com/axios/axios/issues/4261">#4261</a>)</li>
<li>Added a clear() function to the request and response interceptors object so a user can ensure that all interceptors have been removed from an Axios instance <a href="https://redirect.github.com/axios/axios/pull/4248">axios/axios#4248</a></li>
<li>Added generic AxiosAbortSignal TS interface to avoid importing AbortController polyfill (<a href="https://redirect.github.com/axios/axios/issues/4229">#4229</a>)</li>
<li>Fix TS definition for AxiosRequestTransformer (<a href="https://redirect.github.com/axios/axios/issues/4201">#4201</a>)</li>
<li>Use type alias instead of interface for AxiosPromise (<a href="https://redirect.github.com/axios/axios/issues/4505">#4505</a>)</li>
<li>Include request and config when creating a CanceledError instance (<a href="https://redirect.github.com/axios/axios/issues/4659">#4659</a>)</li>
<li>Added generic TS types for the exposed toFormData helper (<a href="https://redirect.github.com/axios/axios/issues/4668">#4668</a>)</li>
<li>Optimized the code that checks cancellation (<a href="https://redirect.github.com/axios/axios/issues/4587">#4587</a>)</li>
<li>Replaced webpack with rollup (<a href="https://redirect.github.com/axios/axios/issues/4596">#4596</a>)</li>
<li>Added stack trace to AxiosError (<a href="https://redirect.github.com/axios/axios/issues/4624">#4624</a>)</li>
<li>Updated AxiosError.config to be optional in the type definition (<a href="https://redirect.github.com/axios/axios/issues/4665">#4665</a>)</li>
<li>Removed incorrect argument for NetworkError constructor (<a href="https://redirect.github.com/axios/axios/issues/4656">#4656</a>)</li>
</ul>
<h2>v0.27.2</h2>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed FormData posting in browser environment by reverting <a href="https://redirect.github.com/axios/axios/issues/3785">#3785</a> (<a href="https://redirect.github.com/axios/axios/pull/4640">#4640</a>)</li>
<li>Enhanced protocol parsing implementation (<a href="https://redirect.github.com/axios/axios/pull/4639">#4639</a>)</li>
<li>Fixed bundle size</li>
</ul>
<h2>v0.27.1</h2>
<h3>Fixes and Functionality:</h3>
<ul>
<li>Removed import of url module in browser build due to huge size overhead and builds being broken (<a href="https://redirect.github.com/axios/axios/pull/4594">#4594</a>)</li>
<li>Bumped follow-redirects to ^1.14.9 (<a href="https://redirect.github.com/axios/axios/pull/4615">#4615</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v0.28.0/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/axios/axios/compare/v0.27.2...v0.28.0">0.28.0</a> (2024-02-12)</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fix(security): fixed CVE-2023-45857 by backporting <code>withXSRFToken</code> option to v0.x (<a href="https://redirect.github.com/axios/axios/issues/6091">#6091</a>)</li>
</ul>
<h3>Backports from v1.x:</h3>
<ul>
<li>Allow null indexes on formSerializer and paramsSerializer v0.x (<a href="https://redirect.github.com/axios/axios/issues/4961">#4961</a>)</li>
<li>Fixing content-type header repeated <a href="https://redirect.github.com/axios/axios/issues/4745">#4745</a></li>
<li>Fixed timeout error message for HTTP 4738</li>
<li>Added <code>axios.formToJSON</code> method (<a href="https://redirect.github.com/axios/axios/issues/4735">#4735</a>)</li>
<li>URL params serializer (<a href="https://redirect.github.com/axios/axios/issues/4734">#4734</a>)</li>
<li>Fixed toFormData Blob issue on node&gt;v17 <a href="https://redirect.github.com/axios/axios/issues/4728">#4728</a></li>
<li>Adding types for progress event callbacks <a href="https://redirect.github.com/axios/axios/issues/4675">#4675</a></li>
<li>Fixed max body length defaults <a href="https://redirect.github.com/axios/axios/issues/4731">#4731</a></li>
<li>Added data URL support for node.js (<a href="https://redirect.github.com/axios/axios/issues/4725">#4725</a>)</li>
<li>Added isCancel type assert (<a href="https://redirect.github.com/axios/axios/issues/4293">#4293</a>)</li>
<li>Added the ability for the <code>url-encoded-form</code> serializer to respect the <code>formSerializer</code> config (<a href="https://redirect.github.com/axios/axios/issues/4721">#4721</a>)</li>
<li>Add <code>string[]</code> to <code>AxiosRequestHeaders</code> type (<a href="https://redirect.github.com/axios/axios/issues/4322">#4322</a>)</li>
<li>Allow type definition for axios instance methods (<a href="https://redirect.github.com/axios/axios/issues/4224">#4224</a>)</li>
<li>Fixed <code>AxiosError</code> stack capturing; (<a href="https://redirect.github.com/axios/axios/issues/4718">#4718</a>)</li>
<li>Fixed <code>AxiosError</code> status code type; (<a href="https://redirect.github.com/axios/axios/issues/4717">#4717</a>)</li>
<li>Adding Canceler parameters config and request (<a href="https://redirect.github.com/axios/axios/issues/4711">#4711</a>)</li>
<li>fix(types): allow to specify partial default headers for instance creation (<a href="https://redirect.github.com/axios/axios/issues/4185">#4185</a>)</li>
<li>Added <code>blob</code> to the list of protocols supported by the browser (<a href="https://redirect.github.com/axios/axios/issues/4678">#4678</a>)</li>
<li>Fixing Z_BUF_ERROR when no content (<a href="https://redirect.github.com/axios/axios/issues/4701">#4701</a>)</li>
<li>Fixed race condition on immediate requests cancellation (<a href="https://redirect.github.com/axios/axios/issues/4261">#4261</a>)</li>
<li>Added a clear() function to the request and response interceptors object so a user can ensure that all interceptors have been removed from an Axios instance <a href="https://redirect.github.com/axios/axios/pull/4248">axios/axios#4248</a></li>
<li>Added generic AxiosAbortSignal TS interface to avoid importing AbortController polyfill (<a href="https://redirect.github.com/axios/axios/issues/4229">#4229</a>)</li>
<li>Fix TS definition for AxiosRequestTransformer (<a href="https://redirect.github.com/axios/axios/issues/4201">#4201</a>)</li>
<li>Use type alias instead of interface for AxiosPromise (<a href="https://redirect.github.com/axios/axios/issues/4505">#4505</a>)</li>
<li>Include request and config when creating a CanceledError instance (<a href="https://redirect.github.com/axios/axios/issues/4659">#4659</a>)</li>
<li>Added generic TS types for the exposed toFormData helper (<a href="https://redirect.github.com/axios/axios/issues/4668">#4668</a>)</li>
<li>Optimized the code that checks cancellation (<a href="https://redirect.github.com/axios/axios/issues/4587">#4587</a>)</li>
<li>Replaced webpack with rollup (<a href="https://redirect.github.com/axios/axios/issues/4596">#4596</a>)</li>
<li>Added stack trace to AxiosError (<a href="https://redirect.github.com/axios/axios/issues/4624">#4624</a>)</li>
<li>Updated AxiosError.config to be optional in the type definition (<a href="https://redirect.github.com/axios/axios/issues/4665">#4665</a>)</li>
<li>Removed incorrect argument for NetworkError constructor (<a href="https://redirect.github.com/axios/axios/issues/4656">#4656</a>)</li>
</ul>
<h2>0.27.2 (April 27, 2022)</h2>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixed FormData posting in browser environment by reverting <a href="https://redirect.github.com/axios/axios/issues/3785">#3785</a> (<a href="https://redirect.github.com/axios/axios/pull/4640">#4640</a>)</li>
<li>Enhanced protocol parsing implementation (<a href="https://redirect.github.com/axios/axios/pull/4639">#4639</a>)</li>
<li>Fixed bundle size</li>
</ul>
<h2>0.27.1 (April 26, 2022)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/3b7635aefc842c05da0ec8c90e8bd09cb54616b8"><code>3b7635a</code></a> [Release] v0.28.0 (<a href="https://redirect.github.com/axios/axios/issues/6211">#6211</a>)</li>
<li><a href="https://github.com/axios/axios/commit/27c007656d8d7ffe780248edc531949d744450b7"><code>27c0076</code></a> feat(backport): added ability for paramsSerializer to handle function; (<a href="https://redirect.github.com/axios/axios/issues/6227">#6227</a>)</li>
<li><a href="https://github.com/axios/axios/commit/80c3d74544197e83ee268b24f9cc1428e04d766c"><code>80c3d74</code></a> chore(ci): backported publish action; (<a href="https://redirect.github.com/axios/axios/issues/6224">#6224</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2755df562b9c194fba6d8b609a383443f6a6e967"><code>2755df5</code></a> fix(security): fixed CVE-2023-45857 by backporting <code>withXSRFToken</code> option to ...</li>
<li><a href="https://github.com/axios/axios/commit/880b42e2b8cdd467ce0c6ecd1cf522ef6ef65682"><code>880b42e</code></a> docs: Fix a typo in README</li>
<li><a href="https://github.com/axios/axios/commit/c4bf0a4afcac9a49e9b58d3ea64570110cba34f8"><code>c4bf0a4</code></a> Allow null indexes on formSerializer and paramsSerializer v0.x (<a href="https://redirect.github.com/axios/axios/issues/4961">#4961</a>)</li>
<li><a href="https://github.com/axios/axios/commit/1e2679f75b2030dd62c661e3292ab265c89497b8"><code>1e2679f</code></a> fix: [Types] Type of header in AxiosRequestConfig / for Axios.create is incor...</li>
<li><a href="https://github.com/axios/axios/commit/80b546c3f1982852aa0047dac5ddde38426e25cb"><code>80b546c</code></a> fix: loosing request header (<a href="https://redirect.github.com/axios/axios/issues/4858">#4858</a>) (<a href="https://redirect.github.com/axios/axios/issues/4871">#4871</a>)</li>
<li><a href="https://github.com/axios/axios/commit/6acb5ef8ff127db65da85189b3ccaeb10b93121a"><code>6acb5ef</code></a> feat: brower platform add data protocol. (<a href="https://redirect.github.com/axios/axios/issues/4814">#4814</a>)</li>
<li><a href="https://github.com/axios/axios/commit/bbb2264614befdce107449baa8a3102d9043a527"><code>bbb2264</code></a> fix(typing): axios response headers can be undefined (<a href="https://redirect.github.com/axios/axios/issues/4813">#4813</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.21.4...v0.28.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.21.4&new-version=0.28.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 10:42:01 +0000 UTC
    </div>
</div>

