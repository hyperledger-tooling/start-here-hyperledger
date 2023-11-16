---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/560" class=".btn">#560</a>
            </td>
            <td>
                <b>
                    Add gather version button
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
Adds a new button under the `settings` tab. it will generate a json file of all component versions, operator fabric versions, and the console version. this is useful for support.

![image](https://github.com/hyperledger-labs/fabric-operations-console/assets/16085295/908daaa8-5503-41df-ab8c-21fa27291dbe)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 18:17:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/559" class=".btn">#559</a>
            </td>
            <td>
                <b>
                    Bump axios from 1.1.3 to 1.6.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.1.3 to 1.6.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
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
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
<h2>Release v1.5.1</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>adapters:</strong> improved adapters loading logic to have clear error messages; (<a href="https://redirect.github.com/axios/axios/issues/5919">#5919</a>) (<a href="https://github.com/axios/axios/commit/e4107797a7a1376f6209fbecfbbce73d3faa7859">e410779</a>)</li>
<li><strong>formdata:</strong> fixed automatic addition of the <code>Content-Type</code> header for FormData in non-browser environments; (<a href="https://redirect.github.com/axios/axios/issues/5917">#5917</a>) (<a href="https://github.com/axios/axios/commit/bc9af51b1886d1b3529617702f2a21a6c0ed5d92">bc9af51</a>)</li>
<li><strong>headers:</strong> allow <code>content-encoding</code> header to handle case-insensitive values (<a href="https://redirect.github.com/axios/axios/issues/5890">#5890</a>) (<a href="https://redirect.github.com/axios/axios/issues/5892">#5892</a>) (<a href="https://github.com/axios/axios/commit/4c89f25196525e90a6e75eda9cb31ae0a2e18acd">4c89f25</a>)</li>
<li><strong>types:</strong> removed duplicated code (<a href="https://github.com/axios/axios/commit/9e6205630e1c9cf863adf141c0edb9e6d8d4b149">9e62056</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+89/-18 ([#5919](https://github.com/axios/axios/issues/5919) [#5917](https://github.com/axios/axios/issues/5917) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/DavidJDallas" title="+11/-5 ()">David Dallas</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/fb-sean" title="+2/-8 ()">Sean Sattler</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/0o001" title="+4/-4 ()">Mustafa Ateş Uzun</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/sfc-gh-pmotacki" title="+2/-1 ([#5892](https://github.com/axios/axios/issues/5892) )">Przemyslaw Motacki</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/Cadienvan" title="+1/-1 ()">Michael Di Prisco</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
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
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
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
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.5.0...v1.5.1">1.5.1</a> (2023-09-26)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>adapters:</strong> improved adapters loading logic to have clear error messages; (<a href="https://redirect.github.com/axios/axios/issues/5919">#5919</a>) (<a href="https://github.com/axios/axios/commit/e4107797a7a1376f6209fbecfbbce73d3faa7859">e410779</a>)</li>
<li><strong>formdata:</strong> fixed automatic addition of the <code>Content-Type</code> header for FormData in non-browser environments; (<a href="https://redirect.github.com/axios/axios/issues/5917">#5917</a>) (<a href="https://github.com/axios/axios/commit/bc9af51b1886d1b3529617702f2a21a6c0ed5d92">bc9af51</a>)</li>
<li><strong>headers:</strong> allow <code>content-encoding</code> header to handle case-insensitive values (<a href="https://redirect.github.com/axios/axios/issues/5890">#5890</a>) (<a href="https://redirect.github.com/axios/axios/issues/5892">#5892</a>) (<a href="https://github.com/axios/axios/commit/4c89f25196525e90a6e75eda9cb31ae0a2e18acd">4c89f25</a>)</li>
<li><strong>types:</strong> removed duplicated code (<a href="https://github.com/axios/axios/commit/9e6205630e1c9cf863adf141c0edb9e6d8d4b149">9e62056</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+89/-18 ([#5919](https://github.com/axios/axios/issues/5919) [#5917](https://github.com/axios/axios/issues/5917) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/DavidJDallas" title="+11/-5 ()">David Dallas</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/fb-sean" title="+2/-8 ()">Sean Sattler</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f6d2cf9763bfa124f15c2dc6a5d5d5d9d3e26169"><code>f6d2cf9</code></a> chore(ci): fix publish action content permission; (<a href="https://redirect.github.com/axios/axios/issues/6061">#6061</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a22f4b918a71a4d4caa57ff23d8247eac93765de"><code>a22f4b9</code></a> chore(release): v1.6.1 (<a href="https://redirect.github.com/axios/axios/issues/6060">#6060</a>)</li>
<li><a href="https://github.com/axios/axios/commit/cb8bb2beb215a94a29f19b0d66ab05d32b390230"><code>cb8bb2b</code></a> chore(ci): Publish to NPM with provenance (<a href="https://redirect.github.com/axios/axios/issues/5835">#5835</a>)</li>
<li><a href="https://github.com/axios/axios/commit/37cbf9214a1140d25c2c1a5ff097666c96721d6a"><code>37cbf92</code></a> chore(ci): added labeling and notification for published PRs; (<a href="https://redirect.github.com/axios/axios/issues/6059">#6059</a>)</li>
<li><a href="https://github.com/axios/axios/commit/dd465ab22bbfa262c6567be6574bf46a057d5288"><code>dd465ab</code></a> fix(formdata): fixed content-type header normalization for non-standard brows...</li>
<li><a href="https://github.com/axios/axios/commit/3dc8369e505e32a4e12c22f154c55fd63ac67fbb"><code>3dc8369</code></a> fix(platform): fixed emulated browser detection in node.js environment; (<a href="https://redirect.github.com/axios/axios/issues/6055">#6055</a>)</li>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v1.1.3...v1.6.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.1.3&new-version=1.6.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-11 07:54:42 +0000 UTC
    </div>
</div>

