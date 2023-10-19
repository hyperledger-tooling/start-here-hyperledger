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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1019" class=".btn">#1019</a>
            </td>
            <td>
                <b>
                    Bump rustix from 0.37.24 to 0.37.25
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rustix](https://github.com/bytecodealliance/rustix) from 0.37.24 to 0.37.25.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/bytecodealliance/rustix/commit/00b84d6aac2364455eab2c68e42afee63d6e3ad3"><code>00b84d6</code></a> chore: Release rustix version 0.37.25</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/cad15a7076d493a0651fb0b7889bd5e5a72a8f17"><code>cad15a7</code></a> Fixes for <code>Dir</code> on macOS, FreeBSD, and WASI.</li>
<li><a href="https://github.com/bytecodealliance/rustix/commit/df3c3a192cf144af0da8a57417fb4addbdc611f6"><code>df3c3a1</code></a> Merge pull request from GHSA-c827-hfw6-qwvm</li>
<li>See full diff in <a href="https://github.com/bytecodealliance/rustix/compare/v0.37.24...v0.37.25">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rustix&package-manager=cargo&previous-version=0.37.24&new-version=0.37.25)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-18 18:46:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1018" class=".btn">#1018</a>
            </td>
            <td>
                <b>
                    Add support for pickup protocol messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ref: https://github.com/hyperledger/aries-rfcs/blob/main/features/0685-pickup-v2/README.md
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 06:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    Present Proof V2.0 message structures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related, almost identical to: https://github.com/hyperledger/aries-vcx/pull/990

NOTE: I've gone with v2.0 (as opposed to v2.1 & v2.2), this is primarily because it seems to be what others (aca-py & AFJ) are targeting and expect. similarly, V2.0 is what AIP2.0 lists as it's requirement: https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0302-aries-interop-profile/README.md#base-requirements

The changes are virtually identical to #990 , other changes include:
* moved `AttachmentFormatSpecifier` to a common place
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 03:06:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1016" class=".btn">#1016</a>
            </td>
            <td>
                <b>
                    Extract primitives and remove Profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the `Profile` trait in favor of using independent components instead. Additionally, it aims to remove the shared usage of primitive components (making them depend on each other) and instead rely on function signatures to specifically ask for the components needed (without hidden implications that passing `Anoncreds` will also pass a `Wallet` instance).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 08:22:49 +0000 UTC
    </div>
</div>

