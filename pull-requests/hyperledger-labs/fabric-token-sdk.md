---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    F certification storage
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
        Created At 2024-01-15 15:58:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/531" class=".btn">#531</a>
            </td>
            <td>
                <b>
                    identity storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR extends the `StorageProvider` to add support for `WalletPathStorage` and `keystore.KVS`.
This further reduces direct dependency to the FSC's KVS.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 09:10:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/530" class=".btn">#530</a>
            </td>
            <td>
                <b>
                    Bump github.com/quic-go/quic-go from 0.38.1 to 0.38.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/quic-go/quic-go](https://github.com/quic-go/quic-go) from 0.38.1 to 0.38.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/quic-go/quic-go/releases">github.com/quic-go/quic-go's releases</a>.</em></p>
<blockquote>
<h2>v0.38.2</h2>
<p>This release contains fixes for a resource exhaustion attack on QUIC's path validation logic (CVE-2023-49295), see <a href="https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation">https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation</a> for details:</p>
<ul>
<li>limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/pull/4199">quic-go/quic-go#4199</a>)</li>
<li>don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/pull/4200">quic-go/quic-go#4200</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/quic-go/quic-go/commit/9aaefe19fc3dc8c8917cc87e6128bb56d9e9e6cc"><code>9aaefe1</code></a> don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/issues/4200">#4200</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/17fc98c2d81dbe685c19702dc694a9d606ac56dc"><code>17fc98c</code></a> limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/issues/4199">#4199</a>)</li>
<li>See full diff in <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/quic-go/quic-go&package-manager=go_modules&previous-version=0.38.1&new-version=0.38.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 15:11:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/529" class=".btn">#529</a>
            </td>
            <td>
                <b>
                    remove kvs from ttxdb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 14:29:36 +0000 UTC
    </div>
</div>

