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
                PR <a href="https://github.com/hyperledger/iroha/pull/4761" class=".btn">#4761</a>
            </td>
            <td>
                <b>
                    chore: move back to the upstream displaydoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Now that the displaydoc has released a version which fixed the nightly warnings, we can migrate back to it.

(We were previously using a git version because of #4567)

### Checklist

- [ ] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 18:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4760" class=".btn">#4760</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.66 to 2.0.67
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.66 to 2.0.67.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.67</h2>
<ul>
<li>Produce more accurate error message locations for errors located at the end of a nested group (<a href="https://redirect.github.com/dtolnay/syn/issues/1679">#1679</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1680">#1680</a>)</li>
<li>Support peeking <code>LitCStr</code> in ParseStream::peek (<a href="https://redirect.github.com/dtolnay/syn/issues/1682">#1682</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/25f6299c982276bf55faac834538d78ea61d6bad"><code>25f6299</code></a> Release 2.0.67</li>
<li><a href="https://github.com/dtolnay/syn/commit/666e15e95ff3763571f14af93be2641eecc5c2d9"><code>666e15e</code></a> Revert &quot;List peekable token types in documentation of Peek trait&quot;</li>
<li><a href="https://github.com/dtolnay/syn/commit/2955706a736b5ca293eff45a3b2cade32baa01aa"><code>2955706</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1683">#1683</a> from dtolnay/peekimpl</li>
<li><a href="https://github.com/dtolnay/syn/commit/0c902919850353ddfe4d90f5ba0474e6ac8aaaa8"><code>0c90291</code></a> List peekable token types in documentation of Peek trait</li>
<li><a href="https://github.com/dtolnay/syn/commit/26ce3d9134644b62298963d0abf0e9a3584f6896"><code>26ce3d9</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1682">#1682</a> from dtolnay/peekcstr</li>
<li><a href="https://github.com/dtolnay/syn/commit/ec0c84b282c8ade12f6afaad7425b90ec5a1fd7d"><code>ec0c84b</code></a> Make LitCStr peekable</li>
<li><a href="https://github.com/dtolnay/syn/commit/8cb56cc59d8ea0117dd6df3915f4c730249618bc"><code>8cb56cc</code></a> Update test suite to nightly-2024-06-20</li>
<li><a href="https://github.com/dtolnay/syn/commit/7cc7eac262467d4c1e6cac8f9beeb20d256f7d49"><code>7cc7eac</code></a> Inline lookahead::is_delimiter into delimiter Token impls</li>
<li><a href="https://github.com/dtolnay/syn/commit/8a2a86bce92d1f440a7b2d6d244ab825d426bb61"><code>8a2a86b</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1681">#1681</a> from dtolnay/offset</li>
<li><a href="https://github.com/dtolnay/syn/commit/e86538ccd80494c8bf239b36550c0f9e298b50c5"><code>e86538c</code></a> Optimize reverse iteration of TokenBuffer</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.66...2.0.67">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.66&new-version=2.0.67)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-21 17:05:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4759" class=".btn">#4759</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.85 to 1.0.86
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.85 to 1.0.86.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.86</h2>
<ul>
<li>Documentation improvements</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/aa9476b27932ae1b1b50bbfe0530b3b261fc1b72"><code>aa9476b</code></a> Release 1.0.86</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/19613587b70633e8bd383dd2fc29856d2d080f45"><code>1961358</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/466">#466</a> from dtolnay/buildrs</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/e1bd2cc29da09be421555bb0e1156c5e2b87df5d"><code>e1bd2cc</code></a> Bring build script comments up to date</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/5b271279521e11ac6eada5435e5a8d87f46d3619"><code>5b27127</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/465">#465</a> from dtolnay/ignorereason</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/0da4629757024ac6dac1680ba3be44bac24af809"><code>0da4629</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.85...1.0.86">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.85&new-version=1.0.86)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-21 17:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4757" class=".btn">#4757</a>
            </td>
            <td>
                <b>
                    fix!: Upgrade executor in separate transaction in genesis block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

`GenesisBlock` now have two transactions, first with single `Upgrade` instruction to set executor, and second with all other instructions. If there are no other instructions, second transaction will be omitted.

### Linked issue

Closes #4743

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
        Created At 2024-06-21 12:09:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4752" class=".btn">#4752</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.8.0 to 25.9.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.8.0 to 25.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.9.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.9.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v25.9.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.9.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.9.0..v25.9.1">v25.9.1 - 2024-06-20</a></h3>
<ul>
<li>Change <code>pydecimal</code> type hint for <code>min_value</code>, <code>max_value</code> to allow <code>int</code>s. Thanks <a href="https://github.com/parsariyahi"><code>@​parsariyahi</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v25.8.0..v25.9.0">v25.9.0 - 2024-06-20</a></h3>
<ul>
<li>Add support for Nigerian Yoruba names and surnames (<code>yo_NG</code>). Thanks <a href="https://github.com/5uru"><code>@​5uru</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/fb42357d0ac30c0fdba200d5339f8fe9f9ce6f81"><code>fb42357</code></a> Bump version: 25.9.0 → 25.9.1</li>
<li><a href="https://github.com/joke2k/faker/commit/7c391c45d840c9b7ea29e723fee6cbfd6ba08d24"><code>7c391c4</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/10c2ba35cda949188c460464f46e79ee0236d605"><code>10c2ba3</code></a> Fix typing on <code>pydecimal</code></li>
<li><a href="https://github.com/joke2k/faker/commit/d0bfbfbf7a30b1831bf466cfb48ac627bb090b15"><code>d0bfbfb</code></a> Change <code>pydecimal</code> type hint for <code>min_value</code>, <code>max_value</code> to <code>numbers.Number</code>...</li>
<li><a href="https://github.com/joke2k/faker/commit/c49ef43bf5ac8ccaaded6ff02866e9eabdaa27b5"><code>c49ef43</code></a> Bump version: 25.8.0 → 25.9.0</li>
<li><a href="https://github.com/joke2k/faker/commit/f375cbc42d8dd973aa170207dbe2e2ab2ea945c3"><code>f375cbc</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/fc329ad841d45967ff3cda49d06c9399d5f56299"><code>fc329ad</code></a> 💄 format code</li>
<li><a href="https://github.com/joke2k/faker/commit/84766274e5476f7698df00bc7e7ba3c3c99ad82f"><code>8476627</code></a> Added support for Nigerian Yoruba names and surnames (yo_NG) (<a href="https://redirect.github.com/joke2k/faker/issues/2054">#2054</a>)</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.8.0...v25.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.8.0&new-version=25.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-20 16:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4750" class=".btn">#4750</a>
            </td>
            <td>
                <b>
                    ci: Modify CodeQuality job branch checkout variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
Attempt to fix `CodeQuality` workflow `checkout` actions that always points to repository defaults branch even if PR is coming from not-default branch.

### Linked issue
https://github.com/orgs/community/discussions/66784
https://github.com/orgs/community/discussions/25220

### Benefits

Perhaps will fix `CodeQuality` workflow.

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
        Created At 2024-06-20 11:29:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4747" class=".btn">#4747</a>
            </td>
            <td>
                <b>
                    chore(deps): bump curve25519-dalek from 4.1.2 to 4.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [curve25519-dalek](https://github.com/dalek-cryptography/curve25519-dalek) from 4.1.2 to 4.1.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/5312a0311ec40df95be953eacfa8a11b9a34bc54"><code>5312a03</code></a> curve: Bump version to 4.1.3 (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/660">#660</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/b4f9e4df92a4689fb59e312a21f940ba06ba7013"><code>b4f9e4d</code></a> SECURITY: fix timing variability in backend/serial/u32/scalar.rs (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/661">#661</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/415892acf1cdf9161bd6a4c99bc2f4cb8fae5e6a"><code>415892a</code></a> SECURITY: fix timing variability in backend/serial/u64/scalar.rs (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/659">#659</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/56bf398d0caed63ef1d1edfbd35eb5335132aba2"><code>56bf398</code></a> Updates license field to valid SPDX format (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/647">#647</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/9252fa5c0d09054fed4ac4d649e63c40fad7abaf"><code>9252fa5</code></a> Mitigate check-cfg until MSRV 1.77 (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/652">#652</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/1efe6a93b176c4389b78e81e52b2cf85d728aac6"><code>1efe6a9</code></a> Fix a minor typo in signing.rs (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/649">#649</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/cc3421a22fa7ee1f557cbe9243b450da53bbe962"><code>cc3421a</code></a> Indicate that the rand_core feature is required (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/641">#641</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/858c4ca8ae03d33fe8b71b4504c4d3f5ff5b45c0"><code>858c4ca</code></a> Address new nightly clippy unnecessary qualifications (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/639">#639</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/31ccb6705067d68782cb135e23c79b640a6a06ee"><code>31ccb67</code></a> Remove platforms in favor using CARGO_CFG_TARGET_POINTER_WIDTH (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/636">#636</a>)</li>
<li><a href="https://github.com/dalek-cryptography/curve25519-dalek/commit/19c7f4a5d5e577adc9cc65a837abef9ed7ebf0a4"><code>19c7f4a</code></a> Fix new nightly redundant import lint warns (<a href="https://redirect.github.com/dalek-cryptography/curve25519-dalek/issues/638">#638</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dalek-cryptography/curve25519-dalek/compare/curve25519-4.1.2...curve25519-4.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=curve25519-dalek&package-manager=cargo&previous-version=4.1.2&new-version=4.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-19 16:09:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4746" class=".btn">#4746</a>
            </td>
            <td>
                <b>
                    chore(deps): bump url from 2.5.1 to 2.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [url](https://github.com/servo/rust-url) from 2.5.1 to 2.5.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/servo/rust-url/commit/54346fa288e16b25b71c45149d7067c752b450e0"><code>54346fa</code></a> Revert &quot;Reimplement idna on top of ICU4X&quot; (<a href="https://redirect.github.com/servo/rust-url/issues/946">#946</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/dcfbed3e90b4bbbb70f121f802f1d9b25adb8f89"><code>dcfbed3</code></a> Update idna to 1.0.1 (<a href="https://redirect.github.com/servo/rust-url/issues/945">#945</a>)</li>
<li><a href="https://github.com/servo/rust-url/commit/467ef63969f477ee44b7456bb450fba95af25780"><code>467ef63</code></a> fix panic on <code>xn--55555577</code> (<a href="https://redirect.github.com/servo/rust-url/issues/940">#940</a>)</li>
<li>See full diff in <a href="https://github.com/servo/rust-url/compare/v2.5.1...v2.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url&package-manager=cargo&previous-version=2.5.1&new-version=2.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-19 16:08:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4745" class=".btn">#4745</a>
            </td>
            <td>
                <b>
                    refactor: send blocks to observing peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of #4392 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 13:00:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4744" class=".btn">#4744</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): early exit from handle_block_sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Exit early from `handle_block_sync` if received block is the same or has smaller or equal view change index.

## Benefits

Improve performance of block sync by avoid doing work where not necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 11:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4742" class=".btn">#4742</a>
            </td>
            <td>
                <b>
                    refactor: move permission migration into executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description


### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

we no longer depend on the `ExecutorDataModel::permissions` being correct. 
It's just for users to query it the same way as `ExecutorDataModel::custom_instruction` is

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
        Created At 2024-06-19 07:51:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4741" class=".btn">#4741</a>
            </td>
            <td>
                <b>
                    refactor!: fix naming convention for assets and permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

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
        Created At 2024-06-18 12:07:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4740" class=".btn">#4740</a>
            </td>
            <td>
                <b>
                    fix: fix unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Fix failing unit tests.

Checked tests locally to verify if errors are resolved.

```
cargo test --all-features --no-fail-fast --workspace --exclude iroha_executor
```

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 11:52:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4739" class=".btn">#4739</a>
            </td>
            <td>
                <b>
                    refactor!: Supply `SignedBlock` instead of `SignedTransaction` to peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This is first part of #4696:
* Added `topology` field to `genesis.json`
* Changed `kagami genesis sign` to generate `SignedBlock`
* Adapted `iroha_swarm` and `test_env.py` to those changes

Planned changes for next PRs:
* Provide hash of genesis block to all peers (#4555)
* Allow multiple peers to submit genesis

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
        Created At 2024-06-18 11:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4738" class=".btn">#4738</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump flake8 from 7.0.0 to 7.1.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [flake8](https://github.com/pycqa/flake8) from 7.0.0 to 7.1.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/PyCQA/flake8/commit/65a38c42a7f1a05ff8d99b313160754fc9b7a0d8"><code>65a38c4</code></a> Release 7.1.0</li>
<li><a href="https://github.com/PyCQA/flake8/commit/34c97e046a459b0682c82660f16c620369abd6b7"><code>34c97e0</code></a> Merge pull request <a href="https://redirect.github.com/pycqa/flake8/issues/1939">#1939</a> from PyCQA/new-pycodestyle</li>
<li><a href="https://github.com/PyCQA/flake8/commit/defd315175b7b77472affb61a410e5720dabdc1a"><code>defd315</code></a> latest pycodestyle</li>
<li><a href="https://github.com/PyCQA/flake8/commit/408d4d695c71b0b232cea576876e757c87a3379c"><code>408d4d6</code></a> Merge pull request <a href="https://redirect.github.com/pycqa/flake8/issues/1930">#1930</a> from mzagol/patch-1</li>
<li><a href="https://github.com/PyCQA/flake8/commit/866ad729c64eea359960a8ac4e3f1201104ee55c"><code>866ad72</code></a> Add --extend-exclude to the TOC</li>
<li><a href="https://github.com/PyCQA/flake8/commit/33e508307ac4545a45472fdc32c6eaadbc7b9580"><code>33e5083</code></a> Merge pull request <a href="https://redirect.github.com/pycqa/flake8/issues/1923">#1923</a> from Viicos/entry-points-docs</li>
<li><a href="https://github.com/PyCQA/flake8/commit/6659b213c9aa8fa49235e13a365fcd34f58cbc6b"><code>6659b21</code></a> Fix toctree ordering in index</li>
<li><a href="https://github.com/PyCQA/flake8/commit/ba0f56610adbd4d8733772ce1c63efcab1b70079"><code>ba0f566</code></a> Use explicit external references</li>
<li><a href="https://github.com/PyCQA/flake8/commit/350f2545fd3ec75640a1605e4995a2f921e8b38b"><code>350f254</code></a> Use explicit external references</li>
<li><a href="https://github.com/PyCQA/flake8/commit/49f52a8598d8a934b07f367a1b3ad87dbe51be5b"><code>49f52a8</code></a> Update documentation regarding entry points</li>
<li>Additional commits viewable in <a href="https://github.com/pycqa/flake8/compare/7.0.0...7.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=flake8&package-manager=pip&previous-version=7.0.0&new-version=7.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 16:55:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4737" class=".btn">#4737</a>
            </td>
            <td>
                <b>
                    chore(deps): bump docker/build-push-action from 4 to 6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [docker/build-push-action](https://github.com/docker/build-push-action) from 4 to 6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v6.0.0</h2>
<ul>
<li>Export build record and generate <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">build summary</a> by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1120">docker/build-push-action#1120</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.24.0 to 0.26.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1132">docker/build-push-action#1132</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1136">docker/build-push-action#1136</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1138">docker/build-push-action#1138</a></li>
<li>Bump braces from 3.0.2 to 3.0.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1137">docker/build-push-action#1137</a></li>
</ul>
<blockquote>
<p>[!NOTE]
This major release adds support for generating <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">Build summary</a> and exporting build record for your build. You can disable this feature by setting <a href="https://docs.docker.com/build/ci/github-actions/build-summary/#disable-job-summary"> <code>DOCKER_BUILD_NO_SUMMARY: true</code> environment variable in your workflow</a>.</p>
</blockquote>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0">https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0</a></p>
<h2>v5.4.0</h2>
<ul>
<li>Show builder information before building by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1128">docker/build-push-action#1128</a></li>
<li>Handle attestations correctly with provenance and sbom inputs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1086">docker/build-push-action#1086</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.24.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1088">docker/build-push-action#1088</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1105">docker/build-push-action#1105</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1121">docker/build-push-action#1121</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1127">docker/build-push-action#1127</a></li>
<li>Bump undici from 5.28.3 to 5.28.4 in <a href="https://redirect.github.com/docker/build-push-action/pull/1090">docker/build-push-action#1090</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0">https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0</a></p>
<h2>v5.3.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1080">docker/build-push-action#1080</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0">https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0</a></p>
<h2>v5.2.0</h2>
<ul>
<li>Disable quotes detection for <code>outputs</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1074">docker/build-push-action#1074</a></li>
<li>Warn about ignored inputs by <a href="https://github.com/favonia"><code>@​favonia</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1019">docker/build-push-action#1019</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.14.0 to 0.18.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1070">docker/build-push-action#1070</a></li>
<li>Bump undici from 5.26.3 to 5.28.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1057">docker/build-push-action#1057</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0">https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0</a></p>
<h2>v5.1.0</h2>
<ul>
<li>Add <code>annotations</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/992">docker/build-push-action#992</a></li>
<li>Add <code>secret-envs</code> input by <a href="https://github.com/elias-lundgren"><code>@​elias-lundgren</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/980">docker/build-push-action#980</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.17.3 to 7.23.2 in <a href="https://redirect.github.com/docker/build-push-action/pull/991">docker/build-push-action#991</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.13.0-rc.1 to 0.14.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/990">docker/build-push-action#990</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1006">docker/build-push-action#1006</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0">https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0</a></p>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/954">docker/build-push-action#954</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/959">docker/build-push-action#959</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0">https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0</a></p>
<h2>v4.2.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/c382f710d39a5bb4e430307530a720f50c2d3318"><code>c382f71</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1120">#1120</a> from crazy-max/build-summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/5a5b70d974381b812e448a9ea8efef0c0781e8a7"><code>5a5b70d</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/dc24cf9e252ee3b05f80a1637b2950c11d305b3d"><code>dc24cf9</code></a> don't generate summary for cloud driver</li>
<li><a href="https://github.com/docker/build-push-action/commit/667cb22c52a8762431790112e70ef7f545dbf2d2"><code>667cb22</code></a> DOCKER_BUILD_NO_SUMMARY env to disable summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/d880b1964b626c7ac1763e83768e139202071136"><code>d880b19</code></a> generate build summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/e51051ad0baf1cdf23788f7f0980f675806b580e"><code>e51051a</code></a> export build record and upload artifact</li>
<li><a href="https://github.com/docker/build-push-action/commit/86c2bd00318427a320d2cee5bbc61251df6f647e"><code>86c2bd0</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1137">#1137</a> from docker/dependabot/npm_and_yarn/braces-3.0.3</li>
<li><a href="https://github.com/docker/build-push-action/commit/268d2b16117932ad41015c96fbc27a7641533625"><code>268d2b1</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1138">#1138</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/2b8dc7f52914dfdd416618a1f33d11277b7d64d2"><code>2b8dc7f</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/840c12be1707e3d7115f8d61da2c8b78442cc538"><code>840c12b</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.25.1 to 0.26.0</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v4...v6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/build-push-action&package-manager=github_actions&previous-version=4&new-version=6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 16:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4736" class=".btn">#4736</a>
            </td>
            <td>
                <b>
                    chore(deps): bump derive_more from 0.99.17 to 0.99.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [derive_more](https://github.com/JelteF/derive_more) from 0.99.17 to 0.99.18.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/JelteF/derive_more/blob/v0.99.18/CHANGELOG.md">derive_more's changelog</a>.</em></p>
<blockquote>
<h2>0.99.18 - 2024-06-15</h2>
<ul>
<li>Update syn to version 2.x</li>
<li>Bump minimum supported rust version to 1.65</li>
</ul>
<h2>0.99.10 - 2020-09-11</h2>
<h3>Improvements</h3>
<ul>
<li><code>From</code> supports additional types for conversion: <code>#[from(types(u8, u16))]</code>.</li>
</ul>
<h2>0.99.7 - 2020-05-16</h2>
<h3>Fixes</h3>
<ul>
<li>Fix generic derives for <code>MulAssign</code></li>
</ul>
<h3>Improvements</h3>
<ul>
<li>When specifying specific features of the crate to only enable specific
derives, the <code>extra-traits</code> feature of  <code>syn</code> is not always enabled
when those the specified features do not require it. This should speed up
compile time of <code>syn</code> when this feature is not needed.</li>
</ul>
<h2>0.99.6 - 2020-05-13</h2>
<h3>Improvements</h3>
<ul>
<li>Make sure output of derives is deterministic, for better support in
rust-analyzer</li>
</ul>
<h2>0.99.5 - 2020-03-28</h2>
<h3>New features</h3>
<ul>
<li>Support for deriving <code>Error</code>!!! (many thanks to <a href="https://github.com/ffuugoo"><code>@​ffuugoo</code></a> and <a href="https://github.com/tyranron"><code>@​tyranron</code></a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>
<p>Fix generic bounds for <code>Deref</code> and <code>DerefMut</code> with <code>forward</code>, i.e. put <code>Deref</code>
bound on whole type, so on <code>where Box&lt;T&gt;: Deref</code> instead of on <code>T: Deref</code>.
(<a href="https://redirect.github.com/JelteF/derive_more/issues/114">#107</a>)</p>
</li>
<li>
<p>The <code>tests</code> directory is now correctly included in the crate (requested by
Debian package maintainers)</p>
</li>
</ul>
<h2>0.99.4 - 2020-03-28</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JelteF/derive_more/commit/678a4735bc540b7363c6dadddc4bb273fdf74468"><code>678a473</code></a> chore: Release derive_more version 0.99.18</li>
<li><a href="https://github.com/JelteF/derive_more/commit/fcde5568cb2a815b8d85fceb6dd8fd56750d2b25"><code>fcde556</code></a> Include example published package</li>
<li><a href="https://github.com/JelteF/derive_more/commit/89cbd82959034284f7a2eeffb1976bc41a75b95f"><code>89cbd82</code></a> Remove track_caller feature detection because msrv was bumped</li>
<li><a href="https://github.com/JelteF/derive_more/commit/db36f6dade1cf512ff71961882bda6467a639a31"><code>db36f6d</code></a> Fix question marks</li>
<li><a href="https://github.com/JelteF/derive_more/commit/f0c2530255b21d9f791ee6e4acb6375c2becc641"><code>f0c2530</code></a> fmt</li>
<li><a href="https://github.com/JelteF/derive_more/commit/461db95716ac91f60ee4877bb94c474b5fa25ca7"><code>461db95</code></a> Fix issue when compiling on 1.65</li>
<li><a href="https://github.com/JelteF/derive_more/commit/39ad36fd7117acb0a8140d3aa63899ecc46b53c6"><code>39ad36f</code></a> Update changelog for v0.99.18</li>
<li><a href="https://github.com/JelteF/derive_more/commit/57b6e1746e1ddf4c67e16b5e82f12e19ef02a3d5"><code>57b6e17</code></a> Update to syn 2</li>
<li><a href="https://github.com/JelteF/derive_more/commit/ea4fa940033682ca16e1040688963011404d02a0"><code>ea4fa94</code></a> Fix tests</li>
<li><a href="https://github.com/JelteF/derive_more/commit/ab82aef0bf0c4f4e5cc837e3de3a78a373bc922b"><code>ab82aef</code></a> Ignore error doctests as it still contains old backtrace logic</li>
<li>Additional commits viewable in <a href="https://github.com/JelteF/derive_more/compare/v0.99.17...v0.99.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=derive_more&package-manager=cargo&previous-version=0.99.17&new-version=0.99.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 16:04:13 +0000 UTC
    </div>
</div>

