---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Bump curve25519-dalek from 4.1.2 to 4.1.3 in the cargo group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps the cargo group with 1 update in the / directory: [curve25519-dalek](https://github.com/dalek-cryptography/curve25519-dalek).

Updates `curve25519-dalek` from 4.1.2 to 4.1.3
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 22:24:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    [ci] update workflow
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
        Created At 2024-06-13 15:22:20 +0000 UTC
    </div>
</div>

