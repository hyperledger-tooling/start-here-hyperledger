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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3134" class=".btn">#3134</a>
            </td>
            <td>
                <b>
                    Add option to enable remote document loading for mobile bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when enabled, documents that are not available locally will be fetch remotely for mobile bindings.

Does replace pull request #3053.

Signed-off-by: Michel Sahli <michel.sahli@adnovum.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 11:30:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3133" class=".btn">#3133</a>
            </td>
            <td>
                <b>
                    test: WACI Issuance BDD tests for Go SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 01:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3132" class=".btn">#3132</a>
            </td>
            <td>
                <b>
                    feat: add pthid to the didcomm v2 message replying to an oobv2 invitation
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
        Created At 2022-01-19 21:39:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3131" class=".btn">#3131</a>
            </td>
            <td>
                <b>
                    fix: smooth out behaviour of version-agnostic didcomm models
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
        Created At 2022-01-19 06:36:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3130" class=".btn">#3130</a>
            </td>
            <td>
                <b>
                    feat: Export Credential Manifest and Output Descriptor validate methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reworked the existing Credential Manifest and Output Descriptor validation methods so that they can be called directly outside of the cm package without requiring json.Unmarshal to be called. This gives callers more flexibility and supports more use cases.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 21:23:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3129" class=".btn">#3129</a>
            </td>
            <td>
                <b>
                    feat: credential manifest resolve - support for arbitrary type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Part of #3092

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 03:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3128" class=".btn">#3128</a>
            </td>
            <td>
                <b>
                    chore(deps): bump follow-redirects from 1.14.4 to 1.14.7 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.4 to 1.14.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/6f5029ae1a0fdab4dc25f6379a5ee303c2319070"><code>6f5029a</code></a> Release version 1.14.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/af706bee57de954414c0bde0a9f33e62beea3e52"><code>af706be</code></a> Ignore null headers.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d01ab7a5c5df3617c7a40a03de7af6427fdfac55"><code>d01ab7a</code></a> Release version 1.14.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/40052ea8aa13559becee5795715c1d45b1f0eb76"><code>40052ea</code></a> Make compatible with Node 17.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/86f7572f9365dadc39f85916259b58973819617f"><code>86f7572</code></a> Fix: clear internal timer on request abort to avoid leakage</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2e1eaf0218c5315a2ab27f53964d0535d4dafb51"><code>2e1eaf0</code></a> Keep Authorization header on subdomain redirects.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ad9e82b6277ae2104f7770e9ff1186cc6da29d4"><code>2ad9e82</code></a> Carry over Host header on relative redirects (<a href="https://github-redirect.dependabot.com/follow-redirects/follow-redirects/issues/172">#172</a>)</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.4...v1.14.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.4&new-version=1.14.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-14 05:14:15 +0000 UTC
    </div>
</div>

