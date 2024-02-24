---
layout: default
title: aries-mediator-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mediator-service
---

# aries-mediator-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mediator-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 42.0.2 to 42.0.4 in /multi-agent-load-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.2 to 42.0.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.4 - 2024-02-20</p>
<pre><code>
* Fixed a null-pointer-dereference and segfault that could occur when creating
  a PKCS#12 bundle. Credit to **Alexander-Programming** for reporting the
  issue. **CVE-2024-26130**
* Fixed ASN.1 encoding for PKCS7/SMIME signed messages. The fields ``SMIMECapabilities``
  and ``SignatureAlgorithmIdentifier`` should now be correctly encoded according to the
  definitions in :rfc:`2633` :rfc:`3370`.
<p>.. _v42-0-3:</p>
<p>42.0.3 - 2024-02-15
</code></pre></p>
<ul>
<li>Fixed an initialization issue that caused key loading failures for some
users.</li>
</ul>
<p>.. _v42-0-2:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/fe18470f7d05f963e7267e34fdf985d81ea6ceea"><code>fe18470</code></a> Bump for 42.0.4 release (<a href="https://redirect.github.com/pyca/cryptography/issues/10445">#10445</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/aaa2dd06ed470695de818405a982d4c459869803"><code>aaa2dd0</code></a> Fix ASN.1 issues in PKCS#7 and S/MIME signing (<a href="https://redirect.github.com/pyca/cryptography/issues/10373">#10373</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10442">#10442</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/7a4d012991061974da5d9cb7614de65eac94f49b"><code>7a4d012</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10422">#10422</a> -- don't crash when a PKCS#12 key and cert don't match (<a href="https://redirect.github.com/pyca/cryptography/issues/10423">#10423</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/df314bb182bdfd661333969a94325e4680d785f6"><code>df314bb</code></a> backport actions m1 switch to 42.0.x (<a href="https://redirect.github.com/pyca/cryptography/issues/10415">#10415</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/c49a7a5271178c6e8ef36fa1c499f62c63ec19b9"><code>c49a7a5</code></a> changelog and version bump for 42.0.3 (<a href="https://redirect.github.com/pyca/cryptography/issues/10396">#10396</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/396bcf64c5be826ec00e7d7f45838c858c049cbc"><code>396bcf6</code></a> fix provider loading take two (<a href="https://redirect.github.com/pyca/cryptography/issues/10390">#10390</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10395">#10395</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0e0e46f5f73f477b8ee9682738c42129d5d60177"><code>0e0e46f</code></a> backport: initialize openssl's legacy provider in rust (<a href="https://redirect.github.com/pyca/cryptography/issues/10323">#10323</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10333">#10333</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.2...42.0.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.2&new-version=42.0.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 20:45:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    build(deps): bump ip from 2.0.0 to 2.0.1 in /afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ip](https://github.com/indutny/node-ip) from 2.0.0 to 2.0.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/indutny/node-ip/commit/3b0994a74eca51df01f08c40d6a65ba0e1845d04"><code>3b0994a</code></a> 2.0.1</li>
<li><a href="https://github.com/indutny/node-ip/commit/32f468f1245574785ec080705737a579be1223aa"><code>32f468f</code></a> lib: fixed CVE-2023-42282 and added unit test</li>
<li>See full diff in <a href="https://github.com/indutny/node-ip/compare/v2.0.0...v2.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ip&package-manager=npm_and_yarn&previous-version=2.0.0&new-version=2.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 21:32:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    build(deps): bump ip from 2.0.0 to 2.0.1 in /load-testing/load-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ip](https://github.com/indutny/node-ip) from 2.0.0 to 2.0.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/indutny/node-ip/commit/3b0994a74eca51df01f08c40d6a65ba0e1845d04"><code>3b0994a</code></a> 2.0.1</li>
<li><a href="https://github.com/indutny/node-ip/commit/32f468f1245574785ec080705737a579be1223aa"><code>32f468f</code></a> lib: fixed CVE-2023-42282 and added unit test</li>
<li>See full diff in <a href="https://github.com/indutny/node-ip/compare/v2.0.0...v2.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ip&package-manager=npm_and_yarn&previous-version=2.0.0&new-version=2.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 21:13:37 +0000 UTC
    </div>
</div>

