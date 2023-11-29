---
layout: default
title: aries-uniffi-wrappers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-uniffi-wrappers
---

# aries-uniffi-wrappers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-uniffi-wrappers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-uniffi-wrappers/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.57 to 0.10.60 in /indy-vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.57 to 0.10.60.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.60</h2>
<h2>What's Changed</h2>
<ul>
<li>Correct off-by-one in minimum output buffer size computation by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2088">sfackler/rust-openssl#2088</a></li>
<li>Expose a few more (bad) ciphers in cipher::Cipher by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2084">sfackler/rust-openssl#2084</a></li>
<li>add temp key bindings by <a href="https://github.com/jmayclin"><code>@​jmayclin</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2076">sfackler/rust-openssl#2076</a></li>
<li>Expose ChaCha20 on LibreSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2093">sfackler/rust-openssl#2093</a></li>
<li>Revert &quot;Correct off-by-one in minimum output buffer size computation&quot; by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2090">sfackler/rust-openssl#2090</a></li>
<li>Added <code>update_unchecked</code> to <code>symm::Crypter</code> by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2100">sfackler/rust-openssl#2100</a></li>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2096">#2096</a> -- deprecate <code>X509StoreRef::objects</code>, it is unsound by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2099">sfackler/rust-openssl#2099</a></li>
<li>Don't leak when overwriting ex data by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2102">sfackler/rust-openssl#2102</a></li>
<li>Release openssl v0.10.60 and openssl-sys v0.9.96 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2104">sfackler/rust-openssl#2104</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.59...openssl-v0.10.60">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.59...openssl-v0.10.60</a></p>
<h2>openssl-v0.10.59</h2>
<h2>What's Changed</h2>
<ul>
<li>Add binding to NID of Chacha20-Poly1305 cipher by <a href="https://github.com/Arnavion"><code>@​Arnavion</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2081">sfackler/rust-openssl#2081</a></li>
<li>Fixed cfg for RSA_PSS by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2079">sfackler/rust-openssl#2079</a></li>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2050">#2050</a> -- build and test on libressl 3.8.2 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2082">sfackler/rust-openssl#2082</a></li>
<li>Release openssl v0.10.59 and openssl-sys v0.9.95 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2083">sfackler/rust-openssl#2083</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Arnavion"><code>@​Arnavion</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2081">sfackler/rust-openssl#2081</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.58...openssl-v0.10.59">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.58...openssl-v0.10.59</a></p>
<h2>openssl-v0.10.58</h2>
<h2>What's Changed</h2>
<ul>
<li>LibreSSL 3.8.1 support by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2035">sfackler/rust-openssl#2035</a></li>
<li>Update vendored version to openssl 3 by <a href="https://github.com/amousset"><code>@​amousset</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1925">sfackler/rust-openssl#1925</a></li>
<li>Test against 3.2.0-alpha1 by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2037">sfackler/rust-openssl#2037</a></li>
<li>Removed reference to non-existent method by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2039">sfackler/rust-openssl#2039</a></li>
<li>Bump CI to 1.1.1w by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2040">sfackler/rust-openssl#2040</a></li>
<li>[openssl-sys] Add X509_check_{host,email,ip,ip_asc} fns by <a href="https://github.com/jgallagher"><code>@​jgallagher</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2042">sfackler/rust-openssl#2042</a></li>
<li>Expose CBC mode for several more (bad) ciphers by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2045">sfackler/rust-openssl#2045</a></li>
<li>Expose two additional Pkey IDs by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2046">sfackler/rust-openssl#2046</a></li>
<li>Add support for CRL extensions and the Authority Information Access e… by <a href="https://github.com/AdmiralGT"><code>@​AdmiralGT</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2003">sfackler/rust-openssl#2003</a></li>
<li>Fix clippy warnings produced by newer Rust by <a href="https://github.com/wiktor-k"><code>@​wiktor-k</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2052">sfackler/rust-openssl#2052</a></li>
<li>Use osslconf on BoringSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2056">sfackler/rust-openssl#2056</a></li>
<li>Make X509_ALGOR opaque for LibreSSL by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2060">sfackler/rust-openssl#2060</a></li>
<li>Don't ignore ECDSA tests without GF2m support by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2061">sfackler/rust-openssl#2061</a></li>
<li>Clarify 'possible LibreSSL bug' by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2062">sfackler/rust-openssl#2062</a></li>
<li>Enable BN_mod_sqrt() for upcoming LibreSSL 3.8.2 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2063">sfackler/rust-openssl#2063</a></li>
<li>Enable SHA-3 for LibreSSL 3.8.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2064">sfackler/rust-openssl#2064</a></li>
<li>Remove DH_generate_parameters for LibreSSL 3.8.2 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2065">sfackler/rust-openssl#2065</a></li>
<li>Use EVP_MD_CTX_{new,free}() in LibreSSL 3.8.2 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2067">sfackler/rust-openssl#2067</a></li>
<li>Enable HKDF support for LibreSSL &gt;= 3.6.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2066">sfackler/rust-openssl#2066</a></li>
<li>Two build script fixes for LibreSSL by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2068">sfackler/rust-openssl#2068</a></li>
<li>Respect OPENSSL_NO_OCB on AES functions by <a href="https://github.com/GuyLewin"><code>@​GuyLewin</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2070">sfackler/rust-openssl#2070</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/8f4b97ae06f5975e02052b5a4d4f63496a1ec760"><code>8f4b97a</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2104">#2104</a> from alex/bump-for-release</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/df66283bbc734f20b968357bfc336def7b309b15"><code>df66283</code></a> Release openssl v0.10.60 and openssl-sys v0.9.96</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/1a09dc8c948fcda66db0f221461303e80e69818e"><code>1a09dc8</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2102">#2102</a> from sfackler/ex-leak</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/b0a1da5ee9f1b923af2d98a36a4805715826ce02"><code>b0a1da5</code></a> Merge branch 'master' into ex-leak</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/f456b609365c9e04a5049415d6dff82cc885edd3"><code>f456b60</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2099">#2099</a> from alex/deprecate-store-ref-objects</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a8413b8b5414af3b9754f02ff9f3b0d91ca57cb1"><code>a8413b8</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2100">#2100</a> from alex/symm-update-unchecked</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a92c23794149dc6bec8a8b1148c68bbe048851c9"><code>a92c237</code></a> clippy</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/e839496d9ed0bd4dcd4f1ec24e049cbe117ef1bb"><code>e839496</code></a> Don't leak when overwriting ex data</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/602d38dca7b8a22a355e1e53199d922742025c5c"><code>602d38d</code></a> Added <code>update_unchecked</code> to <code>symm::Crypter</code></li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/cf9681a55cabd4cb9f1475bde17b5079f2a0384e"><code>cf9681a</code></a> fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2096">#2096</a> -- deprecate <code>X509StoreRef::objects</code>, it is unsound</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.57...openssl-v0.10.60">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.57&new-version=0.10.60)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-uniffi-wrappers/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 21:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-uniffi-wrappers/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.57 to 0.10.60 in /anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.57 to 0.10.60.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.60</h2>
<h2>What's Changed</h2>
<ul>
<li>Correct off-by-one in minimum output buffer size computation by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2088">sfackler/rust-openssl#2088</a></li>
<li>Expose a few more (bad) ciphers in cipher::Cipher by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2084">sfackler/rust-openssl#2084</a></li>
<li>add temp key bindings by <a href="https://github.com/jmayclin"><code>@​jmayclin</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2076">sfackler/rust-openssl#2076</a></li>
<li>Expose ChaCha20 on LibreSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2093">sfackler/rust-openssl#2093</a></li>
<li>Revert &quot;Correct off-by-one in minimum output buffer size computation&quot; by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2090">sfackler/rust-openssl#2090</a></li>
<li>Added <code>update_unchecked</code> to <code>symm::Crypter</code> by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2100">sfackler/rust-openssl#2100</a></li>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2096">#2096</a> -- deprecate <code>X509StoreRef::objects</code>, it is unsound by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2099">sfackler/rust-openssl#2099</a></li>
<li>Don't leak when overwriting ex data by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2102">sfackler/rust-openssl#2102</a></li>
<li>Release openssl v0.10.60 and openssl-sys v0.9.96 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2104">sfackler/rust-openssl#2104</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.59...openssl-v0.10.60">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.59...openssl-v0.10.60</a></p>
<h2>openssl-v0.10.59</h2>
<h2>What's Changed</h2>
<ul>
<li>Add binding to NID of Chacha20-Poly1305 cipher by <a href="https://github.com/Arnavion"><code>@​Arnavion</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2081">sfackler/rust-openssl#2081</a></li>
<li>Fixed cfg for RSA_PSS by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2079">sfackler/rust-openssl#2079</a></li>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2050">#2050</a> -- build and test on libressl 3.8.2 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2082">sfackler/rust-openssl#2082</a></li>
<li>Release openssl v0.10.59 and openssl-sys v0.9.95 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2083">sfackler/rust-openssl#2083</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Arnavion"><code>@​Arnavion</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2081">sfackler/rust-openssl#2081</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.58...openssl-v0.10.59">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.58...openssl-v0.10.59</a></p>
<h2>openssl-v0.10.58</h2>
<h2>What's Changed</h2>
<ul>
<li>LibreSSL 3.8.1 support by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2035">sfackler/rust-openssl#2035</a></li>
<li>Update vendored version to openssl 3 by <a href="https://github.com/amousset"><code>@​amousset</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1925">sfackler/rust-openssl#1925</a></li>
<li>Test against 3.2.0-alpha1 by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2037">sfackler/rust-openssl#2037</a></li>
<li>Removed reference to non-existent method by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2039">sfackler/rust-openssl#2039</a></li>
<li>Bump CI to 1.1.1w by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2040">sfackler/rust-openssl#2040</a></li>
<li>[openssl-sys] Add X509_check_{host,email,ip,ip_asc} fns by <a href="https://github.com/jgallagher"><code>@​jgallagher</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2042">sfackler/rust-openssl#2042</a></li>
<li>Expose CBC mode for several more (bad) ciphers by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2045">sfackler/rust-openssl#2045</a></li>
<li>Expose two additional Pkey IDs by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2046">sfackler/rust-openssl#2046</a></li>
<li>Add support for CRL extensions and the Authority Information Access e… by <a href="https://github.com/AdmiralGT"><code>@​AdmiralGT</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2003">sfackler/rust-openssl#2003</a></li>
<li>Fix clippy warnings produced by newer Rust by <a href="https://github.com/wiktor-k"><code>@​wiktor-k</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2052">sfackler/rust-openssl#2052</a></li>
<li>Use osslconf on BoringSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2056">sfackler/rust-openssl#2056</a></li>
<li>Make X509_ALGOR opaque for LibreSSL by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2060">sfackler/rust-openssl#2060</a></li>
<li>Don't ignore ECDSA tests without GF2m support by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2061">sfackler/rust-openssl#2061</a></li>
<li>Clarify 'possible LibreSSL bug' by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2062">sfackler/rust-openssl#2062</a></li>
<li>Enable BN_mod_sqrt() for upcoming LibreSSL 3.8.2 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2063">sfackler/rust-openssl#2063</a></li>
<li>Enable SHA-3 for LibreSSL 3.8.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2064">sfackler/rust-openssl#2064</a></li>
<li>Remove DH_generate_parameters for LibreSSL 3.8.2 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2065">sfackler/rust-openssl#2065</a></li>
<li>Use EVP_MD_CTX_{new,free}() in LibreSSL 3.8.2 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2067">sfackler/rust-openssl#2067</a></li>
<li>Enable HKDF support for LibreSSL &gt;= 3.6.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2066">sfackler/rust-openssl#2066</a></li>
<li>Two build script fixes for LibreSSL by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2068">sfackler/rust-openssl#2068</a></li>
<li>Respect OPENSSL_NO_OCB on AES functions by <a href="https://github.com/GuyLewin"><code>@​GuyLewin</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2070">sfackler/rust-openssl#2070</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/8f4b97ae06f5975e02052b5a4d4f63496a1ec760"><code>8f4b97a</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2104">#2104</a> from alex/bump-for-release</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/df66283bbc734f20b968357bfc336def7b309b15"><code>df66283</code></a> Release openssl v0.10.60 and openssl-sys v0.9.96</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/1a09dc8c948fcda66db0f221461303e80e69818e"><code>1a09dc8</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2102">#2102</a> from sfackler/ex-leak</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/b0a1da5ee9f1b923af2d98a36a4805715826ce02"><code>b0a1da5</code></a> Merge branch 'master' into ex-leak</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/f456b609365c9e04a5049415d6dff82cc885edd3"><code>f456b60</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2099">#2099</a> from alex/deprecate-store-ref-objects</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a8413b8b5414af3b9754f02ff9f3b0d91ca57cb1"><code>a8413b8</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2100">#2100</a> from alex/symm-update-unchecked</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a92c23794149dc6bec8a8b1148c68bbe048851c9"><code>a92c237</code></a> clippy</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/e839496d9ed0bd4dcd4f1ec24e049cbe117ef1bb"><code>e839496</code></a> Don't leak when overwriting ex data</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/602d38dca7b8a22a355e1e53199d922742025c5c"><code>602d38d</code></a> Added <code>update_unchecked</code> to <code>symm::Crypter</code></li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/cf9681a55cabd4cb9f1475bde17b5079f2a0384e"><code>cf9681a</code></a> fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2096">#2096</a> -- deprecate <code>X509StoreRef::objects</code>, it is unsound</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.57...openssl-v0.10.60">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.57&new-version=0.10.60)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-uniffi-wrappers/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 21:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-uniffi-wrappers/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Release 0.1.1 with updated binary urls
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
        Created At 2023-11-23 04:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-uniffi-wrappers/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Release 0.1.1
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
        Created At 2023-11-23 04:27:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-uniffi-wrappers/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    export RevocationRegistryDefinitionPrivate as a local struct
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
        Created At 2023-11-23 02:52:49 +0000 UTC
    </div>
</div>

