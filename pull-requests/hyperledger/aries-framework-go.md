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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3473" class=".btn">#3473</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Holder: Add Holder Binding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Holder MAY add an optional JWT to prove Holder Binding to the Verifier. Nonce and aud claims are included to show that the proof is intended for the Verifier.

Closes #3470

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 22:55:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3472" class=".btn">#3472</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Issuer: Add Holder Public Key Claim (JWK)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the Issuer wants to enable Holder Binding, it MAY include a public key associated with the Holder, or a reference thereto.

We use confirmation "cnf" claim to include raw public key by value in SD-JWT.

In this first iteration of "cnf" claim we will use "jwk" confirmation method and include public key information in JWK format. Other confirmation methods such as "jwe", "kid" and "jku" may be implemented at later time (if required).

Closes #3469 

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 18:57:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3468" class=".btn">#3468</a>
            </td>
            <td>
                <b>
                    fix: Presentation Without Holder Binding should end with ~
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: Presentation Without Holder Binding should end with ~

Also, rename SDJWT to CombinedPresentation and JWTSerialized to SDJWT to follow spec terms.

And add parsing and serializing of combined presentation parts with holder binding. 

Holder Binding functionality will be added in separate PRs. 

Closes #3467

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 20:53:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3466" class=".btn">#3466</a>
            </td>
            <td>
                <b>
                    feat: Add decoy digests to SD-JWT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add decoy digests to SD-JWT (if enabled)

Closes #3463

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 18:27:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3465" class=".btn">#3465</a>
            </td>
            <td>
                <b>
                    fix: disable JSON-LD validation on JWT credentials
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
        Created At 2023-01-09 15:50:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3464" class=".btn">#3464</a>
            </td>
            <td>
                <b>
                    chore(deps): bump json5 from 1.0.1 to 1.0.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 1.0.1 to 1.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v1.0.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>). This has been backported to v1. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/298">#298</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>Unreleased [<a href="https://github.com/json5/json5/tree/main">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.3...HEAD">diff</a>]</h3>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/a62db1e51e1031d92ac260f5bb38bbed1fdbc754"><code>a62db1e</code></a> 1.0.2</li>
<li><a href="https://github.com/json5/json5/commit/e0c23fe458a77c0b2cdb271376be5d8d0908133c"><code>e0c23fe</code></a> docs: update CHANGELOG for v1.0.2</li>
<li><a href="https://github.com/json5/json5/commit/62a65408408d40aeea14c7869ed327acead12972"><code>62a6540</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li>See full diff in <a href="https://github.com/json5/json5/compare/v1.0.1...v1.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=1.0.1&new-version=1.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-07 14:27:56 +0000 UTC
    </div>
</div>

