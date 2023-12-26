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
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    fix test case for #166
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                try to fix https://github.com/hyperledger/fabric-admin-sdk/actions/runs/7262230071/job/19819802821?pr=166#step:4:392
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-23 14:15:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/protobuf from 1.31.0 to 1.32.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.31.0 to 1.32.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.31.0&new-version=1.32.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-22 14:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.60.0 to 1.60.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.60.0 to 1.60.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release v1.60.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>server: fix two bugs that could lead to panics at shutdown when using <a href="https://pkg.go.dev/google.golang.org/grpc#NumStreamWorkers">NumStreamWorkers</a> (experimental feature).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dbbcf59957fec0bd58063224cbf105b3b3698d4e"><code>dbbcf59</code></a> Update version.go to 1.60.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6865">#6865</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6e384cfd437a759b6c21af9496c4e32bd890af2e"><code>6e384cf</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6856">#6856</a> to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6864">#6864</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6430548ff97b036ffaea26b9381252b46352d385"><code>6430548</code></a> Change version to 1.60.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6793">#6793</a>)</li>
<li>See full diff in <a href="https://github.com/grpc/grpc-go/compare/v1.60.0...v1.60.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.60.0&new-version=1.60.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-19 14:26:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    Updated MSPID from Org1 to Org2
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
        Created At 2023-12-19 13:04:43 +0000 UTC
    </div>
</div>

