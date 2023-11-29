---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump axios from 1.5.0 to 1.6.2 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.5.0 to 1.6.2.
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
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v1.5.0...v1.6.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.5.0&new-version=1.6.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-rs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 15:40:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    SNYK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Git did not allow me to push to the other branch anymore, not sure how to resolve that so I just created a new PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 13:31:54 +0000 UTC
    </div>
</div>

