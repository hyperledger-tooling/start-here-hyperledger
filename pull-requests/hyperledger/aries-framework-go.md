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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3163" class=".btn">#3163</a>
            </td>
            <td>
                <b>
                    chore(deps): bump follow-redirects from 1.14.4 to 1.14.8 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.4 to 1.14.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/3d81dc3237b4ffe8b722bb3d1c70a7866657166e"><code>3d81dc3</code></a> Release version 1.14.8 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/62e546a99c07c3ee5e4e0718c84a6ca127c5c445"><code>62e546a</code></a> Drop confidential headers across schemes.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/6f5029ae1a0fdab4dc25f6379a5ee303c2319070"><code>6f5029a</code></a> Release version 1.14.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/af706bee57de954414c0bde0a9f33e62beea3e52"><code>af706be</code></a> Ignore null headers.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d01ab7a5c5df3617c7a40a03de7af6427fdfac55"><code>d01ab7a</code></a> Release version 1.14.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/40052ea8aa13559becee5795715c1d45b1f0eb76"><code>40052ea</code></a> Make compatible with Node 17.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/86f7572f9365dadc39f85916259b58973819617f"><code>86f7572</code></a> Fix: clear internal timer on request abort to avoid leakage</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2e1eaf0218c5315a2ab27f53964d0535d4dafb51"><code>2e1eaf0</code></a> Keep Authorization header on subdomain redirects.</li>
<li>Additional commits viewable in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.4...v1.14.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.4&new-version=1.14.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-13 07:02:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3162" class=".btn">#3162</a>
            </td>
            <td>
                <b>
                    chore(deps): bump ajv from 6.11.0 to 6.12.6 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ajv](https://github.com/ajv-validator/ajv) from 6.11.0 to 6.12.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ajv-validator/ajv/releases">ajv's releases</a>.</em></p>
<blockquote>
<h2>v6.12.6</h2>
<p>Fix performance issue of &quot;url&quot; format.</p>
<h2>v6.12.5</h2>
<p>Fix uri scheme validation (<a href="https://github.com/ChALkeR"><code>@​ChALkeR</code></a>).
Fix boolean schemas with strictKeywords option (<a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1270">#1270</a>)</p>
<h2>v6.12.4</h2>
<p>Fix: coercion of one-item arrays to scalar that should fail validation (<a href="https://runkit.com/esp/5f3672ba2f6642001ae27411">failing example</a>).</p>
<h2>v6.12.3</h2>
<p>Pass schema object to processCode function
Option for strictNumbers (<a href="https://github.com/issacgerges"><code>@​issacgerges</code></a>, <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1128">#1128</a>)
Fixed vulnerability related to untrusted schemas (<a href="https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=CVE-2020-15366">CVE-2020-15366</a>)</p>
<h2>v6.12.2</h2>
<p>Removed post-install script</p>
<h2>v6.12.1</h2>
<p>Docs and dependency updates</p>
<h2>v6.12.0</h2>
<p>Improved hostname validation (<a href="https://github.com/sambauers"><code>@​sambauers</code></a>, <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1143">#1143</a>)
Option <code>keywords</code> to add custom keywords (<a href="https://github.com/franciscomorais"><code>@​franciscomorais</code></a>, <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1137">#1137</a>)
Types fixes (<a href="https://github.com/boenrobot"><code>@​boenrobot</code></a>, <a href="https://github.com/MattiAstedrone"><code>@​MattiAstedrone</code></a>)
Docs:</p>
<ul>
<li><a href="https://github.com/epoberezkin/ajv#error-logging">error logging</a> example (<a href="https://github.com/RadiationSickness"><code>@​RadiationSickness</code></a>)</li>
<li>TypeScript usage notes (<a href="https://github.com/thetric"><code>@​thetric</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ajv-validator/ajv/commit/fe591439f34e24030f69df9eb8d91e6d037a3af7"><code>fe59143</code></a> 6.12.6</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/d580d3e8ac6a467670d68d86e3a39fd661ac8c23"><code>d580d3e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1298">#1298</a> from ajv-validator/fix-url</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/fd363896a8d6c5697b5da41f4d9a400a84efaf8e"><code>fd36389</code></a> fix: regular expression for &quot;url&quot; format</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/490e34c4846064db5c962a77087e17078954c2f6"><code>490e34c</code></a> docs: link to v7-beta branch</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/9cd93a1bdbdefd5a7ba3db5e123d20c84d1d1d0e"><code>9cd93a1</code></a> docs: note about v7 in readme</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/877d286e7f145b1b2127da66c6800b071533f28f"><code>877d286</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/ajv-validator/ajv/issues/1262">#1262</a> from b4h0-c4t/refactor-opt-object-type</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/f1c8e45b9cdff918be28becf03bf0b339321c398"><code>f1c8e45</code></a> 6.12.5</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/764035e201d7733b8d700d4a04dd079fef9f4d30"><code>764035e</code></a> Merge branch 'ChALkeR-chalker/fix-comma'</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/37981602ce6d43313ae106644b372b021626a8af"><code>3798160</code></a> Merge branch 'chalker/fix-comma' of git://github.com/ChALkeR/ajv into ChALkeR...</li>
<li><a href="https://github.com/ajv-validator/ajv/commit/a3c7ebab222e4cce07b5e30ebcbb809da7f934e8"><code>a3c7eba</code></a> Merge branch 'refactor-opt-object-type' of github.com:b4h0-c4t/ajv into refac...</li>
<li>Additional commits viewable in <a href="https://github.com/ajv-validator/ajv/compare/v6.11.0...v6.12.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ajv&package-manager=npm_and_yarn&previous-version=6.11.0&new-version=6.12.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-13 00:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3161" class=".btn">#3161</a>
            </td>
            <td>
                <b>
                    fix: webredirect info in Problem Report V2
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
        Created At 2022-02-11 19:22:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3160" class=".btn">#3160</a>
            </td>
            <td>
                <b>
                    fix: add present-proof webredirect v2 properties to Done/Abandoned state props
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
        Created At 2022-02-11 19:08:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3159" class=".btn">#3159</a>
            </td>
            <td>
                <b>
                    add content type to webhook request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Webhook message has no content type

**Description:**
Add the content type to the request header in webhook
 Issue: https://github.com/hyperledger/aries-framework-go/issues/3158

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 11:49:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3157" class=".btn">#3157</a>
            </td>
            <td>
                <b>
                    fix: use thread id for present-proof PIID, except in problem report
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
        Created At 2022-02-09 19:34:37 +0000 UTC
    </div>
</div>

