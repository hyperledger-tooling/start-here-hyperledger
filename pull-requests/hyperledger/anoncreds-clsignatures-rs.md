---
layout: default
title: anoncreds-clsignatures-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-clsignatures-rs
---

# anoncreds-clsignatures-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-clsignatures-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Remove separate m2^ value from non-revocation proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a breaking change to the proof format. The verifier *could* be made backward-compatible and accept the previous proof format.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 22:27:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Pairing optimizations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In my tests this reduces the time for proving and verification by 20-25% for revocable credentials (still in the ms range).

I found some inconsistencies with `sub_mod` and `mod_neg` for GroupOrderElement so there is a test added, and modifications to normalize the inner value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 16:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.54 to 0.10.55
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.54 to 0.10.55.
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
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.54...openssl-v0.10.55">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.54&new-version=0.10.55)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-clsignatures-rs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 22:58:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Cleanups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Include `openssl_bn` flag when `openssl_vendored` is used
- Remove duplicated tests
- Restore benchmark of prover witness creation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 16:43:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Handle invalid curve points
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also replaces some invalid test data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 16:23:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Perform issuer operations without accessing tails file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A revocation witness is now created during the issuance process, which matches the usual pattern of usage, and is much faster for the issuer to create than for the prover.

Large updates to the revocation registry may be faster depending on I/O speed (which is no longer a factor).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 00:06:50 +0000 UTC
    </div>
</div>

