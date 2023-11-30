---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1078" class=".btn">#1078</a>
            </td>
            <td>
                <b>
                    feat: implement RecordWallet for askar 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                extracted from https://github.com/hyperledger/aries-vcx/pull/1063 as it was growing too large.

I can't really set https://github.com/hyperledger/aries-vcx/pull/1071 as a base for merge since I opened it from my fork, but the commits here are separated, so it should still be possible to view only the implementation part with a relative ease.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 14:22:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    fix(message_macros):  explicit lifetime declaration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add explicit static lifetime rather than let the compiler guess. As per suggestion of lint `ELIDED_LIFETIMES_IN_ASSOCIATED_CONSTANT`

https://github.com/rust-lang/rust/issues/115010

This should fix the clippy warning we are seeing
(the ones point to `MessageType` trait derive macro)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 17:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1076" class=".btn">#1076</a>
            </td>
            <td>
                <b>
                    fix(mediator-client): use standard endpoint intended for mediator clients
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/decentralized-identity/didcomm-messaging/blob/main/extensions/return_route/main.md#queue-transport
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 16:10:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1075" class=".btn">#1075</a>
            </td>
            <td>
                <b>
                    draft: change: simplify didcore components, did-exchange protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Yet quite a bit of work outstanding to get this even compiling. WIP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 14:09:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1074" class=".btn">#1074</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.57 to 0.10.60
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 21:45:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1073" class=".btn">#1073</a>
            </td>
            <td>
                <b>
                    docs: Update location of aries agents
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
        Created At 2023-11-28 12:16:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    WIP: feat(mediator): Better errors for MediatorPersistence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the first part of effort to introduce better structured errors to the mediator. 
We are using this_error library for the same. And designing the error hierarchy/mapping from bottom up. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 08:57:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1071" class=".btn">#1071</a>
            </td>
            <td>
                <b>
                    feat: Add new Wallet trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A new trait for wallet heavily inspired by #1042. Associated types are leveraged to provide flexibility to various implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-27 14:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    refactor: encryption envelope
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - minor refactoring of encryption envelope which came up in progress of improving did-exchange implementation - a lot more can be done here (and will)
- On top of https://github.com/hyperledger/aries-vcx/pull/1069, please merge that first for clean changelog
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-26 21:34:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1069" class=".btn">#1069</a>
            </td>
            <td>
                <b>
                    feature: Derive Display for all aries messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">review:level-2</span>
            </td>
            <td>
                - Derives `Display` trait for all aries messages 
- Removed default Decorators type parameter `D = NoDecorators` - turned out somewhat problematic in conjunction with the custom `Display` proc macro. Not a big price to pay though, only slightly inconveniences developer working in `messages` crate, but not `messages` consumers.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 23:16:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1068" class=".btn">#1068</a>
            </td>
            <td>
                <b>
                    refactor: uniffi project reorganize
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this PR addresses major reorganize of uniffi project in accordance to #1045 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 21:57:46 +0000 UTC
    </div>
</div>

