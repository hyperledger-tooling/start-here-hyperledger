---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    get code up to date
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
        Created At 2022-10-24 16:56:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    Bump jsrsasign from 10.5.20 to 10.5.25
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsrsasign](https://github.com/kjur/jsrsasign) from 10.5.20 to 10.5.25.
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
<h2>X509.getParam bugfix for v1 certificate</h2>
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
<h2>BitString parsing bug fix</h2>
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
<h2>DERBitString, KeyUsage and  tsp PKIFailureInfo critical bug fix</h2>
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
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/blob/master/ChangeLog.txt">jsrsasign's changelog</a>.</em></p>
<blockquote>
<p>ChangeLog for jsrsasign</p>
<p>extend CertificationRequestInfo class for challengePassword and unstructuredName</p>
<ul>
<li>Changes from 10.5.26 to 10.5.27 (2022-Aug-19)
<ul>
<li>src/asn1csr.js
<ul>
<li>CertificationRequestInfo class
<ul>
<li>add support for challengePassword and unstructuredName (<a href="https://github-redirect.dependabot.com/kjur/jsrsasign/issues/522">#522</a>)</li>
<li>&quot;attrs&quot; member support in constructure argument</li>
</ul>
</li>
</ul>
</li>
<li>test/qunit-do-asn1csr.html</li>
</ul>
</li>
</ul>
<p>CSRUtil class enhancement</p>
<ul>
<li>Changes from 10.5.25 to 10.5.26 (2022-Jul-14)
<ul>
<li>src/asn1csr.js
<ul>
<li>CSRUtil.verifySignature method added</li>
<li>CSRUtil.getParam enhanced to support optional argument flagTBS</li>
</ul>
</li>
<li>test/qunit-do-asn1csr.html
<ul>
<li>update some test cases for above</li>
</ul>
</li>
</ul>
</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjur/jsrsasign/commit/4536a6e9e8bcf1a644ab7c07ed96e453347dae41"><code>4536a6e</code></a> CVE-2022-25898 Security fix in JWS and JWT validation</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/3edc0070846922daea98d9588978e91d855577ec"><code>3edc007</code></a> 10.5.24 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/f6b7916b551ff9962d6148f9a2a7720b144bb795"><code>f6b7916</code></a> 10.5.23 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/2613c64559768b91dde9793dfa318feacb7c3b8a"><code>2613c64</code></a> 10.5.22 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/4274a59818983958d9eb7b58d37eee98f823689b"><code>4274a59</code></a> 10.5.21 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/f11615a8c78b7cedabe00653948fadf65328261c"><code>f11615a</code></a> ResponderID API doc update</li>
<li>See full diff in <a href="https://github.com/kjur/jsrsasign/compare/10.5.20...10.5.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsrsasign&package-manager=npm_and_yarn&previous-version=10.5.20&new-version=10.5.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 21:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    update code, encrypt wallet private key when stored in database
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
        Created At 2022-10-18 20:59:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Added deployment steps for besu network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: adityajoshi12 <adityaprakashjoshi1@gmail.com>

**Changes**
- Added steps and network configuration for deploying besu network using bevel

**Linked Issue**
#631  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 06:32:29 +0000 UTC
    </div>
</div>

