---
layout: default
title: fabric-admin-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-admin-sdk
---

# fabric-admin-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-admin-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.61.0 to 1.61.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.61.0 to 1.61.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.61.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>server: wait to close connection until incoming socket is drained (with timeout) to prevent data loss on client-side (<a href="https://redirect.github.com/grpc/grpc-go/issues/6977">#6977</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/s-matyukevich"><code>@​s-matyukevich</code></a> for discovering the root cause</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/c6e7f04eb9a3d9535c055b68aea36b723e46d470"><code>c6e7f04</code></a> Change version to 1.61.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6981">#6981</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/dbd4cbcef164059f14ecc355d8a22b58c02a7fb8"><code>dbd4cbc</code></a> cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6977">#6977</a> to 1.61.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6980">#6980</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/57ed608e2fd7f49761db00d3710ba881cb0944c9"><code>57ed608</code></a> Change version to 1.61.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6937">#6937</a>)</li>
<li>See full diff in <a href="https://github.com/grpc/grpc-go/compare/v1.61.0...v1.61.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.61.0&new-version=1.61.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-14 14:08:51 +0000 UTC
    </div>
</div>

