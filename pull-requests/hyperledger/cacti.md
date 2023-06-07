---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2443" class=".btn">#2443</a>
            </td>
            <td>
                <b>
                    chore(besu): remove web3-eea typings file 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes hyperledger#1218

Signed-off-by: micoferdinand98 <ferdinand.m.b.mico@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 07:36:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2442" class=".btn">#2442</a>
            </td>
            <td>
                <b>
                    test: fix path of and name of RIFUtil.test.ts #1515
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed name of `RIFUtil.test.ts` to `rifUtil.test.ts` and moved the file to unit test directory.

fixes: #1515
Signed-off-by: Arnab Nandi <arnabnandi2002@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-03 08:01:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2441" class=".btn">#2441</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 39.0.1 to 41.0.0 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 39.0.1 to 41.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.0 - 2023-05-30</p>
<pre><code>
* **BACKWARDS INCOMPATIBLE:** Support for OpenSSL less than 1.1.1d has been
  removed.  Users on older version of OpenSSL will need to upgrade.
* **BACKWARDS INCOMPATIBLE:** Support for Python 3.6 has been removed.
* **BACKWARDS INCOMPATIBLE:** Dropped support for LibreSSL &lt; 3.6.
* Updated the minimum supported Rust version (MSRV) to 1.56.0, from 1.48.0.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.1.
* Added support for the :class:`~cryptography.x509.OCSPAcceptableResponses`
  OCSP extension.
* Added support for the :class:`~cryptography.x509.MSCertificateTemplate`
  proprietary Microsoft certificate extension.
* Implemented support for equality checks on all asymmetric public key types.
* Added support for ``aes256-gcm@openssh.com`` encrypted keys in
  :func:`~cryptography.hazmat.primitives.serialization.load_ssh_private_key`.
* Added support for obtaining X.509 certificate signature algorithm parameters
  (including PSS) via
  :meth:`~cryptography.x509.Certificate.signature_algorithm_parameters`.
* Support signing :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`
  X.509 certificates via the new keyword-only argument ``rsa_padding`` on
  :meth:`~cryptography.x509.CertificateBuilder.sign`.
* Added support for
  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`
  on BoringSSL.
<p>.. _v40-0-2:</p>
<p>40.0.2 - 2023-04-14
</code></pre></p>
<ul>
<li>Fixed compilation when using LibreSSL 3.7.2.</li>
<li>Added some functions to support an upcoming <code>pyOpenSSL</code> release.</li>
</ul>
<p>.. _v40-0-1:</p>
<p>40.0.1 - 2023-03-24</p>
<pre><code>
* Fixed a bug where certain operations would fail if an object happened to be
  in the top-half of the memory-space. This only impacted 32-bit systems.
<p>.. _v40-0-0:</p>
<p>40.0.0 - 2023-03-24
</code></pre></p>
<ul>
<li><strong>BACKWARDS INCOMPATIBLE:</strong> As announced in the 39.0.0 changelog, the way
<code>cryptography</code> links OpenSSL has changed. This only impacts users who</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/c4d494fd3ee907316bd846e90cbf4a8df75a25ac"><code>c4d494f</code></a> 41.0.0 version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/8991">#8991</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8708245ccdeaff21d65eea68a4f8d2a7c5949a22"><code>8708245</code></a> new openssl day (<a href="https://redirect.github.com/pyca/cryptography/issues/8990">#8990</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/31436a486661cd863d4c77e40facf93fbb2d9f54"><code>31436a4</code></a> admit to the existence of nuance in HKDF (<a href="https://redirect.github.com/pyca/cryptography/issues/8987">#8987</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/91e41898e6d1d2a9a6e980c39e2f8baa2fa8a1f8"><code>91e4189</code></a> Port DSA to Rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8978">#8978</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f302d28b81607aab28d22b653da78d564824f267"><code>f302d28</code></a> Update CI for new LibreSSL releases (<a href="https://redirect.github.com/pyca/cryptography/issues/8975">#8975</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/851d8ccb340bfc93c827b9e80af939a216b34925"><code>851d8cc</code></a> Bump openssl from 0.10.52 to 0.10.53 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8986">#8986</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0918c7236c94c29272e0790ba0227cfa9401943b"><code>0918c72</code></a> Bump coverage from 7.2.6 to 7.2.7 (<a href="https://redirect.github.com/pyca/cryptography/issues/8985">#8985</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/730a5ce11a91f40c1bb0f881ab22bc52d6cecef6"><code>730a5ce</code></a> Bump openssl-sys from 0.9.87 to 0.9.88 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8984">#8984</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/88e8c288975709228005e70301644034463d9823"><code>88e8c28</code></a> Bump BoringSSL and/or OpenSSL in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/8983">#8983</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/3e24e44527a69884ca0c3247e1b5e9c8bbf590c9"><code>3e24e44</code></a> Bump once_cell from 1.17.1 to 1.17.2 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8982">#8982</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pyca/cryptography/compare/39.0.1...41.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=39.0.1&new-version=41.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 20:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 39.0.1 to 41.0.0 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 39.0.1 to 41.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.0 - 2023-05-30</p>
<pre><code>
* **BACKWARDS INCOMPATIBLE:** Support for OpenSSL less than 1.1.1d has been
  removed.  Users on older version of OpenSSL will need to upgrade.
* **BACKWARDS INCOMPATIBLE:** Support for Python 3.6 has been removed.
* **BACKWARDS INCOMPATIBLE:** Dropped support for LibreSSL &lt; 3.6.
* Updated the minimum supported Rust version (MSRV) to 1.56.0, from 1.48.0.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.1.
* Added support for the :class:`~cryptography.x509.OCSPAcceptableResponses`
  OCSP extension.
* Added support for the :class:`~cryptography.x509.MSCertificateTemplate`
  proprietary Microsoft certificate extension.
* Implemented support for equality checks on all asymmetric public key types.
* Added support for ``aes256-gcm@openssh.com`` encrypted keys in
  :func:`~cryptography.hazmat.primitives.serialization.load_ssh_private_key`.
* Added support for obtaining X.509 certificate signature algorithm parameters
  (including PSS) via
  :meth:`~cryptography.x509.Certificate.signature_algorithm_parameters`.
* Support signing :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`
  X.509 certificates via the new keyword-only argument ``rsa_padding`` on
  :meth:`~cryptography.x509.CertificateBuilder.sign`.
* Added support for
  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`
  on BoringSSL.
<p>.. _v40-0-2:</p>
<p>40.0.2 - 2023-04-14
</code></pre></p>
<ul>
<li>Fixed compilation when using LibreSSL 3.7.2.</li>
<li>Added some functions to support an upcoming <code>pyOpenSSL</code> release.</li>
</ul>
<p>.. _v40-0-1:</p>
<p>40.0.1 - 2023-03-24</p>
<pre><code>
* Fixed a bug where certain operations would fail if an object happened to be
  in the top-half of the memory-space. This only impacted 32-bit systems.
<p>.. _v40-0-0:</p>
<p>40.0.0 - 2023-03-24
</code></pre></p>
<ul>
<li><strong>BACKWARDS INCOMPATIBLE:</strong> As announced in the 39.0.0 changelog, the way
<code>cryptography</code> links OpenSSL has changed. This only impacts users who</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/c4d494fd3ee907316bd846e90cbf4a8df75a25ac"><code>c4d494f</code></a> 41.0.0 version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/8991">#8991</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8708245ccdeaff21d65eea68a4f8d2a7c5949a22"><code>8708245</code></a> new openssl day (<a href="https://redirect.github.com/pyca/cryptography/issues/8990">#8990</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/31436a486661cd863d4c77e40facf93fbb2d9f54"><code>31436a4</code></a> admit to the existence of nuance in HKDF (<a href="https://redirect.github.com/pyca/cryptography/issues/8987">#8987</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/91e41898e6d1d2a9a6e980c39e2f8baa2fa8a1f8"><code>91e4189</code></a> Port DSA to Rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8978">#8978</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f302d28b81607aab28d22b653da78d564824f267"><code>f302d28</code></a> Update CI for new LibreSSL releases (<a href="https://redirect.github.com/pyca/cryptography/issues/8975">#8975</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/851d8ccb340bfc93c827b9e80af939a216b34925"><code>851d8cc</code></a> Bump openssl from 0.10.52 to 0.10.53 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8986">#8986</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0918c7236c94c29272e0790ba0227cfa9401943b"><code>0918c72</code></a> Bump coverage from 7.2.6 to 7.2.7 (<a href="https://redirect.github.com/pyca/cryptography/issues/8985">#8985</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/730a5ce11a91f40c1bb0f881ab22bc52d6cecef6"><code>730a5ce</code></a> Bump openssl-sys from 0.9.87 to 0.9.88 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8984">#8984</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/88e8c288975709228005e70301644034463d9823"><code>88e8c28</code></a> Bump BoringSSL and/or OpenSSL in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/8983">#8983</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/3e24e44527a69884ca0c3247e1b5e9c8bbf590c9"><code>3e24e44</code></a> Bump once_cell from 1.17.1 to 1.17.2 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8982">#8982</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pyca/cryptography/compare/39.0.1...41.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=39.0.1&new-version=41.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 20:18:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2439" class=".btn">#2439</a>
            </td>
            <td>
                <b>
                    style: changes made for fixing #1357
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                submitting fixes for issue #1357 minus the linter warning ID 79 and 80 as they have been already solved in batch 9 #1478.
I have added types of variables and objects wherever necessary in place of 'any' and for packages/cactus-common/src/test/typescript/unit/logging/logger.test.ts I have declared a interface for prototyping the stdOutDataHandler function.

fixes #1357
Signed-off-by: Arnab Nandi arnabnandi2002@gmail.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 15:22:24 +0000 UTC
    </div>
</div>

