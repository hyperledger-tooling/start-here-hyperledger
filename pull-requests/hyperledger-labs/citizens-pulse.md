---
layout: default
title: citizens-pulse
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/citizens-pulse
---

# citizens-pulse <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/citizens-pulse){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/citizens-pulse/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Bump node-forge from 0.9.1 to 1.3.0 in /network/sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [node-forge](https://github.com/digitalbazaar/forge) from 0.9.1 to 1.3.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/digitalbazaar/forge/blob/main/CHANGELOG.md">node-forge's changelog</a>.</em></p>
<blockquote>
<h2>1.3.0 - 2022-03-17</h2>
<h3>Security</h3>
<ul>
<li>Three RSA PKCS#1 v1.5 signature verification issues were reported by Moosa
Yahyazadeh (<a href="mailto:moosa-yahyazadeh@uiowa.edu">moosa-yahyazadeh@uiowa.edu</a>).</li>
<li><strong>HIGH</strong>: Leniency in checking <code>digestAlgorithm</code> structure can lead to
signature forgery.
<ul>
<li>The code is lenient in checking the digest algorithm structure. This can
allow a crafted structure that steals padding bytes and uses unchecked
portion of the PKCS#1 encoded message to forge a signature when a low
public exponent is being used. For more information, please see
<a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24771">CVE-2022-24771</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-cfm4-qjh2-4765">GHSA-cfm4-qjh2-4765</a></li>
</ul>
</li>
<li><strong>HIGH</strong>: Failing to check tailing garbage bytes can lead to signature
forgery.
<ul>
<li>The code does not check for tailing garbage bytes after decoding a
<code>DigestInfo</code> ASN.1 structure. This can allow padding bytes to be removed
and garbage data added to forge a signature when a low public exponent is
being used.  For more information, please see <a href="https://mailarchive.ietf.org/arch/msg/openpgp/5rnE9ZRN1AokBVj3VqblGlP63QE/">&quot;Bleichenbacher's RSA
signature forgery based on implementation
error&quot;</a>
by Hal Finney.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24772">CVE-2022-24772</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-x4jg-mjrx-434g">GHSA-x4jg-mjrx-434g</a></li>
</ul>
</li>
<li><strong>MEDIUM</strong>: Leniency in checking type octet.
<ul>
<li><code>DigestInfo</code> is not properly checked for proper ASN.1 structure. This can
lead to successful verification with signatures that contain invalid
structures but a valid digest.</li>
<li>CVE ID: <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24773">CVE-2022-24773</a></li>
<li>GHSA ID: <a href="https://github.com/digitalbazaar/forge/security/advisories/GHSA-2r2c-g63r-vccr">GHSA-2r2c-g63r-vccr</a></li>
</ul>
</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>[asn1] Add fallback to pretty print invalid UTF8 data.</li>
<li>[asn1] <code>fromDer</code> is now more strict and will default to ensuring all input
bytes are parsed or throw an error. A new option <code>parseAllBytes</code> can disable
this behavior.
<ul>
<li><strong>NOTE</strong>: The previous behavior is being changed since it can lead to
security issues with crafted inputs. It is possible that code doing custom
DER parsing may need to adapt to this new behavior and optional flag.</li>
</ul>
</li>
<li>[rsa] Add and use a validator to check for proper structure of parsed ASN.1
<code>RSASSA-PKCS-v1_5</code> <code>DigestInfo</code> data. Additionally check that the hash
algorithm identifier is a known value from RFC 8017
<code>PKCS1-v1-5DigestAlgorithms</code>. An invalid <code>DigestInfo</code> or algorithm identifier
will now throw an error.
<ul>
<li><strong>NOTE</strong>: The previous lenient behavior is being changed to be more strict
since it could lead to security issues with crafted inputs. It is possible
that code may have to handle the errors from these stricter checks.</li>
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
<li><a href="https://github.com/digitalbazaar/forge/commit/6c5b90133d46af63d139b98bf65371732c8c7dad"><code>6c5b901</code></a> Release 1.3.0.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/0f3972ad5883a9869703c6f54a0627bc454bca47"><code>0f3972a</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/dc77b39dd347e7f8b60a0f25a311fe5f06130579"><code>dc77b39</code></a> Fix error checking.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/bb822c02df0b61211836472e29b9790cc541cdb2"><code>bb822c0</code></a> Add advisory links.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/d4395fec831622837ecfec9e428d4620e208f9a8"><code>d4395fe</code></a> Update changelog.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/a4405bb9d6b638084df478fa4ac60a410332c2d8"><code>a4405bb</code></a> Improve signature verification tests.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/aa9372d6dd78eb1479392b9274457036c2404b66"><code>aa9372d</code></a> Add missing RFC 8017 algorithm identifiers.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/3f0b49a0573ef1bb7af7f5673c0cfebf00424df1"><code>3f0b49a</code></a> Fix signature verification issues.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/c20f309311d83445e11abe7c313cc4b467c18914"><code>c20f309</code></a> Adjust remaining length.</li>
<li><a href="https://github.com/digitalbazaar/forge/commit/e27f61230f19fb9f085a163f31d0573305271b84"><code>e27f612</code></a> Remove unused option.</li>
<li>Additional commits viewable in <a href="https://github.com/digitalbazaar/forge/compare/0.9.1...v1.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-forge&package-manager=npm_and_yarn&previous-version=0.9.1&new-version=1.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/citizens-pulse/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 11:13:40 +0000 UTC
    </div>
</div>

