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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1196" class=".btn">#1196</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.195 to 1.0.203 in /aries/misc/anoncreds_types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.195 to 1.0.203.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.203</h2>
<ul>
<li>Documentation improvements (<a href="https://redirect.github.com/serde-rs/serde/issues/2747">#2747</a>)</li>
</ul>
<h2>v1.0.202</h2>
<ul>
<li>Provide public access to RenameAllRules in serde_derive_internals (<a href="https://redirect.github.com/serde-rs/serde/issues/2743">#2743</a>)</li>
</ul>
<h2>v1.0.201</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/serde-rs/serde/issues/2737">#2737</a>)</li>
</ul>
<h2>v1.0.200</h2>
<ul>
<li>Fix formatting of &quot;invalid type&quot; and &quot;invalid value&quot; deserialization error messages containing NaN or infinite floats (<a href="https://redirect.github.com/serde-rs/serde/issues/2733">#2733</a>, thanks <a href="https://github.com/jamessan"><code>@​jamessan</code></a>)</li>
</ul>
<h2>v1.0.199</h2>
<ul>
<li>Fix ambiguous associated item when <code>forward_to_deserialize_any!</code> is used on an enum with <code>Error</code> variant (<a href="https://redirect.github.com/serde-rs/serde/issues/2732">#2732</a>, thanks <a href="https://github.com/aatifsyed"><code>@​aatifsyed</code></a>)</li>
</ul>
<h2>v1.0.198</h2>
<ul>
<li>Support serializing and deserializing <code>Saturating&lt;T&gt;</code> (<a href="https://redirect.github.com/serde-rs/serde/issues/2709">#2709</a>, thanks <a href="https://github.com/jbethune"><code>@​jbethune</code></a>)</li>
</ul>
<h2>v1.0.197</h2>
<ul>
<li>Fix unused_imports warnings when compiled by rustc 1.78</li>
<li>Optimize code size of some Display impls (<a href="https://redirect.github.com/serde-rs/serde/issues/2697">#2697</a>, thanks <a href="https://github.com/nyurik"><code>@​nyurik</code></a>)</li>
</ul>
<h2>v1.0.196</h2>
<ul>
<li>Improve formatting of &quot;invalid type&quot; error messages involving floats (<a href="https://redirect.github.com/serde-rs/serde/issues/2682">#2682</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/d5bc546ca53be0b31984a06a8ad587cbea4ca5ce"><code>d5bc546</code></a> Release 1.0.203</li>
<li><a href="https://github.com/serde-rs/serde/commit/45ae217728e9163103c47f9bd04502368caaf446"><code>45ae217</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2747">#2747</a> from dtolnay/variadic</li>
<li><a href="https://github.com/serde-rs/serde/commit/b7b97dda7333baf6474517e3646754be54e3796b"><code>b7b97dd</code></a> Unindent implementation inside tuple_impl_body macro</li>
<li><a href="https://github.com/serde-rs/serde/commit/5d3c563d469ef36ce5a01f1612f53883fee20db5"><code>5d3c563</code></a> Document tuple impls as fake variadic</li>
<li><a href="https://github.com/serde-rs/serde/commit/376185458b48aeb2774ecc26422cc9499e564117"><code>3761854</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2745">#2745</a> from dtolnay/docsrs</li>
<li><a href="https://github.com/serde-rs/serde/commit/a8f14840ab3ff58f533cd27d0f91955d57f12a65"><code>a8f1484</code></a> Rely on docs.rs to define --cfg=docsrs by default</li>
<li><a href="https://github.com/serde-rs/serde/commit/9e32a40b1c745d1d67d451cc983fab5751d394a5"><code>9e32a40</code></a> Release 1.0.202</li>
<li><a href="https://github.com/serde-rs/serde/commit/87f635e54d5359fa0eb94b1ef0a684ee3d24cb85"><code>87f635e</code></a> Release serde_derive_internals 0.29.1</li>
<li><a href="https://github.com/serde-rs/serde/commit/d4b2dfbde288e0ba5d4dc7852e1b8029208cf9b6"><code>d4b2dfb</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2743">#2743</a> from dtolnay/renameallrules</li>
<li><a href="https://github.com/serde-rs/serde/commit/f6ab0bc56f3df6d03974d233ffce352b0725ae09"><code>f6ab0bc</code></a> Provide public access to RenameAllRules in serde_derive_internals</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/serde/compare/v1.0.195...v1.0.203">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.195&new-version=1.0.203)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1195" class=".btn">#1195</a>
            </td>
            <td>
                <b>
                    chore(deps): update sodiumoxide requirement from 0.0.16 to 0.2.7 in /aries/misc/legacy/libvdrtools/indy-utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [sodiumoxide](https://github.com/sodiumoxide/sodiumoxide) to permit the latest version.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sodiumoxide/sodiumoxide/blob/master/CHANGELOG.md">sodiumoxide's changelog</a>.</em></p>
<blockquote>
<h1>0.2.7 (Jun 21, 2021)</h1>
<ul>
<li>Add ed25519 to x25519 conversion methods (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/456">#456</a>)</li>
<li>Update prebuilt windows binaries to those published at 2020-12-31 at libsodium.org</li>
<li>Update libsodium submodule to stable branch commit 8acd227</li>
<li>Fix no_std build</li>
<li>Expose the sodium_pad and sodium_unpad functions</li>
<li>Switch from using xcopy to using walkdir + fs::copy in build script</li>
<li>Add support for the AES256-GCM AEAD construction</li>
<li>Expose randombytes_buf_deterministic function (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/431">#431</a>)</li>
</ul>
<h1>0.2.6 (Jul 19, 2020)</h1>
<ul>
<li>Remove support for using vcpkg for windows (msvc) builds since it was undertested</li>
<li>Update prebuilt windows binaries to those published at 2020-06-30 at libsodium.org</li>
<li>Update libsodium submodule to latest stable branch commit. (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/420">#420</a>, <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/400">#400</a>)</li>
<li>Avoid ptr_cast feature as it was not yet stable in Rust 1.36. (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/408">#408</a>)</li>
<li>Fix build script by using the correct arguments for xcopy (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/407">#407</a>)</li>
<li>Avoid dev dependencies on tar and libflate by including libsodium as a Git submodule. (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/393">#393</a>)</li>
<li>Add bindings to KDF functions (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/351">#351</a>)</li>
<li>Expose libsodium's hexadecimal encoding/decoding helper functions (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/390">#390</a>)</li>
<li>Expose libsodium's Base64 encoding/decoding helper functions (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/391">#391</a>)</li>
<li>remove ill-advised gen_nonce functions (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/395">#395</a>)</li>
</ul>
<h1>0.2.5 (Oct 11, 2019)</h1>
<ul>
<li>Fix Digest PartialEq (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/381">#381</a>)</li>
<li>Fix compiler warnings (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/380">#380</a>)</li>
<li>Use copy_from_slice instead of manual loop where possible (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/378">#378</a>)</li>
</ul>
<h1>0.2.4 (Sep 3, 2019)</h1>
<ul>
<li>Fixed erronoeus dependency on older libsodium-sys</li>
<li>Fixed use of deprecated try! macro (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/369">#369</a>)</li>
</ul>
<h1>0.2.3 (Sep 1, 2019)</h1>
<ul>
<li>Allow reusing Vec for secretstream (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/357">#357</a>)</li>
<li>Replace mem::uninitialized with MaybeUninit (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/350">#350</a>, <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/356">#356</a>)</li>
<li>Fix warning about deprecated uint64_t (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/358">#358</a>)</li>
<li>Fix path to ./configure script (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/355">#355</a>)</li>
<li>Add API to derive Ed25519 public keys from secret keys (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/345">#345</a>)</li>
<li>Add DEP_SODIUM_INCLUDE &amp; DEP_SODIUM_LIB env variables (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/344">#344</a>)</li>
<li>Update libsodium to 1.0.18 (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/342">#342</a>)</li>
</ul>
<h1>0.2.2 (May 16, 2019)</h1>
<ul>
<li>Bundle libsodium .a .lib for win &amp; cygwin (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/332">#332</a>)</li>
<li>Add <code>AsRef&lt;[u8]&gt;</code> for newtypes (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/323">#323</a>)</li>
<li>Implement memory locking and unlocking (<a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/324">#324</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/179e13c5bc3941e46f87f6748bfb3f9ed95936ba"><code>179e13c</code></a> Merge pull request <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/466">#466</a> from ValHeimer/release_0_2_7</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/139c67bfb0dea5ea35d561443f92c3e3347d7761"><code>139c67b</code></a> Bump version (0.2.7) and update changelog</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/f067482076597a03c957f2260100fbe709c9a475"><code>f067482</code></a> Merge <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/456">#456</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/f3fec5da6d22d0b89fa05f882c1ca33e316e5dad"><code>f3fec5d</code></a> Run cargo fmt</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/3ee2795e6ee97a5aca80dedd4eb82f84ae6427e7"><code>3ee2795</code></a> Make PR <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/362">#362</a> requested changes</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/dfd876979da10e7864abfe0e7aaa22be69825755"><code>dfd8769</code></a> apply cargo fmt</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/c7cfb9e8a69ea156369350abc32c11288b2adbf7"><code>c7cfb9e</code></a> added ed25519 to x25519 conversion via TryInto on &amp;T</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/9f6a18d40a4db253edfebac9f2ce5c22d09b1f47"><code>9f6a18d</code></a> Merge <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/455">#455</a></li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/a440d011196ae10ececd92abeb07943bd5cfab80"><code>a440d01</code></a> Do not call Vec::set_len before the data is initialised</li>
<li><a href="https://github.com/sodiumoxide/sodiumoxide/commit/dc1d2a87e0e95af2f6055f33fe953e24c0e2bd85"><code>dc1d2a8</code></a> Merge <a href="https://redirect.github.com/sodiumoxide/sodiumoxide/issues/398">#398</a></li>
<li>Additional commits viewable in <a href="https://github.com/sodiumoxide/sodiumoxide/compare/sodiumoxide-0.0.16...0.2.7">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-01 02:33:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1194" class=".btn">#1194</a>
            </td>
            <td>
                <b>
                    chore(deps): bump regex from 1.10.3 to 1.10.4 in /aries/misc/anoncreds_types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [regex](https://github.com/rust-lang/regex) from 1.10.3 to 1.10.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/regex/commit/aa2d8bd8be283471b17b4ab6faeae5b751553572"><code>aa2d8bd</code></a> 1.10.4</li>
<li><a href="https://github.com/rust-lang/regex/commit/088d7f3269665a11aabadd89335eb09316e9c785"><code>088d7f3</code></a> api: add Cow guarantee to replace API</li>
<li><a href="https://github.com/rust-lang/regex/commit/a5ae35153a6ec61e64cb297155f7d91c11b629c7"><code>a5ae351</code></a> regex-automata-0.4.6</li>
<li><a href="https://github.com/rust-lang/regex/commit/9cf4a42a9361f42d9aa6afd1245c0e37dc0c8771"><code>9cf4a42</code></a> automata: fix bug where reverse NFA lacked an unanchored prefix</li>
<li><a href="https://github.com/rust-lang/regex/commit/10fe722a3fcfdc17068b21f3262189cc52227bb5"><code>10fe722</code></a> style: clean up some recent lint violations</li>
<li><a href="https://github.com/rust-lang/regex/commit/d7f9347f2a8a7f4e7583c88876411da12a09b572"><code>d7f9347</code></a> regex-automata-0.4.5</li>
<li><a href="https://github.com/rust-lang/regex/commit/07ef7f1550d59a548ee58631cf2bca263e67cb8e"><code>07ef7f1</code></a> automata: make additional prefileter metadata public</li>
<li>See full diff in <a href="https://github.com/rust-lang/regex/compare/1.10.3...1.10.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=regex&package-manager=cargo&previous-version=1.10.3&new-version=1.10.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1193" class=".btn">#1193</a>
            </td>
            <td>
                <b>
                    chore(deps): bump androidx.activity:activity-compose from 1.5.1 to 1.9.0 in /aries/agents/mobile_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps androidx.activity:activity-compose from 1.5.1 to 1.9.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=androidx.activity:activity-compose&package-manager=gradle&previous-version=1.5.1&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1192" class=".btn">#1192</a>
            </td>
            <td>
                <b>
                    chore(deps): bump alpine from 3.15.4 to 3.20.0 in /aries/agents/aath-backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps alpine from 3.15.4 to 3.20.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=alpine&package-manager=docker&previous-version=3.15.4&new-version=3.20.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    chore(deps): bump alpine from 3.17.1 to 3.20.0 in /.github/ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps alpine from 3.17.1 to 3.20.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=alpine&package-manager=docker&previous-version=3.17.1&new-version=3.20.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    chore(deps): bump com.google.code.gson:gson from 2.8.9 to 2.11.0 in /aries/agents/mobile_demo/app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [com.google.code.gson:gson](https://github.com/google/gson) from 2.8.9 to 2.11.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/google/gson/releases">com.google.code.gson:gson's releases</a>.</em></p>
<blockquote>
<h2>Gson 2.11.0</h2>
<h1>Most important changes</h1>
<ul>
<li>Added default ProGuard / R8 rules (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2397">#2397</a>, <a href="https://redirect.github.com/google/gson/issues/2420">#2420</a>; <a href="https://github.com/sgjesse"><code>@​sgjesse</code></a>, <a href="https://redirect.github.com/google/gson/issues/2448">#2448</a>; <a href="https://github.com/sfreilich"><code>@​sfreilich</code></a>)<br />
If you are using ProGuard or R8 (for example for Android projects) you might not need any special Gson configuration anymore if your classes have a no-args constructor and use <code>@SerializedName</code> for their fields.</li>
<li>On Android, Gson now requires API level 21 or newer</li>
<li>Added new <code>Strictness</code> API (<a href="https://github.com/marten-voorberg"><code>@​marten-voorberg</code></a> &amp; fellow students, <a href="https://redirect.github.com/google/gson/issues/2437">#2437</a>)<br />
Some of Gson's API is still lenient by default, but you can now use the newly added methods <code>GsonBuilder#setStrictness</code>, <code>JsonReader#setStrictness</code> and <code>JsonWriter#setStrictness</code> with <code>Strictness.STRICT</code> to override this behavior and to instead strictly adhere to the JSON specification when parsing.</li>
<li>New <code>FormattingStyle</code> class to allow configuring line breaks in JSON output (<a href="https://github.com/mihnita"><code>@​mihnita</code></a>, <a href="https://redirect.github.com/google/gson/issues/2231">#2231</a>)<br />
Can be set using <code>GsonBuilder#setFormattingStyle</code> and <code>JsonWriter#setFormattingStyle</code>.</li>
<li><code>TypeToken</code> can no longer capture type variables by default (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2376">#2376</a>)<br />
This was previously a common source of issues. The newly thrown exception refers to a <a href="https://github.com/google/gson/blob/main/Troubleshooting.md#typetoken-type-variable">Troubleshooting Guide article</a> which explains this in more detail and provides suggestions for updating affected code.</li>
<li>Added serialization support for anonymous and local classes with a custom adapter (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2498">#2498</a>)<br />
This affects for example <code>List</code> implementations returned by libraries such as Guava which are implemented as anonymous class, which were previously serialized as <code>null</code>. Anonymous and local classes without custom adapter will still be serialized as <code>null</code>.</li>
<li>Added dependency on <code>com.google.errorprone:error_prone_annotations</code><br />
Your project can use Maven or Gradle dependency exclusions to remove the transitive error_prone_annotations dependency from Gson. Or if you are manually maintaining dependencies as JARs in your project you can omit error_prone_annotations. And it should still work correctly.<br />
But Gson itself does declare it as a required dependency, and if you don't perform any custom configuration, then Maven or Gradle will by default try to download and use it.</li>
<li>Many exception messages now refer to the <a href="https://github.com/google/gson/blob/main/Troubleshooting.md">Troubleshooting Guide</a> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2357">#2357</a>)<br />
Feedback regarding the Troubleshooting Guide is appreciated!</li>
<li>Officially documented that JVM languages other than Java might not be fully supported, see the <a href="https://github.com/google/gson/blob/main/README.md">README</a>.</li>
<li>Guarantee that <code>JsonElement#toString</code> produces JSON output (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2659">#2659</a>)</li>
</ul>
<h1>Other changes</h1>
<h2>Bug fixes</h2>
<ul>
<li>Fixed incorrect <code>JsonPrimitive#equals</code> results for large <code>BigInteger</code> values (<a href="https://github.com/MaicolAntali"><code>@​MaicolAntali</code></a>, <a href="https://redirect.github.com/google/gson/issues/2311">#2311</a>)</li>
<li>Fixed incorrect <code>JsonPrimitive#equals</code> results for large <code>BigDecimal</code> values (<a href="https://github.com/MaicolAntali"><code>@​MaicolAntali</code></a>, <a href="https://redirect.github.com/google/gson/issues/2364">#2364</a>)</li>
<li>Fixed <code>JsonReader</code> throwing <code>NumberFormatException</code> instead of <code>MalformedJsonException</code> for malformed Unicode escape sequences (<a href="https://github.com/MaicolAntali"><code>@​MaicolAntali</code></a>, <a href="https://redirect.github.com/google/gson/issues/2337">#2337</a>)</li>
<li>Fixed <code>TypeToken#getParameterized</code> returning bogus <code>ParameterizedType</code> for non-generic types (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2447">#2447</a>)</li>
<li>Fixed Java Record adapter not working for GraalVM Native Image (<a href="https://github.com/eamonnmcmanus"><code>@​eamonnmcmanus</code></a>, <a href="https://redirect.github.com/google/gson/issues/2465">#2465</a>)</li>
<li>Fixed <code>JsonWriter#name</code> not throwing exception when no JSON object is currently being written (<a href="https://github.com/shivam-sehgal"><code>@​shivam-sehgal</code></a>, <a href="https://redirect.github.com/google/gson/issues/2475">#2475</a>; <a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2476">#2476</a>)</li>
<li>Fixed <code>Gson#getDelegateAdapter</code> not working properly for <code>@JsonAdapter</code> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2435">#2435</a>)<br />
Note that <code>null</code> is now not allowed as <code>skipPast</code> value anymore, which was previously allowed but undocumented.</li>
<li>Fixed <code>GsonBuilder</code> not rejecting type adapters for <code>Object</code> and <code>JsonElement</code>, whose default adapters cannot be overridden (<a href="https://github.com/sachinp97"><code>@​sachinp97</code></a>; <a href="https://redirect.github.com/google/gson/issues/2479">#2479</a>)</li>
<li>Fixed no limits being enforced when deserializing <code>BigDecimal</code> and <code>BigInteger</code> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2510">#2510</a>)<br />
The new limits prevent potential performance problems when user code uses the deserialized numbers. Gson itself was and is not affected by these performance problems. The limits should be high enough to not cause issues for most use cases, but feedback is appreciated.</li>
<li>Fixed <code>GsonBuilder#setDateFormat</code> not rejecting invalid date formats (<a href="https://github.com/Carpe-Wang"><code>@​Carpe-Wang</code></a>, <a href="https://redirect.github.com/google/gson/issues/2538">#2538</a>)</li>
<li>Fixed <code>GsonBuilder#setDateFormat</code> not rejecting invalid date styles (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2545">#2545</a>)</li>
<li>Fixed <code>GsonBuilder#setDateFormat</code> ignoring partial DEFAULT style (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2556">#2556</a>)</li>
<li>Fixed <code>TypeToken#isAssignableFrom</code> throwing <code>AssertionError</code> in some cases (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2544">#2544</a>)</li>
<li>Fixed date adapters not restoring time zone after parsing (<a href="https://github.com/Carpe-Wang"><code>@​Carpe-Wang</code></a>, <a href="https://redirect.github.com/google/gson/issues/2549">#2549</a>)</li>
<li>Fixed <code>TypeToken#equals</code> erroneously returning <code>false</code> for equal generic type parameters in some cases (<a href="https://github.com/d-william"><code>@​d-william</code></a>, <a href="https://redirect.github.com/google/gson/issues/2599">#2599</a>)</li>
<li>Fixed incorrect inherited URLs in <code>pom.xml</code> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2351">#2351</a>)</li>
</ul>
<h2>Performance improvements</h2>
<ul>
<li>Slightly reduce memory usage for reflection-based adapter (<a href="https://github.com/sembseth"><code>@​sembseth</code></a>, <a href="https://redirect.github.com/google/gson/issues/2325">#2325</a>; <a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2440">#2440</a>)</li>
<li>Improved parsing speed of <code>ToNumberPolicy#LONG_OR_DOUBLE</code> (<a href="https://github.com/ctasada"><code>@​ctasada</code></a>, <a href="https://redirect.github.com/google/gson/issues/2674">#2674</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/google/gson/blob/main/CHANGELOG.md">com.google.code.gson:gson's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>The change log for versions newer than 2.10 is available only on the <a href="https://github.com/google/gson/releases">GitHub Releases page</a>.</p>
<h2>Version 2.10</h2>
<ul>
<li>Support for serializing and deserializing Java records, on Java ≥ 16. (<a href="https://redirect.github.com/google/gson/pull/2201">google/gson#2201</a>)</li>
<li>Add <code>JsonArray.asList</code> and <code>JsonObject.asMap</code> view methods (<a href="https://redirect.github.com/google/gson/pull/2225">google/gson#2225</a>)</li>
<li>Fix <code>TypeAdapterRuntimeTypeWrapper</code> not detecting reflective <code>TreeTypeAdapter</code> and <code>FutureTypeAdapter</code> (<a href="https://redirect.github.com/google/gson/pull/1787">google/gson#1787</a>)</li>
<li>Improve <code>JsonReader.skipValue()</code> (<a href="https://redirect.github.com/google/gson/pull/2062">google/gson#2062</a>)</li>
<li>Perform numeric conversion for primitive numeric type adapters (<a href="https://redirect.github.com/google/gson/pull/2158">google/gson#2158</a>)</li>
<li>Add <code>Gson.fromJson(..., TypeToken)</code> overloads (<a href="https://redirect.github.com/google/gson/pull/1700">google/gson#1700</a>)</li>
<li>Fix changes to <code>GsonBuilder</code> affecting existing <code>Gson</code> instances (<a href="https://redirect.github.com/google/gson/pull/1815">google/gson#1815</a>)</li>
<li>Make <code>JsonElement</code> conversion methods more consistent and fix javadoc (<a href="https://redirect.github.com/google/gson/pull/2178">google/gson#2178</a>)</li>
<li>Throw <code>UnsupportedOperationException</code> when <code>JsonWriter.jsonValue</code> is not supported (<a href="https://redirect.github.com/google/gson/pull/1651">google/gson#1651</a>)</li>
<li>Disallow <code>JsonObject</code> <code>Entry.setValue(null)</code> (<a href="https://redirect.github.com/google/gson/pull/2167">google/gson#2167</a>)</li>
<li>Fix <code>TypeAdapter.toJson</code> throwing AssertionError for custom IOException (<a href="https://redirect.github.com/google/gson/pull/2172">google/gson#2172</a>)</li>
<li>Convert null to JsonNull for <code>JsonArray.set</code> (<a href="https://redirect.github.com/google/gson/pull/2170">google/gson#2170</a>)</li>
<li>Fixed nullSafe usage. (<a href="https://redirect.github.com/google/gson/pull/1555">google/gson#1555</a>)</li>
<li>Validate <code>TypeToken.getParameterized</code> arguments (<a href="https://redirect.github.com/google/gson/pull/2166">google/gson#2166</a>)</li>
<li>Fix <a href="https://redirect.github.com/google/gson/issues/1702">#1702</a>: Gson.toJson creates CharSequence which does not implement toString (<a href="https://redirect.github.com/google/gson/pull/1703">google/gson#1703</a>)</li>
<li>Prefer existing adapter for concurrent <code>Gson.getAdapter</code> calls (<a href="https://redirect.github.com/google/gson/pull/2153">google/gson#2153</a>)</li>
<li>Improve <code>ArrayTypeAdapter</code> for <code>Object[]</code> (<a href="https://redirect.github.com/google/gson/pull/1716">google/gson#1716</a>)</li>
<li>Improve <code>AppendableWriter</code> performance (<a href="https://redirect.github.com/google/gson/pull/1706">google/gson#1706</a>)</li>
</ul>
<h2>Version 2.9.1</h2>
<ul>
<li>Make <code>Object</code> and <code>JsonElement</code> deserialization iterative rather than
recursive (<a href="https://redirect.github.com/google/gson/pull/1912">google/gson#1912</a>)</li>
<li>Added parsing support for enum that has overridden toString() method (<a href="https://redirect.github.com/google/gson/pull/1950">google/gson#1950</a>)</li>
<li>Removed support for building Gson with Gradle (<a href="https://redirect.github.com/google/gson/pull/2081">google/gson#2081</a>)</li>
<li>Removed obsolete <code>codegen</code> hierarchy (<a href="https://redirect.github.com/google/gson/pull/2099">google/gson#2099</a>)</li>
<li>Add support for reflection access filter (<a href="https://redirect.github.com/google/gson/pull/1905">google/gson#1905</a>)</li>
<li>Improve <code>TypeToken</code> creation validation (<a href="https://redirect.github.com/google/gson/pull/2072">google/gson#2072</a>)</li>
<li>Add explicit support for <code>float</code> in <code>JsonWriter</code> (<a href="https://redirect.github.com/google/gson/pull/2130">google/gson#2130</a>, <a href="https://redirect.github.com/google/gson/pull/2132">google/gson#2132</a>)</li>
<li>Fail when parsing invalid local date (<a href="https://redirect.github.com/google/gson/pull/2134">google/gson#2134</a>)</li>
</ul>
<p>Also many small improvements to javadoc.</p>
<h2>Version 2.9.0</h2>
<p><strong>The minimum supported Java version changes from 6 to 7.</strong></p>
<ul>
<li>Change target Java version to 7 (<a href="https://redirect.github.com/google/gson/pull/2043">google/gson#2043</a>)</li>
<li>Put <code>module-info.class</code> into Multi-Release JAR folder (<a href="https://redirect.github.com/google/gson/pull/2013">google/gson#2013</a>)</li>
<li>Improve error message when abstract class cannot be constructed (<a href="https://redirect.github.com/google/gson/pull/1814">google/gson#1814</a>)</li>
<li>Support EnumMap deserialization (<a href="https://redirect.github.com/google/gson/pull/2071">google/gson#2071</a>)</li>
<li>Add LazilyParsedNumber default adapter (<a href="https://redirect.github.com/google/gson/pull/2060">google/gson#2060</a>)</li>
<li>Fix JsonReader.hasNext() returning true at end of document (<a href="https://redirect.github.com/google/gson/pull/2061">google/gson#2061</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/google/gson/commit/828a97be0f8d58108b140b77df8dc76b657f4a87"><code>828a97b</code></a> [maven-release-plugin] prepare release gson-parent-2.11.0</li>
<li><a href="https://github.com/google/gson/commit/93bc0f23a13f9e9df3bf71894d479dbd5d952ba6"><code>93bc0f2</code></a> Skip signing graal-native-test module. (<a href="https://redirect.github.com/google/gson/issues/2675">#2675</a>)</li>
<li><a href="https://github.com/google/gson/commit/b153ca18bfef611edff4dbea85de79e153ea4809"><code>b153ca1</code></a> [maven-release-plugin] rollback the release of gson-parent-2.11.0</li>
<li><a href="https://github.com/google/gson/commit/0e3d2aab622fb50addb98b10b0a661cadda0f989"><code>0e3d2aa</code></a> [maven-release-plugin] prepare for next development iteration</li>
<li><a href="https://github.com/google/gson/commit/545b802d639917c50928ec96bcab49b0c70dbb7a"><code>545b802</code></a> [maven-release-plugin] prepare release gson-parent-2.11.0</li>
<li><a href="https://github.com/google/gson/commit/8bfdbb4e14172b013c3d1f56c3a36812075e2886"><code>8bfdbb4</code></a> Guarantee that <code>JsonElement.toString()</code> produces JSON (<a href="https://redirect.github.com/google/gson/issues/2659">#2659</a>)</li>
<li><a href="https://github.com/google/gson/commit/9008b093ac40f226643df17c767357aa1947984a"><code>9008b09</code></a> Extend Troubleshooting Guide with some ProGuard / R8 information (<a href="https://redirect.github.com/google/gson/issues/2656">#2656</a>)</li>
<li><a href="https://github.com/google/gson/commit/05652c3b7dea68a9ffc781b2cdf89076fce56b12"><code>05652c3</code></a> Document that other JVM languages are not fully supported (<a href="https://redirect.github.com/google/gson/issues/2666">#2666</a>)</li>
<li><a href="https://github.com/google/gson/commit/454a49127f9416f45221eecf311eefdca50e4cdc"><code>454a491</code></a> Improved Long-Double Number Policy (<a href="https://redirect.github.com/google/gson/issues/2674">#2674</a>)</li>
<li><a href="https://github.com/google/gson/commit/570d91194e223132982d56b6fa499af15fd7b1ea"><code>570d911</code></a> Bump the github-actions group with 4 updates (<a href="https://redirect.github.com/google/gson/issues/2671">#2671</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/google/gson/compare/gson-parent-2.8.9...gson-parent-2.11.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.code.gson:gson&package-manager=gradle&previous-version=2.8.9&new-version=2.11.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1189" class=".btn">#1189</a>
            </td>
            <td>
                <b>
                    chore(deps): bump androidx.camera:camera-camera2 from 1.2.3 to 1.3.3 in /aries/agents/mobile_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps androidx.camera:camera-camera2 from 1.2.3 to 1.3.3.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=androidx.camera:camera-camera2&package-manager=gradle&previous-version=1.2.3&new-version=1.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    chore(deps): bump androidx.compose:compose-bom from 2022.10.00 to 2022.12.00 in /aries/agents/mobile_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps androidx.compose:compose-bom from 2022.10.00 to 2022.12.00.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=androidx.compose:compose-bom&package-manager=gradle&previous-version=2022.10.00&new-version=2022.12.00)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1187" class=".btn">#1187</a>
            </td>
            <td>
                <b>
                    chore: minor readme updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates Aries VCX Community Call timing
Adds note about aries-vcx-agent is not production ready and that a new framework is in development that will fill end developer's needs (as discussed on [5-15-24 community call](https://wiki.hyperledger.org/display/ARIES/2024-5-15+Aries-vcx+community+call))
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-31 16:11:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    Update MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates discord username formats
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 23:07:02 +0000 UTC
    </div>
</div>

