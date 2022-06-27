---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jsrsasign from 10.5.24 to 10.5.25 in /opssc-api-server/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsrsasign](https://github.com/kjur/jsrsasign) from 10.5.24 to 10.5.25.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/releases">jsrsasign's releases</a>.</em></p>
<blockquote>
<h2>CVE-2022-25898 Security fix in JWS and JWT validation</h2>
<ul>
<li>Changes from 10.5.24 to 10.5.25 (2022-Jun-23)
<ul>
<li>src/jws.js
<ul>
<li>JWS.verify and JWS.verifyJWT
<ul>
<li>CVE-2022-25898 SECURITY FIX:
verify and verifyJWT may accept signature with special characters
or \number characters by mistake.
Please see security advisory:
<a href="https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf">https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf</a></li>
</ul>
</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function isBase64URLDot added</li>
</ul>
</li>
<li>test/qunit-do-jwt-veri.html</li>
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
<p>CVE-2022-25898 Security fix in JWS and JWT validation</p>
<ul>
<li>Changes from 10.5.24 to 10.5.25 (2022-Jun-23)
<ul>
<li>src/jws.js
<ul>
<li>JWS.verify and JWS.verifyJWT
<ul>
<li>CVE-2022-25898 SECURITY FIX:
verify and verifyJWT may accept signature with special characters
or \number characters by mistake.
Please see security advisory:
<a href="https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf">https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf</a></li>
</ul>
</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function isBase64URLDot added</li>
</ul>
</li>
<li>test/qunit-do-jwt-veri.html</li>
</ul>
</li>
</ul>
<p>X509.getParam bugfix for v1 certificate</p>
<ul>
<li>Changes from 10.5.23 to 10.5.24 (2022-Jun-04)
<ul>
<li>src/x509.js
<ul>
<li>X509.getParam bugfix for X.509v1 certificate without extension</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>BitString parsing bug fix</p>
<ul>
<li>Changes from 10.5.22 to 10.5.23 (2022-May-27)
<ul>
<li>src/base64x.js
<ul>
<li>bitstrtobinstr bugfix fix</li>
</ul>
</li>
<li>src/asn1hex.js
<ul>
<li>ASN1HEX.parse change for bin string range</li>
</ul>
</li>
<li>npm/lib/footers.js
<ul>
<li>add missed exports (bitstrtobinstr, binstrtobitstr,
namearraytobinstr, extendClass)</li>
</ul>
</li>
<li>test/qunit-do-{asn1hex-parse,base64x}.html
<ul>
<li>add and fix some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>DERBitString, KeyUsage and  tsp PKIFailureInfo critical bug fix</p>
<ul>
<li>Changes from 10.5.21 to 10.5.22 (2022-May-24)
<ul>
<li>src/asn1.js
<ul>
<li>DERBitString critical bugfix</li>
</ul>
</li>
<li>src/asn1tsp.js
<ul>
<li>PKIFailureInfo critical bugfix</li>
</ul>
</li>
<li>src/asn1x509.js
<ul>
<li>KeyUsage critical bugfix</li>
</ul>
</li>
<li>src/base64.x
<ul>
<li>namearraytobinstr critical bugfix</li>
</ul>
</li>
<li>test/qunit-do-{asn1,asn1tsp,asn1x509,base64x}.html
<ul>
<li>add and fix some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>DERBitString, KeyUsage and  tsp PKIFailureInfo fix</p>
<ul>
<li>Changes from 10.5.20 to 10.5.21 (2022-May-23) <em>RELEASE RESIGNED</em>
<ul>
<li>src/asn1x509.js
<ul>
<li>KeyUsage bugfix, refactoring</li>
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
<li><a href="https://github.com/kjur/jsrsasign/commit/4536a6e9e8bcf1a644ab7c07ed96e453347dae41"><code>4536a6e</code></a> CVE-2022-25898 Security fix in JWS and JWT validation</li>
<li>See full diff in <a href="https://github.com/kjur/jsrsasign/compare/10.5.24...10.5.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsrsasign&package-manager=npm_and_yarn&previous-version=10.5.24&new-version=10.5.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 07:28:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jsrsasign from 10.5.24 to 10.5.25 in /opssc-agent/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsrsasign](https://github.com/kjur/jsrsasign) from 10.5.24 to 10.5.25.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/releases">jsrsasign's releases</a>.</em></p>
<blockquote>
<h2>CVE-2022-25898 Security fix in JWS and JWT validation</h2>
<ul>
<li>Changes from 10.5.24 to 10.5.25 (2022-Jun-23)
<ul>
<li>src/jws.js
<ul>
<li>JWS.verify and JWS.verifyJWT
<ul>
<li>CVE-2022-25898 SECURITY FIX:
verify and verifyJWT may accept signature with special characters
or \number characters by mistake.
Please see security advisory:
<a href="https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf">https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf</a></li>
</ul>
</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function isBase64URLDot added</li>
</ul>
</li>
<li>test/qunit-do-jwt-veri.html</li>
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
<p>CVE-2022-25898 Security fix in JWS and JWT validation</p>
<ul>
<li>Changes from 10.5.24 to 10.5.25 (2022-Jun-23)
<ul>
<li>src/jws.js
<ul>
<li>JWS.verify and JWS.verifyJWT
<ul>
<li>CVE-2022-25898 SECURITY FIX:
verify and verifyJWT may accept signature with special characters
or \number characters by mistake.
Please see security advisory:
<a href="https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf">https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf</a></li>
</ul>
</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function isBase64URLDot added</li>
</ul>
</li>
<li>test/qunit-do-jwt-veri.html</li>
</ul>
</li>
</ul>
<p>X509.getParam bugfix for v1 certificate</p>
<ul>
<li>Changes from 10.5.23 to 10.5.24 (2022-Jun-04)
<ul>
<li>src/x509.js
<ul>
<li>X509.getParam bugfix for X.509v1 certificate without extension</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>BitString parsing bug fix</p>
<ul>
<li>Changes from 10.5.22 to 10.5.23 (2022-May-27)
<ul>
<li>src/base64x.js
<ul>
<li>bitstrtobinstr bugfix fix</li>
</ul>
</li>
<li>src/asn1hex.js
<ul>
<li>ASN1HEX.parse change for bin string range</li>
</ul>
</li>
<li>npm/lib/footers.js
<ul>
<li>add missed exports (bitstrtobinstr, binstrtobitstr,
namearraytobinstr, extendClass)</li>
</ul>
</li>
<li>test/qunit-do-{asn1hex-parse,base64x}.html
<ul>
<li>add and fix some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>DERBitString, KeyUsage and  tsp PKIFailureInfo critical bug fix</p>
<ul>
<li>Changes from 10.5.21 to 10.5.22 (2022-May-24)
<ul>
<li>src/asn1.js
<ul>
<li>DERBitString critical bugfix</li>
</ul>
</li>
<li>src/asn1tsp.js
<ul>
<li>PKIFailureInfo critical bugfix</li>
</ul>
</li>
<li>src/asn1x509.js
<ul>
<li>KeyUsage critical bugfix</li>
</ul>
</li>
<li>src/base64.x
<ul>
<li>namearraytobinstr critical bugfix</li>
</ul>
</li>
<li>test/qunit-do-{asn1,asn1tsp,asn1x509,base64x}.html
<ul>
<li>add and fix some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>DERBitString, KeyUsage and  tsp PKIFailureInfo fix</p>
<ul>
<li>Changes from 10.5.20 to 10.5.21 (2022-May-23) <em>RELEASE RESIGNED</em>
<ul>
<li>src/asn1x509.js
<ul>
<li>KeyUsage bugfix, refactoring</li>
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
<li><a href="https://github.com/kjur/jsrsasign/commit/4536a6e9e8bcf1a644ab7c07ed96e453347dae41"><code>4536a6e</code></a> CVE-2022-25898 Security fix in JWS and JWT validation</li>
<li>See full diff in <a href="https://github.com/kjur/jsrsasign/compare/10.5.24...10.5.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsrsasign&package-manager=npm_and_yarn&previous-version=10.5.24&new-version=10.5.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 07:27:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jsrsasign from 10.5.24 to 10.5.25 in /common/src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsrsasign](https://github.com/kjur/jsrsasign) from 10.5.24 to 10.5.25.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/releases">jsrsasign's releases</a>.</em></p>
<blockquote>
<h2>CVE-2022-25898 Security fix in JWS and JWT validation</h2>
<ul>
<li>Changes from 10.5.24 to 10.5.25 (2022-Jun-23)
<ul>
<li>src/jws.js
<ul>
<li>JWS.verify and JWS.verifyJWT
<ul>
<li>CVE-2022-25898 SECURITY FIX:
verify and verifyJWT may accept signature with special characters
or \number characters by mistake.
Please see security advisory:
<a href="https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf">https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf</a></li>
</ul>
</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function isBase64URLDot added</li>
</ul>
</li>
<li>test/qunit-do-jwt-veri.html</li>
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
<p>CVE-2022-25898 Security fix in JWS and JWT validation</p>
<ul>
<li>Changes from 10.5.24 to 10.5.25 (2022-Jun-23)
<ul>
<li>src/jws.js
<ul>
<li>JWS.verify and JWS.verifyJWT
<ul>
<li>CVE-2022-25898 SECURITY FIX:
verify and verifyJWT may accept signature with special characters
or \number characters by mistake.
Please see security advisory:
<a href="https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf">https://github.com/kjur/jsrsasign/security/advisories/GHSA-3fvg-4v2m-98jf</a></li>
</ul>
</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function isBase64URLDot added</li>
</ul>
</li>
<li>test/qunit-do-jwt-veri.html</li>
</ul>
</li>
</ul>
<p>X509.getParam bugfix for v1 certificate</p>
<ul>
<li>Changes from 10.5.23 to 10.5.24 (2022-Jun-04)
<ul>
<li>src/x509.js
<ul>
<li>X509.getParam bugfix for X.509v1 certificate without extension</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>BitString parsing bug fix</p>
<ul>
<li>Changes from 10.5.22 to 10.5.23 (2022-May-27)
<ul>
<li>src/base64x.js
<ul>
<li>bitstrtobinstr bugfix fix</li>
</ul>
</li>
<li>src/asn1hex.js
<ul>
<li>ASN1HEX.parse change for bin string range</li>
</ul>
</li>
<li>npm/lib/footers.js
<ul>
<li>add missed exports (bitstrtobinstr, binstrtobitstr,
namearraytobinstr, extendClass)</li>
</ul>
</li>
<li>test/qunit-do-{asn1hex-parse,base64x}.html
<ul>
<li>add and fix some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>DERBitString, KeyUsage and  tsp PKIFailureInfo critical bug fix</p>
<ul>
<li>Changes from 10.5.21 to 10.5.22 (2022-May-24)
<ul>
<li>src/asn1.js
<ul>
<li>DERBitString critical bugfix</li>
</ul>
</li>
<li>src/asn1tsp.js
<ul>
<li>PKIFailureInfo critical bugfix</li>
</ul>
</li>
<li>src/asn1x509.js
<ul>
<li>KeyUsage critical bugfix</li>
</ul>
</li>
<li>src/base64.x
<ul>
<li>namearraytobinstr critical bugfix</li>
</ul>
</li>
<li>test/qunit-do-{asn1,asn1tsp,asn1x509,base64x}.html
<ul>
<li>add and fix some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>DERBitString, KeyUsage and  tsp PKIFailureInfo fix</p>
<ul>
<li>Changes from 10.5.20 to 10.5.21 (2022-May-23) <em>RELEASE RESIGNED</em>
<ul>
<li>src/asn1x509.js
<ul>
<li>KeyUsage bugfix, refactoring</li>
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
<li><a href="https://github.com/kjur/jsrsasign/commit/4536a6e9e8bcf1a644ab7c07ed96e453347dae41"><code>4536a6e</code></a> CVE-2022-25898 Security fix in JWS and JWT validation</li>
<li>See full diff in <a href="https://github.com/kjur/jsrsasign/compare/10.5.24...10.5.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsrsasign&package-manager=npm_and_yarn&previous-version=10.5.24&new-version=10.5.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-opssc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 07:27:30 +0000 UTC
    </div>
</div>

