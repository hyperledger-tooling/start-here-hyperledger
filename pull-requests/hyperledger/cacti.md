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
                PR <a href="https://github.com/hyperledger/cacti/pull/2592" class=".btn">#2592</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 41.0.2 to 41.0.3 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 41.0.2 to 41.0.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.3 - 2023-08-01</p>
<pre><code>
* Fixed performance regression loading DH public keys.
* Fixed a memory leak when using
  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.2.
<p>.. _v41-0-2:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/b22271cf3c3dd8dc8978f8f4b00b5c7060b6538d"><code>b22271c</code></a> bump for 41.0.3 (<a href="https://redirect.github.com/pyca/cryptography/issues/9330">#9330</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/774a4a16cbd22a89fdb4195ade9e4fcee27a7afa"><code>774a4a1</code></a> Only check DH key validity when loading a private key. (<a href="https://redirect.github.com/pyca/cryptography/issues/9071">#9071</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/9319">#9319</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/bfa4d95f0f356f2d535efd5c775e0fb3efe90ef2"><code>bfa4d95</code></a> changelog for 41.0.3 (<a href="https://redirect.github.com/pyca/cryptography/issues/9320">#9320</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0da7165aa73c0a4865b0a4d9e019db3c16eea55a"><code>0da7165</code></a> backport fix the memory leak in fixedpool (<a href="https://redirect.github.com/pyca/cryptography/issues/9272">#9272</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/9309">#9309</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/41.0.2...41.0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=41.0.2&new-version=41.0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-08-02 02:26:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2591" class=".btn">#2591</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 41.0.2 to 41.0.3 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 41.0.2 to 41.0.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.3 - 2023-08-01</p>
<pre><code>
* Fixed performance regression loading DH public keys.
* Fixed a memory leak when using
  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.2.
<p>.. _v41-0-2:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/b22271cf3c3dd8dc8978f8f4b00b5c7060b6538d"><code>b22271c</code></a> bump for 41.0.3 (<a href="https://redirect.github.com/pyca/cryptography/issues/9330">#9330</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/774a4a16cbd22a89fdb4195ade9e4fcee27a7afa"><code>774a4a1</code></a> Only check DH key validity when loading a private key. (<a href="https://redirect.github.com/pyca/cryptography/issues/9071">#9071</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/9319">#9319</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/bfa4d95f0f356f2d535efd5c775e0fb3efe90ef2"><code>bfa4d95</code></a> changelog for 41.0.3 (<a href="https://redirect.github.com/pyca/cryptography/issues/9320">#9320</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0da7165aa73c0a4865b0a4d9e019db3c16eea55a"><code>0da7165</code></a> backport fix the memory leak in fixedpool (<a href="https://redirect.github.com/pyca/cryptography/issues/9272">#9272</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/9309">#9309</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/41.0.2...41.0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=41.0.2&new-version=41.0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-08-02 02:24:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2589" class=".btn">#2589</a>
            </td>
            <td>
                <b>
                    build(openapi): license presence check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Adds a custom check that ensures that all the properties of the
license object are specified (name, identifier, url).
2. Optimized the custom-check that verifies the opan API json specs so
that it ignores **/node_modules/ not just node_modules (meaning that it
was only excluding the root dir not all sub-dirs of the packages as well)

Fixes #490

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 00:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2588" class=".btn">#2588</a>
            </td>
            <td>
                <b>
                    test(test-geth-ledger): add test for test-geth-ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add tests for geth-test-ledger
- fix small errors in GethTestLedger class
    
Closes: #2579 
Depends on: #2577
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 15:41:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2587" class=".btn">#2587</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in example-carbon-accounting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2062
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 06:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2586" class=".btn">#2586</a>
            </td>
            <td>
                <b>
                    build(cmd-api-server): upgrade to Artillery v2.x or migrate to loadtest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2234
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 04:40:51 +0000 UTC
    </div>
</div>

