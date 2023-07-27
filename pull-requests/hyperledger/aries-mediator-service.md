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
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    build(deps): bump flask from 2.3.1 to 2.3.2 in /multi-agent-load-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [flask](https://github.com/pallets/flask) from 2.3.1 to 2.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/flask/releases">flask's releases</a>.</em></p>
<blockquote>
<h2>2.3.2</h2>
<p>This is a security fix release for the 2.3.x release branch.</p>
<ul>
<li>Security advisory: <a href="https://github.com/pallets/flask/security/advisories/GHSA-m2qf-hxjv-5gpq">https://github.com/pallets/flask/security/advisories/GHSA-m2qf-hxjv-5gpq</a>, CVE-2023-30861</li>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-2">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/29?closed=1">https://github.com/pallets/flask/milestone/29?closed=1</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/flask/blob/main/CHANGES.rst">flask's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.3.2</h2>
<p>Released 2023-05-01</p>
<ul>
<li>Set <code>Vary: Cookie</code> header when the session is accessed, modified, or refreshed.</li>
<li>Update Werkzeug requirement to &gt;=2.3.3 to apply recent bug fixes.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/flask/commit/f3b8f570545200c87465d18386f3fc9f2258307a"><code>f3b8f57</code></a> release version 2.3.2</li>
<li><a href="https://github.com/pallets/flask/commit/c990bba94ab9bc81adf2d33e83c9a9628a2098f2"><code>c990bba</code></a> update min test env</li>
<li><a href="https://github.com/pallets/flask/commit/adedb2a64ea7703369bc89021710b439ee79f8dc"><code>adedb2a</code></a> Merge pull request <a href="https://redirect.github.com/pallets/flask/issues/5101">#5101</a> from pallets/update-werkzeug</li>
<li><a href="https://github.com/pallets/flask/commit/e1aedecdc689cc9a79131851dbdabf6c3bc49c9e"><code>e1aedec</code></a> update werkzeug</li>
<li><a href="https://github.com/pallets/flask/commit/37badc3ce8b0665e3454547839196a676729309f"><code>37badc3</code></a> update changelog</li>
<li><a href="https://github.com/pallets/flask/commit/70f906c51ce49c485f1d355703e9cc3386b1cc2b"><code>70f906c</code></a> Merge pull request from GHSA-m2qf-hxjv-5gpq</li>
<li><a href="https://github.com/pallets/flask/commit/8705dd39c4fa563ea0fe0bf84c85da8fcc98b88d"><code>8705dd3</code></a> set <code>Vary: Cookie</code> header consistently for session</li>
<li><a href="https://github.com/pallets/flask/commit/9532cba45d2339e90ebf04f178b1e4f2064e7328"><code>9532cba</code></a> fix mypy finding</li>
<li><a href="https://github.com/pallets/flask/commit/0bc7356ce1ae11e633426902aba76d525f4523da"><code>0bc7356</code></a> start version 2.3.2</li>
<li><a href="https://github.com/pallets/flask/commit/f07fb2b607c1eaa724ca9bfe43e2dc20d97d34de"><code>f07fb2b</code></a> Merge pull request <a href="https://redirect.github.com/pallets/flask/issues/5086">#5086</a> from pallets/release-2.3.1</li>
<li>See full diff in <a href="https://github.com/pallets/flask/compare/2.3.1...2.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=flask&package-manager=pip&previous-version=2.3.1&new-version=2.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 15:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/90" class=".btn">#90</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 40.0.2 to 41.0.2 in /multi-agent-load-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 40.0.2 to 41.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.2 - 2023-07-10</p>
<pre><code>
* Fixed bugs in creating and parsing SSH certificates where critical options
  with values were handled incorrectly. Certificates are now created correctly
  and parsing accepts correct values as well as the previously generated
  invalid forms with a warning. In the next release, support for parsing these
  invalid forms will be removed.
<p>.. _v41-0-1:</p>
<p>41.0.1 - 2023-06-01
</code></pre></p>
<ul>
<li>Temporarily allow invalid ECDSA signature algorithm parameters in X.509
certificates, which are generated by older versions of Java.</li>
<li>Allow null bytes in pass phrases when serializing private keys.</li>
</ul>
<p>.. _v41-0-0:</p>
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
<p>.. _v40-0-2:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/7431db737cf0407560fac689d24f1d2e5efc349d"><code>7431db7</code></a> bump for 41.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/9215">#9215</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/e190ef190525999d1f599cf8c3aef5cb7f3a8bc4"><code>e190ef1</code></a> Backport ssh cert fix (<a href="https://redirect.github.com/pyca/cryptography/issues/9211">#9211</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/bb204c8ca7bc0df0c24b6f6c1f59ed5f5bee9226"><code>bb204c8</code></a> Backport: Added PyPy 3.10 to CI (<a href="https://redirect.github.com/pyca/cryptography/issues/8933">#8933</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/9210">#9210</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/d02de9f26e9a2353e89427c1cea8b9ed2bae969e"><code>d02de9f</code></a> changelog and version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/9008">#9008</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/53dc686431f59658d892b83383a330d796105843"><code>53dc686</code></a> Backport null fix (<a href="https://redirect.github.com/pyca/cryptography/issues/9007">#9007</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/b99900596e65f31543d62cf1a52069c709ba7970"><code>b999005</code></a> Backport tolerate (<a href="https://redirect.github.com/pyca/cryptography/issues/9006">#9006</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/c4d494fd3ee907316bd846e90cbf4a8df75a25ac"><code>c4d494f</code></a> 41.0.0 version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/8991">#8991</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8708245ccdeaff21d65eea68a4f8d2a7c5949a22"><code>8708245</code></a> new openssl day (<a href="https://redirect.github.com/pyca/cryptography/issues/8990">#8990</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/31436a486661cd863d4c77e40facf93fbb2d9f54"><code>31436a4</code></a> admit to the existence of nuance in HKDF (<a href="https://redirect.github.com/pyca/cryptography/issues/8987">#8987</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/91e41898e6d1d2a9a6e980c39e2f8baa2fa8a1f8"><code>91e4189</code></a> Port DSA to Rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8978">#8978</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pyca/cryptography/compare/40.0.2...41.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=40.0.2&new-version=41.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 15:14:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    build(deps): bump requests from 2.29.0 to 2.31.0 in /multi-agent-load-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.29.0 to 2.31.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.31.0</h2>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>v2.30.0</h2>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4"><code>147c851</code></a> v2.31.0</li>
<li><a href="https://github.com/psf/requests/commit/74ea7cf7a6a27a4eeb2ae24e162bcc942a6706d5"><code>74ea7cf</code></a> Merge pull request from GHSA-j8r2-6x86-q33q</li>
<li><a href="https://github.com/psf/requests/commit/302225334678490ec66b3614a9dddb8a02c5f4fe"><code>3022253</code></a> test on pypy 3.8 and pypy 3.9 on windows and macos (<a href="https://redirect.github.com/psf/requests/issues/6424">#6424</a>)</li>
<li><a href="https://github.com/psf/requests/commit/b639e66c816514e40604d46f0088fbceec1a5149"><code>b639e66</code></a> test on py3.12 (<a href="https://redirect.github.com/psf/requests/issues/6448">#6448</a>)</li>
<li><a href="https://github.com/psf/requests/commit/d3d504436ef0c2ac7ec8af13738b04dcc8c694be"><code>d3d5044</code></a> Fixed a small typo (<a href="https://redirect.github.com/psf/requests/issues/6452">#6452</a>)</li>
<li><a href="https://github.com/psf/requests/commit/2ad18e0e10e7d7ecd5384c378f25ec8821a10a29"><code>2ad18e0</code></a> v2.30.0</li>
<li><a href="https://github.com/psf/requests/commit/f2629e9e3c7ce3c3c8c025bcd8db551101cbc773"><code>f2629e9</code></a> Remove strict parameter (<a href="https://redirect.github.com/psf/requests/issues/6434">#6434</a>)</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.29.0...v2.31.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.29.0&new-version=2.31.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mediator-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 15:14:42 +0000 UTC
    </div>
</div>

