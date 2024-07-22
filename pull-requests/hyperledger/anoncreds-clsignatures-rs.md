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
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.64 to 0.10.66
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.64 to 0.10.66.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.66</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed invariant violation in <code>MemBio::get_buf</code> with empty results by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2266">sfackler/rust-openssl#2266</a></li>
<li>Release openssl v0.10.66 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2267">sfackler/rust-openssl#2267</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.65...openssl-v0.10.66">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.65...openssl-v0.10.66</a></p>
<h2>openssl-v0.10.65</h2>
<h2>What's Changed</h2>
<ul>
<li>don't emit rerun-if-changed when vendoring by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2177">sfackler/rust-openssl#2177</a></li>
<li>Prepare for openssl-sys 0.9.101 release by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2182">sfackler/rust-openssl#2182</a></li>
<li>don't emit rerun-if-changed unless the path exists and is readable by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2187">sfackler/rust-openssl#2187</a></li>
<li>Added support for LibreSSL 3.9.0 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2202">sfackler/rust-openssl#2202</a></li>
<li>Support stable LibreSSL 3.9.x by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2209">sfackler/rust-openssl#2209</a></li>
<li>openssl-sys 0.9.102 release by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2210">sfackler/rust-openssl#2210</a></li>
<li>Add repository field to openssl-macros crate by <a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2211">sfackler/rust-openssl#2211</a></li>
<li>Add missing openssl-sys dependency by <a href="https://github.com/pieterdd"><code>@​pieterdd</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2212">sfackler/rust-openssl#2212</a></li>
<li>Test OpenSSL 3.3.0-beta1 by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2216">sfackler/rust-openssl#2216</a></li>
<li>test against 3.3.0 final by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2218">sfackler/rust-openssl#2218</a></li>
<li>fix min-versions in CI by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2228">sfackler/rust-openssl#2228</a></li>
<li>Make X509_VAL opaque for LibreSSL 4.0.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2227">sfackler/rust-openssl#2227</a></li>
<li>Use the newer names for STACK_OF(T) functions with BoringSSL by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2231">sfackler/rust-openssl#2231</a></li>
<li>Only declare OpensslCallbacks in bindgen builds by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2234">sfackler/rust-openssl#2234</a></li>
<li>Fix building with latest BoringSSL by <a href="https://github.com/davidben"><code>@​davidben</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2230">sfackler/rust-openssl#2230</a></li>
<li>Emit rustc-check-cfg for nightly by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2235">sfackler/rust-openssl#2235</a></li>
<li>Configure OpenSSL data dir on vendored builds. by <a href="https://github.com/DanielSidhion"><code>@​DanielSidhion</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2122">sfackler/rust-openssl#2122</a></li>
<li>Add boringssl keylog callback support by <a href="https://github.com/mspublic"><code>@​mspublic</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2237">sfackler/rust-openssl#2237</a></li>
<li>Correct the name of the <code>pkgconf</code> package on some distros  by <a href="https://github.com/JonathanBrouwer"><code>@​JonathanBrouwer</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2253">sfackler/rust-openssl#2253</a></li>
<li>Add some OpenSSL 3 QUIC raw bindings by <a href="https://github.com/bdbai"><code>@​bdbai</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2257">sfackler/rust-openssl#2257</a></li>
<li>Initialize OpenSSL in MD constructors by <a href="https://github.com/sfackler"><code>@​sfackler</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2258">sfackler/rust-openssl#2258</a></li>
<li>Switch Pkey::from_ to use set1 functions by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2262">sfackler/rust-openssl#2262</a></li>
<li>Release openssl v0.10.65 and openssl-sys v0.9.103 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2265">sfackler/rust-openssl#2265</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2211">sfackler/rust-openssl#2211</a></li>
<li><a href="https://github.com/pieterdd"><code>@​pieterdd</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2212">sfackler/rust-openssl#2212</a></li>
<li><a href="https://github.com/DanielSidhion"><code>@​DanielSidhion</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2122">sfackler/rust-openssl#2122</a></li>
<li><a href="https://github.com/mspublic"><code>@​mspublic</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2237">sfackler/rust-openssl#2237</a></li>
<li><a href="https://github.com/JonathanBrouwer"><code>@​JonathanBrouwer</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2253">sfackler/rust-openssl#2253</a></li>
<li><a href="https://github.com/bdbai"><code>@​bdbai</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2257">sfackler/rust-openssl#2257</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.64...openssl-v0.10.65">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.64...openssl-v0.10.65</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/ad70a0bea581e53fc5086afffa5bdfe6eb1b5f49"><code>ad70a0b</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2267">#2267</a> from alex/bump-for-release</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/5ce473b4e56e8c68e11428d2e9fdb0abf984aa59"><code>5ce473b</code></a> Release openssl v0.10.66</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/aef36e0f3950653148d6644309ee41ccf16e02bb"><code>aef36e0</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2266">#2266</a> from alex/mem-bio-invariant</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/142deef717bad843fc04c5afb925bfd9e7dc4305"><code>142deef</code></a> Fixed invariant violation in <code>MemBio::get_buf</code> with empty results</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/32f150b05a8996a14561741bceab66a95043cd57"><code>32f150b</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2265">#2265</a> from alex/bump-for-release</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/98addd271ec1edf3cd598ed093c1c82a081b91eb"><code>98addd2</code></a> Release openssl v0.10.65 and openssl-sys v0.9.103</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/7c7958d436cec622c5af39063db8541b4641e73e"><code>7c7958d</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2262">#2262</a> from alex/pkey-api</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/d7b12ccf1f6864f99ba24080567b38bbd82f39ab"><code>d7b12cc</code></a> Switch Pkey::from_ to use set1 functions</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/22ffa9add64d962782d993fae0cd9b348d3b43cd"><code>22ffa9a</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2258">#2258</a> from sfackler/init-md</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/9de3794474d8440e80d362531f82d0d9ce07c22a"><code>9de3794</code></a> Initialize OpenSSL in MD constructors</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.64...openssl-v0.10.66">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.64&new-version=0.10.66)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-22 11:11:00 +0000 UTC
    </div>
</div>

