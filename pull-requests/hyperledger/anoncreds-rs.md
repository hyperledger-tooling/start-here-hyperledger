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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade expo-status-bar from 1.6.0 to 1.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade expo-status-bar from 1.6.0 to 1.9.0.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **4 versions** ahead of your current version.
- The recommended version was released **a month ago**, on 2023-10-17.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>expo-status-bar</b></summary>
    <ul>
      <li>
        <b>1.9.0</b> - 2023-10-17
      </li>
      <li>
        <b>1.8.0</b> - 2023-09-15
      </li>
      <li>
        <b>1.7.1</b> - 2023-08-02
      </li>
      <li>
        <b>1.7.0</b> - 2023-07-28
      </li>
      <li>
        <b>1.6.0</b> - 2023-06-21
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/expo/expo/releases">expo-status-bar GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>expo-status-bar</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/da25937e2a99661cbe5eb60ca1d8d6245fc96a50">da25937</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/ee7897097f5f946ad7fcb94447eed789b984dd02">ee78970</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/f242ff9b614d4fef5e9a1f1849d881ed033a39fa">f242ff9</a> [cli][config] warn when dynamic config doesn&#x27;t use static config present in project (#24308)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/551de2991b26cee84769165decd58fe829d4c186">551de29</a> update haptics docs (#24876)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/c7cdf53ffdd47e09e50435252a05caf223d6ae0b">c7cdf53</a> preserve jsx across Expo SDK (#24889)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/17161dc0ecddb887a54f7cd38f9e8ed7d1b0ea17">17161dc</a> [expo-av][iOS] Fix compilation on tvOS (#24864)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/767bbe499cc4ebf6b027cceb7411610234890eb4">767bbe4</a> [core][Android] Fix &#x60;null&#x60; or &#x60;undefined&#x60; wasn&#x27;t converted to &#x60;JavaScriptValue&#x60; (#24899)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/82c0de2d1347c00e1dd57f2d0e300cb8462ada8c">82c0de2</a> [core][Android] Add &#x60;CommonExceptions.ModuleNotFound&#x60; (#24898)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/01136e7c5b54de35aa5ac0c66834e1617071540e">01136e7</a> [core][Android] Add type converter for the &#x60;Set&#x60; class (#24897)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/66a72535725d6275f4d46ec5d9d27cd090314bfc">66a7253</a> [ios][application] Migrate to Expo Modules API (#24871)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/1ffca92739c49322f6beef3a394fa62f0214a7ce">1ffca92</a> [expo-image][iOS] ImageView - check macCatalyst support to use ImageAnalyzer (#24880)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/3bd96242183683f3aaf21143f17dd134af437cab">3bd9624</a> [expo-image] [ENG-10268] support tintColor for SVGs on Android (part 2) (#24888)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/5da49f817864b2415e480830f4e2fc1ffa6dfc5e">5da49f8</a> [docs] Update local app development doc to clarify a couple points</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/923016204c239cdad07b89626ac65eb505623d98">9230162</a> [font] config plugin to link fonts in the native projects (#24772)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/174dee96aa2c99ab33e2a768118c9a28e476ce05">174dee9</a> [docs] install prettier with eslint (#24872)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/a62b155fbcdc8bd04b67ebc3083b6906e574831a">a62b155</a> [docs] remove unnecessary import from router docs (#24869)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/30a430ac2ec9e346b99e92b57840ad7ee29a297f">30a430a</a> Revert &quot;Revert &quot;[build-properties] Support modifying &lt;queries&gt; tag in android manifest (#24619)&quot;&quot;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/248319fac2e24e9c0b4d63fbf53e3466cb9cd71b">248319f</a> Revert &quot;[build-properties] Support modifying &lt;queries&gt; tag in android manifest (#24619)&quot;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/fe399504a43df191399bde7c84151f1982026c84">fe39950</a> [core] fix shared object exception for thread issues (#24836)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/995844a20418c1d341f38809ca857e049efc4677">995844a</a> [android][ios] Upgrade react-native-webview to 13.6.2 (#24850)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/64705e7f25ccd329343f056feca9901e3d12205b">64705e7</a> Update @ react-native-picker/picker to 2.5.1 (#24839)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/954cc4a6dd4d0458c441782578f09fc22ce54f9c">954cc4a</a> [actions] remove &#x27;need review&#x27; label if an issue is accepted (#24855)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/2740dee1a618e0e5c5ffd66a0cbe3c873b932ed9">2740dee</a> [build-properties] Support modifying &lt;queries&gt; tag in android manifest (#24619)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/05fecad5d0d1ccbb9b50411dde4f477b9dd1312f">05fecad</a> commit yarn.lock</li>
    </ul>

   <a href="https://snyk.io/redirect/github/expo/expo/compare/fa5ecca8251986b9f197cc14074eec0ab6dfb6db...da25937e2a99661cbe5eb60ca1d8d6245fc96a50">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiIzNzAzZDU3NS1jZGQ5LTRjZDUtYjA0My05MzlhMTJiMjEyMDYiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjM3MDNkNTc1LWNkZDktNGNkNS1iMDQzLTkzOWExMmIyMTIwNiJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?pkg&#x3D;expo-status-bar&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"3703d575-cdd9-4cd5-b043-939a12b21206","prPublicId":"3703d575-cdd9-4cd5-b043-939a12b21206","dependencies":[{"name":"expo-status-bar","from":"1.6.0","to":"1.9.0"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"adcadd64-fca2-41e4-9476-aa9d33532df3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":4,"publishedDate":"2023-10-17T20:28:08.927Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 17:00:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade expo-splash-screen from 0.20.5 to 0.24.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade expo-splash-screen from 0.20.5 to 0.24.0.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **6 versions** ahead of your current version.
- The recommended version was released **a month ago**, on 2023-10-17.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>expo-splash-screen</b></summary>
    <ul>
      <li>
        <b>0.24.0</b> - 2023-10-17
      </li>
      <li>
        <b>0.23.1</b> - 2023-09-18
      </li>
      <li>
        <b>0.23.0</b> - 2023-09-15
      </li>
      <li>
        <b>0.22.0</b> - 2023-09-04
      </li>
      <li>
        <b>0.21.1</b> - 2023-08-02
      </li>
      <li>
        <b>0.21.0</b> - 2023-07-28
      </li>
      <li>
        <b>0.20.5</b> - 2023-07-29
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/expo/expo/releases">expo-splash-screen GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>expo-splash-screen</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/da25937e2a99661cbe5eb60ca1d8d6245fc96a50">da25937</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/ee7897097f5f946ad7fcb94447eed789b984dd02">ee78970</a> Publish packages</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/f242ff9b614d4fef5e9a1f1849d881ed033a39fa">f242ff9</a> [cli][config] warn when dynamic config doesn&#x27;t use static config present in project (#24308)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/551de2991b26cee84769165decd58fe829d4c186">551de29</a> update haptics docs (#24876)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/c7cdf53ffdd47e09e50435252a05caf223d6ae0b">c7cdf53</a> preserve jsx across Expo SDK (#24889)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/17161dc0ecddb887a54f7cd38f9e8ed7d1b0ea17">17161dc</a> [expo-av][iOS] Fix compilation on tvOS (#24864)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/767bbe499cc4ebf6b027cceb7411610234890eb4">767bbe4</a> [core][Android] Fix &#x60;null&#x60; or &#x60;undefined&#x60; wasn&#x27;t converted to &#x60;JavaScriptValue&#x60; (#24899)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/82c0de2d1347c00e1dd57f2d0e300cb8462ada8c">82c0de2</a> [core][Android] Add &#x60;CommonExceptions.ModuleNotFound&#x60; (#24898)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/01136e7c5b54de35aa5ac0c66834e1617071540e">01136e7</a> [core][Android] Add type converter for the &#x60;Set&#x60; class (#24897)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/66a72535725d6275f4d46ec5d9d27cd090314bfc">66a7253</a> [ios][application] Migrate to Expo Modules API (#24871)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/1ffca92739c49322f6beef3a394fa62f0214a7ce">1ffca92</a> [expo-image][iOS] ImageView - check macCatalyst support to use ImageAnalyzer (#24880)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/3bd96242183683f3aaf21143f17dd134af437cab">3bd9624</a> [expo-image] [ENG-10268] support tintColor for SVGs on Android (part 2) (#24888)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/5da49f817864b2415e480830f4e2fc1ffa6dfc5e">5da49f8</a> [docs] Update local app development doc to clarify a couple points</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/923016204c239cdad07b89626ac65eb505623d98">9230162</a> [font] config plugin to link fonts in the native projects (#24772)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/174dee96aa2c99ab33e2a768118c9a28e476ce05">174dee9</a> [docs] install prettier with eslint (#24872)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/a62b155fbcdc8bd04b67ebc3083b6906e574831a">a62b155</a> [docs] remove unnecessary import from router docs (#24869)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/30a430ac2ec9e346b99e92b57840ad7ee29a297f">30a430a</a> Revert &quot;Revert &quot;[build-properties] Support modifying &lt;queries&gt; tag in android manifest (#24619)&quot;&quot;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/248319fac2e24e9c0b4d63fbf53e3466cb9cd71b">248319f</a> Revert &quot;[build-properties] Support modifying &lt;queries&gt; tag in android manifest (#24619)&quot;</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/fe399504a43df191399bde7c84151f1982026c84">fe39950</a> [core] fix shared object exception for thread issues (#24836)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/995844a20418c1d341f38809ca857e049efc4677">995844a</a> [android][ios] Upgrade react-native-webview to 13.6.2 (#24850)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/64705e7f25ccd329343f056feca9901e3d12205b">64705e7</a> Update @ react-native-picker/picker to 2.5.1 (#24839)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/954cc4a6dd4d0458c441782578f09fc22ce54f9c">954cc4a</a> [actions] remove &#x27;need review&#x27; label if an issue is accepted (#24855)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/2740dee1a618e0e5c5ffd66a0cbe3c873b932ed9">2740dee</a> [build-properties] Support modifying &lt;queries&gt; tag in android manifest (#24619)</li>
      <li><a href="https://snyk.io/redirect/github/expo/expo/commit/05fecad5d0d1ccbb9b50411dde4f477b9dd1312f">05fecad</a> commit yarn.lock</li>
    </ul>

   <a href="https://snyk.io/redirect/github/expo/expo/compare/0d774d352ca6d11f83a3223199c8e5f6ba4c8e09...da25937e2a99661cbe5eb60ca1d8d6245fc96a50">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiIyMGM5N2YxNi0wYjg5LTRlMjEtYTk5Ni1jYTFjMDU0MWU3YTQiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjIwYzk3ZjE2LTBiODktNGUyMS1hOTk2LWNhMWMwNTQxZTdhNCJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3/settings/integration?pkg&#x3D;expo-splash-screen&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"20c97f16-0b89-4e21-a996-ca1c0541e7a4","prPublicId":"20c97f16-0b89-4e21-a996-ca1c0541e7a4","dependencies":[{"name":"expo-splash-screen","from":"0.20.5","to":"0.24.0"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/adcadd64-fca2-41e4-9476-aa9d33532df3?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"adcadd64-fca2-41e4-9476-aa9d33532df3","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":6,"publishedDate":"2023-10-17T20:27:52.531Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 17:00:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Address SNYK warnings
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
        Created At 2023-11-22 14:15:35 +0000 UTC
    </div>
</div>

