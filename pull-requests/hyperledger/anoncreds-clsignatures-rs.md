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
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Bignum cleanups: remove code duplication and bignum context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Avoid duplication of `generates_semiprime_subgroup` and `random_qr` across bignum backends
- Eliminate use of BigNumContext outside of the openssl backend (always use a thread-local context)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 04:18:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.59 to 0.10.60
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.59 to 0.10.60.
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.59...openssl-v0.10.60">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.59&new-version=0.10.60)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-clsignatures-rs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 21:45:51 +0000 UTC
    </div>
</div>

