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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    bump: weaver/testutils version in all go modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also following changes:
* Update go-gen-checksum script to handle error cases.
* Update go-mod-tidy to be useful to fix broken go.mods.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 17:12:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    build(deps): Bump the npm_and_yarn group across 3 directories with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 1 update in the /common/policy-dsl directory: [tough-cookie](https://github.com/salesforce/tough-cookie).
Bumps the npm_and_yarn group with 1 update in the /samples/fabric/fabric-cli directory: [pkg](https://github.com/vercel/pkg).
Bumps the npm_and_yarn group with 1 update in the /sdks/fabric/interoperation-node-sdk directory: [jsrsasign](https://github.com/kjur/jsrsasign).

Updates `tough-cookie` from 4.0.0 to 4.1.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/salesforce/tough-cookie/releases">tough-cookie's releases</a>.</em></p>
<blockquote>
<h2>v4.1.4</h2>
<p><a href="https://www.npmjs.com/package/tough-cookie/v/4.1.4">https://www.npmjs.com/package/tough-cookie/v/4.1.4</a></p>
<h2>What's Changed</h2>
<ul>
<li>Add local alias for <code>toString</code> by <a href="https://github.com/corvidism"><code>@​corvidism</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/409">salesforce/tough-cookie#409</a></li>
<li>Fix incorrect string validation for URL by <a href="https://github.com/coditva"><code>@​coditva</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/261">salesforce/tough-cookie#261</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/corvidism"><code>@​corvidism</code></a> made their first contribution in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/409">salesforce/tough-cookie#409</a></li>
<li><a href="https://github.com/coditva"><code>@​coditva</code></a> made their first contribution in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/261">salesforce/tough-cookie#261</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.3...v4.1.4">https://github.com/salesforce/tough-cookie/compare/v4.1.3...v4.1.4</a></p>
<h2>4.1.3</h2>
<p>Security fix for Prototype Pollution discovery in <a href="https://redirect.github.com/salesforce/tough-cookie/issues/282">#282</a>. This is a minor release, although output from the <code>inspect</code> utility is affected by this change, we felt this change was important enough to be pushed into the next patch.</p>
<h2>4.1.2 -- Patch and Bugfix Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow set cookies with localhost by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/253">salesforce/tough-cookie#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2">https://github.com/salesforce/tough-cookie/compare/v4.1.1...v4.1.2</a></p>
<h2>4.1.1</h2>
<h2>Patch Release</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: allow special use domains by default by <a href="https://github.com/colincasey"><code>@​colincasey</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/249">salesforce/tough-cookie#249</a></li>
<li>4.1.1 Patch -- allow special use domains by default by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/250">salesforce/tough-cookie#250</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1">https://github.com/salesforce/tough-cookie/compare/v4.1.0...v4.1.1</a></p>
<h2>4.1.0</h2>
<p>v4.1.0</p>
<p>Minor release, focused mainly on resolving reported issues and some minor feature work.</p>
<h2>What's Changed</h2>
<ul>
<li>Create CHANGELOG.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/189">salesforce/tough-cookie#189</a></li>
<li>Missing param validation issue145 by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/193">salesforce/tough-cookie#193</a></li>
<li>Create SECURITY.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/201">salesforce/tough-cookie#201</a></li>
<li>Create CODE_OF_CONDUCT.md by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/200">salesforce/tough-cookie#200</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/195">#195</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/202">salesforce/tough-cookie#202</a></li>
<li>Add explanation and more special-use domains by <a href="https://github.com/ShivanKaul"><code>@​ShivanKaul</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/203">salesforce/tough-cookie#203</a></li>
<li>Sync of constructor options for serialization by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/204">salesforce/tough-cookie#204</a></li>
<li>Returned null in case of empty cookie value by <a href="https://github.com/vsin12"><code>@​vsin12</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/196">salesforce/tough-cookie#196</a></li>
<li>132 str trim not a function by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/209">salesforce/tough-cookie#209</a></li>
<li>Fix for issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/153">#153</a> by <a href="https://github.com/medelibero-sfdc"><code>@​medelibero-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/210">salesforce/tough-cookie#210</a></li>
<li>Fix permuteDomain with trailing dot by <a href="https://github.com/ruoho-sfdc"><code>@​ruoho-sfdc</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/216">salesforce/tough-cookie#216</a></li>
<li>Issue <a href="https://redirect.github.com/salesforce/tough-cookie/issues/213">#213</a> -- added gh-actions flow for building and testing tough-co… by <a href="https://github.com/awaterma"><code>@​awaterma</code></a> in <a href="https://redirect.github.com/salesforce/tough-cookie/pull/218">salesforce/tough-cookie#218</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/salesforce/tough-cookie/commit/cacbc37936bd4824693d885e1e65dca626ed3c8c"><code>cacbc37</code></a> Bump version to 4.1.4</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/a48fb3a6ba2bbce41595a20e1db56543d974057b"><code>a48fb3a</code></a> Add tests for url validation</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/50e69bf9372c13a1e573b77c179a879198a240e3"><code>50e69bf</code></a> Merge pull request <a href="https://redirect.github.com/salesforce/tough-cookie/issues/261">#261</a> from postmanlabs/fix/url-string-validation</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/1253d58825378c2327e3a71e2228b65812d1cf7c"><code>1253d58</code></a> Merge pull request <a href="https://redirect.github.com/salesforce/tough-cookie/issues/409">#409</a> from corvidism/validators-to-string</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/238367e2f1d8a2c72cc25cc80a6eeecb612983d6"><code>238367e</code></a> Add local alias for <code>toString</code></li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/4ff4d29f6cefd279a412b8d62a21142ebd410b36"><code>4ff4d29</code></a> 4.1.3 release preparation, update the package and lib/version to 4.1.3. (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/284">#284</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/12d474791bb856004e858fdb1c47b7608d09cf6e"><code>12d4747</code></a> Prevent prototype pollution in cookie memstore (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/283">#283</a>)</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/f06b72d1d447f33dfa6222c0a3c0c5e063558248"><code>f06b72d</code></a> Fix documentation for store.findCookies, missing allowSpecialUseDomain proper...</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/cf6debd15f16df43030f36719251fcce0ed27dfc"><code>cf6debd</code></a> Fix incorrect string validation for URL</li>
<li><a href="https://github.com/salesforce/tough-cookie/commit/b1a8898ee3f8af52c6c1c355555d9f50ebe626ce"><code>b1a8898</code></a> fix: allow set cookies with localhost (<a href="https://redirect.github.com/salesforce/tough-cookie/issues/253">#253</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/salesforce/tough-cookie/compare/v4.0.0...v4.1.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ccasey">ccasey</a>, a new releaser for tough-cookie since your current version.</p>
</details>
<br />

Updates `pkg` from 4.5.1 to 5.8.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vercel/pkg/releases">pkg's releases</a>.</em></p>
<blockquote>
<h2>5.8.1</h2>
<h3>Patches</h3>
<ul>
<li>Producer: properly call &quot;prebuild-install&quot; if N-API is used: dd9de59c9fca2751bf5d22b57bd9b03d43e85e80</li>
<li>Chore: clean up obsolete eslint disable comments: <a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a></li>
<li>Chore: add prettier check in linting step: <a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a></li>
<li>Chore: separate individual test scripts: <a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a></li>
<li>Chore: use <code>@types/babel__generator</code> package: <a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a></li>
<li>Chore: remove unused entry: <a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a></li>
<li>Chore: upgrade actions runners: <a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a></li>
<li>Style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js: <a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a></li>
<li>Chore: bump prebuild-install@7.1.1: <a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a></li>
<li>Fix: add force flag to codesign to avoid already signed error: <a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a></li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/ignatiusmb"><code>@​ignatiusmb</code></a>, <a href="https://github.com/eltociear"><code>@​eltociear</code></a>, <a href="https://github.com/PraveenAnaparthi"><code>@​PraveenAnaparthi</code></a>, and <a href="https://github.com/brianunlam"><code>@​brianunlam</code></a> for helping!</p>
<h2>5.8.0</h2>
<h2>Highlights</h2>
<ul>
<li>Support more language features, including but not limited to <code>classPrivateMethods</code> (<a href="https://redirect.github.com/vercel/pkg/issues/1248">#1248</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1249">#1249</a>)
<ul>
<li>Note: pkg uses Babel to trace dependencies. It does NOT transform your sources. You should make sure that your code can run on the target Node.js version.</li>
</ul>
</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.2 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1693">vercel/pkg#1693</a>
<ul>
<li>Add Node 14.20.0, 16.16.0 and 18.5.0 binaries</li>
<li><a href="https://nodejs.org/en/blog/vulnerability/july-2022-security-releases">https://nodejs.org/en/blog/vulnerability/july-2022-security-releases</a></li>
</ul>
</li>
<li>detector: use Babel AST and default plugins by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1648">vercel/pkg#1648</a></li>
<li>test: rearrange and fix order by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1650">vercel/pkg#1650</a></li>
<li>fix: typo in fabricator.ts by <a href="https://github.com/eltociear"><code>@​eltociear</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/eltociear"><code>@​eltociear</code></a> made their first contribution in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/vercel/pkg/compare/5.7.0...5.8.0">https://github.com/vercel/pkg/compare/5.7.0...5.8.0</a></p>
<h2>5.7.0</h2>
<h2>Highlights</h2>
<ul>
<li>Node 18 is now supported!</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.1 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1616">vercel/pkg#1616</a>
<ul>
<li>No longer take NODE_OPTIONS from the environment of the end-user. Only the users (developers who use pkg to package their project) should have control over the flags via the &quot;bake in&quot; (--options) mechanism (Fixes: <a href="https://redirect.github.com/vercel/pkg/issues/954">vercel/pkg#954</a>, <a href="https://redirect.github.com/vercel/pkg/issues/989">vercel/pkg#989</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1194">vercel/pkg#1194</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1517">vercel/pkg#1517</a>)</li>
<li>Patched Node: bump to 16.15.0, add 18.1.0 and drop 17</li>
</ul>
</li>
<li>fix broken tests on node 12; latest pnpm requires node &gt;= 14.19 by <a href="https://github.com/kldzj"><code>@​kldzj</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1613">vercel/pkg#1613</a></li>
<li>dependencies: bump (minor) by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1615">vercel/pkg#1615</a></li>
<li>fix(bootstrap): prevent to override existing node addon file by <a href="https://github.com/renkei"><code>@​renkei</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1611">vercel/pkg#1611</a></li>
</ul>
<h2>New Contributors</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vercel/pkg/commit/5dc987b90ffd191263eb0202833dc382cea0d47d"><code>5dc987b</code></a> 5.8.1</li>
<li><a href="https://github.com/vercel/pkg/commit/f19285db72f4592110f49335923d9199da49a137"><code>f19285d</code></a> fix: add force flag to codesign to avoid already signed error (<a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/e3ac4902e9cb023f0ac2a596e21ff9166d2e268c"><code>e3ac490</code></a> chore: bump prebuild-install@7.1.1 (<a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/be1123c474b3653abf3bfb89c068378f66b3849b"><code>be1123c</code></a> style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js (<a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/614c02a06830e0a4a898e6cf4eb35dbbf6110af3"><code>614c02a</code></a> chore: upgrade actions runners (<a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/39e99859fe2fd33fb59c4a75318389b477c1a443"><code>39e9985</code></a> chore: remove unused entry (<a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/b8deba40c0c9dced29e5c15aaefe575285e716d6"><code>b8deba4</code></a> chore: use <code>@types/babel__generator</code> package (<a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/332c7d971a6a8f918f6d24470557f2dcb1de5abf"><code>332c7d9</code></a> chore: separate individual test scripts (<a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/6efa7cfbbac323a019680609c2c78bbf7b9fff0f"><code>6efa7cf</code></a> chore: add prettier check in linting step (<a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/56135b583b901d552e3780e749e79e70e71fd3ea"><code>56135b5</code></a> chore: clean up obsolete eslint disable comments (<a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vercel/pkg/compare/4.5.1...5.8.1">compare view</a></li>
</ul>
</details>
<br />

Updates `jsrsasign` from 10.9.0 to 11.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/releases">jsrsasign's releases</a>.</em></p>
<blockquote>
<h2>restore KJUR.crypto.Cipher class without RSA/RSAOAEP support</h2>
<ul>
<li>Changes from 11.0.0 to 11.1.0 (2024-Feb-01)
<ul>
<li>src/crypto.js
<ul>
<li>restore KJUR.crypto.Cipher class without RSA and RSAOAEP encryption/decryption support</li>
</ul>
</li>
</ul>
</li>
</ul>
<h2>remove RSA and RSAOAEP encryption for Marvin attack</h2>
<ul>
<li>Changes from 10.9.0 to 11.0.0 (2024-Jan-16)
<ul>
<li>remove RSA PKCS#1.5 end OAEP encryption/decryption for Marvin attack (<a href="https://redirect.github.com/kjur/jsrsasign/issues/598">#598</a>)</li>
<li>src/crypto.js
<ul>
<li>remove KJUR.crypto.Cipher class for RSA and RSAOAEP encryption/decryption</li>
</ul>
</li>
<li>ext/{rsa,rsa2}.js
remove encrypt/decrypt/encryptOAEP/decryptOAEP for RSAKey class</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/blob/master/ChangeLog.txt">jsrsasign's changelog</a>.</em></p>
<blockquote>
<p>ChangeLog for jsrsasign</p>
<p>restore KJUR.crypto.Cipher class without RSA/RSAOAEP support</p>
<ul>
<li>Changes from 11.0.0 to 11.1.0 (2024-Feb-01)
<ul>
<li>src/crypto.js
<ul>
<li>restore KJUR.crypto.Cipher class without RSA and RSAOAEP encryption/decryption support</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>remove RSA and RSAOAEP encryption for Marvin attack</p>
<ul>
<li>Changes from 10.9.0 to 11.0.0 (2024-Jan-16)
<ul>
<li>remove RSA PKCS#1.5 end OAEP encryption/decryption for Marvin attack (<a href="https://redirect.github.com/kjur/jsrsasign/issues/598">#598</a>)</li>
<li>src/crypto.js
<ul>
<li>remove KJUR.crypto.Cipher class for RSA and RSAOAEP encryption/decryption</li>
</ul>
</li>
<li>ext/{rsa,rsa2}.js
remove encrypt/decrypt/encryptOAEP/decryptOAEP for RSAKey class</li>
</ul>
</li>
</ul>
<p>enhanced support for encrypted PKCS8</p>
<ul>
<li>Changes from 10.8.6 to 10.9.0 (2023-Nov-27)
<ul>
<li>KEYUTIL.getPEM is updated not to use weak ciphers (<a href="https://redirect.github.com/kjur/jsrsasign/issues/599">#599</a>)
<ul>
<li>default encryptionScheme is changed from des-EDE3-CBC to aes256-CBC</li>
<li>default prf is changed from hmacWithSHA1 to hmacWithSHA256</li>
</ul>
</li>
<li>src/keyutil.js
<ul>
<li>more encrypted PKCS#8 private key support
<ul>
<li>KEYUTIL.getKey now supports encrypted PKCS#8 private key with
aes128-CBC, aes256-CBC encrypted and using hmacWithSHA224/256/384/512 as
psudorandom function.</li>
<li>KEYUTIL.getPEM now supports such as above encrypted PKCS#8 PEM
priavte key.</li>
</ul>
</li>
</ul>
</li>
<li>src/crypto.js
<ul>
<li>Cipher.decrypt/encrypt now supports symmetric ciphers (des-EDE3-CBC,aes128-CBC,aes256-CBC)</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function inttohex and twoscompl are added</li>
</ul>
</li>
<li>src/asn1.js
<ul>
<li>ASN1Util.bigIntToMinTwosComplementsHex is now DEPRECATED. use twoscompl.</li>
</ul>
</li>
<li>src/asn1x509.js
<ul>
<li>aes*-CBC and hmacWithSHA* OIDs are added</li>
</ul>
</li>
<li>test/qunit-do-{base64x,crypto-cipher,keyutil-eprv,keyutil,keyutil-p8egen}.html
<ul>
<li>update and add some test cases for above</li>
</ul>
</li>
<li>stop bower support (bower.json removed)</li>
</ul>
</li>
</ul>
<p>X509.getExtSubjectDirectoryAttributes another bugfix</p>
<ul>
<li>Changes from 10.8.5 to 10.8.6 (2023-Apr-26)
<ul>
<li>src/x509.js
<ul>
<li>another bugfix X509.getExtSubjectDirectoryAttributes method</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>X509.getExtSubjectDirectoryAttributes bugfix</p>
<ul>
<li>Changes from 10.8.4 to 10.8.5 (2023-Apr-26)
<ul>
<li>src/x509.js
<ul>
<li>bugfix X509.getExtSubjectDirectoryAttributes method</li>
</ul>
</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjur/jsrsasign/commit/58bb24192f501927014b67911bbde8ef27532319"><code>58bb241</code></a> 11.1.0 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/726c216efacbaa42461d5c8d2ccdefc303ed1fdd"><code>726c216</code></a> update readme</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/3f1def8b37e782c7c5b33fadd5636e21227ecf1f"><code>3f1def8</code></a> update readme</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/d73befc129a1a344fa7dc3f672a9b813528fb197"><code>d73befc</code></a> 11.0.0 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/32f73aff77ecf4fdbccbd503dee380bc9cfb0473"><code>32f73af</code></a> update jsdoc</li>
<li>See full diff in <a href="https://github.com/kjur/jsrsasign/compare/10.9.0...11.1.0">compare view</a></li>
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
        Created At 2024-05-21 14:03:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    build(deps): Bump the cargo group across 1 directory with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps the cargo group with 3 updates in the /core/relay directory: [h2](https://github.com/hyperium/h2), [mio](https://github.com/tokio-rs/mio) and [rustix](https://github.com/bytecodealliance/rustix).

Updates `h2` from 0.3.17 to 0.3.26
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.26</h2>
<h2>What's Changed</h2>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<p>See <a href="https://seanmonstar.com/blog/hyper-http2-continuation-flood/">https://seanmonstar.com/blog/hyper-http2-continuation-flood/</a> for more info.</p>
<h2>v0.3.25</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: optimize header list size calculations by <a href="https://github.com/Noah-Kennedy"><code>@​Noah-Kennedy</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/750">hyperium/h2#750</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25">https://github.com/hyperium/h2/compare/v0.3.24...v0.3.25</a></p>
<h2>v0.3.24</h2>
<h2>Fixed</h2>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h2>v0.3.23</h2>
<h2>What's Changed</h2>
<ul>
<li>cherry-pick fix: streams awaiting capacity lockout in <a href="https://redirect.github.com/hyperium/h2/pull/734">hyperium/h2#734</a></li>
</ul>
<h2>v0.3.22</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>header_table_size(usize)</code> option to client and server builders.</li>
<li>Improve throughput when vectored IO is not available.</li>
<li>Update indexmap to 2.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/tottoto"><code>@​tottoto</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/714">hyperium/h2#714</a></li>
<li><a href="https://github.com/xiaoyawei"><code>@​xiaoyawei</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/712">hyperium/h2#712</a></li>
<li><a href="https://github.com/Protryon"><code>@​Protryon</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/719">hyperium/h2#719</a></li>
<li><a href="https://github.com/4JX"><code>@​4JX</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/638">hyperium/h2#638</a></li>
<li><a href="https://github.com/vuittont60"><code>@​vuittont60</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/724">hyperium/h2#724</a></li>
</ul>
<h2>v0.3.21</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix opening of new streams over peer's max concurrent limit.</li>
<li>Fix <code>RecvStream</code> to return data even if it has received a <code>CANCEL</code> stream error.</li>
<li>Update MSRV to 1.63.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/DDtKey"><code>@​DDtKey</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/703">hyperium/h2#703</a></li>
<li><a href="https://github.com/jwilm"><code>@​jwilm</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/707">hyperium/h2#707</a></li>
</ul>
<h2>v0.3.20</h2>
<h2>Bug Fixes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/v0.3.26/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.26 (April 3, 2024)</h1>
<ul>
<li>Limit number of CONTINUATION frames for misbehaving connections.</li>
</ul>
<h1>0.3.25 (March 15, 2024)</h1>
<ul>
<li>Improve performance decoding many headers.</li>
</ul>
<h1>0.3.24 (January 17, 2024)</h1>
<ul>
<li>Limit error resets for misbehaving connections.</li>
</ul>
<h1>0.3.23 (January 10, 2024)</h1>
<ul>
<li>Backport fix from 0.4.1 for stream capacity assignment.</li>
</ul>
<h1>0.3.22 (November 15, 2023)</h1>
<ul>
<li>Add <code>header_table_size(usize)</code> option to client and server builders.</li>
<li>Improve throughput when vectored IO is not available.</li>
<li>Update indexmap to 2.</li>
</ul>
<h1>0.3.21 (August 21, 2023)</h1>
<ul>
<li>Fix opening of new streams over peer's max concurrent limit.</li>
<li>Fix <code>RecvStream</code> to return data even if it has received a <code>CANCEL</code> stream error.</li>
<li>Update MSRV to 1.63.</li>
</ul>
<h1>0.3.20 (June 26, 2023)</h1>
<ul>
<li>Fix panic if a server received a request with a <code>:status</code> pseudo header in the 1xx range.</li>
<li>Fix panic if a reset stream had pending push promises that were more than allowed.</li>
<li>Fix potential flow control overflow by subtraction, instead returning a connection error.</li>
</ul>
<h1>0.3.19 (May 12, 2023)</h1>
<ul>
<li>Fix counting reset streams when triggered by a GOAWAY.</li>
<li>Send <code>too_many_resets</code> in opaque debug data of GOAWAY when too many resets received.</li>
</ul>
<h1>0.3.18 (April 17, 2023)</h1>
<ul>
<li>Fix panic because of opposite check in <code>is_remote_local()</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/357127e279c06935830fe2140378312eac801494"><code>357127e</code></a> v0.3.26</li>
<li><a href="https://github.com/hyperium/h2/commit/1a357aaefc7243fdfa9442f45d90be17794a4004"><code>1a357aa</code></a> fix: limit number of CONTINUATION frames allowed</li>
<li><a href="https://github.com/hyperium/h2/commit/5b6c9e0da092728d702dff3607626aafb7809d77"><code>5b6c9e0</code></a> refactor: cleanup new unused warnings (<a href="https://redirect.github.com/hyperium/h2/issues/757">#757</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/3a798327211345b9b2bf797e2e4f3aca4e0ddfee"><code>3a79832</code></a> v0.3.25</li>
<li><a href="https://github.com/hyperium/h2/commit/94e80b1c72bec282bb5d13596803e6fb341fec4c"><code>94e80b1</code></a> perf: optimize header list size calculations (<a href="https://redirect.github.com/hyperium/h2/issues/750">#750</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/7243ab5854b2375213a5a2cdfd543f1d669661e2"><code>7243ab5</code></a> Prepare v0.3.24</li>
<li><a href="https://github.com/hyperium/h2/commit/d919cd6fd8e0f4f5d1f6282fab0b38a1b4bf999c"><code>d919cd6</code></a> streams: limit error resets for misbehaving connections</li>
<li><a href="https://github.com/hyperium/h2/commit/a7eb14a487c0094187314fca63cfe4de4d3d78ef"><code>a7eb14a</code></a> v0.3.23</li>
<li><a href="https://github.com/hyperium/h2/commit/b668c7fbe22e0cb4a76b0a67498cbb4d0aacbc75"><code>b668c7f</code></a> fix: streams awaiting capacity lockout (<a href="https://redirect.github.com/hyperium/h2/issues/730">#730</a>) (<a href="https://redirect.github.com/hyperium/h2/issues/734">#734</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/0f412d8b9c8d309966197873ad1d065adc23c794"><code>0f412d8</code></a> v0.3.22</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/h2/compare/v0.3.17...v0.3.26">compare view</a></li>
</ul>
</details>
<br />

Updates `mio` from 0.8.6 to 0.8.11
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/mio/blob/master/CHANGELOG.md">mio's changelog</a>.</em></p>
<blockquote>
<h1>0.8.11</h1>
<ul>
<li>Fix receiving IOCP events after deregistering a Windows named pipe
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1760">tokio-rs/mio#1760</a>, backport pr:
<a href="https://redirect.github.com/tokio-rs/mio/pull/1761">tokio-rs/mio#1761</a>).</li>
</ul>
<h1>0.8.10</h1>
<h2>Added</h2>
<ul>
<li>Solaris support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1724">tokio-rs/mio#1724</a>).</li>
</ul>
<h1>0.8.9</h1>
<h2>Added</h2>
<ul>
<li>ESP-IDF framework support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1692">tokio-rs/mio#1692</a>).</li>
<li>AIX operating system support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1704">tokio-rs/mio#1704</a>).</li>
<li>Vita support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1721">tokio-rs/mio#1721</a>).</li>
<li><code>{UnixListener,UnixStream}:bind_addr</code>
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1630">tokio-rs/mio#1630</a>).</li>
<li><code>mio_unsupported_force_poll_poll</code> and <code>mio_unsupported_force_waker_pipe</code>
<strong>unsupported</strong> configuration flags to force a specific poll or waker
implementation
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1684">tokio-rs/mio#1684</a>,
<a href="https://redirect.github.com/tokio-rs/mio/pull/1685">tokio-rs/mio#1685</a>,
<a href="https://redirect.github.com/tokio-rs/mio/pull/1692">tokio-rs/mio#1692</a>).</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>The <code>pipe(2)</code> based waker (swapped file descriptors)
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1722">tokio-rs/mio#1722</a>).</li>
<li>The duplicate waker check to work correctly with cloned <code>Registry</code>s.
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1706">tokio-rs/mio#1706</a>).</li>
</ul>
<h1>0.8.8</h1>
<h2>Fixed</h2>
<ul>
<li>Fix compilation on WASI (<a href="https://redirect.github.com/tokio-rs/mio/pull/1676">tokio-rs/mio#1676</a>).</li>
</ul>
<h1>0.8.7</h1>
<h2>Added</h2>
<ul>
<li>Add/fix support for tvOS and watchOS, Mio should now build for tvOS and</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/mio/commit/0328bdef900b6396b8d00d33c825cd8af748553d"><code>0328bde</code></a> Release v0.8.11</li>
<li><a href="https://github.com/tokio-rs/mio/commit/708449851283b57eb6f514c8f289b66e982720b3"><code>7084498</code></a> Fix warnings</li>
<li><a href="https://github.com/tokio-rs/mio/commit/90d4fe00df870acd3d38f3dc4face9aacab8fbb9"><code>90d4fe0</code></a> named-pipes: fix receiving IOCP events after deregister</li>
<li><a href="https://github.com/tokio-rs/mio/commit/c710a307f8627c4d63ac1003252aa45175e08399"><code>c710a30</code></a> Add v0.8.x to the CI</li>
<li><a href="https://github.com/tokio-rs/mio/commit/c29e21c244b2b835e8b3e015b92c708c33c7d70a"><code>c29e21c</code></a> Release v0.8.10</li>
<li><a href="https://github.com/tokio-rs/mio/commit/f6a20da1c81c2d56a78bc6f6832b9904b9215914"><code>f6a20da</code></a> Add Solaris operating system support (<a href="https://redirect.github.com/tokio-rs/mio/issues/1724">#1724</a>)</li>
<li><a href="https://github.com/tokio-rs/mio/commit/e80c3b21b59b92238f4c8c331fcfc4a71508d1c5"><code>e80c3b2</code></a> Release v0.8.9</li>
<li><a href="https://github.com/tokio-rs/mio/commit/862786bbbf719886be55631c0d150d4813a9a1b6"><code>862786b</code></a> Fix importing of IoSourceState</li>
<li><a href="https://github.com/tokio-rs/mio/commit/40348728e4f06f5e150783d8f1559ee974e5e834"><code>4034872</code></a> Add support for vita target</li>
<li><a href="https://github.com/tokio-rs/mio/commit/8eb4010a92bede550850e177d3dd7c4c76eb90ba"><code>8eb4010</code></a> Fix receiver and sender fd in pipe based waker</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/mio/compare/v0.8.6...v0.8.11">compare view</a></li>
</ul>
</details>
<br />

Updates `rustix` from 0.37.4 to 0.37.27
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/bytecodealliance/rustix/releases">rustix's releases</a>.</em></p>
<blockquote>
<h2>0.37.20</h2>
<ul>
<li>Fix decoding of abstract unix sockets (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/661">#661</a>)</li>
<li>Fix the fstat/statat/etc. fallback when statx fails with EPERM. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/666">#666</a>)</li>
<li>Add a <code>rustix::pty</code> module. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/673">#673</a>)</li>
<li>process: Add aliaseses for <code>parent_process_death_signal</code> (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/677">#677</a>)</li>
<li>Fix panic on dropping <code>RecvAncillaryBuffer</code> after failed <code>recvmsg</code> (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/676">#676</a>)</li>
</ul>
<h2>0.37.19</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix no-std builds for MacOS and BSDs by <a href="https://github.com/niluxv"><code>@​niluxv</code></a> in <a href="https://redirect.github.com/bytecodealliance/rustix/pull/647">bytecodealliance/rustix#647</a></li>
<li>Make <code>linkat</code>, <code>unlinkat</code>, and <code>renameat</code> weak on macos. by <a href="https://github.com/sunfishcode"><code>@​sunfishcode</code></a> in <a href="https://redirect.github.com/bytecodealliance/rustix/pull/649">bytecodealliance/rustix#649</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/bytecodealliance/rustix/compare/v0.37.18...v0.37.19">https://github.com/bytecodealliance/rustix/compare/v0.37.18...v0.37.19</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/bytecodealliance/rustix/commit/b38dc512628b5db8d08c26449ee2beed7ed51dcc"><code>b38dc51</code></a> chore: Release rustix version 0.37.27</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/a2d9c8ee1a0c1548f17e5ec6096f3a005111d481"><code>a2d9c8e</code></a> Fix p{read,write}v{,v2}'s encoding of the offset argument on Linux. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/896">#896</a>) (#...</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/dce277762238d5fd40c57ccf0151645d8de3d33d"><code>dce2777</code></a> chore: Release rustix version 0.37.26</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/06dbe83c60cbfa603c9437aef9dfd119f068b1df"><code>06dbe83</code></a> Fix <code>sendmsg_unix</code>'s address encoding. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/885">#885</a>) (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/886">#886</a>)</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/00b84d6aac2364455eab2c68e42afee63d6e3ad3"><code>00b84d6</code></a> chore: Release rustix version 0.37.25</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/cad15a7076d493a0651fb0b7889bd5e5a72a8f17"><code>cad15a7</code></a> Fixes for <code>Dir</code> on macOS, FreeBSD, and WASI.</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/df3c3a192cf144af0da8a57417fb4addbdc611f6"><code>df3c3a1</code></a> Merge pull request from GHSA-c827-hfw6-qwvm</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/b78aeff1a271863ecc75ccca37f014d33b9f6705"><code>b78aeff</code></a> chore: Release rustix version 0.37.24</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/c0c3f01d7c8296ebadb23ad0b4f82a9a082252ae"><code>c0c3f01</code></a> Add GNU/Hurd support (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/852">#852</a>)</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/f416b6b27b8d0540e8be14f8d30153ea3e3d7476"><code>f416b6b</code></a> Fix the <code>test_ttyname_ok</code> test when /dev/stdin is inaccessable. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/821">#821</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/bytecodealliance/rustix/compare/v0.37.4...v0.37.27">compare view</a></li>
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
        Created At 2024-05-21 13:01:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/463" class=".btn">#463</a>
            </td>
            <td>
                <b>
                    build(deps): Bump webpki from 0.22.0 to 0.22.4 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [webpki](https://github.com/briansmith/webpki) from 0.22.0 to 0.22.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/briansmith/webpki/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpki&package-manager=cargo&previous-version=0.22.0&new-version=0.22.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 12:55:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    build(deps): Bump webpki from 0.22.0 to 0.22.4 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [webpki](https://github.com/briansmith/webpki) from 0.22.0 to 0.22.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/briansmith/webpki/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpki&package-manager=cargo&previous-version=0.22.0&new-version=0.22.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 12:52:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    build(deps): Bump rustix from 0.37.7 to 0.37.27 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rustix](https://github.com/bytecodealliance/rustix) from 0.37.7 to 0.37.27.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/bytecodealliance/rustix/releases">rustix's releases</a>.</em></p>
<blockquote>
<h2>0.37.20</h2>
<ul>
<li>Fix decoding of abstract unix sockets (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/661">#661</a>)</li>
<li>Fix the fstat/statat/etc. fallback when statx fails with EPERM. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/666">#666</a>)</li>
<li>Add a <code>rustix::pty</code> module. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/673">#673</a>)</li>
<li>process: Add aliaseses for <code>parent_process_death_signal</code> (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/677">#677</a>)</li>
<li>Fix panic on dropping <code>RecvAncillaryBuffer</code> after failed <code>recvmsg</code> (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/676">#676</a>)</li>
</ul>
<h2>0.37.19</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix no-std builds for MacOS and BSDs by <a href="https://github.com/niluxv"><code>@​niluxv</code></a> in <a href="https://redirect.github.com/bytecodealliance/rustix/pull/647">bytecodealliance/rustix#647</a></li>
<li>Make <code>linkat</code>, <code>unlinkat</code>, and <code>renameat</code> weak on macos. by <a href="https://github.com/sunfishcode"><code>@​sunfishcode</code></a> in <a href="https://redirect.github.com/bytecodealliance/rustix/pull/649">bytecodealliance/rustix#649</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/bytecodealliance/rustix/compare/v0.37.18...v0.37.19">https://github.com/bytecodealliance/rustix/compare/v0.37.18...v0.37.19</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/bytecodealliance/rustix/commit/b38dc512628b5db8d08c26449ee2beed7ed51dcc"><code>b38dc51</code></a> chore: Release rustix version 0.37.27</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/a2d9c8ee1a0c1548f17e5ec6096f3a005111d481"><code>a2d9c8e</code></a> Fix p{read,write}v{,v2}'s encoding of the offset argument on Linux. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/896">#896</a>) (#...</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/dce277762238d5fd40c57ccf0151645d8de3d33d"><code>dce2777</code></a> chore: Release rustix version 0.37.26</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/06dbe83c60cbfa603c9437aef9dfd119f068b1df"><code>06dbe83</code></a> Fix <code>sendmsg_unix</code>'s address encoding. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/885">#885</a>) (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/886">#886</a>)</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/00b84d6aac2364455eab2c68e42afee63d6e3ad3"><code>00b84d6</code></a> chore: Release rustix version 0.37.25</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/cad15a7076d493a0651fb0b7889bd5e5a72a8f17"><code>cad15a7</code></a> Fixes for <code>Dir</code> on macOS, FreeBSD, and WASI.</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/df3c3a192cf144af0da8a57417fb4addbdc611f6"><code>df3c3a1</code></a> Merge pull request from GHSA-c827-hfw6-qwvm</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/b78aeff1a271863ecc75ccca37f014d33b9f6705"><code>b78aeff</code></a> chore: Release rustix version 0.37.24</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/c0c3f01d7c8296ebadb23ad0b4f82a9a082252ae"><code>c0c3f01</code></a> Add GNU/Hurd support (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/852">#852</a>)</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/f416b6b27b8d0540e8be14f8d30153ea3e3d7476"><code>f416b6b</code></a> Fix the <code>test_ttyname_ok</code> test when /dev/stdin is inaccessable. (<a href="https://redirect.github.com/bytecodealliance/rustix/issues/821">#821</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/bytecodealliance/rustix/compare/v0.37.7...v0.37.27">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rustix&package-manager=cargo&previous-version=0.37.7&new-version=0.37.27)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 12:33:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/460" class=".btn">#460</a>
            </td>
            <td>
                <b>
                    build(deps): Bump openssl from 0.10.55 to 0.10.64 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.55 to 0.10.64.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.64</h2>
<h2>What's Changed</h2>
<ul>
<li>Make _STACK opaque for LibreSSL &gt;= 3.9.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2153">sfackler/rust-openssl#2153</a></li>
<li>enable x509 verify and groups list for boringssl by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2155">sfackler/rust-openssl#2155</a></li>
<li>Cleanup some not-required Path::new invocations by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2158">sfackler/rust-openssl#2158</a></li>
<li>fixed a clippy (nightly) warning by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2161">sfackler/rust-openssl#2161</a></li>
<li>Bump actions versions by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2162">sfackler/rust-openssl#2162</a></li>
<li>Add support for setting the nonce type and digest on a PKEY_CTX by <a href="https://github.com/facutuesca"><code>@​facutuesca</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2144">sfackler/rust-openssl#2144</a></li>
<li>rebuild openssl-sys if the underlying openssl has changed by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2157">sfackler/rust-openssl#2157</a></li>
<li>Added binding for EVP_default_properties_enable_fips by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2168">sfackler/rust-openssl#2168</a></li>
<li>LibreSSL 3.9: fix CRYPTO_malloc/free signatures by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2170">sfackler/rust-openssl#2170</a></li>
<li>Expose alias on X509 structs by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2167">sfackler/rust-openssl#2167</a></li>
<li>bump openssl and openssl-sys + changelogs by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2175">sfackler/rust-openssl#2175</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.63...openssl-v0.10.64">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.63...openssl-v0.10.64</a></p>
<h2>openssl-v0.10.63</h2>
<h2>What's Changed</h2>
<ul>
<li>Allow passing a passphrase callback when loading a public key by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2135">sfackler/rust-openssl#2135</a></li>
<li>Expose several additional ciphers for symmetry with symm by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2140">sfackler/rust-openssl#2140</a></li>
<li>brew: add openssl@3.0 (for 3.0.x LTS releases) by <a href="https://github.com/chenrui333"><code>@​chenrui333</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2141">sfackler/rust-openssl#2141</a></li>
<li>Add PKey::from_dhx by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2142">sfackler/rust-openssl#2142</a></li>
<li>Make X509_PURPOSE opaque for LibreSSL &gt;= 3.9.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2145">sfackler/rust-openssl#2145</a></li>
<li>PEM parsing: check last error instead of first by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2148">sfackler/rust-openssl#2148</a></li>
<li>Expose brainpool NIDs on libressl by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2150">sfackler/rust-openssl#2150</a></li>
<li>Add two methods to the PKCS7 API by <a href="https://github.com/facutuesca"><code>@​facutuesca</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2111">sfackler/rust-openssl#2111</a></li>
<li>add more boringssl methods by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2138">sfackler/rust-openssl#2138</a></li>
<li>Release openssl v0.10.63 and openssl-sys v0.9.99 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2152">sfackler/rust-openssl#2152</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.62...openssl-v0.10.63">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.62...openssl-v0.10.63</a></p>
<h2>openssl-v0.10.62</h2>
<h2>What's Changed</h2>
<ul>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2119">#2119</a> -- use ErrorStack abstraction in X.509 error handling by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2120">sfackler/rust-openssl#2120</a></li>
<li>Fix building with latest BoringSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2121">sfackler/rust-openssl#2121</a></li>
<li>Fix tests on macOS by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2123">sfackler/rust-openssl#2123</a></li>
<li>Upcoming API changes in LibreSSL 3.9 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2124">sfackler/rust-openssl#2124</a></li>
<li>Add <code>rand_priv_bytes</code> by <a href="https://github.com/overvenus"><code>@​overvenus</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2126">sfackler/rust-openssl#2126</a></li>
<li>Add nid constant for curve brainpoolP320r1 by <a href="https://github.com/nicklaswj"><code>@​nicklaswj</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2129">sfackler/rust-openssl#2129</a></li>
<li>Release openssl v0.10.62 and openssl-sys v0.9.98 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2133">sfackler/rust-openssl#2133</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/overvenus"><code>@​overvenus</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2126">sfackler/rust-openssl#2126</a></li>
<li><a href="https://github.com/nicklaswj"><code>@​nicklaswj</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2129">sfackler/rust-openssl#2129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.62">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.62</a></p>
<h2>openssl v0.10.61</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4a19cd48259e0755d9a9067f4c1a51ee63844c66"><code>4a19cd4</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2175">#2175</a> from reaperhulk/changelog</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4e0e05a6293043cf7b9392c0e286c8397ce75996"><code>4e0e05a</code></a> bump openssl and openssl-sys + changelogs</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/c2b124aa2c36b5fc792239391e614df7f6f1fb24"><code>c2b124a</code></a> Be explicit that aliases are not part of X.509 certificates</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/1abf4a5b792228f6e9d8676015623d6315def4c1"><code>1abf4a5</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2167">#2167</a> from alex/expose-alias</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a644ec2542473c854a02b7fe642621e813517979"><code>a644ec2</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2170">#2170</a> from botovq/crypto-free</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/83940d14e30ed4e7c885dd44e3002c1955d5d5ed"><code>83940d1</code></a> LibreSSL 3.9: fix CRYPTO_malloc/free signatures</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/51fc5694821d66983d8639d3b0b4a58024f92a1f"><code>51fc569</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2168">#2168</a> from sfackler/alex-patch-1</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/3c53dee153d4ab801cde3e10d914a16789464a6b"><code>3c53dee</code></a> Added binding for EVP_default_properties_enable_fips</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a12abe1b92c526f6995632ba43f6bfc433b5997d"><code>a12abe1</code></a> Expose alias on X509 structs</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/3acf2eff0baf7db1a5722c14def50cf5b068538e"><code>3acf2ef</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2157">#2157</a> from reaperhulk/rebuild-if-changed</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.55...openssl-v0.10.64">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.55&new-version=0.10.64)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 12:33:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump @babel/traverse from 7.17.9 to 7.24.5 in /common/policy-dsl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@babel/traverse](https://github.com/babel/babel/tree/HEAD/packages/babel-traverse) from 7.17.9 to 7.24.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/traverse</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<p>Thanks <a href="https://github.com/romgrk"><code>@​romgrk</code></a> and <a href="https://github.com/sossost"><code>@​sossost</code></a> for your first PRs!</p>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 6</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>Rom Grk (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
<li>ynnsuis (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<p>Thanks <a href="https://github.com/Dunqing"><code>@​Dunqing</code></a>, <a href="https://github.com/luiscubal"><code>@​luiscubal</code></a>, and <a href="https://github.com/samualtnorman"><code>@​samualtnorman</code></a> for your first PRs!</p>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/traverse</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16402">#16402</a> fix: Correctly prints <code>{ [key in Bar]? }</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16394">#16394</a> fix: Correctly generate <code>TSMappedType</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16390">#16390</a> Create bugfix plugin for classes in computed keys in Firefox (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16387">#16387</a> fix: support mutated outer decorated class binding (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16385">#16385</a> fix: Decorators when <code>super()</code> exists and <code>protoInit</code> is not needed (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-block-scoping</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16384">#16384</a> fix: Transform scoping for <code>for X</code> in loop (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16368">#16368</a> fix: Capture <code>let</code> when the <code>for</code> body is not a block (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-core</code>, <code>babel-plugin-transform-block-scoped-functions</code>, <code>babel-plugin-transform-block-scoping</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/ddbea7d4e6314f799eb371cc10e16f96ac2c96b2"><code>ddbea7d</code></a> v7.24.5</li>
<li><a href="https://github.com/babel/babel/commit/e779cad081d47bd6a91302e274dbb93f08bd1d51"><code>e779cad</code></a> fix: TypeScript annotation affects output (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16377">#16377</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ee4875443db7563b87ef8e11e1fb75582ac72ac1"><code>ee48754</code></a> Use multiple TypeScript projects (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16430">#16430</a>)</li>
<li><a href="https://github.com/babel/babel/commit/4d8b2d0fd79630aec51e2c35daca46cdb2ddd4c3"><code>4d8b2d0</code></a> Make <code>NodePath\&lt;T | U&gt;</code> distributive (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16439">#16439</a>)</li>
<li><a href="https://github.com/babel/babel/commit/a84ec282c0bea68bb184e091742ed9d996a0342f"><code>a84ec28</code></a> Enable <code>eqeqeq</code> rule (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16404">#16404</a>)</li>
<li><a href="https://github.com/babel/babel/commit/822b025fc9d43263e69aed8a9fc80e8c6b8ebf6d"><code>822b025</code></a> v7.24.1</li>
<li><a href="https://github.com/babel/babel/commit/fc0d5ad56e948f2b3d1704adb6367bbde0f25e59"><code>fc0d5ad</code></a> Update typescript and lint tools (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16351">#16351</a>)</li>
<li><a href="https://github.com/babel/babel/commit/69e792887ea7e5d1cd7375ef7f6f3254ff4f2695"><code>69e7928</code></a> Consider well-known and registered symbols as literals (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16342">#16342</a>)</li>
<li><a href="https://github.com/babel/babel/commit/40110e9d707e2b2b81f6e2b99820722a7014132a"><code>40110e9</code></a> Update source map deps (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16327">#16327</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ce59160e34e21e8f1ac2fc55ae037f7b043e8d20"><code>ce59160</code></a> v7.24.0</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.24.5/packages/babel-traverse">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/traverse&package-manager=npm_and_yarn&previous-version=7.17.9&new-version=7.24.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    build(deps): Bump mio from 0.8.6 to 0.8.11 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [mio](https://github.com/tokio-rs/mio) from 0.8.6 to 0.8.11.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/mio/blob/master/CHANGELOG.md">mio's changelog</a>.</em></p>
<blockquote>
<h1>0.8.11</h1>
<ul>
<li>Fix receiving IOCP events after deregistering a Windows named pipe
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1760">tokio-rs/mio#1760</a>, backport pr:
<a href="https://redirect.github.com/tokio-rs/mio/pull/1761">tokio-rs/mio#1761</a>).</li>
</ul>
<h1>0.8.10</h1>
<h2>Added</h2>
<ul>
<li>Solaris support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1724">tokio-rs/mio#1724</a>).</li>
</ul>
<h1>0.8.9</h1>
<h2>Added</h2>
<ul>
<li>ESP-IDF framework support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1692">tokio-rs/mio#1692</a>).</li>
<li>AIX operating system support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1704">tokio-rs/mio#1704</a>).</li>
<li>Vita support
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1721">tokio-rs/mio#1721</a>).</li>
<li><code>{UnixListener,UnixStream}:bind_addr</code>
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1630">tokio-rs/mio#1630</a>).</li>
<li><code>mio_unsupported_force_poll_poll</code> and <code>mio_unsupported_force_waker_pipe</code>
<strong>unsupported</strong> configuration flags to force a specific poll or waker
implementation
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1684">tokio-rs/mio#1684</a>,
<a href="https://redirect.github.com/tokio-rs/mio/pull/1685">tokio-rs/mio#1685</a>,
<a href="https://redirect.github.com/tokio-rs/mio/pull/1692">tokio-rs/mio#1692</a>).</li>
</ul>
<h2>Fixed</h2>
<ul>
<li>The <code>pipe(2)</code> based waker (swapped file descriptors)
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1722">tokio-rs/mio#1722</a>).</li>
<li>The duplicate waker check to work correctly with cloned <code>Registry</code>s.
(<a href="https://redirect.github.com/tokio-rs/mio/pull/1706">tokio-rs/mio#1706</a>).</li>
</ul>
<h1>0.8.8</h1>
<h2>Fixed</h2>
<ul>
<li>Fix compilation on WASI (<a href="https://redirect.github.com/tokio-rs/mio/pull/1676">tokio-rs/mio#1676</a>).</li>
</ul>
<h1>0.8.7</h1>
<h2>Added</h2>
<ul>
<li>Add/fix support for tvOS and watchOS, Mio should now build for tvOS and</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/mio/commit/0328bdef900b6396b8d00d33c825cd8af748553d"><code>0328bde</code></a> Release v0.8.11</li>
<li><a href="https://github.com/tokio-rs/mio/commit/708449851283b57eb6f514c8f289b66e982720b3"><code>7084498</code></a> Fix warnings</li>
<li><a href="https://github.com/tokio-rs/mio/commit/90d4fe00df870acd3d38f3dc4face9aacab8fbb9"><code>90d4fe0</code></a> named-pipes: fix receiving IOCP events after deregister</li>
<li><a href="https://github.com/tokio-rs/mio/commit/c710a307f8627c4d63ac1003252aa45175e08399"><code>c710a30</code></a> Add v0.8.x to the CI</li>
<li><a href="https://github.com/tokio-rs/mio/commit/c29e21c244b2b835e8b3e015b92c708c33c7d70a"><code>c29e21c</code></a> Release v0.8.10</li>
<li><a href="https://github.com/tokio-rs/mio/commit/f6a20da1c81c2d56a78bc6f6832b9904b9215914"><code>f6a20da</code></a> Add Solaris operating system support (<a href="https://redirect.github.com/tokio-rs/mio/issues/1724">#1724</a>)</li>
<li><a href="https://github.com/tokio-rs/mio/commit/e80c3b21b59b92238f4c8c331fcfc4a71508d1c5"><code>e80c3b2</code></a> Release v0.8.9</li>
<li><a href="https://github.com/tokio-rs/mio/commit/862786bbbf719886be55631c0d150d4813a9a1b6"><code>862786b</code></a> Fix importing of IoSourceState</li>
<li><a href="https://github.com/tokio-rs/mio/commit/40348728e4f06f5e150783d8f1559ee974e5e834"><code>4034872</code></a> Add support for vita target</li>
<li><a href="https://github.com/tokio-rs/mio/commit/8eb4010a92bede550850e177d3dd7c4c76eb90ba"><code>8eb4010</code></a> Fix receiver and sender fd in pipe based waker</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/mio/compare/v0.8.6...v0.8.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mio&package-manager=cargo&previous-version=0.8.6&new-version=0.8.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:25:12 +0000 UTC
    </div>
</div>

