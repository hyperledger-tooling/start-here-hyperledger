---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Upgrade fastapi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrade fastapi for security issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 22:35:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Update dev container docker-in-docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Was getting dev container crashes. I think related to poetry upgrade but not entirely sure. 

This is an update config.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 22:13:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 41.0.7 to 42.0.0 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 41.0.7 to 42.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.0 - 2024-01-22</p>
<pre><code>
* **BACKWARDS INCOMPATIBLE:** Dropped support for LibreSSL &lt; 3.7.
* **BACKWARDS INCOMPATIBLE:** Loading a PKCS7 with no content field using
  :func:`~cryptography.hazmat.primitives.serialization.pkcs7.load_pem_pkcs7_certificates`
  or
  :func:`~cryptography.hazmat.primitives.serialization.pkcs7.load_der_pkcs7_certificates`
  will now raise a ``ValueError`` rather than return an empty list.
* Parsing SSH certificates no longer permits malformed critical options with
  values, as documented in the 41.0.2 release notes.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.0.
* Updated the minimum supported Rust version (MSRV) to 1.63.0, from 1.56.0.
* We now publish both ``py37`` and ``py39`` ``abi3`` wheels. This should
  resolve some errors relating to initializing a module multiple times per
  process.
* Support :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS` for
  X.509 certificate signing requests and certificate revocation lists with the
  keyword-only argument ``rsa_padding`` on the ``sign`` methods for
  :class:`~cryptography.x509.CertificateSigningRequestBuilder` and
  :class:`~cryptography.x509.CertificateRevocationListBuilder`.
* Added support for obtaining X.509 certificate signing request signature
  algorithm parameters (including PSS) via
  :meth:`~cryptography.x509.CertificateSigningRequest.signature_algorithm_parameters`.
* Added support for obtaining X.509 certificate revocation list signature
  algorithm parameters (including PSS) via
  :meth:`~cryptography.x509.CertificateRevocationList.signature_algorithm_parameters`.
* Added ``mgf`` property to
  :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`.
* Added ``algorithm`` and ``mgf`` properties to
  :class:`~cryptography.hazmat.primitives.asymmetric.padding.OAEP`.
* Added the following properties that return timezone-aware ``datetime`` objects:
  :meth:`~cryptography.x509.Certificate.not_valid_before_utc`,
  :meth:`~cryptography.x509.Certificate.not_valid_after_utc`,
  :meth:`~cryptography.x509.RevokedCertificate.revocation_date_utc`,
  :meth:`~cryptography.x509.CertificateRevocationList.next_update_utc`,
  :meth:`~cryptography.x509.CertificateRevocationList.last_update_utc`.
  These are timezone-aware variants of existing properties that return naïve
  ``datetime`` objects.
* Deprecated the following properties that return naïve ``datetime`` objects:
  :meth:`~cryptography.x509.Certificate.not_valid_before`,
  :meth:`~cryptography.x509.Certificate.not_valid_after`,
  :meth:`~cryptography.x509.RevokedCertificate.revocation_date`,
  :meth:`~cryptography.x509.CertificateRevocationList.next_update`,
  :meth:`~cryptography.x509.CertificateRevocationList.last_update`
  in favor of the new timezone-aware variants mentioned above.
* Added support for
  :class:`~cryptography.hazmat.primitives.ciphers.algorithms.ChaCha20`
  on LibreSSL.
* Added support for RSA PSS signatures in PKCS7 with
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/4e64baf360a3a89bd92582f59344c12b5c0bd3fd"><code>4e64baf</code></a> 42.0.0 version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10232">#10232</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/7cb13a3bc91b7537c6231674fb5b0d2132a7edbe"><code>7cb13a3</code></a> we'll ship 3.2.0 for 42 (<a href="https://redirect.github.com/pyca/cryptography/issues/9951">#9951</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/605c74e41c75edc717f21afaa5e6a0eee9863a10"><code>605c74e</code></a> Bump x509-limbo and/or wycheproof in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10231">#10231</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/97578b98ffc417864e07d0ff9b76c02d2cb4e6da"><code>97578b9</code></a> Bump BoringSSL and/or OpenSSL in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10230">#10230</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/972a7b5896a6047ea43a86db87820ab474d898ff"><code>972a7b5</code></a> verification: add test_verify_tz_aware (<a href="https://redirect.github.com/pyca/cryptography/issues/10229">#10229</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/41daf2d86dd9bf18081802fa5d851a7953810786"><code>41daf2d</code></a> Migrate PKCS7 backend to Rust (<a href="https://redirect.github.com/pyca/cryptography/issues/10228">#10228</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/d54093e62e7e68c02efbb4d6a09162ddb39bf72f"><code>d54093e</code></a> Remove some skips in tests that aren't needed anymore (<a href="https://redirect.github.com/pyca/cryptography/issues/10223">#10223</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/71929bd91f34213b9f4a3a0a493c218c35fa25eb"><code>71929bd</code></a> Remove binding that's not used anymore (<a href="https://redirect.github.com/pyca/cryptography/issues/10224">#10224</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/7ea4b89cea553ce0f641ed29e1ce2e3e34278f1d"><code>7ea4b89</code></a> fixed formatting in changelog (<a href="https://redirect.github.com/pyca/cryptography/issues/10225">#10225</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/410f4a1ee4cbf46fe7e969bb48fccf261f74bbcd"><code>410f4a1</code></a> Allow brainpool on libressl (<a href="https://redirect.github.com/pyca/cryptography/issues/10222">#10222</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pyca/cryptography/compare/41.0.7...42.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=41.0.7&new-version=42.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 19:14:03 +0000 UTC
    </div>
</div>

