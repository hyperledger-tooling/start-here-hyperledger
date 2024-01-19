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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/591" class=".btn">#591</a>
            </td>
            <td>
                <b>
                    Bump jsrsasign from 10.5.25 to 11.0.0 in /packages/athena
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsrsasign](https://github.com/kjur/jsrsasign) from 10.5.25 to 11.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjur/jsrsasign/releases">jsrsasign's releases</a>.</em></p>
<blockquote>
<h2>remove RSA and RSAOAEP encryption for Marvin attack</h2>
<ul>
<li>Changes from 10.9.0 to 11.0.0 (2024-Jan-16)
<ul>
<li>remove RSA PKCS#1.5 end OAEP encryption/decryption for Marvin attack (<a href="https://redirect.github.com/kjur/jsrsasign/issues/598">#598</a>)</li>
<li>src/crypto.js
<ul>
<li>remove KJUR.crypto.Cipher class for RSA and RSAOAEP encryption/decryption</li>
</ul>
</li>
<li>ext/{rsa,rsa2}.js
remove encrypt/decrypt/encryptOAEP/decryptOAEP for RSAKey class</li>
</ul>
</li>
</ul>
<h2>enhanced support for encrypted PKCS8</h2>
<ul>
<li>Changes from 10.8.6 to 10.9.0 (2023-Nov-27)
<ul>
<li>KEYUTIL.getPEM is updated not to use weak ciphers (<a href="https://redirect.github.com/kjur/jsrsasign/issues/599">#599</a>)
<ul>
<li>default encryptionScheme is changed from des-EDE3-CBC to aes256-CBC</li>
<li>default prf is changed from hmacWithSHA1 to hmacWithSHA256</li>
</ul>
</li>
<li>src/keyutil.js
<ul>
<li>more encrypted PKCS#8 private key support
<ul>
<li>KEYUTIL.getKey now supports encrypted PKCS#8 private key with
aes128-CBC, aes256-CBC encrypted and using hmacWithSHA224/256/384/512 as
psudorandom function.</li>
<li>KEYUTIL.getPEM now supports such as above encrypted PKCS#8 PEM
priavte key.</li>
</ul>
</li>
</ul>
</li>
<li>src/crypto.js
<ul>
<li>Cipher.decrypt/encrypt now supports symmetric ciphers (des-EDE3-CBC,aes128-CBC,aes256-CBC)</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function inttohex and twoscompl are added</li>
</ul>
</li>
<li>src/asn1.js
<ul>
<li>ASN1Util.bigIntToMinTwosComplementsHex is now DEPRECATED. use twoscompl.</li>
</ul>
</li>
<li>src/asn1x509.js
<ul>
<li>aes*-CBC and hmacWithSHA* OIDs are added</li>
</ul>
</li>
<li>test/qunit-do-{base64x,crypto-cipher,keyutil-eprv,keyutil,keyutil-p8egen}.html
<ul>
<li>update and add some test cases for above</li>
</ul>
</li>
<li>stop bower support (bower.json removed)</li>
</ul>
</li>
</ul>
<h2>X509.getExtSubjectDirectoryAttributes another bugfix</h2>
<ul>
<li>Changes from 10.8.5 to 10.8.6 (2023-Apr-26)
<ul>
<li>src/x509.js
<ul>
<li>another bugfix X509.getExtSubjectDirectoryAttributes method</li>
</ul>
</li>
</ul>
</li>
</ul>
<h2>X509.getExtSubjectDirectoryAttributes bugfix</h2>
<ul>
<li>Changes from 10.8.4 to 10.8.5 (2023-Apr-26)
<ul>
<li>src/x509.js
<ul>
<li>bugfix X509.getExtSubjectDirectoryAttributes method</li>
</ul>
</li>
</ul>
</li>
</ul>
<h2>more SubjectDirectoryExtension support</h2>
<ul>
<li>Changes from 10.8.3 to 10.8.4 (2023-Apr-26)
<ul>
<li>src/asn1x509.js
<ul>
<li>SubjectDirectoryAttributes class
<ul>
<li>add array of array support for arbitrary attribute value</li>
</ul>
</li>
</ul>
</li>
<li>src/x509.js
<ul>
<li>add X509.getExtSubjectDirectoryAttributes method for
ExtSubjectDirectoryAttributes extension</li>
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
<p>remove RSA and RSAOAEP encryption for Marvin attack</p>
<ul>
<li>Changes from 10.9.0 to 11.0.0 (2024-Jan-16)
<ul>
<li>remove RSA PKCS#1.5 end OAEP encryption/decryption for Marvin attack (<a href="https://redirect.github.com/kjur/jsrsasign/issues/598">#598</a>)</li>
<li>src/crypto.js
<ul>
<li>remove KJUR.crypto.Cipher class for RSA and RSAOAEP encryption/decryption</li>
</ul>
</li>
<li>ext/{rsa,rsa2}.js
remove encrypt/decrypt/encryptOAEP/decryptOAEP for RSAKey class</li>
</ul>
</li>
</ul>
<p>enhanced support for encrypted PKCS8</p>
<ul>
<li>Changes from 10.8.6 to 10.9.0 (2023-Nov-27)
<ul>
<li>KEYUTIL.getPEM is updated not to use weak ciphers (<a href="https://redirect.github.com/kjur/jsrsasign/issues/599">#599</a>)
<ul>
<li>default encryptionScheme is changed from des-EDE3-CBC to aes256-CBC</li>
<li>default prf is changed from hmacWithSHA1 to hmacWithSHA256</li>
</ul>
</li>
<li>src/keyutil.js
<ul>
<li>more encrypted PKCS#8 private key support
<ul>
<li>KEYUTIL.getKey now supports encrypted PKCS#8 private key with
aes128-CBC, aes256-CBC encrypted and using hmacWithSHA224/256/384/512 as
psudorandom function.</li>
<li>KEYUTIL.getPEM now supports such as above encrypted PKCS#8 PEM
priavte key.</li>
</ul>
</li>
</ul>
</li>
<li>src/crypto.js
<ul>
<li>Cipher.decrypt/encrypt now supports symmetric ciphers (des-EDE3-CBC,aes128-CBC,aes256-CBC)</li>
</ul>
</li>
<li>src/base64x.js
<ul>
<li>function inttohex and twoscompl are added</li>
</ul>
</li>
<li>src/asn1.js
<ul>
<li>ASN1Util.bigIntToMinTwosComplementsHex is now DEPRECATED. use twoscompl.</li>
</ul>
</li>
<li>src/asn1x509.js
<ul>
<li>aes*-CBC and hmacWithSHA* OIDs are added</li>
</ul>
</li>
<li>test/qunit-do-{base64x,crypto-cipher,keyutil-eprv,keyutil,keyutil-p8egen}.html
<ul>
<li>update and add some test cases for above</li>
</ul>
</li>
<li>stop bower support (bower.json removed)</li>
</ul>
</li>
</ul>
<p>X509.getExtSubjectDirectoryAttributes another bugfix</p>
<ul>
<li>Changes from 10.8.5 to 10.8.6 (2023-Apr-26)
<ul>
<li>src/x509.js
<ul>
<li>another bugfix X509.getExtSubjectDirectoryAttributes method</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>X509.getExtSubjectDirectoryAttributes bugfix</p>
<ul>
<li>Changes from 10.8.4 to 10.8.5 (2023-Apr-26)
<ul>
<li>src/x509.js
<ul>
<li>bugfix X509.getExtSubjectDirectoryAttributes method</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>more SubjectDirectoryExtension support</p>
<ul>
<li>Changes from 10.8.3 to 10.8.4 (2023-Apr-26)
<ul>
<li>src/asn1x509.js
<ul>
<li>SubjectDirectoryAttributes class
<ul>
<li>add array of array support for arbitrary attribute value</li>
</ul>
</li>
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
<li><a href="https://github.com/kjur/jsrsasign/commit/d73befc129a1a344fa7dc3f672a9b813528fb197"><code>d73befc</code></a> 11.0.0 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/32f73aff77ecf4fdbccbd503dee380bc9cfb0473"><code>32f73af</code></a> update jsdoc</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/df54d0b291fafda9d0bc65d1d38feb63a40dc0c3"><code>df54d0b</code></a> enhanced support for encrypted PKCS8</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/59920c4a502ac1b8eb35d7a0bcad205f63a1884b"><code>59920c4</code></a> 10.8.6 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/c195be81ed5b751affc563a5b784dbc97bcad79d"><code>c195be8</code></a> 10.8.5 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/04af7f528399b06e78f612700a332fde8adffc64"><code>04af7f5</code></a> 10.8.4 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/d679050bb81bfbddea314571f1be5b7b555b4788"><code>d679050</code></a> 10.8.3 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/97921fb2a0a0e1acafadf1a8247e3d6ace1ceeaa"><code>97921fb</code></a> 10.8.2 release</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/d332357a78332ab7e1758ba28fe42123b712dd8b"><code>d332357</code></a> Merge pull request <a href="https://redirect.github.com/kjur/jsrsasign/issues/583">#583</a> from davedoesdev/master</li>
<li><a href="https://github.com/kjur/jsrsasign/commit/1cfd9394429b23bd2d00b484a62e0072037b606c"><code>1cfd939</code></a> Fix OAEP padding</li>
<li>Additional commits viewable in <a href="https://github.com/kjur/jsrsasign/compare/10.5.25...11.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsrsasign&package-manager=npm_and_yarn&previous-version=10.5.25&new-version=11.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-01-19 15:07:40 +0000 UTC
    </div>
</div>

