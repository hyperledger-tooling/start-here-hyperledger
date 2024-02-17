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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:59:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/115" class=".btn">#115</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:59:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:59:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:59:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:58:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:58:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:58:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.0 to 42.0.2 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.0 to 42.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.2 - 2024-01-30</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.2.1.
* Fixed an issue that prevented the use of Python buffer protocol objects in
  ``sign`` and ``verify`` methods on asymmetric keys.
* Fixed an issue with incorrect keyword-argument naming with ``EllipticCurvePrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.exchange`,
  ``X25519PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x25519.X25519PrivateKey.exchange`,
  ``X448PrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey.exchange`,
  and ``DHPrivateKey``
  :meth:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey.exchange`.
<p>.. _v42-0-1:</p>
<p>42.0.1 - 2024-01-24
</code></pre></p>
<ul>
<li>Fixed an issue with incorrect keyword-argument naming with <code>EllipticCurvePrivateKey</code>
:meth:<code>~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.sign</code>.</li>
<li>Resolved compatibility issue with loading certain RSA public keys in
:func:<code>~cryptography.hazmat.primitives.serialization.load_pem_public_key</code>.</li>
</ul>
<p>.. _v42-0-0:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/2202123b50de1b8788f909a3e5afe350c56ad81e"><code>2202123</code></a> changelog and version bump 42.0.2 (<a href="https://redirect.github.com/pyca/cryptography/issues/10268">#10268</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f7032bdd409838f67fc2b93343f897fb5f397d80"><code>f7032bd</code></a> bump openssl in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/10298">#10298</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10299">#10299</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/002e886f16d8857151c09b11dc86b35f2ac9aec3"><code>002e886</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10294">#10294</a> -- correct accidental change to exchange kwarg (<a href="https://redirect.github.com/pyca/cryptography/issues/10295">#10295</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/92fa9f2f606caea5d499c825e832be5bac6f0c23"><code>92fa9f2</code></a> support bytes-like consistently across our asym sign/verify APIs (<a href="https://redirect.github.com/pyca/cryptography/issues/10260">#10260</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/6478f7e28be54b51931277235de01b249ceabd96"><code>6478f7e</code></a> explicitly support bytes-like for signature/data in RSA sign/verify (<a href="https://redirect.github.com/pyca/cryptography/issues/10259">#10259</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/4bb8596ae02d95bb054dbcf55e8771379dbe0c19"><code>4bb8596</code></a> fix the release script (<a href="https://redirect.github.com/pyca/cryptography/issues/10233">#10233</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/337437dc2e62772bde4ad5544f4b1db9ee7572d9"><code>337437d</code></a> 42.0.1 bump (<a href="https://redirect.github.com/pyca/cryptography/issues/10252">#10252</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/56255de6b2d1a2d2e502b0275231ca81907f33f1"><code>56255de</code></a> allow SPKI RSA keys to be parsed even if they have an incorrect delimiter (<a href="https://redirect.github.com/pyca/cryptography/issues/1">#1</a>...</li>
<li><a href="https://github.com/pyca/cryptography/commit/12f038b38af76e36efe8cef09597010c97647e8f"><code>12f038b</code></a> fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10237">#10237</a> -- correct EC sign parameter name (<a href="https://redirect.github.com/pyca/cryptography/issues/10239">#10239</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10240">#10240</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.0...42.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.0&new-version=42.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:58:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump fastapi from 0.68.2 to 0.109.1 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [fastapi](https://github.com/tiangolo/fastapi) from 0.68.2 to 0.109.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tiangolo/fastapi/releases">fastapi's releases</a>.</em></p>
<blockquote>
<h2>0.109.1</h2>
<h3>Security fixes</h3>
<ul>
<li>⬆️ Upgrade minimum version of <code>python-multipart</code> to <code>&gt;=0.0.7</code> to fix a vulnerability when using form data with a ReDos attack. You can also simply upgrade <code>python-multipart</code>.</li>
</ul>
<p>Read more in the <a href="https://github.com/tiangolo/fastapi/security/advisories/GHSA-qf9m-vfgh-m389">advisory: Content-Type Header ReDoS</a>.</p>
<h3>Features</h3>
<ul>
<li>✨  Include HTTP 205 in status codes with no body. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10969">#10969</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
<h3>Refactors</h3>
<ul>
<li>✅ Refactor tests for duplicate operation ID generation for compatibility with other tools running the FastAPI test suite. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10876">#10876</a> by <a href="https://github.com/emmettbutler"><code>@​emmettbutler</code></a>.</li>
<li>♻️ Simplify string format with f-strings in <code>fastapi/utils.py</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10576">#10576</a> by <a href="https://github.com/eukub"><code>@​eukub</code></a>.</li>
<li>🔧 Fix Ruff configuration unintentionally enabling and re-disabling mccabe complexity check. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10893">#10893</a> by <a href="https://github.com/jiridanek"><code>@​jiridanek</code></a>.</li>
<li>✅ Re-enable test in <code>tests/test_tutorial/test_header_params/test_tutorial003.py</code> after fix in Starlette. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10904">#10904</a> by <a href="https://github.com/ooknimm"><code>@​ooknimm</code></a>.</li>
</ul>
<h3>Docs</h3>
<ul>
<li>📝 Tweak wording in <code>help-fastapi.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11040">#11040</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>📝 Tweak docs for Behind a Proxy. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11038">#11038</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>📝 Add External Link: 10 Tips for adding SQLAlchemy to FastAPI. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11036">#11036</a> by <a href="https://github.com/Donnype"><code>@​Donnype</code></a>.</li>
<li>📝 Add External Link: Tips on migrating from Flask to FastAPI and vice-versa. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11029">#11029</a> by <a href="https://github.com/jtemporal"><code>@​jtemporal</code></a>.</li>
<li>📝 Deprecate old tutorials: Peewee, Couchbase, encode/databases. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10979">#10979</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>✏️ Fix typo in <code>fastapi/security/oauth2.py</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10972">#10972</a> by <a href="https://github.com/RafalSkolasinski"><code>@​RafalSkolasinski</code></a>.</li>
<li>📝 Update <code>HTTPException</code> details in <code>docs/en/docs/tutorial/handling-errors.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5418">#5418</a> by <a href="https://github.com/papb"><code>@​papb</code></a>.</li>
<li>✏️ A few tweaks in <code>docs/de/docs/tutorial/first-steps.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10959">#10959</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>✏️ Fix link in <code>docs/en/docs/advanced/async-tests.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10960">#10960</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>✏️ Fix typos for Spanish documentation. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10957">#10957</a> by <a href="https://github.com/jlopezlira"><code>@​jlopezlira</code></a>.</li>
<li>📝 Add warning about lifespan functions and backwards compatibility with events. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10734">#10734</a> by <a href="https://github.com/jacob-indigo"><code>@​jacob-indigo</code></a>.</li>
<li>✏️ Fix broken link in <code>docs/tutorial/sql-databases.md</code> in several languages. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10716">#10716</a> by <a href="https://github.com/theoohoho"><code>@​theoohoho</code></a>.</li>
<li>✏️ Remove broken links from <code>external_links.yml</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10943">#10943</a> by <a href="https://github.com/Torabek"><code>@​Torabek</code></a>.</li>
<li>📝 Update template docs with more info about <code>url_for</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5937">#5937</a> by <a href="https://github.com/EzzEddin"><code>@​EzzEddin</code></a>.</li>
<li>📝 Update usage of Token model in security docs. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/9313">#9313</a> by <a href="https://github.com/piotrszacilowski"><code>@​piotrszacilowski</code></a>.</li>
<li>✏️ Update highlighted line in <code>docs/en/docs/tutorial/bigger-applications.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5490">#5490</a> by <a href="https://github.com/papb"><code>@​papb</code></a>.</li>
<li>📝 Add External Link: Explore How to Effectively Use JWT With FastAPI. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10212">#10212</a> by <a href="https://github.com/aanchlia"><code>@​aanchlia</code></a>.</li>
<li>📝 Add hyperlink to <code>docs/en/docs/tutorial/static-files.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10243">#10243</a> by <a href="https://github.com/hungtsetse"><code>@​hungtsetse</code></a>.</li>
<li>📝 Add External Link: Instrument a FastAPI service adding tracing with OpenTelemetry and send/show traces in Grafana Tempo. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/9440">#9440</a> by <a href="https://github.com/softwarebloat"><code>@​softwarebloat</code></a>.</li>
<li>📝 Review and rewording of <code>en/docs/contributing.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10480">#10480</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>📝 Add External Link: ML serving and monitoring with FastAPI and Evidently. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/9701">#9701</a> by <a href="https://github.com/mnrozhkov"><code>@​mnrozhkov</code></a>.</li>
<li>📝 Reword in docs, from &quot;have in mind&quot; to &quot;keep in mind&quot;. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10376">#10376</a> by <a href="https://github.com/malicious"><code>@​malicious</code></a>.</li>
<li>📝 Add External Link: Talk by Jeny Sadadia. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10265">#10265</a> by <a href="https://github.com/JenySadadia"><code>@​JenySadadia</code></a>.</li>
<li>📝 Add location info to <code>tutorial/bigger-applications.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10552">#10552</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>✏️ Fix Pydantic method name in <code>docs/en/docs/advanced/path-operation-advanced-configuration.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10826">#10826</a> by <a href="https://github.com/ahmedabdou14"><code>@​ahmedabdou14</code></a>.</li>
</ul>
<h3>Translations</h3>
<ul>
<li>🌐 Add Spanish translation for <code>docs/es/docs/external-links.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10933">#10933</a> by <a href="https://github.com/pablocm83"><code>@​pablocm83</code></a>.</li>
<li>🌐 Update Korean translation for <code>docs/ko/docs/tutorial/first-steps.md</code>, <code>docs/ko/docs/tutorial/index.md</code>, <code>docs/ko/docs/tutorial/path-params.md</code>, and <code>docs/ko/docs/tutorial/query-params.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/4218">#4218</a> by <a href="https://github.com/SnowSuno"><code>@​SnowSuno</code></a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tiangolo/fastapi/commit/7633d1571cc0c2792b766f67172edb9427c66899"><code>7633d15</code></a> 🔖 Release version 0.109.1</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/a4de147521bf1546f700aa494d99fce1bed0741b"><code>a4de147</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/9d34ad0ee8a0dfbbcce06f76c2d5d851085024fc"><code>9d34ad0</code></a> Merge pull request from GHSA-qf9m-vfgh-m389</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/ebf972349431043170c1f6a4550bd29642f09cd2"><code>ebf9723</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/8590d0c2ec301d01da68ad3032f9b119d616a644"><code>8590d0c</code></a> 👥 Update FastAPI People (<a href="https://redirect.github.com/tiangolo/fastapi/issues/11074">#11074</a>)</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/063d7ffb15c4d1fe88745a8d2d2c9202d44046c5"><code>063d7ff</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/3c81e622f3783920ef3e3d4ecfae12c5511747bf"><code>3c81e62</code></a> 🌐 Add Spanish translation for <code>docs/es/docs/external-links.md</code> (<a href="https://redirect.github.com/tiangolo/fastapi/issues/10933">#10933</a>)</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/6c4a143fd0fb2a9963ca60938c4a2bf69573aeca"><code>6c4a143</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/d254e2f6ad773cf6694b7c1917c5792e9f805fd0"><code>d254e2f</code></a> 🌐 Update Korean translation for <code>docs/ko/docs/tutorial/first-steps.md</code>, `docs...</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/6f6e786979eb3156b85e7c2f44d0b8af5cf0af17"><code>6f6e786</code></a> 📝 Update release notes</li>
<li>Additional commits viewable in <a href="https://github.com/tiangolo/fastapi/compare/0.68.2...0.109.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=fastapi&package-manager=pip&previous-version=0.68.2&new-version=0.109.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:25:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump fastapi from 0.68.2 to 0.109.1 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [fastapi](https://github.com/tiangolo/fastapi) from 0.68.2 to 0.109.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tiangolo/fastapi/releases">fastapi's releases</a>.</em></p>
<blockquote>
<h2>0.109.1</h2>
<h3>Security fixes</h3>
<ul>
<li>⬆️ Upgrade minimum version of <code>python-multipart</code> to <code>&gt;=0.0.7</code> to fix a vulnerability when using form data with a ReDos attack. You can also simply upgrade <code>python-multipart</code>.</li>
</ul>
<p>Read more in the <a href="https://github.com/tiangolo/fastapi/security/advisories/GHSA-qf9m-vfgh-m389">advisory: Content-Type Header ReDoS</a>.</p>
<h3>Features</h3>
<ul>
<li>✨  Include HTTP 205 in status codes with no body. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10969">#10969</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
<h3>Refactors</h3>
<ul>
<li>✅ Refactor tests for duplicate operation ID generation for compatibility with other tools running the FastAPI test suite. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10876">#10876</a> by <a href="https://github.com/emmettbutler"><code>@​emmettbutler</code></a>.</li>
<li>♻️ Simplify string format with f-strings in <code>fastapi/utils.py</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10576">#10576</a> by <a href="https://github.com/eukub"><code>@​eukub</code></a>.</li>
<li>🔧 Fix Ruff configuration unintentionally enabling and re-disabling mccabe complexity check. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10893">#10893</a> by <a href="https://github.com/jiridanek"><code>@​jiridanek</code></a>.</li>
<li>✅ Re-enable test in <code>tests/test_tutorial/test_header_params/test_tutorial003.py</code> after fix in Starlette. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10904">#10904</a> by <a href="https://github.com/ooknimm"><code>@​ooknimm</code></a>.</li>
</ul>
<h3>Docs</h3>
<ul>
<li>📝 Tweak wording in <code>help-fastapi.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11040">#11040</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>📝 Tweak docs for Behind a Proxy. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11038">#11038</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>📝 Add External Link: 10 Tips for adding SQLAlchemy to FastAPI. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11036">#11036</a> by <a href="https://github.com/Donnype"><code>@​Donnype</code></a>.</li>
<li>📝 Add External Link: Tips on migrating from Flask to FastAPI and vice-versa. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/11029">#11029</a> by <a href="https://github.com/jtemporal"><code>@​jtemporal</code></a>.</li>
<li>📝 Deprecate old tutorials: Peewee, Couchbase, encode/databases. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10979">#10979</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>✏️ Fix typo in <code>fastapi/security/oauth2.py</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10972">#10972</a> by <a href="https://github.com/RafalSkolasinski"><code>@​RafalSkolasinski</code></a>.</li>
<li>📝 Update <code>HTTPException</code> details in <code>docs/en/docs/tutorial/handling-errors.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5418">#5418</a> by <a href="https://github.com/papb"><code>@​papb</code></a>.</li>
<li>✏️ A few tweaks in <code>docs/de/docs/tutorial/first-steps.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10959">#10959</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>✏️ Fix link in <code>docs/en/docs/advanced/async-tests.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10960">#10960</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>✏️ Fix typos for Spanish documentation. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10957">#10957</a> by <a href="https://github.com/jlopezlira"><code>@​jlopezlira</code></a>.</li>
<li>📝 Add warning about lifespan functions and backwards compatibility with events. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10734">#10734</a> by <a href="https://github.com/jacob-indigo"><code>@​jacob-indigo</code></a>.</li>
<li>✏️ Fix broken link in <code>docs/tutorial/sql-databases.md</code> in several languages. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10716">#10716</a> by <a href="https://github.com/theoohoho"><code>@​theoohoho</code></a>.</li>
<li>✏️ Remove broken links from <code>external_links.yml</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10943">#10943</a> by <a href="https://github.com/Torabek"><code>@​Torabek</code></a>.</li>
<li>📝 Update template docs with more info about <code>url_for</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5937">#5937</a> by <a href="https://github.com/EzzEddin"><code>@​EzzEddin</code></a>.</li>
<li>📝 Update usage of Token model in security docs. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/9313">#9313</a> by <a href="https://github.com/piotrszacilowski"><code>@​piotrszacilowski</code></a>.</li>
<li>✏️ Update highlighted line in <code>docs/en/docs/tutorial/bigger-applications.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5490">#5490</a> by <a href="https://github.com/papb"><code>@​papb</code></a>.</li>
<li>📝 Add External Link: Explore How to Effectively Use JWT With FastAPI. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10212">#10212</a> by <a href="https://github.com/aanchlia"><code>@​aanchlia</code></a>.</li>
<li>📝 Add hyperlink to <code>docs/en/docs/tutorial/static-files.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10243">#10243</a> by <a href="https://github.com/hungtsetse"><code>@​hungtsetse</code></a>.</li>
<li>📝 Add External Link: Instrument a FastAPI service adding tracing with OpenTelemetry and send/show traces in Grafana Tempo. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/9440">#9440</a> by <a href="https://github.com/softwarebloat"><code>@​softwarebloat</code></a>.</li>
<li>📝 Review and rewording of <code>en/docs/contributing.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10480">#10480</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>📝 Add External Link: ML serving and monitoring with FastAPI and Evidently. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/9701">#9701</a> by <a href="https://github.com/mnrozhkov"><code>@​mnrozhkov</code></a>.</li>
<li>📝 Reword in docs, from &quot;have in mind&quot; to &quot;keep in mind&quot;. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10376">#10376</a> by <a href="https://github.com/malicious"><code>@​malicious</code></a>.</li>
<li>📝 Add External Link: Talk by Jeny Sadadia. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10265">#10265</a> by <a href="https://github.com/JenySadadia"><code>@​JenySadadia</code></a>.</li>
<li>📝 Add location info to <code>tutorial/bigger-applications.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10552">#10552</a> by <a href="https://github.com/nilslindemann"><code>@​nilslindemann</code></a>.</li>
<li>✏️ Fix Pydantic method name in <code>docs/en/docs/advanced/path-operation-advanced-configuration.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10826">#10826</a> by <a href="https://github.com/ahmedabdou14"><code>@​ahmedabdou14</code></a>.</li>
</ul>
<h3>Translations</h3>
<ul>
<li>🌐 Add Spanish translation for <code>docs/es/docs/external-links.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/10933">#10933</a> by <a href="https://github.com/pablocm83"><code>@​pablocm83</code></a>.</li>
<li>🌐 Update Korean translation for <code>docs/ko/docs/tutorial/first-steps.md</code>, <code>docs/ko/docs/tutorial/index.md</code>, <code>docs/ko/docs/tutorial/path-params.md</code>, and <code>docs/ko/docs/tutorial/query-params.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/4218">#4218</a> by <a href="https://github.com/SnowSuno"><code>@​SnowSuno</code></a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tiangolo/fastapi/commit/7633d1571cc0c2792b766f67172edb9427c66899"><code>7633d15</code></a> 🔖 Release version 0.109.1</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/a4de147521bf1546f700aa494d99fce1bed0741b"><code>a4de147</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/9d34ad0ee8a0dfbbcce06f76c2d5d851085024fc"><code>9d34ad0</code></a> Merge pull request from GHSA-qf9m-vfgh-m389</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/ebf972349431043170c1f6a4550bd29642f09cd2"><code>ebf9723</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/8590d0c2ec301d01da68ad3032f9b119d616a644"><code>8590d0c</code></a> 👥 Update FastAPI People (<a href="https://redirect.github.com/tiangolo/fastapi/issues/11074">#11074</a>)</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/063d7ffb15c4d1fe88745a8d2d2c9202d44046c5"><code>063d7ff</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/3c81e622f3783920ef3e3d4ecfae12c5511747bf"><code>3c81e62</code></a> 🌐 Add Spanish translation for <code>docs/es/docs/external-links.md</code> (<a href="https://redirect.github.com/tiangolo/fastapi/issues/10933">#10933</a>)</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/6c4a143fd0fb2a9963ca60938c4a2bf69573aeca"><code>6c4a143</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/d254e2f6ad773cf6694b7c1917c5792e9f805fd0"><code>d254e2f</code></a> 🌐 Update Korean translation for <code>docs/ko/docs/tutorial/first-steps.md</code>, `docs...</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/6f6e786979eb3156b85e7c2f44d0b8af5cf0af17"><code>6f6e786</code></a> 📝 Update release notes</li>
<li>Additional commits viewable in <a href="https://github.com/tiangolo/fastapi/compare/0.68.2...0.109.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=fastapi&package-manager=pip&previous-version=0.68.2&new-version=0.109.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-17 00:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the all-actions group with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 3 updates: [actions/checkout](https://github.com/actions/checkout), [tj-actions/changed-files](https://github.com/tj-actions/changed-files) and [actions/setup-python](https://github.com/actions/setup-python).

Updates `actions/checkout` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li>Support fetching without the --progress option by <a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
<li>Release 4.0.0 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1447">actions/checkout#1447</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li><a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v4.0.0">https://github.com/actions/checkout/compare/v3...v4.0.0</a></p>
<h2>v3.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Mark test scripts with Bash'isms to be run via Bash by <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1377">actions/checkout#1377</a></li>
<li>Add option to fetch tags even if fetch-depth &gt; 0 by <a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li>Release 3.6.0 by <a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li><a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.3...v3.6.0">https://github.com/actions/checkout/compare/v3.5.3...v3.6.0</a></p>
<h2>v3.5.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Checkout Issue in self hosted runner due to faulty submodule check-ins by <a href="https://github.com/megamanics"><code>@​megamanics</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li>Fix typos found by codespell by <a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li>Add support for sparse checkouts by <a href="https://github.com/dscho"><code>@​dscho</code></a> and <a href="https://github.com/dfdez"><code>@​dfdez</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
<li>Release v3.5.3 by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1376">actions/checkout#1376</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/megamanics"><code>@​megamanics</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li><a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li><a href="https://github.com/dfdez"><code>@​dfdez</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v3.5.3">https://github.com/actions/checkout/compare/v3...v3.5.3</a></p>
<h2>v3.5.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Use correct API url / endpoint in GHES by <a href="https://github.com/fhammerl"><code>@​fhammerl</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1289">actions/checkout#1289</a> based on <a href="https://redirect.github.com/actions/checkout/issues/1286">#1286</a> by <a href="https://github.com/1newsr"><code>@​1newsr</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.1...v3.5.2">https://github.com/actions/checkout/compare/v3.5.1...v3.5.2</a></p>
<h2>v3.5.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Improve checkout performance on Windows runners by upgrading <code>@​actions/github</code> dependency by <a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v4.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1396">Add support for partial checkout filters</a></li>
</ul>
<h2>v4.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1067">Support fetching without the --progress option</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1436">Update to node20</a></li>
</ul>
<h2>v3.6.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1377">Fix: Mark test scripts with Bash'isms to be run via Bash</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/579">Add option to fetch tags even if fetch-depth &gt; 0</a></li>
</ul>
<h2>v3.5.3</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1196">Fix: Checkout fail in self-hosted runners when faulty submodule are checked-in</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1287">Fix typos found by codespell</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1369">Add support for sparse checkouts</a></li>
</ul>
<h2>v3.5.2</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1289">Fix api endpoint for GHES</a></li>
</ul>
<h2>v3.5.1</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1246">Fix slow checkout on Windows</a></li>
</ul>
<h2>v3.5.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1237">Add new public key for known_hosts</a></li>
</ul>
<h2>v3.4.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1209">Upgrade codeql actions to v2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1210">Upgrade dependencies</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1225">Upgrade <code>@​actions/io</code></a></li>
</ul>
<h2>v3.3.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1045">Implement branch list using callbacks from exec function</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1050">Add in explicit reference to private checkout options</a></li>
<li>[Fix comment typos (that got added in <a href="https://redirect.github.com/actions/checkout/issues/770">#770</a>)](<a href="https://redirect.github.com/actions/checkout/pull/1057">actions/checkout#1057</a>)</li>
</ul>
<h2>v3.2.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/942">Add GitHub Action to perform release</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/967">Fix status badge</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1002">Replace datadog/squid with ubuntu/squid Docker image</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/964">Wrap pipeline commands for submoduleForeach in quotes</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1029">Update <code>@​actions/io</code> to 1.1.2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1039">Upgrading version to 3.2.0</a></li>
</ul>
<h2>v3.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/939">Use <code>@​actions/core</code> <code>saveState</code> and <code>getState</code></a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/922">Add <code>github-server-url</code> input</a></li>
</ul>
<h2>v3.0.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/b4ffde65f46336ab88eb53be808477a3936bae11"><code>b4ffde6</code></a> Link to release page from what's new section (<a href="https://redirect.github.com/actions/checkout/issues/1514">#1514</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8530928916aaef40f59e6f221989ccb31f5759e7"><code>8530928</code></a> Correct link to GitHub Docs (<a href="https://redirect.github.com/actions/checkout/issues/1511">#1511</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/7cdaf2fbc075e6f3b9ca94cfd6cec5adc8a75622"><code>7cdaf2f</code></a> Update CODEOWNERS to Launch team (<a href="https://redirect.github.com/actions/checkout/issues/1510">#1510</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8ade135a41bc03ea155e62e844d188df1ea18608"><code>8ade135</code></a> Prepare 4.1.0 release (<a href="https://redirect.github.com/actions/checkout/issues/1496">#1496</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/c533a0a4cfc4962971818edcfac47a2899e69799"><code>c533a0a</code></a> Add support for partial checkout filters (<a href="https://redirect.github.com/actions/checkout/issues/1396">#1396</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/72f2cec99f417b1a1c5e2e88945068983b7965f9"><code>72f2cec</code></a> Update README.md for V4 (<a href="https://redirect.github.com/actions/checkout/issues/1452">#1452</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/3df4ab11eba7bda6032a0b82a6bb43b11571feac"><code>3df4ab1</code></a> Release 4.0.0 (<a href="https://redirect.github.com/actions/checkout/issues/1447">#1447</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8b5e8b768746b50394015010d25e690bfab9dfbc"><code>8b5e8b7</code></a> Support fetching without the --progress option (<a href="https://redirect.github.com/actions/checkout/issues/1067">#1067</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/97a652b80035363df47baee5031ec8670b8878ac"><code>97a652b</code></a> Update default runtime to node20 (<a href="https://redirect.github.com/actions/checkout/issues/1436">#1436</a>)</li>
<li>See full diff in <a href="https://github.com/actions/checkout/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `tj-actions/changed-files` from 41 to 42
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tj-actions/changed-files/releases">tj-actions/changed-files's releases</a>.</em></p>
<blockquote>
<h2>v42</h2>
<h1>Changes in v42.0.2</h1>
<h2>What's Changed</h2>
<ul>
<li>Upgraded to v42.0.1 by <a href="https://github.com/tj-actions-bot"><code>@​tj-actions-bot</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1884">tj-actions/changed-files#1884</a></li>
<li>feat: enhance error handling for non-git directories by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1885">tj-actions/changed-files#1885</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tj-actions/changed-files/compare/v42...v42.0.2">https://github.com/tj-actions/changed-files/compare/v42...v42.0.2</a></p>
<hr />
<h1>Changes in v42.0.1</h1>
<h2>What's Changed</h2>
<ul>
<li>Upgraded to v42 by <a href="https://github.com/tj-actions-bot"><code>@​tj-actions-bot</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1874">tj-actions/changed-files#1874</a></li>
<li>chore(deps): update tj-actions/eslint-changed-files action to v23 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1875">tj-actions/changed-files#1875</a></li>
<li>chore(deps): lock file maintenance by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1876">tj-actions/changed-files#1876</a></li>
<li>chore: update README.md by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1877">tj-actions/changed-files#1877</a></li>
<li>chore: rename example worflows from test to example by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1878">tj-actions/changed-files#1878</a></li>
<li>chore(deps): lock file maintenance by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1879">tj-actions/changed-files#1879</a></li>
<li>chore(deps): update dependency ts-jest to v29.1.2 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1880">tj-actions/changed-files#1880</a></li>
<li>chore(deps): update typescript-eslint monorepo to v6.19.1 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1881">tj-actions/changed-files#1881</a></li>
<li>chore(deps): update dependency <code>@​types/node</code> to v20.11.6 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1883">tj-actions/changed-files#1883</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tj-actions/changed-files/compare/v42...v42.0.1">https://github.com/tj-actions/changed-files/compare/v42...v42.0.1</a></p>
<hr />
<h1>Changes in v42.0.0</h1>
<h2>🔥🔥 BREAKING CHANGE 🔥🔥</h2>
<ul>
<li>Input file patterns that end with a <code>/</code> would now match all sub-files within the directory without requiring you to specify the globstar pattern.</li>
</ul>
<h3></h3>
<pre lang="yaml"><code>...
      - name: Get changed files
        id: changed-files
        uses: tj-actions/changed-files@v42
        with:
          files: 'dir/'  # Would also be the same as dir/** 
</code></pre>
<h2>What's Changed</h2>
<ul>
<li>Upgraded to v41.1.2 by <a href="https://github.com/tj-actions-bot"><code>@​tj-actions-bot</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1869">tj-actions/changed-files#1869</a></li>
<li>chore(deps): update dependency prettier to v3.2.4 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1871">tj-actions/changed-files#1871</a></li>
<li>fix: update input warning by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1870">tj-actions/changed-files#1870</a></li>
<li>rename: unsupported REST API inputs constant name by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1872">tj-actions/changed-files#1872</a></li>
<li>feat: add support for include/exclude all nested files when a directory is specified and ends with a slash by <a href="https://github.com/jackton1"><code>@​jackton1</code></a> in <a href="https://redirect.github.com/tj-actions/changed-files/pull/1873">tj-actions/changed-files#1873</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tj-actions/changed-files/blob/main/HISTORY.md">tj-actions/changed-files's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1><a href="https://github.com/tj-actions/changed-files/compare/v42.0.1...v42.0.2">42.0.2</a> - (2024-01-25)</h1>
<h2><!-- raw HTML omitted -->🚀 Features</h2>
<ul>
<li>Enhance error handling for non-git directories (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1885">#1885</a>) (<a href="https://github.com/tj-actions/changed-files/commit/90a06d6ba9543371ab4df8eeca0be07ca6054959">90a06d6</a>)  - (Tonye Jack)</li>
</ul>
<h2><!-- raw HTML omitted -->⬆️ Upgrades</h2>
<ul>
<li>Upgraded to v42.0.1 (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1884">#1884</a>)</li>
</ul>
<p>Co-authored-by: jackton1 <a href="mailto:jackton1@users.noreply.github.com">jackton1@users.noreply.github.com</a> (<a href="https://github.com/tj-actions/changed-files/commit/2cb2c9234e9dc3b8eaac2ababc3f355e80e47963">2cb2c92</a>)  - (tj-actions[bot])</p>
<h1><a href="https://github.com/tj-actions/changed-files/compare/v42.0.0...v42.0.1">42.0.1</a> - (2024-01-24)</h1>
<h2><!-- raw HTML omitted -->➕ Add</h2>
<ul>
<li>Added missing changes and modified dist assets.
(<a href="https://github.com/tj-actions/changed-files/commit/ea024b2d7f80389ba16e7084b20265cb7dfe230f">ea024b2</a>)  - (GitHub Action)</li>
<li>Added missing changes and modified dist assets.
(<a href="https://github.com/tj-actions/changed-files/commit/3af07c2040da68166f613248bd8e9cd28fb581e3">3af07c2</a>)  - (GitHub Action)</li>
</ul>
<h2><!-- raw HTML omitted -->🔄 Update</h2>
<ul>
<li>Update env.ts (<a href="https://github.com/tj-actions/changed-files/commit/3680129aa2971333ef3d148024520cdc5327a6b7">3680129</a>)  - (Tonye Jack)</li>
</ul>
<h2><!-- raw HTML omitted -->⚙️ Miscellaneous Tasks</h2>
<ul>
<li><strong>deps:</strong> Update dependency <code>@​types/node</code> to v20.11.6 (<a href="https://github.com/tj-actions/changed-files/commit/ac21d93904fb48e7f76ce4bd2a4d197f67e34abe">ac21d93</a>)  - (renovate[bot])</li>
<li><strong>deps:</strong> Update typescript-eslint monorepo to v6.19.1 (<a href="https://github.com/tj-actions/changed-files/commit/a4637ea6e7d9a502f6edb845b6c65086c5bce55f">a4637ea</a>)  - (renovate[bot])</li>
<li><strong>deps:</strong> Update dependency ts-jest to v29.1.2 (<a href="https://github.com/tj-actions/changed-files/commit/fd9998cf5fcac4b0fff205a58ec694bf596169c8">fd9998c</a>)  - (renovate[bot])</li>
<li><strong>deps:</strong> Lock file maintenance (<a href="https://github.com/tj-actions/changed-files/commit/db4e5848448e4b540e7e7dcbdc7aab3c88bfcf47">db4e584</a>)  - (renovate[bot])</li>
<li>Rename example worflows from test to example (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1878">#1878</a>) (<a href="https://github.com/tj-actions/changed-files/commit/c6543c497aea61c2263b735dece03b23383441f0">c6543c4</a>)  - (Tonye Jack)</li>
<li>Update README.md (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1877">#1877</a>) (<a href="https://github.com/tj-actions/changed-files/commit/88f9f3efbb5a8fe2acff4139babc1d6aeafa5e72">88f9f3e</a>)  - (Tonye Jack)</li>
<li><strong>deps:</strong> Lock file maintenance (<a href="https://github.com/tj-actions/changed-files/commit/5d866cbe77002ed91912202826ed253b808a9133">5d866cb</a>)  - (renovate[bot])</li>
<li><strong>deps:</strong> Update tj-actions/eslint-changed-files action to v23 (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1875">#1875</a>) (<a href="https://github.com/tj-actions/changed-files/commit/346f237a1734287fa772ee254047beecabcdbdf2">346f237</a>)  - (renovate[bot])</li>
</ul>
<h2><!-- raw HTML omitted -->⬆️ Upgrades</h2>
<ul>
<li>Upgraded to v42 (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1874">#1874</a>)</li>
</ul>
<p>Co-authored-by: jackton1 <a href="mailto:jackton1@users.noreply.github.com">jackton1@users.noreply.github.com</a> (<a href="https://github.com/tj-actions/changed-files/commit/c037f1e7c56c7884b2d7d24c36cd8a0bc2c20687">c037f1e</a>)  - (tj-actions[bot])</p>
<h1><a href="https://github.com/tj-actions/changed-files/compare/v41.1.2...v42.0.0">42.0.0</a> - (2024-01-18)</h1>
<h2><!-- raw HTML omitted -->🚀 Features</h2>
<ul>
<li>Add support for include/exclude all nested files when a directory is specified and ends with a slash (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1873">#1873</a>) (<a href="https://github.com/tj-actions/changed-files/commit/ae82ed4ae04587b665efad2f206578aa6f0e8539">ae82ed4</a>)  - (Tonye Jack)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tj-actions/changed-files/commit/90a06d6ba9543371ab4df8eeca0be07ca6054959"><code>90a06d6</code></a> feat: enhance error handling for non-git directories (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1885">#1885</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/2cb2c9234e9dc3b8eaac2ababc3f355e80e47963"><code>2cb2c92</code></a> Upgraded to v42.0.1 (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1884">#1884</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/ac21d93904fb48e7f76ce4bd2a4d197f67e34abe"><code>ac21d93</code></a> chore(deps): update dependency <code>@​types/node</code> to v20.11.6</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/a4637ea6e7d9a502f6edb845b6c65086c5bce55f"><code>a4637ea</code></a> chore(deps): update typescript-eslint monorepo to v6.19.1</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/fd9998cf5fcac4b0fff205a58ec694bf596169c8"><code>fd9998c</code></a> chore(deps): update dependency ts-jest to v29.1.2</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/ea024b2d7f80389ba16e7084b20265cb7dfe230f"><code>ea024b2</code></a> Added missing changes and modified dist assets.</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/db4e5848448e4b540e7e7dcbdc7aab3c88bfcf47"><code>db4e584</code></a> chore(deps): lock file maintenance</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/c6543c497aea61c2263b735dece03b23383441f0"><code>c6543c4</code></a> chore: rename example worflows from test to example (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1878">#1878</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/88f9f3efbb5a8fe2acff4139babc1d6aeafa5e72"><code>88f9f3e</code></a> chore: update README.md (<a href="https://redirect.github.com/tj-actions/changed-files/issues/1877">#1877</a>)</li>
<li><a href="https://github.com/tj-actions/changed-files/commit/3af07c2040da68166f613248bd8e9cd28fb581e3"><code>3af07c2</code></a> Added missing changes and modified dist assets.</li>
<li>Additional commits viewable in <a href="https://github.com/tj-actions/changed-files/compare/v41...v42">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/setup-python` from 4 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-python/releases">actions/setup-python's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release, we update node version runtime from node16 to node20 (<a href="https://redirect.github.com/actions/setup-python/pull/772">actions/setup-python#772</a>). Besides, we update dependencies to the latest versions.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4.8.0...v5.0.0">https://github.com/actions/setup-python/compare/v4.8.0...v5.0.0</a></p>
<h2>v4.8.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release we added support for GraalPy (<a href="https://redirect.github.com/actions/setup-python/pull/694">actions/setup-python#694</a>). You can use this snippet to set up GraalPy:</p>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v4
- uses: actions/setup-python@v4 
  with:
    python-version: 'graalpy-22.3' 
- run: python my_script.py
</code></pre>
<p>Besides, the release contains such changes as:</p>
<ul>
<li>Trim python version when reading from file by <a href="https://github.com/FerranPares"><code>@​FerranPares</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/628">actions/setup-python#628</a></li>
<li>Use non-deprecated versions in examples by <a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/724">actions/setup-python#724</a></li>
<li>Change deprecation comment to past tense by <a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/723">actions/setup-python#723</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.9.0 to 7.23.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/743">actions/setup-python#743</a></li>
<li>advanced-usage.md: Encourage the use actions/checkout@v4 by <a href="https://github.com/cclauss"><code>@​cclauss</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/729">actions/setup-python#729</a></li>
<li>Examples now use checkout@v4 by <a href="https://github.com/simonw"><code>@​simonw</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/738">actions/setup-python#738</a></li>
<li>Update actions/checkout to v4 by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/761">actions/setup-python#761</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/FerranPares"><code>@​FerranPares</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/628">actions/setup-python#628</a></li>
<li><a href="https://github.com/timfel"><code>@​timfel</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/694">actions/setup-python#694</a></li>
<li><a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/724">actions/setup-python#724</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4...v4.8.0">https://github.com/actions/setup-python/compare/v4...v4.8.0</a></p>
<h2>v4.7.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump word-wrap from 1.2.3 to 1.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/702">actions/setup-python#702</a></li>
<li>Add range validation for toml files by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/726">actions/setup-python#726</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4...v4.7.1">https://github.com/actions/setup-python/compare/v4...v4.7.1</a></p>
<h2>v4.7.0</h2>
<p>In scope of this release, the support for reading python version from pyproject.toml was added (<a href="https://redirect.github.com/actions/setup-python/pull/669">actions/setup-python#669</a>).</p>
<pre lang="yaml"><code>      - name: Setup Python
        uses: actions/setup-python@v4
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-python/commit/0a5c61591373683505ea898e09a3ea4f39ef2b9c"><code>0a5c615</code></a> Update action to node20 (<a href="https://redirect.github.com/actions/setup-python/issues/772">#772</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/0ae58361cdfd39e2950bed97a1e26aa20c3d8955"><code>0ae5836</code></a> Add example of GraalPy to docs (<a href="https://redirect.github.com/actions/setup-python/issues/773">#773</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/b64ffcaf5b410884ad320a9cfac8866006a109aa"><code>b64ffca</code></a> update actions/checkout to v4 (<a href="https://redirect.github.com/actions/setup-python/issues/761">#761</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/8d2896179abf658742de432b3f203d2c2d86a587"><code>8d28961</code></a> Examples now use checkout@v4 (<a href="https://redirect.github.com/actions/setup-python/issues/738">#738</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/7bc6abb01e0555719edc2dbca70a2fde309e5e56"><code>7bc6abb</code></a> advanced-usage.md: Encourage the use actions/checkout@v4 (<a href="https://redirect.github.com/actions/setup-python/issues/729">#729</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/e8111cec9d3dc15220d8a3b638f08419f57b906a"><code>e8111ce</code></a> Bump <code>@​babel/traverse</code> from 7.9.0 to 7.23.2 (<a href="https://redirect.github.com/actions/setup-python/issues/743">#743</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/a00ea43da65e7c04d2bdae58b3afecd77057eb9e"><code>a00ea43</code></a> add fix for graalpy ci (<a href="https://redirect.github.com/actions/setup-python/issues/741">#741</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/8635b1ccc5934e73ed3510980fd2e7790b85839b"><code>8635b1c</code></a> Change deprecation comment to past tense (<a href="https://redirect.github.com/actions/setup-python/issues/723">#723</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/f6cc428f535856f9c23558d01765a42a4d6cf758"><code>f6cc428</code></a> Use non-deprecated versions in examples (<a href="https://redirect.github.com/actions/setup-python/issues/724">#724</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/5f2af211d616f86005883b44826180b21abb4060"><code>5f2af21</code></a> Add GraalPy support (<a href="https://redirect.github.com/actions/setup-python/issues/694">#694</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-python/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />


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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Add Dependabot configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Configure Dependabot to automatically maintain dependencies for GitHub Actions.
  - Check for updates once a week.
  - Group all updates into a single PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 17:06:15 +0000 UTC
    </div>
</div>

