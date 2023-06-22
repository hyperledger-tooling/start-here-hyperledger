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
                PR <a href="https://github.com/hyperledger/cacti/pull/2516" class=".btn">#2516</a>
            </td>
            <td>
                <b>
                     feat (cacti-cmd-gui-app): feat extend common cacti gui app to operate with fabric hyperledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add feature and options to switch in GUI app to visualize fabric hyperledger ledger data stored in supabase by persistence plugins

Depends on: https://github.com/hyperledger/cacti/pull/2331

Signed-off-by: Barnaba Pawelczak [barnaba.pawelczak@fujitsu.com](mailto:barnaba.pawelczak@fujitsu.com)

former  pull 2363
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 11:57:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2515" class=".btn">#2515</a>
            </td>
            <td>
                <b>
                    build(deps): bump openssl from 0.10.52 to 0.10.55 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.52 to 0.10.55.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.55</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix warnings from BoringSSL on Rust 1.70 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1948">sfackler/rust-openssl#1948</a></li>
<li>Honor OPENSSL_NO_OCB if OpenSSL was built this way by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1952">sfackler/rust-openssl#1952</a></li>
<li>Fix some deprecated patterns when using BoringSSL by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1945">sfackler/rust-openssl#1945</a></li>
<li>add get_asn1_flag to EcGroupRef by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1947">sfackler/rust-openssl#1947</a></li>
<li>Fixed type mutability on asn1_flag by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1954">sfackler/rust-openssl#1954</a></li>
<li>allow affine_coordinates on boring and libre by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1955">sfackler/rust-openssl#1955</a></li>
<li>add support for EVP_PKEY_derive_set_peer_ex in OpenSSL 3 by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1956">sfackler/rust-openssl#1956</a></li>
<li>Use type-safe wrappers instead of EVP_PKEY_assign by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1959">sfackler/rust-openssl#1959</a></li>
<li>add Nid::SM2 and pkey Id::SM2 by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1962">sfackler/rust-openssl#1962</a></li>
<li>Fix handling of empty host strings by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1968">sfackler/rust-openssl#1968</a></li>
<li>Remove old codes that belows supported Rust version. by <a href="https://github.com/tesuji"><code>@​tesuji</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1966">sfackler/rust-openssl#1966</a></li>
<li>Release openssl v0.10.55 and openssl-sys v0.9.89 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1970">sfackler/rust-openssl#1970</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/davidben"><code>@​davidben</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1952">sfackler/rust-openssl#1952</a></li>
<li><a href="https://github.com/tesuji"><code>@​tesuji</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1966">sfackler/rust-openssl#1966</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.54...openssl-v0.10.55">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.54...openssl-v0.10.55</a></p>
<h2>openssl-v0.10.54</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove converting PKCS#8 passphrase to CString by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1941">sfackler/rust-openssl#1941</a></li>
<li>Version bump for openssl v0.10.54 release by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1942">sfackler/rust-openssl#1942</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.53...openssl-v0.10.54">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.53...openssl-v0.10.54</a></p>
<h2>openssl-v0.10.53</h2>
<h2>What's Changed</h2>
<ul>
<li>Check for OPENSSL_NO_RC4 when using EVP_rc4 by <a href="https://github.com/oskirby"><code>@​oskirby</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1910">sfackler/rust-openssl#1910</a></li>
<li>Fix link errors for X509_get0_authority_xxx methods on Ubuntu/bionic by <a href="https://github.com/oskirby"><code>@​oskirby</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1909">sfackler/rust-openssl#1909</a></li>
<li>add X509::pathlen by <a href="https://github.com/zh-jq-b"><code>@​zh-jq-b</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1916">sfackler/rust-openssl#1916</a></li>
<li>Add bindings to SSL_bytes_to_cipher_list by <a href="https://github.com/RoastVeg"><code>@​RoastVeg</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1921">sfackler/rust-openssl#1921</a></li>
<li>Add boringssl hkdf derivation by <a href="https://github.com/AndrewScull"><code>@​AndrewScull</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1926">sfackler/rust-openssl#1926</a></li>
<li>add other name support by <a href="https://github.com/huettner94"><code>@​huettner94</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1915">sfackler/rust-openssl#1915</a></li>
<li>LibreSSL 3.8.0 by <a href="https://github.com/vishwin"><code>@​vishwin</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1935">sfackler/rust-openssl#1935</a></li>
<li>add Dsa<!-- raw HTML omitted --> with some helper functions by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1937">sfackler/rust-openssl#1937</a></li>
<li>reimplement Dsa::generate in terms of generate_params/generate_key by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1938">sfackler/rust-openssl#1938</a></li>
<li>Added DER serialization for <code>DSAPrivateKey</code> by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1939">sfackler/rust-openssl#1939</a></li>
<li>version bump 0.9.88 and 0.10.53 by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1940">sfackler/rust-openssl#1940</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/oskirby"><code>@​oskirby</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1910">sfackler/rust-openssl#1910</a></li>
<li><a href="https://github.com/zh-jq-b"><code>@​zh-jq-b</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1916">sfackler/rust-openssl#1916</a></li>
<li><a href="https://github.com/RoastVeg"><code>@​RoastVeg</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1921">sfackler/rust-openssl#1921</a></li>
<li><a href="https://github.com/huettner94"><code>@​huettner94</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1915">sfackler/rust-openssl#1915</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.52...openssl-v0.10.53">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.52...openssl-v0.10.53</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/d7dae6fb45aca39ae9793be6365d92e870e0b8ee"><code>d7dae6f</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1970">#1970</a> from alex/bump-for-release</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/983b9e210ac27895a39e0ed11a407b7936192313"><code>983b9e2</code></a> Release openssl v0.10.55 and openssl-sys v0.9.89</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/28b3925a329967f3ce1d3a1a7be2db55b75dd5e6"><code>28b3925</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1966">#1966</a> from tesuji/tidy-old-msrv</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/f03a2dc8074ff87bf8502194d955f6d60c8fff65"><code>f03a2dc</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1968">#1968</a> from sfackler/empty-domain-segfault</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/155b3dc71700d2ff31651bbc99b991765a718c4e"><code>155b3dc</code></a> Fix handling of empty host strings</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/978435639b0e1a93a953a7f211216c33aaedc450"><code>9784356</code></a> chore: simplify cfg attributes</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/8ab3c3f3a8e6102b734d849132aaeb9728cec669"><code>8ab3c3f</code></a> update min-version passed to bindgen</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/8587ff88431fc9ef495eda1b5bcfab4d310ef3cd"><code>8587ff8</code></a> chore: use pre-existing clean APIs instead</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/b1e16e927622b8c044f88de802523dead0b0ec5e"><code>b1e16e9</code></a> clippy: use strip_prefix instead of manually strip</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/fb5ae60cbb1dbbb2e34d47e113b25bc31f4acc37"><code>fb5ae60</code></a> clippy: remove unused allow attributes</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.52...openssl-v0.10.55">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.52&new-version=0.10.55)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-21 22:57:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2514" class=".btn">#2514</a>
            </td>
            <td>
                <b>
                    build(deps): bump openssl from 0.10.49 to 0.10.55 in /weaver/core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.49 to 0.10.55.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.55</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix warnings from BoringSSL on Rust 1.70 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1948">sfackler/rust-openssl#1948</a></li>
<li>Honor OPENSSL_NO_OCB if OpenSSL was built this way by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1952">sfackler/rust-openssl#1952</a></li>
<li>Fix some deprecated patterns when using BoringSSL by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1945">sfackler/rust-openssl#1945</a></li>
<li>add get_asn1_flag to EcGroupRef by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1947">sfackler/rust-openssl#1947</a></li>
<li>Fixed type mutability on asn1_flag by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1954">sfackler/rust-openssl#1954</a></li>
<li>allow affine_coordinates on boring and libre by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1955">sfackler/rust-openssl#1955</a></li>
<li>add support for EVP_PKEY_derive_set_peer_ex in OpenSSL 3 by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1956">sfackler/rust-openssl#1956</a></li>
<li>Use type-safe wrappers instead of EVP_PKEY_assign by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1959">sfackler/rust-openssl#1959</a></li>
<li>add Nid::SM2 and pkey Id::SM2 by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1962">sfackler/rust-openssl#1962</a></li>
<li>Fix handling of empty host strings by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1968">sfackler/rust-openssl#1968</a></li>
<li>Remove old codes that belows supported Rust version. by <a href="https://github.com/tesuji"><code>@​tesuji</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1966">sfackler/rust-openssl#1966</a></li>
<li>Release openssl v0.10.55 and openssl-sys v0.9.89 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1970">sfackler/rust-openssl#1970</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/davidben"><code>@​davidben</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1952">sfackler/rust-openssl#1952</a></li>
<li><a href="https://github.com/tesuji"><code>@​tesuji</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1966">sfackler/rust-openssl#1966</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.54...openssl-v0.10.55">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.54...openssl-v0.10.55</a></p>
<h2>openssl-v0.10.54</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove converting PKCS#8 passphrase to CString by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1941">sfackler/rust-openssl#1941</a></li>
<li>Version bump for openssl v0.10.54 release by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1942">sfackler/rust-openssl#1942</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.53...openssl-v0.10.54">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.53...openssl-v0.10.54</a></p>
<h2>openssl-v0.10.53</h2>
<h2>What's Changed</h2>
<ul>
<li>Check for OPENSSL_NO_RC4 when using EVP_rc4 by <a href="https://github.com/oskirby"><code>@​oskirby</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1910">sfackler/rust-openssl#1910</a></li>
<li>Fix link errors for X509_get0_authority_xxx methods on Ubuntu/bionic by <a href="https://github.com/oskirby"><code>@​oskirby</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1909">sfackler/rust-openssl#1909</a></li>
<li>add X509::pathlen by <a href="https://github.com/zh-jq-b"><code>@​zh-jq-b</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1916">sfackler/rust-openssl#1916</a></li>
<li>Add bindings to SSL_bytes_to_cipher_list by <a href="https://github.com/RoastVeg"><code>@​RoastVeg</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1921">sfackler/rust-openssl#1921</a></li>
<li>Add boringssl hkdf derivation by <a href="https://github.com/AndrewScull"><code>@​AndrewScull</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1926">sfackler/rust-openssl#1926</a></li>
<li>add other name support by <a href="https://github.com/huettner94"><code>@​huettner94</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1915">sfackler/rust-openssl#1915</a></li>
<li>LibreSSL 3.8.0 by <a href="https://github.com/vishwin"><code>@​vishwin</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1935">sfackler/rust-openssl#1935</a></li>
<li>add Dsa<!-- raw HTML omitted --> with some helper functions by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1937">sfackler/rust-openssl#1937</a></li>
<li>reimplement Dsa::generate in terms of generate_params/generate_key by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1938">sfackler/rust-openssl#1938</a></li>
<li>Added DER serialization for <code>DSAPrivateKey</code> by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1939">sfackler/rust-openssl#1939</a></li>
<li>version bump 0.9.88 and 0.10.53 by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1940">sfackler/rust-openssl#1940</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/oskirby"><code>@​oskirby</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1910">sfackler/rust-openssl#1910</a></li>
<li><a href="https://github.com/zh-jq-b"><code>@​zh-jq-b</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1916">sfackler/rust-openssl#1916</a></li>
<li><a href="https://github.com/RoastVeg"><code>@​RoastVeg</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1921">sfackler/rust-openssl#1921</a></li>
<li><a href="https://github.com/huettner94"><code>@​huettner94</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1915">sfackler/rust-openssl#1915</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.52...openssl-v0.10.53">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.52...openssl-v0.10.53</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/d7dae6fb45aca39ae9793be6365d92e870e0b8ee"><code>d7dae6f</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1970">#1970</a> from alex/bump-for-release</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/983b9e210ac27895a39e0ed11a407b7936192313"><code>983b9e2</code></a> Release openssl v0.10.55 and openssl-sys v0.9.89</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/28b3925a329967f3ce1d3a1a7be2db55b75dd5e6"><code>28b3925</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1966">#1966</a> from tesuji/tidy-old-msrv</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/f03a2dc8074ff87bf8502194d955f6d60c8fff65"><code>f03a2dc</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1968">#1968</a> from sfackler/empty-domain-segfault</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/155b3dc71700d2ff31651bbc99b991765a718c4e"><code>155b3dc</code></a> Fix handling of empty host strings</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/978435639b0e1a93a953a7f211216c33aaedc450"><code>9784356</code></a> chore: simplify cfg attributes</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/8ab3c3f3a8e6102b734d849132aaeb9728cec669"><code>8ab3c3f</code></a> update min-version passed to bindgen</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/8587ff88431fc9ef495eda1b5bcfab4d310ef3cd"><code>8587ff8</code></a> chore: use pre-existing clean APIs instead</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/b1e16e927622b8c044f88de802523dead0b0ec5e"><code>b1e16e9</code></a> clippy: use strip_prefix instead of manually strip</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/fb5ae60cbb1dbbb2e34d47e113b25bc31f4acc37"><code>fb5ae60</code></a> clippy: remove unused allow attributes</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.49...openssl-v0.10.55">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.49&new-version=0.10.55)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-21 22:56:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2513" class=".btn">#2513</a>
            </td>
            <td>
                <b>
                    fix(iin): changed the way to install dependencies in dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue #2500 
Changed the line 24 of the dockerfile, to remove the use of the erroneous setup.py to replace it with a full line of all the dependencies modeled from the same file. 

@VRamakrishna Kindly check 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 14:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2512" class=".btn">#2512</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.9.1 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.9.1 to 4.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p</a>.</p>
</blockquote>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.2/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.2 (2023-06-16)</h2>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e50c24f5839db17f46991478384bfda14acfb830"><code>e50c24f</code></a> Release v4.9.2 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4364">#4364</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4d2383e17186be3e8ccf5a442e9686ecc7de1c55"><code>4d2383e</code></a> Merge pull request from GHSA-wprv-93r4-jj2p</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/f03420b5c77ae3cfa73fce4ffc7f4778cfa2b503"><code>f03420b</code></a> Remove automatic conflict resolution for merge from release branch (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4362">#4362</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ded8c9eedb9a03b0703b65d430e6d0076cb0e444"><code>ded8c9e</code></a> Update index.adoc (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4336">#4336</a>)</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.9.1...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.9.1&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-19 20:16:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2511" class=".btn">#2511</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.9.1 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.9.1 to 4.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p</a>.</p>
</blockquote>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/v4.9.2/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.2 (2023-06-16)</h2>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/bc95521e34dcd49792065e264a7ad2b5a86f0091"><code>bc95521</code></a> Transpile e50c24f5</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/e7d20ee1cecbfa36bd75ffb4b2e5dad4c47801f1"><code>e7d20ee</code></a> Transpile 4d2383e1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/8aac85b00f7f0a96b431a85ab96db81d356514a7"><code>8aac85b</code></a> Transpile f03420b5</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/953a201b0b60f70337ea4d2245500552f58fb5d5"><code>953a201</code></a> Transpile ded8c9ee</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.9.1...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.9.1&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-19 19:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2466" class=".btn">#2466</a>
            </td>
            <td>
                <b>
                    ci(github): evaluate cache viability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WORK IN PROGRESS

Fixes #2117

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 05:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2465" class=".btn">#2465</a>
            </td>
            <td>
                <b>
                    test(fabric-all-in-one): fix sed write error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrade the base images to docker:24.0.2-dind
which contain the fix for the cgroup v2 problems.

The images built locally from this commit are pushed to ghcr.io as

ghcr.io/hyperledger/cactus-fabric-all-in-one:2023-06-16-d436ef26e-issue2464-dind-v24
and
ghcr.io/hyperledger/cactus-fabric2-all-in-one:2023-06-16-d436ef26e-issue2464-dind-v24

Additional context:

The root cause analysis can be found here [1][2]
which states that the solution is to upgrade the
dind image to a version of at least 20.10.16

[1] docker-library/docker#308
[2] testcontainers/dind-drone-plugin#18

Fixes #2464

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 03:06:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2462" class=".btn">#2462</a>
            </td>
            <td>
                <b>
                    build(codegen): fix openapi concurrent jar download
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a script to  warm up the file-system cache where the
.jar files are downloaded (which contain the OpenAPI generator)

This way the .jar download does not happen concurrently for 26
packages but instead just the one time right before the codegen
script is executed.

IMPORTANT NOTE: If you change the OpenAPI generator version
that is being used by the project from the current v5.2.1 and v6.3.0
then these warm-up scripts must also be updated at the same time
otherwise the same issue that we are fixing here now will creep back
in immediately.

 Fixes #2461

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 05:10:54 +0000 UTC
    </div>
</div>

