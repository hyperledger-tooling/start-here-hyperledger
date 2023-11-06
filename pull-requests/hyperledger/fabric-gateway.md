---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    Use go.uber.org/mock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a currently maintained fork of the (no longer maintained) github.com/golang/mock module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 23:54:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    Define separate module for Go scenario tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Avoids polluting the fabric-gateway module with scenario test dependencies.
- Scenario tests more closely model a client application.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 11:20:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/654" class=".btn">#654</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.57.0 to 1.57.1 in /scenario/fixtures/chaincode/golang/basic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.57.0 to 1.57.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.57.1</h2>
<h1>Security</h1>
<ul>
<li>
<p>server: prohibit more than MaxConcurrentStreams handlers from running at once (CVE-2023-44487)</p>
<p>In addition to this change, applications should ensure they do not leave running tasks behind related to the RPC before returning from method handlers, or should enforce appropriate limits on any such work.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/d9c4eab5e1086d726510c775819fd042498f6d92"><code>d9c4eab</code></a> Change version to 1.57.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6712">#6712</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6a1400d526dfe16aafc960c882507dcdcf3b0f61"><code>6a1400d</code></a> server: prohibit more than MaxConcurrentStreams handlers from running at once...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/7511ddf04b1ba74195e69d50ab175de18c414015"><code>7511ddf</code></a> Change version to 1.57.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6449">#6449</a>)</li>
<li>See full diff in <a href="https://github.com/grpc/grpc-go/compare/v1.57.0...v1.57.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.57.0&new-version=1.57.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-gateway/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 07:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/653" class=".btn">#653</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.57.0 to 1.57.1 in /scenario/fixtures/chaincode/golang/private
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.57.0 to 1.57.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.57.1</h2>
<h1>Security</h1>
<ul>
<li>
<p>server: prohibit more than MaxConcurrentStreams handlers from running at once (CVE-2023-44487)</p>
<p>In addition to this change, applications should ensure they do not leave running tasks behind related to the RPC before returning from method handlers, or should enforce appropriate limits on any such work.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/d9c4eab5e1086d726510c775819fd042498f6d92"><code>d9c4eab</code></a> Change version to 1.57.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6712">#6712</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6a1400d526dfe16aafc960c882507dcdcf3b0f61"><code>6a1400d</code></a> server: prohibit more than MaxConcurrentStreams handlers from running at once...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/7511ddf04b1ba74195e69d50ab175de18c414015"><code>7511ddf</code></a> Change version to 1.57.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6449">#6449</a>)</li>
<li>See full diff in <a href="https://github.com/grpc/grpc-go/compare/v1.57.0...v1.57.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.57.0&new-version=1.57.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-gateway/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 07:36:27 +0000 UTC
    </div>
</div>

