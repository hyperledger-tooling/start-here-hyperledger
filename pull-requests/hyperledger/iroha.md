---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4657" class=".btn">#4657</a>
            </td>
            <td>
                <b>
                    ci: Remove coveralls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

1. Remove coveralls tool for coverage since it's useless while having it in the workflow trigger type (btw, it's still might be possible to fix). However, coverage is uploading in Sonarqube now.
2. Modify concurrency.
3. Run clippy and lcov jobs in the head branch context.
4. Remove defecdojo output print.
5. Trigger workflow within one parent workflow onlyto reduce parallel jobs creation.


### Benefits

Remove coveralls that doesn't work.
Reduce the possible amount of parallel runs of I2::Dev::CodeQuality workflow.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 20:06:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4656" class=".btn">#4656</a>
            </td>
            <td>
                <b>
                    chore(deps): bump alpine from 3.19 to 3.20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps alpine from 3.19 to 3.20.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=alpine&package-manager=docker&previous-version=3.19&new-version=3.20)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4655" class=".btn">#4655</a>
            </td>
            <td>
                <b>
                    chore(deps): bump libsodium-sys-stable from 1.20.7 to 1.20.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [libsodium-sys-stable](https://github.com/jedisct1/libsodium-sys-stable) from 1.20.7 to 1.20.9.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/398d1f1a23027db3abe87813a6f5d73680323983"><code>398d1f1</code></a> Update to libsodium 1.0.20</li>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/2da70a0da6789374ca36d9a152b29d3ce0f992da"><code>2da70a0</code></a> Update libsodium</li>
<li>See full diff in <a href="https://github.com/jedisct1/libsodium-sys-stable/compare/1.20.7...1.20.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=libsodium-sys-stable&package-manager=cargo&previous-version=1.20.7&new-version=1.20.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:37:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4654" class=".btn">#4654</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.83 to 1.0.84
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.83 to 1.0.84.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.84</h2>
<ul>
<li>Documentation improvements (<a href="https://redirect.github.com/dtolnay/proc-macro2/issues/455">#455</a>, thanks <a href="https://github.com/CensoredUsername"><code>@​CensoredUsername</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/33c95785826bbd1fa353c48989dfc5a7ca62f54c"><code>33c9578</code></a> Release 1.0.84</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/d850da5cf78a7705185e2c37c1269fb3e8c8d042"><code>d850da5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/455">#455</a> from CensoredUsername/master</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/eabac1560e2f672172623bf79e1cb8b5a9d1fe98"><code>eabac15</code></a> Add a warning to Delimiter::None that rustc currently does not respect it.</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.83...1.0.84">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.83&new-version=1.0.84)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4653" class=".btn">#4653</a>
            </td>
            <td>
                <b>
                    chore(deps): bump zeroize from 1.7.0 to 1.8.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [zeroize](https://github.com/RustCrypto/utils) from 1.7.0 to 1.8.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/RustCrypto/utils/commit/7050a8402b44344023cd8d27fe6e0e4055d6bdde"><code>7050a84</code></a> zeroize v1.8.1 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1075">#1075</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/4b7b782b89800109dfa51d1fbdd7389d607dcdaa"><code>4b7b782</code></a> zeroize: move <code>zeroize_derive</code> to toplevel (<a href="https://redirect.github.com/RustCrypto/utils/issues/1074">#1074</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/6b341bbacc58e6bfc1c260bbc88a7ca19221ef6f"><code>6b341bb</code></a> zeroize: feature-gate AVX-512 under <code>simd</code>; MSRV 1.60 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1073">#1073</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/f46a14777a6cb1c553dcc6dbdce26de8e1baf04e"><code>f46a147</code></a> zeroize: note v1.8.0 was yanked in CHANGELOG.md (<a href="https://redirect.github.com/RustCrypto/utils/issues/1071">#1071</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/a7eddc620ed683216b97d924deeab7ea4f84a5af"><code>a7eddc6</code></a> zeroize: fix unnecessary qualifications (<a href="https://redirect.github.com/RustCrypto/utils/issues/1072">#1072</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/9bbfb49e6541d710aea6f7a95c68c9f3d99140e2"><code>9bbfb49</code></a> zeroize 1.8.0 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1065">#1065</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/c0eab7f7abfc244e9fcd482520542329da31f87c"><code>c0eab7f</code></a> cpufeatures: fix macOS build (<a href="https://redirect.github.com/RustCrypto/utils/issues/1066">#1066</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/6d383a554b76df2c6796d8d2982a6a8535342617"><code>6d383a5</code></a> zeroize: always enable AArch64 support (<a href="https://redirect.github.com/RustCrypto/utils/issues/1064">#1064</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/24decb93793936110ae564b6c8e475d91f4e4e44"><code>24decb9</code></a> zeroize: use <code>doc_auto_cfg</code> (<a href="https://redirect.github.com/RustCrypto/utils/issues/1063">#1063</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/cd3a147d62f5f2bf8d5bd10185a52c90f842395b"><code>cd3a147</code></a> build(deps): bump prettyplease from 0.2.16 to 0.2.19 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1061">#1061</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/RustCrypto/utils/compare/zeroize-v1.7.0...zeroize-v1.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zeroize&package-manager=cargo&previous-version=1.7.0&new-version=1.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:36:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4652" class=".btn">#4652</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.202 to 1.0.203
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.202 to 1.0.203.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.203</h2>
<ul>
<li>Documentation improvements (<a href="https://redirect.github.com/serde-rs/serde/issues/2747">#2747</a>)</li>
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
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.202...v1.0.203">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.202&new-version=1.0.203)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:35:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4651" class=".btn">#4651</a>
            </td>
            <td>
                <b>
                    chore(deps): bump parking_lot from 0.12.2 to 0.12.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [parking_lot](https://github.com/Amanieu/parking_lot) from 0.12.2 to 0.12.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Amanieu/parking_lot/blob/master/CHANGELOG.md">parking_lot's changelog</a>.</em></p>
<blockquote>
<h2>parking_lot 0.12.3 (2024-05-24)</h2>
<ul>
<li>Export types provided by arc_lock feature (<a href="https://redirect.github.com/Amanieu/parking_lot/issues/442">#442</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Amanieu/parking_lot/commit/a29dd3d4ff661f73fd5cf638584bc4c5de2ad347"><code>a29dd3d</code></a> Release parking_lot 0.12.3</li>
<li><a href="https://github.com/Amanieu/parking_lot/commit/f7efcae51161c25f7839cddd20cc1b809441e5e8"><code>f7efcae</code></a> Merge pull request <a href="https://redirect.github.com/Amanieu/parking_lot/issues/442">#442</a> from iwanders/add-arc_lock-feature-top-level-exports</li>
<li><a href="https://github.com/Amanieu/parking_lot/commit/c357017decfa0f21ca597a4958745ad0999cf9eb"><code>c357017</code></a> Export types provided by arc_lock feature.</li>
<li>See full diff in <a href="https://github.com/Amanieu/parking_lot/compare/0.12.2...0.12.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=parking_lot&package-manager=cargo&previous-version=0.12.2&new-version=0.12.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:34:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4650" class=".btn">#4650</a>
            </td>
            <td>
                <b>
                    fix(crypto): do not panic if the passed Ed25519Sha512 public key is of invalid length
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Change the conversion of unsized slice to array reference to be infallible and form a better error message.

This prevents a panic during `parity_scale_cli`'s type probing

### Linked issue

Closes #4649 

### Checklist

- [ ] make CI pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 14:14:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4647" class=".btn">#4647</a>
            </td>
            <td>
                <b>
                    refactor: replace u64 with usize internally
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

would you welcome this change?

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 11:26:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4646" class=".btn">#4646</a>
            </td>
            <td>
                <b>
                    chore: update CODEOWNERS
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
        Created At 2024-05-27 06:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4645" class=".btn">#4645</a>
            </td>
            <td>
                <b>
                    feat: Custom instructions in executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Added ISI for custom instructions, and two tests demonstrating possible use:
* Test with one custom instruction `MintAssetForAllAccounts`
* Test with simple expression system

### Linked issue

Closes #4599

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-24 19:42:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4644" class=".btn">#4644</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.65 to 2.0.66
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.65 to 2.0.66.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.66</h2>
<ul>
<li>Allow braced structs when parsing ExprLet (<a href="https://redirect.github.com/dtolnay/syn/issues/1671">#1671</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/b992916bdac459d279bb15098507d43b1febc50e"><code>b992916</code></a> Release 2.0.66</li>
<li><a href="https://github.com/dtolnay/syn/commit/4f0a23f7e147e801a996975662b0d6e6d8a7d13b"><code>4f0a23f</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1671">#1671</a> from dtolnay/exprlet</li>
<li><a href="https://github.com/dtolnay/syn/commit/c6d87a7aa0fda4a8ef867e833d14d105d07ca62b"><code>c6d87a7</code></a> Allow braced structs when parsing ExprLet</li>
<li><a href="https://github.com/dtolnay/syn/commit/747f42f235f8e1b5551a6aeca1d2779dce413408"><code>747f42f</code></a> Update with proc-macro2 1.0.83's syntax tree sizes</li>
<li>See full diff in <a href="https://github.com/dtolnay/syn/compare/2.0.65...2.0.66">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.65&new-version=2.0.66)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-24 16:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4642" class=".btn">#4642</a>
            </td>
            <td>
                <b>
                    refactor(executor): remove `Visit` bound from `Validate`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4237.

<!-- Link if e.g. JIRA issue or  from another repository -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 13:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4640" class=".btn">#4640</a>
            </td>
            <td>
                <b>
                    refactor: remove association between domains and triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Remove the association between domains and triggers.

### Linked issue

Closes #4630.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 08:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4639" class=".btn">#4639</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): Use proper view_change_index on init block load
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of #4612

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 13:45:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4638" class=".btn">#4638</a>
            </td>
            <td>
                <b>
                    feat!: Add traits for iterable and non-iterable queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This PR is a first step towards more type-safe queries (#4569). It adds traits for singular and iterable queries and prohibits supplying filters, sorting, pagination and batching parameters in compile time (it is already a runtime error to do so).

### Linked issue

Partially addresses #4569

### Benefits

- less error prone API
- lays foundation to allow type-checking query filters

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 12:46:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4636" class=".btn">#4636</a>
            </td>
            <td>
                <b>
                    feat: add get_original_transaction_by_hash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Added a method to retrieve a pending partially signed transaction by its transaction hash from the queue. Previously, existing methods required the entire transaction payload, which was cumbersome for other users who needed to build the entire transaction for signing. Now, only the transaction hash is needed.

### Benefits

This improvement simplifies the process for users who need to sign transactions, as they no longer need to reconstruct the entire transaction payload. Instead, they can simply use the transaction hash. This change aligns more closely with real-world use cases, making the signing process more practical and efficient.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 07:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4635" class=".btn">#4635</a>
            </td>
            <td>
                <b>
                    refactor: rename `PermissionToken` to `Permission`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Just a huge rename refactor, according to https://github.com/hyperledger/iroha/pull/4597#discussion_r1607746197. This should significantly reduce the noise of #4597 itself.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 23:51:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4634" class=".btn">#4634</a>
            </td>
            <td>
                <b>
                    docs: update the contributing guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

Updated the contributing guide with reference to issues #4502, #4501, #4433.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4585 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [X] I've read `CONTRIBUTING.md`
- [X] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 19:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4632" class=".btn">#4632</a>
            </td>
            <td>
                <b>
                    refactor(executor): Check custom visit functions in `#[derive(Visit)]`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

While working on #4599, I noticed that in custom executor it is possible to derive `Visit` with invalid `#[visit(custom())]` functions which will be ignored (only rustc error that function is unused). This PR adds check for custom visit function names to avoid potential bugs. Also I updated documentation of some proc-macros related to custom executor.

```rust
#[derive(Constructor, ValidateEntrypoints, Validate, Visit)]
#[visit(custom(visit_register_domain2))]  // typo in visit_register_domain
struct Executor {
    verdict: Result,
    block_height: u64,
}
fn visit_register_domain(...) { ... }
```

### Linked issue

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 16:30:05 +0000 UTC
    </div>
</div>

