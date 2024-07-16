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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    add config flag for retries for selectors
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
        Created At 2024-07-15 15:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    update FSC (f-dispose)
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
        Created At 2024-07-15 07:35:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Fix duration metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                * Added different implementations to fetch the tokens. Behind these implementations we implement optimizations on how to fetch the tokens. The lazy one queries the database every time. The eager one polls the database and returns the cached result. The mixed one first serves the cached result and then the lazy one. Further strategies can be implemented as: a. Return the cached result if it is fresh enough. b. Listen for DB inserts in the token table and update the cache.
* Minimized the information we fetched from the database to avoid spooling big byte arrays
* Permutating the tokens every selector takes to avoid racing for the same tokens in the same order
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 22:01:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    fix data race in local membership
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevent some data race for the function `GetDefaultIdentifier` (reading list of resolvers) when called from `mapStringToID`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 13:49:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    orion update
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
        Created At 2024-07-10 17:25:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.64.0 to 1.64.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.64.0 to 1.64.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.64.1</h2>
<h1>Dependencies</h1>
<ul>
<li>Update x/net/http2 to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-45288">CVE-2023-45288</a> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7352">#7352</a>)</li>
<li>metadata: remove String method from MD to make printing consistent (<a href="https://redirect.github.com/grpc/grpc-go/issues/7374">#7374</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/4d833de0e0ea4345c2f8333f5e1d1155f93c5222"><code>4d833de</code></a> Change version to 1.64.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/7381">#7381</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e9193a42987f93cf634aedb7c6f32d607281f8c4"><code>e9193a4</code></a> *: update deps (<a href="https://redirect.github.com/grpc/grpc-go/issues/7375">#7375</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ab292411ddc0f3b7a7786754d1fe05264c3021eb"><code>ab29241</code></a> metadata: remove String method (<a href="https://redirect.github.com/grpc/grpc-go/issues/7374">#7374</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/355b9a557b63896fc569d8be1518905eabde0026"><code>355b9a5</code></a> Change version to 1.64.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/7219">#7219</a>)</li>
<li>See full diff in <a href="https://github.com/grpc/grpc-go/compare/v1.64.0...v1.64.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.64.0&new-version=1.64.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 22:01:26 +0000 UTC
    </div>
</div>

