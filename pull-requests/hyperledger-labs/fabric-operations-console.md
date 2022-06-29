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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    fix msp import if there are no intermediate_certs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes an error when importing a MSP json file with no `intermediate_certs` field. This field can be blank or missing and the import should still succeed.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 18:17:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    Bump jsrsasign from 10.2.0 to 10.5.25 in /packages/athena
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jsrsasign](https://github.com/kjur/jsrsasign) from 10.2.0 to 10.5.25.
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
<h2>OCSP ResponderID object udpate</h2>
<ul>
<li>Changes from 10.5.19 to 10.5.20 (2022-Apr-25)
<ul>
<li>src/asn1ocsp.js
<ul>
<li>ResponderID class now also supports PEM certificate or
X509 object for key and name field.</li>
</ul>
</li>
<li>test/qunit-do-asn1ocsp.html
<ul>
<li>add some test cases and fix for above</li>
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
<li><a href="https://github.com/kjur/jsrsasign/commit/3edc0070846922daea98d9588978e91d855577ec"><code>3edc007</code></a> 10.5.24 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/f6b7916b551ff9962d6148f9a2a7720b144bb795"><code>f6b7916</code></a> 10.5.23 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/2613c64559768b91dde9793dfa318feacb7c3b8a"><code>2613c64</code></a> 10.5.22 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/4274a59818983958d9eb7b58d37eee98f823689b"><code>4274a59</code></a> 10.5.21 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/f11615a8c78b7cedabe00653948fadf65328261c"><code>f11615a</code></a> ResponderID API doc update</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/5efa282c82d1a34d8f6126eca60bb4c3416b1d01"><code>5efa282</code></a> 10.5.20 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/041564e2cb9ea0d0909467c2e9e88cd2c252c9dc"><code>041564e</code></a> 10.5.19 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/751ee07a30e77be9737476b79f8120a65b20f5eb"><code>751ee07</code></a> 10.5.18 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/52d2b5528d1174d0ee7ad591cb853d37874e98dd"><code>52d2b55</code></a> 10.5.17 release</li>
<li>Additional commits viewable in <a href="https://github.com/kjur/jsrsasign/compare/10.2.0...10.5.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsrsasign&package-manager=npm_and_yarn&previous-version=10.2.0&new-version=10.5.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 07:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    warn about consenter issues when removing a systemless OSN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
- when removing an ordering node that is not using a system channel, warn if its a consenter and prevent the delete unless the user overrides it.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 21:42:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    add ability to append ordering node to systemless
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
- Added the ability to append ordering nodes to an existing cluster that are * not * using a system channel.
- This also introduces some performance improvements by eliminating some redundant apis/spam


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 18:41:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Bump got from 11.8.2 to 11.8.5 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) from 11.8.2 to 11.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v11.8.5</h2>
<ul>
<li>Backport security fix <a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc">https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc</a>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5">https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5</a></p>
<h2>v11.8.3</h2>
<ul>
<li>Bump cacheable-request dependency (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1921">#1921</a>)  9463bb6</li>
<li>Fix <code>HTTPError</code> missing <code>.code</code> property (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1739">#1739</a>)  0e167b8</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.2...v11.8.3">https://github.com/sindresorhus/got/compare/v11.8.2...v11.8.3</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/5e17bb748c260b02e4cf716c2f4079a1c6a7481e"><code>5e17bb7</code></a> 11.8.5</li>
<li><a href="https://github.com/sindresorhus/got/commit/bce8ce7d528a675bd5a8d996e110b73674e290d2"><code>bce8ce7</code></a> Backport 861ccd9ac2237df762a9e2beed7edd88c60782dc</li>
<li><a href="https://github.com/sindresorhus/got/commit/8ced19215603f3eda25a9f5dce390f1b152fe9a3"><code>8ced192</code></a> Fix build</li>
<li><a href="https://github.com/sindresorhus/got/commit/670eb04b5b01622f489277d6fb1dd04a41d3cb51"><code>670eb04</code></a> 11.8.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/20f29fe3726a4ddd104f557456dbd5275685e879"><code>20f29fe</code></a> Backport <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1543">#1543</a>: Initialize globalResponse in case of ignored HTTPError (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2017">#2017</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/0da732f4650c398f3b2fea672f8916e6c7004c8f"><code>0da732f</code></a> 11.8.3</li>
<li><a href="https://github.com/sindresorhus/got/commit/9463bb696d4ee909970e3fc609ee40b7644e3f6c"><code>9463bb6</code></a> Bump cacheable-request dependency (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1921">#1921</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/0e167b8b9505a7e9e4a4bbe39e9baeb1f5c4a1fd"><code>0e167b8</code></a> HTTPError code set to 'HTTPError' <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1711">#1711</a> (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1739">#1739</a>)</li>
<li>See full diff in <a href="https://github.com/sindresorhus/got/compare/v11.8.2...v11.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=got&package-manager=npm_and_yarn&previous-version=11.8.2&new-version=11.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 08:31:37 +0000 UTC
    </div>
</div>

