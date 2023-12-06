---
layout: default
title: learning-tokens
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/learning-tokens
---

# learning-tokens <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/learning-tokens){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Bump vite from 4.4.11 to 4.4.12 in /src/learning-token-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) from 4.4.11 to 4.4.12.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v4.4.12/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->4.4.12 (2023-12-04)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: backport <a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15223">#15223</a>, proxy html path should be encoded (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15226">#15226</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15227">#15227</a>) (<a href="https://github.com/vitejs/vite/commit/fe8b209">fe8b209</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15223">#15223</a> <a href="https://redirect.github.com/vitejs/vite/issues/15226">#15226</a> <a href="https://redirect.github.com/vitejs/vite/issues/15227">#15227</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/09626f898bbb9e3d68facd0330d4a0acef0cba6a"><code>09626f8</code></a> release: v4.4.12</li>
<li><a href="https://github.com/vitejs/vite/commit/fe8b2090236805bb5ad6c2a5b422976523e21da1"><code>fe8b209</code></a> fix: backport <a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15223">#15223</a>, proxy html path should be encoded (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15226">#15226</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15227">#15227</a>)</li>
<li>See full diff in <a href="https://github.com/vitejs/vite/commits/v4.4.12/packages/vite">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=vite&package-manager=npm_and_yarn&previous-version=4.4.11&new-version=4.4.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 00:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Bump axios from 1.5.1 to 1.6.2 in /src/learning-token
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.5.1 to 1.6.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.2</h2>
<h2>Release notes:</h2>
<h3>Features</h3>
<ul>
<li><strong>withXSRFToken:</strong> added withXSRFToken option as a workaround to achieve the old <code>withCredentials</code> behavior; (<a href="https://redirect.github.com/axios/axios/issues/6046">#6046</a>) (<a href="https://github.com/axios/axios/commit/cff996779b272a5e94c2b52f5503ccf668bc42dc">cff9967</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>feat(withXSRFToken): added withXSRFToken option as a workaround to achieve the old `withCredentials` behavior; ( <a href="https://api.github.com/repos/axios/axios/pulls/6046">#6046</a> )</li>
</ul>
<pre><code>
📢 This PR added &amp;#x27;withXSRFToken&amp;#x27; option as a replacement for old withCredentials behaviour. 
You should now use withXSRFToken along with withCredential to get the old behavior.
This functionality is considered as a fix.
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+271/-146 ([#6081](https://github.com/axios/axios/issues/6081) [#6080](https://github.com/axios/axios/issues/6080) [#6079](https://github.com/axios/axios/issues/6079) [#6078](https://github.com/axios/axios/issues/6078) [#6046](https://github.com/axios/axios/issues/6046) [#6064](https://github.com/axios/axios/issues/6064) [#6063](https://github.com/axios/axios/issues/6063) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/ckng0221" title="+4/-4 ([#6073](https://github.com/axios/axios/issues/6073) )">Ng Choon Khon (CK)</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/mnomanmemon" title="+2/-2 ([#6048](https://github.com/axios/axios/issues/6048) )">Muhammad Noman</a></li>
</ul>
<h2>Release v1.6.1</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>formdata:</strong> fixed content-type header normalization for non-standard browser environments; (<a href="https://redirect.github.com/axios/axios/issues/6056">#6056</a>) (<a href="https://github.com/axios/axios/commit/dd465ab22bbfa262c6567be6574bf46a057d5288">dd465ab</a>)</li>
<li><strong>platform:</strong> fixed emulated browser detection in node.js environment; (<a href="https://redirect.github.com/axios/axios/issues/6055">#6055</a>) (<a href="https://github.com/axios/axios/commit/3dc8369e505e32a4e12c22f154c55fd63ac67fbb">3dc8369</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+432/-65 ([#6059](https://github.com/axios/axios/issues/6059) [#6056](https://github.com/axios/axios/issues/6056) [#6055](https://github.com/axios/axios/issues/6055) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/meyfa" title="+5/-2 ([#5835](https://github.com/axios/axios/issues/5835) )">Fabian Meyer</a></li>
</ul>
<h2>Release v1.6.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/axios/axios/compare/v1.6.1...v1.6.2">1.6.2</a> (2023-11-14)</h2>
<h3>Features</h3>
<ul>
<li><strong>withXSRFToken:</strong> added withXSRFToken option as a workaround to achieve the old <code>withCredentials</code> behavior; (<a href="https://redirect.github.com/axios/axios/issues/6046">#6046</a>) (<a href="https://github.com/axios/axios/commit/cff996779b272a5e94c2b52f5503ccf668bc42dc">cff9967</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>feat(withXSRFToken): added withXSRFToken option as a workaround to achieve the old `withCredentials` behavior; ( <a href="https://api.github.com/repos/axios/axios/pulls/6046">#6046</a> )</li>
</ul>
<pre><code>
📢 This PR added &amp;#x27;withXSRFToken&amp;#x27; option as a replacement for old withCredentials behaviour. 
You should now use withXSRFToken along with withCredential to get the old behavior.
This functionality is considered as a fix.
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+271/-146 ([#6081](https://github.com/axios/axios/issues/6081) [#6080](https://github.com/axios/axios/issues/6080) [#6079](https://github.com/axios/axios/issues/6079) [#6078](https://github.com/axios/axios/issues/6078) [#6046](https://github.com/axios/axios/issues/6046) [#6064](https://github.com/axios/axios/issues/6064) [#6063](https://github.com/axios/axios/issues/6063) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/ckng0221" title="+4/-4 ([#6073](https://github.com/axios/axios/issues/6073) )">Ng Choon Khon (CK)</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/mnomanmemon" title="+2/-2 ([#6048](https://github.com/axios/axios/issues/6048) )">Muhammad Noman</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.6.0...v1.6.1">1.6.1</a> (2023-11-08)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>formdata:</strong> fixed content-type header normalization for non-standard browser environments; (<a href="https://redirect.github.com/axios/axios/issues/6056">#6056</a>) (<a href="https://github.com/axios/axios/commit/dd465ab22bbfa262c6567be6574bf46a057d5288">dd465ab</a>)</li>
<li><strong>platform:</strong> fixed emulated browser detection in node.js environment; (<a href="https://redirect.github.com/axios/axios/issues/6055">#6055</a>) (<a href="https://github.com/axios/axios/commit/3dc8369e505e32a4e12c22f154c55fd63ac67fbb">3dc8369</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+432/-65 ([#6059](https://github.com/axios/axios/issues/6059) [#6056](https://github.com/axios/axios/issues/6056) [#6055](https://github.com/axios/axios/issues/6055) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/meyfa" title="+5/-2 ([#5835](https://github.com/axios/axios/issues/5835) )">Fabian Meyer</a></li>
</ul>
<h3>PRs</h3>
<ul>
<li>feat(withXSRFToken): added withXSRFToken option as a workaround to achieve the old `withCredentials` behavior; ( <a href="https://api.github.com/repos/axios/axios/pulls/6046">#6046</a> )</li>
</ul>
<pre><code>
📢 This PR added &amp;#x27;withXSRFToken&amp;#x27; option as a replacement for old withCredentials behaviour. 
You should now use withXSRFToken along with withCredential to get the old behavior.
This functionality is considered as a fix.
</code></pre>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/b3be36585884ba1e237fdd0eacf55f678aefc396"><code>b3be365</code></a> chore(release): v1.6.2 (<a href="https://redirect.github.com/axios/axios/issues/6082">#6082</a>)</li>
<li><a href="https://github.com/axios/axios/commit/8739acbd28eeb6b62c3565c8cf06309d15c5ed4b"><code>8739acb</code></a> chore(ci): removed redundant release action; (<a href="https://redirect.github.com/axios/axios/issues/6081">#6081</a>)</li>
<li><a href="https://github.com/axios/axios/commit/bfa9c305238bd14d1034af9af04b6749f9dba9b4"><code>bfa9c30</code></a> chore(docs): fix outdated grunt to npm scripts (<a href="https://redirect.github.com/axios/axios/issues/6073">#6073</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a2b0fb314f5bd62deb4e9b3cb4d2e868734dd5bd"><code>a2b0fb3</code></a> chore(docs): update README.md (<a href="https://redirect.github.com/axios/axios/issues/6048">#6048</a>)</li>
<li><a href="https://github.com/axios/axios/commit/b12a6083f33539ac3883e5a9938e46a76f99305d"><code>b12a608</code></a> chore(ci): removed paths-ignore filter; (<a href="https://redirect.github.com/axios/axios/issues/6080">#6080</a>)</li>
<li><a href="https://github.com/axios/axios/commit/0c9d88602bf305926f8826bd6c1374465ddfd780"><code>0c9d886</code></a> chore(ci): reworked ignoring files logic; (<a href="https://redirect.github.com/axios/axios/issues/6079">#6079</a>)</li>
<li><a href="https://github.com/axios/axios/commit/30873ee5a8f35aef3eabcece9c81a18ae9bec7bf"><code>30873ee</code></a> chore(ci): add paths-ignore config to testing action; (<a href="https://redirect.github.com/axios/axios/issues/6078">#6078</a>)</li>
<li><a href="https://github.com/axios/axios/commit/cff996779b272a5e94c2b52f5503ccf668bc42dc"><code>cff9967</code></a> feat(withXSRFToken): added withXSRFToken option as a workaround to achieve th...</li>
<li><a href="https://github.com/axios/axios/commit/7009715369a50740ba2ce00534012c1caf269ad2"><code>7009715</code></a> chore(ci): fixed release notification action; (<a href="https://redirect.github.com/axios/axios/issues/6064">#6064</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7144f10dc51a841527167b62b7d792e2989656c2"><code>7144f10</code></a> chore(ci): fixed release notification action; (<a href="https://redirect.github.com/axios/axios/issues/6063">#6063</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.5.1&new-version=1.6.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Bump next from 13.4.19 to 13.5.1 in /src/quorum-test-network/dapps/quorumToken/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [next](https://github.com/vercel/next.js) from 13.4.19 to 13.5.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vercel/next.js/commit/0c1c7f847ee820f93bdf08e809b1e2e62230ab4b"><code>0c1c7f8</code></a> v13.5.1</li>
<li><a href="https://github.com/vercel/next.js/commit/974428583e2fe83e3484523b021b0909961b6ad5"><code>9744285</code></a> v13.5.1-canary.1</li>
<li><a href="https://github.com/vercel/next.js/commit/44eba020c615f0d9efe431f84ada67b81576f3f5"><code>44eba02</code></a> improve publish-release (<a href="https://redirect.github.com/vercel/next.js/issues/55597">#55597</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/c652dc881185b62ce4e146cf6bd40b84915322f1"><code>c652dc8</code></a> v13.5.1-canary.0</li>
<li><a href="https://github.com/vercel/next.js/commit/ffafad2c35a3f9677bb520f68e989f58f192b931"><code>ffafad2</code></a> v13.5.0</li>
<li><a href="https://github.com/vercel/next.js/commit/4a589ed83db304b07b2a18002fff419cb4727222"><code>4a589ed</code></a> v13.4.20-canary.41</li>
<li><a href="https://github.com/vercel/next.js/commit/deb81cf246d83233a7d2c0320f19bc4518a37ae4"><code>deb81cf</code></a> fix styled-jsx alias (<a href="https://redirect.github.com/vercel/next.js/issues/55581">#55581</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/1a9b0f6f7a03ccdc825f92c654b8ca991f27d3fc"><code>1a9b0f6</code></a> improve internal error logging (<a href="https://redirect.github.com/vercel/next.js/issues/55582">#55582</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/063154918c28b4f2a45ffd8d506fc44924483d6e"><code>0631549</code></a> Fix react packages are not bundled for metadata routes (<a href="https://redirect.github.com/vercel/next.js/issues/55579">#55579</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/bad53655e8669389e534578980791079b37ea37f"><code>bad5365</code></a> Update supported config options for Turbopack (<a href="https://redirect.github.com/vercel/next.js/issues/55556">#55556</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vercel/next.js/compare/v13.4.19...v13.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=next&package-manager=npm_and_yarn&previous-version=13.4.19&new-version=13.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie and eth-gas-reporter in /src/quorum-test-network/dapps/quorumToken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [tough-cookie](https://github.com/salesforce/tough-cookie). It's no longer used after updating ancestor dependency [eth-gas-reporter](https://github.com/cgewecke/eth-gas-reporter). These dependencies need to be updated together.

Removes `tough-cookie`

Updates `eth-gas-reporter` from 0.2.25 to 0.2.27
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cgewecke/eth-gas-reporter/releases">eth-gas-reporter's releases</a>.</em></p>
<blockquote>
<h2>v0.2.27</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove <code>@​ethersproject/abi</code>, use ethers.utils by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/301">cgewecke/eth-gas-reporter#301</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.26...v0.2.27">https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.26...v0.2.27</a></p>
<h2>v0.2.26</h2>
<h2>What's Changed</h2>
<ul>
<li>Update Mocha to v10 by <a href="https://github.com/frangio"><code>@​frangio</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/295">cgewecke/eth-gas-reporter#295</a></li>
<li>Bump ethers version by <a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/296">cgewecke/eth-gas-reporter#296</a></li>
<li>Remove unused request package by <a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/297">cgewecke/eth-gas-reporter#297</a></li>
<li>Replace request-promise-native with axios by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/299">cgewecke/eth-gas-reporter#299</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> made their first contribution in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/296">cgewecke/eth-gas-reporter#296</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.2...v0.2.26">https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.2...v0.2.26</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cgewecke/eth-gas-reporter/blob/master/CHANGELOG.md">eth-gas-reporter's changelog</a>.</em></p>
<blockquote>
<h1>0.2.27 / 2023-09-30</h1>
<ul>
<li>Remove <code>@​ethersproject/abi</code>, use ethers.utils instead (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/301">cgewecke/eth-gas-reporter#301</a>)</li>
</ul>
<h1>0.2.26 / 2023-09-29</h1>
<ul>
<li>Replace request-promise-native with axios / avoid default price API calls (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/299">cgewecke/eth-gas-reporter#299</a>)</li>
<li>Remove request package (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/297">cgewecke/eth-gas-reporter#297</a>)</li>
<li>Bump ethers version (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/296">cgewecke/eth-gas-reporter#296</a>)</li>
<li>Update Mocha to v10 (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/295">cgewecke/eth-gas-reporter#295</a>)</li>
</ul>
<h1>0.2.23 / 2021-11-26</h1>
<ul>
<li>Add notes to README about missing price data &amp; remote data fetching race condition</li>
<li>Add support for multiple gas price tokens (BNB, MATIC, AVAX, HR, MOVR) (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/251">cgewecke/eth-gas-reporter#251</a>)</li>
<li>Make <code>@​codechecks/client</code> peer dep optional (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/257">cgewecke/eth-gas-reporter#257</a>)</li>
<li>Update <code>@​solidity-parser/parser</code> to 0.14.0 (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/261">cgewecke/eth-gas-reporter#261</a>)</li>
</ul>
<h1>0.2.22 / 2021-03-04</h1>
<ul>
<li>Update <code>@​solidity-parser/parser</code> to ^0.12.0 (support Panic keyword in catch blocks) (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/243">cgewecke/eth-gas-reporter#243</a>)</li>
</ul>
<h1>0.2.21 / 2021-02-16</h1>
<ul>
<li>Fix missing truffle migration deployments data (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/240">cgewecke/eth-gas-reporter#240</a>)</li>
<li>Upgrade solidity-parser/parser to 0.11.1 (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/239">cgewecke/eth-gas-reporter#239</a>)</li>
</ul>
<h1>0.2.20 / 2020-12-01</h1>
<ul>
<li>Add support for remote contracts data pre-loading (hardhat-gas-reporter feature)</li>
</ul>
<h1>0.2.19 / 2020-10-29</h1>
<ul>
<li>Delegate contract loading/parsing to artifactor &amp; make optional (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/227">#227</a>)</li>
</ul>
<h1>0.2.18 / 2020-10-13</h1>
<ul>
<li>Support multiple codechecks reports per CI run</li>
<li>Add CI error threshold options: maxMethodDiff, maxDeploymentDiff</li>
<li>Add async collection methods for BuidlerEVM</li>
<li>Update solidity-parser/parser to 0.8.0 (contribution: <a href="https://github.com/vicnaum"><code>@​vicnaum</code></a>)</li>
<li>Update dev deps / use Node 12 in CI</li>
</ul>
<h1>0.2.17 / 2020-04-13</h1>
<ul>
<li>Use <code>@​solidity-parser/parser</code> for better solc 0.6.x parsing</li>
<li>Upgrade Mocha to ^7.1.1 (to remove minimist vuln warning)</li>
<li>Stop crashing when parser or ABI Encoder fails</li>
<li>Update <code>@​ethersproject/abi</code> to ^5.0.0-beta.146 (and unpin)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/cgewecke/eth-gas-reporter/commits/v0.2.27">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Bump postcss and next in /src/quorum-test-network/dapps/quorumToken/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) to 8.4.31 and updates ancestor dependency [next](https://github.com/vercel/next.js). These dependencies need to be updated together.

Updates `postcss` from 8.4.14 to 8.4.31
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by <a href="https://github.com/idoros"><code>@​idoros</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/coliff"><code>@​coliff</code></a>).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
<h2>8.4.27</h2>
<ul>
<li>Fixed <code>Container</code> clone methods types.</li>
</ul>
<h2>8.4.26</h2>
<ul>
<li>Fixed clone methods types.</li>
</ul>
<h2>8.4.25</h2>
<ul>
<li>Improve stringify performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/vikaskaliramna07"><code>@​vikaskaliramna07</code></a>).</li>
</ul>
<h2>8.4.24</h2>
<ul>
<li>Fixed <code>Plugin</code> types.</li>
</ul>
<h2>8.4.23</h2>
<ul>
<li>Fixed warnings in TypeDoc.</li>
</ul>
<h2>8.4.22</h2>
<ul>
<li>Fixed TypeScript support with <code>node16</code> (by <a href="https://github.com/remcohaszing"><code>@​remcohaszing</code></a>).</li>
</ul>
<h2>8.4.21</h2>
<ul>
<li>Fixed <code>Input#error</code> types (by <a href="https://github.com/hudochenkov"><code>@​hudochenkov</code></a>).</li>
</ul>
<h2>8.4.20</h2>
<ul>
<li>Fixed source map generation for childless at-rules like <code>@layer</code>.</li>
</ul>
<h2>8.4.19</h2>
<ul>
<li>Fixed whitespace preserving after AST transformations (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.18</h2>
<ul>
<li>Fixed an error on <code>absolute: true</code> with empty <code>sourceContent</code> (by <a href="https://github.com/KingSora"><code>@​KingSora</code></a>).</li>
</ul>
<h2>8.4.17</h2>
<ul>
<li>Fixed <code>Node.before()</code> unexpected behavior (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added TOC to docs (by <a href="https://github.com/muddv"><code>@​muddv</code></a>).</li>
</ul>
<h2>8.4.16</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/main/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by Romain Menke).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by Ido Rosenthal).</li>
<li>Fixed docs (by Christian Oliff).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by Romain Menke).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
<h2>8.4.27</h2>
<ul>
<li>Fixed <code>Container</code> clone methods types.</li>
</ul>
<h2>8.4.26</h2>
<ul>
<li>Fixed clone methods types.</li>
</ul>
<h2>8.4.25</h2>
<ul>
<li>Improve stringify performance (by Romain Menke).</li>
<li>Fixed docs (by <a href="https://github.com/vikaskaliramna07"><code>@​vikaskaliramna07</code></a>).</li>
</ul>
<h2>8.4.24</h2>
<ul>
<li>Fixed <code>Plugin</code> types.</li>
</ul>
<h2>8.4.23</h2>
<ul>
<li>Fixed warnings in TypeDoc.</li>
</ul>
<h2>8.4.22</h2>
<ul>
<li>Fixed TypeScript support with <code>node16</code> (by Remco Haszing).</li>
</ul>
<h2>8.4.21</h2>
<ul>
<li>Fixed <code>Input#error</code> types (by Aleks Hudochenkov).</li>
</ul>
<h2>8.4.20</h2>
<ul>
<li>Fixed source map generation for childless at-rules like <code>@layer</code>.</li>
</ul>
<h2>8.4.19</h2>
<ul>
<li>Fixed whitespace preserving after AST transformations (by Romain Menke).</li>
</ul>
<h2>8.4.18</h2>
<ul>
<li>Fixed an error on <code>absolute: true</code> with empty <code>sourceContent</code> (by Rene Haas).</li>
</ul>
<h2>8.4.17</h2>
<ul>
<li>Fixed <code>Node.before()</code> unexpected behavior (by Romain Menke).</li>
<li>Added TOC to docs (by Mikhail Dedov).</li>
</ul>
<h2>8.4.16</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/90208de8805dd762596c0028b8637ffbed23e371"><code>90208de</code></a> Release 8.4.31 version</li>
<li><a href="https://github.com/postcss/postcss/commit/58cc860b4c1707510c9cd1bc1fa30b423a9ad6c5"><code>58cc860</code></a> Fix carrier return parsing</li>
<li><a href="https://github.com/postcss/postcss/commit/4fff8e4cdc237619df1d73a444c0a8329701c1e2"><code>4fff8e4</code></a> Improve pnpm test output</li>
<li><a href="https://github.com/postcss/postcss/commit/cd43ed123274a92ebc13a1e8cccf1d65b8198f84"><code>cd43ed1</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/caa916bdcbf66c51321574e2dde112ab13e8b306"><code>caa916b</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/8972f76923e921a3c9655822382039b31b1c8e1a"><code>8972f76</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/11a5286f781d2a637f2c545c5e9cd661055acaab"><code>11a5286</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/45c55017776fc61f7815d1ea8e92d5291ca5d6c8"><code>45c5501</code></a> Release 8.4.30 version</li>
<li><a href="https://github.com/postcss/postcss/commit/bc3c341f589f9c15f1b56838a33d908374e537e0"><code>bc3c341</code></a> Update linter</li>
<li><a href="https://github.com/postcss/postcss/commit/b2be58a2eb788d12474ee1335f8ecdb9fa6225aa"><code>b2be58a</code></a> Merge pull request <a href="https://redirect.github.com/postcss/postcss/issues/1881">#1881</a> from romainmenke/improve-sourcemap-performance--phil...</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/8.4.14...8.4.31">compare view</a></li>
</ul>
</details>
<br />

Updates `next` from 13.4.19 to 13.5.6
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vercel/next.js/commit/9051bc44d969a6e0ab65a955a2fc0af522a83911"><code>9051bc4</code></a> v13.5.6</li>
<li><a href="https://github.com/vercel/next.js/commit/a9e796eb7c8510efb2bf41ca7e8132f2c59b57d0"><code>a9e796e</code></a> update version script</li>
<li><a href="https://github.com/vercel/next.js/commit/70f93bfe748ccc0cc8dbbc441b699d65d5844fb6"><code>70f93bf</code></a> update ci config</li>
<li><a href="https://github.com/vercel/next.js/commit/7db2ce3b8db4e06c18f49145c7acc3601ba32cc3"><code>7db2ce3</code></a> Upgrade edge-runtime/cookies (<a href="https://redirect.github.com/vercel/next.js/issues/57021">#57021</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/40965ebd27a60bb9ca12994f2f338a24333851db"><code>40965eb</code></a> Patch React with fix for write-after-close for ReadableStream (<a href="https://redirect.github.com/vercel/next.js/issues/57011">#57011</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/54145b49f93faf116dd8518e35fe1e008dcac616"><code>54145b4</code></a> v13.5.5</li>
<li><a href="https://github.com/vercel/next.js/commit/1609da2d9552fed48ab45969bdc5631230c6d356"><code>1609da2</code></a> v13.5.5-canary.19</li>
<li><a href="https://github.com/vercel/next.js/commit/8a51ebcb6794988bd5c11393819278dcbb3ed2c0"><code>8a51ebc</code></a> Revert &quot;feat(turbopack): support basic next/dynamic&quot; (<a href="https://redirect.github.com/vercel/next.js/issues/56885">#56885</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/c1c419fde0858fe8e1c4641f7f6994fb450236dc"><code>c1c419f</code></a> v13.5.5-canary.18</li>
<li><a href="https://github.com/vercel/next.js/commit/4e435e2fe6b2297bf63ca5d17ade07169ad2c35e"><code>4e435e2</code></a> Skip webpack specific tests in Turbopack test run (<a href="https://redirect.github.com/vercel/next.js/issues/56877">#56877</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vercel/next.js/compare/v13.4.19...v13.5.6">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Bump zod and next in /src/quorum-test-network/dapps/quorumToken/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [zod](https://github.com/colinhacks/zod). It's no longer used after updating ancestor dependency [next](https://github.com/vercel/next.js). These dependencies need to be updated together.

Removes `zod`

Updates `next` from 13.4.19 to 13.5.6
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vercel/next.js/commit/9051bc44d969a6e0ab65a955a2fc0af522a83911"><code>9051bc4</code></a> v13.5.6</li>
<li><a href="https://github.com/vercel/next.js/commit/a9e796eb7c8510efb2bf41ca7e8132f2c59b57d0"><code>a9e796e</code></a> update version script</li>
<li><a href="https://github.com/vercel/next.js/commit/70f93bfe748ccc0cc8dbbc441b699d65d5844fb6"><code>70f93bf</code></a> update ci config</li>
<li><a href="https://github.com/vercel/next.js/commit/7db2ce3b8db4e06c18f49145c7acc3601ba32cc3"><code>7db2ce3</code></a> Upgrade edge-runtime/cookies (<a href="https://redirect.github.com/vercel/next.js/issues/57021">#57021</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/40965ebd27a60bb9ca12994f2f338a24333851db"><code>40965eb</code></a> Patch React with fix for write-after-close for ReadableStream (<a href="https://redirect.github.com/vercel/next.js/issues/57011">#57011</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/54145b49f93faf116dd8518e35fe1e008dcac616"><code>54145b4</code></a> v13.5.5</li>
<li><a href="https://github.com/vercel/next.js/commit/1609da2d9552fed48ab45969bdc5631230c6d356"><code>1609da2</code></a> v13.5.5-canary.19</li>
<li><a href="https://github.com/vercel/next.js/commit/8a51ebcb6794988bd5c11393819278dcbb3ed2c0"><code>8a51ebc</code></a> Revert &quot;feat(turbopack): support basic next/dynamic&quot; (<a href="https://redirect.github.com/vercel/next.js/issues/56885">#56885</a>)</li>
<li><a href="https://github.com/vercel/next.js/commit/c1c419fde0858fe8e1c4641f7f6994fb450236dc"><code>c1c419f</code></a> v13.5.5-canary.18</li>
<li><a href="https://github.com/vercel/next.js/commit/4e435e2fe6b2297bf63ca5d17ade07169ad2c35e"><code>4e435e2</code></a> Skip webpack specific tests in Turbopack test run (<a href="https://redirect.github.com/vercel/next.js/issues/56877">#56877</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vercel/next.js/compare/v13.4.19...v13.5.6">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Bump flat, eth-gas-reporter and solidity-coverage in /src/quorum-test-network/dapps/quorumToken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [flat](https://github.com/hughsk/flat) to 5.0.2 and updates ancestor dependencies [flat](https://github.com/hughsk/flat), [eth-gas-reporter](https://github.com/cgewecke/eth-gas-reporter) and [solidity-coverage](https://github.com/sc-forks/solidity-coverage). These dependencies need to be updated together.

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

Updates `eth-gas-reporter` from 0.2.25 to 0.2.27
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cgewecke/eth-gas-reporter/releases">eth-gas-reporter's releases</a>.</em></p>
<blockquote>
<h2>v0.2.27</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove <code>@​ethersproject/abi</code>, use ethers.utils by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/301">cgewecke/eth-gas-reporter#301</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.26...v0.2.27">https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.26...v0.2.27</a></p>
<h2>v0.2.26</h2>
<h2>What's Changed</h2>
<ul>
<li>Update Mocha to v10 by <a href="https://github.com/frangio"><code>@​frangio</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/295">cgewecke/eth-gas-reporter#295</a></li>
<li>Bump ethers version by <a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/296">cgewecke/eth-gas-reporter#296</a></li>
<li>Remove unused request package by <a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/297">cgewecke/eth-gas-reporter#297</a></li>
<li>Replace request-promise-native with axios by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/299">cgewecke/eth-gas-reporter#299</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> made their first contribution in <a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/296">cgewecke/eth-gas-reporter#296</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.2...v0.2.26">https://github.com/cgewecke/eth-gas-reporter/compare/v0.2.2...v0.2.26</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cgewecke/eth-gas-reporter/blob/master/CHANGELOG.md">eth-gas-reporter's changelog</a>.</em></p>
<blockquote>
<h1>0.2.27 / 2023-09-30</h1>
<ul>
<li>Remove <code>@​ethersproject/abi</code>, use ethers.utils instead (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/301">cgewecke/eth-gas-reporter#301</a>)</li>
</ul>
<h1>0.2.26 / 2023-09-29</h1>
<ul>
<li>Replace request-promise-native with axios / avoid default price API calls (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/299">cgewecke/eth-gas-reporter#299</a>)</li>
<li>Remove request package (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/297">cgewecke/eth-gas-reporter#297</a>)</li>
<li>Bump ethers version (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/296">cgewecke/eth-gas-reporter#296</a>)</li>
<li>Update Mocha to v10 (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/295">cgewecke/eth-gas-reporter#295</a>)</li>
</ul>
<h1>0.2.23 / 2021-11-26</h1>
<ul>
<li>Add notes to README about missing price data &amp; remote data fetching race condition</li>
<li>Add support for multiple gas price tokens (BNB, MATIC, AVAX, HR, MOVR) (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/251">cgewecke/eth-gas-reporter#251</a>)</li>
<li>Make <code>@​codechecks/client</code> peer dep optional (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/257">cgewecke/eth-gas-reporter#257</a>)</li>
<li>Update <code>@​solidity-parser/parser</code> to 0.14.0 (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/pull/261">cgewecke/eth-gas-reporter#261</a>)</li>
</ul>
<h1>0.2.22 / 2021-03-04</h1>
<ul>
<li>Update <code>@​solidity-parser/parser</code> to ^0.12.0 (support Panic keyword in catch blocks) (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/243">cgewecke/eth-gas-reporter#243</a>)</li>
</ul>
<h1>0.2.21 / 2021-02-16</h1>
<ul>
<li>Fix missing truffle migration deployments data (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/240">cgewecke/eth-gas-reporter#240</a>)</li>
<li>Upgrade solidity-parser/parser to 0.11.1 (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/239">cgewecke/eth-gas-reporter#239</a>)</li>
</ul>
<h1>0.2.20 / 2020-12-01</h1>
<ul>
<li>Add support for remote contracts data pre-loading (hardhat-gas-reporter feature)</li>
</ul>
<h1>0.2.19 / 2020-10-29</h1>
<ul>
<li>Delegate contract loading/parsing to artifactor &amp; make optional (<a href="https://redirect.github.com/cgewecke/eth-gas-reporter/issues/227">#227</a>)</li>
</ul>
<h1>0.2.18 / 2020-10-13</h1>
<ul>
<li>Support multiple codechecks reports per CI run</li>
<li>Add CI error threshold options: maxMethodDiff, maxDeploymentDiff</li>
<li>Add async collection methods for BuidlerEVM</li>
<li>Update solidity-parser/parser to 0.8.0 (contribution: <a href="https://github.com/vicnaum"><code>@​vicnaum</code></a>)</li>
<li>Update dev deps / use Node 12 in CI</li>
</ul>
<h1>0.2.17 / 2020-04-13</h1>
<ul>
<li>Use <code>@​solidity-parser/parser</code> for better solc 0.6.x parsing</li>
<li>Upgrade Mocha to ^7.1.1 (to remove minimist vuln warning)</li>
<li>Stop crashing when parser or ABI Encoder fails</li>
<li>Update <code>@​ethersproject/abi</code> to ^5.0.0-beta.146 (and unpin)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/cgewecke/eth-gas-reporter/commits/v0.2.27">compare view</a></li>
</ul>
</details>
<br />

Updates `solidity-coverage` from 0.8.4 to 0.8.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/releases">solidity-coverage's releases</a>.</em></p>
<blockquote>
<h2>0.8.5</h2>
<h2>What's Changed</h2>
<ul>
<li>Update mocha version to fix deprecated debug package by <a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/810">sc-forks/solidity-coverage#810</a></li>
<li>Remove all mentions to buidler by <a href="https://github.com/fvictorio"><code>@​fvictorio</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/778">sc-forks/solidity-coverage#778</a></li>
<li>change <code>.solcoverjs</code> occurencies to <code>.solcover.js</code> by <a href="https://github.com/joaoh9"><code>@​joaoh9</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/777">sc-forks/solidity-coverage#777</a></li>
<li>Add a package description by <a href="https://github.com/ilovehackathons"><code>@​ilovehackathons</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/775">sc-forks/solidity-coverage#775</a></li>
<li>Add dependabot config by <a href="https://github.com/jtakalai"><code>@​jtakalai</code></a> in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/759">sc-forks/solidity-coverage#759</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ChristopherDedominici"><code>@​ChristopherDedominici</code></a> made their first contribution in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/810">sc-forks/solidity-coverage#810</a></li>
<li><a href="https://github.com/joaoh9"><code>@​joaoh9</code></a> made their first contribution in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/777">sc-forks/solidity-coverage#777</a></li>
<li><a href="https://github.com/ilovehackathons"><code>@​ilovehackathons</code></a> made their first contribution in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/775">sc-forks/solidity-coverage#775</a></li>
<li><a href="https://github.com/jtakalai"><code>@​jtakalai</code></a> made their first contribution in <a href="https://redirect.github.com/sc-forks/solidity-coverage/pull/759">sc-forks/solidity-coverage#759</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.4...v0.8.5">https://github.com/sc-forks/solidity-coverage/compare/v0.8.4...v0.8.5</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/blob/master/CHANGELOG.md">solidity-coverage's changelog</a>.</em></p>
<blockquote>
<h1>0.8.5 / 2023-09-21</h1>
<ul>
<li>Update contributor list (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/812">sc-forks/solidity-coverage#812</a>)</li>
<li>Add dependabot config (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/759">sc-forks/solidity-coverage#759</a>)</li>
<li>Add a package description to package.json (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/775">sc-forks/solidity-coverage#775</a>)</li>
<li>change .solcoverjs occurencies to .solcover.js (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/777">sc-forks/solidity-coverage#777</a>)</li>
<li>Remove all mentions to buidler (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/778">sc-forks/solidity-coverage#778</a>)</li>
<li>Update HH dev dep &amp; fix Zeppelin E2E test (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/811">sc-forks/solidity-coverage#811</a>)</li>
<li>Update mocha version to 10.2.0, fix deprecated debug package (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/810">sc-forks/solidity-coverage#810</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/fb5fd6e1d4455eb662eb1dc6f0e1cd79e4fbd7d5"><code>fb5fd6e</code></a> Update changelog: 0.8.5</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/bfe149c4c020306aa31ada4925f765ea5fd1c9f1"><code>bfe149c</code></a> 0.8.5</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/34beea7169717ff5036d5ee9c1d26f1b44183e3e"><code>34beea7</code></a> Update contributor list (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/812">#812</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/255d7008d9d5b541e555b1a5531e6c81d3a67089"><code>255d700</code></a> Add dependabot config (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/759">#759</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/70a50840319fc8b85bbab067f54881d49e24dd4d"><code>70a5084</code></a> Add a package description to package.json (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/775">#775</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/c680e5416bb23b2118151378c6ba30281de2252a"><code>c680e54</code></a> change <code>.solcoverjs</code> occurencies to <code>.solcover.js</code> (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/777">#777</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/dea15cd82570de37b61370a071120f312ec5dac6"><code>dea15cd</code></a> Remove all mentions to buidler (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/778">#778</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/b56f2093ba3c11b79b2a01e9ff083195914d4b41"><code>b56f209</code></a> Update HH dev dep &amp; fix Zeppelin E2E test (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/811">#811</a>)</li>
<li><a href="https://github.com/sc-forks/solidity-coverage/commit/d5c134b80ff80b27dbd22a5e9c971fa7d241978c"><code>d5c134b</code></a> Update mocha version to 10.2.0, fix deprecated debug package (<a href="https://redirect.github.com/sc-forks/solidity-coverage/issues/810">#810</a>)</li>
<li>See full diff in <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.4...v0.8.5">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.23.0 to 5.28.2 in /src/quorum-test-network/dapps/quorumToken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.23.0 to 5.28.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.28.2</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: remove optional chainning for compatible with Nodejs12 and below by <a href="https://github.com/bugb"><code>@​bugb</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2470">nodejs/undici#2470</a></li>
<li>fix: remove <code>node:</code> prefix by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2471">nodejs/undici#2471</a></li>
<li>perf: avoid Headers initialization by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2468">nodejs/undici#2468</a></li>
<li>fix: handle SharedArrayBuffer correctly by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2466">nodejs/undici#2466</a></li>
<li>fix: Add <code>null</code> type to <code>signal</code> in <code>RequestInit</code> by <a href="https://github.com/gebsh"><code>@​gebsh</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2455">nodejs/undici#2455</a></li>
<li>fix: correctly handle data URL with hashes. by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2475">nodejs/undici#2475</a></li>
<li>fix: check response for timinginfo allow flag by <a href="https://github.com/ToshB"><code>@​ToshB</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2477">nodejs/undici#2477</a></li>
<li>Make call to onBodySent conditional in RetryHandler by <a href="https://github.com/MzUgM"><code>@​MzUgM</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2478">nodejs/undici#2478</a></li>
<li>refactor: better integrity check by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2462">nodejs/undici#2462</a></li>
<li>fix: Added support for inline URL username:password proxy auth by <a href="https://github.com/matt-way"><code>@​matt-way</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2473">nodejs/undici#2473</a></li>
<li>build(deps-dev): bump jsdom from 22.1.0 to 23.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2472">nodejs/undici#2472</a></li>
<li>build(deps-dev): bump sinon from 16.1.3 to 17.0.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2405">nodejs/undici#2405</a></li>
<li>build(deps): bump ossf/scorecard-action from 2.2.0 to 2.3.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2396">nodejs/undici#2396</a></li>
<li>build(deps): bump actions/setup-node from 3.8.1 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2395">nodejs/undici#2395</a></li>
<li>build(deps): bump step-security/harden-runner from 2.5.0 to 2.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2392">nodejs/undici#2392</a></li>
<li>build(deps-dev): bump formdata-node from 4.4.1 to 6.0.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2389">nodejs/undici#2389</a></li>
<li>build(deps): bump actions/upload-artifact from 3.1.2 to 3.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2302">nodejs/undici#2302</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/bugb"><code>@​bugb</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2470">nodejs/undici#2470</a></li>
<li><a href="https://github.com/gebsh"><code>@​gebsh</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2455">nodejs/undici#2455</a></li>
<li><a href="https://github.com/ToshB"><code>@​ToshB</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2477">nodejs/undici#2477</a></li>
<li><a href="https://github.com/MzUgM"><code>@​MzUgM</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2478">nodejs/undici#2478</a></li>
<li><a href="https://github.com/matt-way"><code>@​matt-way</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2473">nodejs/undici#2473</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.28.1...v5.28.2">https://github.com/nodejs/undici/compare/v5.28.1...v5.28.2</a></p>
<h2>v5.28.1</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: Improve <code>normalizeMethod</code> by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2456">nodejs/undici#2456</a></li>
<li>fix: dispatch error handling by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2459">nodejs/undici#2459</a></li>
<li>perf(request): optimize if headers are given by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2454">nodejs/undici#2454</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.28.0...v5.28.1">https://github.com/nodejs/undici/compare/v5.28.0...v5.28.1</a></p>
<h2>v5.28.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(parseHeaders): util.parseHeaders handle correctly array of buffer… by <a href="https://github.com/mdoria12"><code>@​mdoria12</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2398">nodejs/undici#2398</a></li>
<li>docs: add license to undici-types by <a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2401">nodejs/undici#2401</a></li>
<li>perf: optimize Readable.dump by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2402">nodejs/undici#2402</a></li>
<li>perf(headers): Improve Headers by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2397">nodejs/undici#2397</a></li>
<li>test: re-enable conditional WPT Report for websockets by <a href="https://github.com/panva"><code>@​panva</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2407">nodejs/undici#2407</a></li>
<li>fix: delay abort on 'close' by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2408">nodejs/undici#2408</a></li>
<li>refactor: use <code>substring</code> instead of <code>substr</code> by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2411">nodejs/undici#2411</a></li>
<li>add additional http2 test with fetch by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2419">nodejs/undici#2419</a></li>
<li>fix: HTTPToken check by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2410">nodejs/undici#2410</a></li>
<li>perf: optimize HeadersList.get by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2420">nodejs/undici#2420</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/9a14e5f32a118fa93e769cc15ae8de9de552f2e4"><code>9a14e5f</code></a> Bumped v5.28.2</li>
<li><a href="https://github.com/nodejs/undici/commit/fcdfe878d792c4347b81179bc31a2d1b1f06e8fb"><code>fcdfe87</code></a> build(deps): bump actions/upload-artifact from 3.1.2 to 3.1.3 (<a href="https://redirect.github.com/nodejs/undici/issues/2302">#2302</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/169c157f9a576e4422a20060f57db1dc4693b373"><code>169c157</code></a> build(deps-dev): bump formdata-node from 4.4.1 to 6.0.3 (<a href="https://redirect.github.com/nodejs/undici/issues/2389">#2389</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/97881779e6ba41d2fdbfe27b5c9cc0563dc60134"><code>9788177</code></a> build(deps): bump step-security/harden-runner from 2.5.0 to 2.6.0 (<a href="https://redirect.github.com/nodejs/undici/issues/2392">#2392</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/1f6d1597648d332c0705befec74387631d5df9ff"><code>1f6d159</code></a> build(deps): bump actions/setup-node from 3.8.1 to 4.0.0 (<a href="https://redirect.github.com/nodejs/undici/issues/2395">#2395</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/a393a86d09581945ce4e601d2359023e901b2dd0"><code>a393a86</code></a> build(deps): bump ossf/scorecard-action from 2.2.0 to 2.3.1 (<a href="https://redirect.github.com/nodejs/undici/issues/2396">#2396</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ea2f606e6b101fcbc578a407c8d4f9d10d17756e"><code>ea2f606</code></a> build(deps-dev): bump sinon from 16.1.3 to 17.0.1 (<a href="https://redirect.github.com/nodejs/undici/issues/2405">#2405</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/80979edc78c458e87786e25194bc64ed0a2184b4"><code>80979ed</code></a> build(deps-dev): bump jsdom from 22.1.0 to 23.0.0 (<a href="https://redirect.github.com/nodejs/undici/issues/2472">#2472</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/08183ea1d25964de9eac3b9944b0c933fe693e6f"><code>08183ea</code></a> fix: Added support for inline URL username:password proxy auth (<a href="https://redirect.github.com/nodejs/undici/issues/2473">#2473</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/28759f406ff808afa7a102e9e248291123ef59cb"><code>28759f4</code></a> refactor: better integrity check (<a href="https://redirect.github.com/nodejs/undici/issues/2462">#2462</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.23.0...v5.28.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.23.0&new-version=5.28.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:18:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    hyperledger learning token update 2023
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
        Created At 2023-12-04 18:03:30 +0000 UTC
    </div>
</div>

