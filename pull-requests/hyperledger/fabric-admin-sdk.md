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
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/crypto from 0.14.0 to 0.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.14.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/crypto/commit/9d2ee975ef9fe627bf0a6f01c1f69e8ef1d4f05d"><code>9d2ee97</code></a> ssh: implement strict KEX protocol changes</li>
<li><a href="https://github.com/golang/crypto/commit/4e5a26183ecb4f9a0f85c8f8dbe7982885435436"><code>4e5a261</code></a> ssh: close net.Conn on all NewServerConn errors</li>
<li><a href="https://github.com/golang/crypto/commit/152cdb1503ebc13bc0fbb68f92ee189ebf9e3d00"><code>152cdb1</code></a> x509roots/fallback: update bundle</li>
<li><a href="https://github.com/golang/crypto/commit/fdfe1f8531a1adcc300c8eba98cb372044826d62"><code>fdfe1f8</code></a> ssh: defer channel window adjustment</li>
<li><a href="https://github.com/golang/crypto/commit/b8ffc16e10063067bac0e15c6d7f7995937503ce"><code>b8ffc16</code></a> blake2b: drop Go 1.6, Go 1.8 compatibility</li>
<li><a href="https://github.com/golang/crypto/commit/7e6fbd82c804e1760feb603fe21caecb0af0a124"><code>7e6fbd8</code></a> ssh: wrap errors from client handshake</li>
<li><a href="https://github.com/golang/crypto/commit/bda2f3f5cfce3f27039acccd823693f6d67c2a74"><code>bda2f3f</code></a> argon2: avoid clobbering BP</li>
<li><a href="https://github.com/golang/crypto/commit/325b735346247f48971d2b37d24dd180a35f391f"><code>325b735</code></a> ssh/test: skip TestSSHCLIAuth on Windows</li>
<li><a href="https://github.com/golang/crypto/commit/1eadac50a566dfaa1b603ca15e8ad3cbd1c77b20"><code>1eadac5</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/crypto/commit/b2d7c26edb17864f117d8b0ee73c1843bcc6090f"><code>b2d7c26</code></a> ssh: add (*Client).DialContext method</li>
<li>Additional commits viewable in <a href="https://github.com/golang/crypto/compare/v0.14.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.14.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-admin-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 23:31:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.59.0 to 1.60.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.59.0 to 1.60.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.60.0</h2>
<h1>Security</h1>
<ul>
<li>credentials/tls: if not set, set TLS MinVersion to 1.2 and CipherSuites according to supported suites not forbidden by RFC7540.
<ul>
<li>This is a behavior change to bring us into better alignment with RFC 7540.</li>
</ul>
</li>
</ul>
<h1>API Changes</h1>
<ul>
<li>resolver: remove deprecated and experimental <code>ClientConn.NewServiceConfig</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6784">#6784</a>)</li>
<li>client: remove deprecated <code>grpc.WithServiceConfig</code> <code>DialOption</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6800">#6800</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>client: fix race that could cause a deadlock while entering idle mode and receiving a name resolver update (<a href="https://redirect.github.com/grpc/grpc-go/issues/6804">#6804</a>)</li>
<li>client: always enable TCP keepalives with OS defaults (<a href="https://redirect.github.com/grpc/grpc-go/issues/6834">#6834</a>)</li>
<li>credentials/alts: fix a bug preventing ALTS from connecting to the metadata server if the default scheme is overridden (<a href="https://redirect.github.com/grpc/grpc-go/issues/6686">#6686</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/mjamaloney"><code>@​mjamaloney</code></a></li>
</ul>
</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>server: Do not return from Stop() or GracefulStop() until all resources are released (<a href="https://redirect.github.com/grpc/grpc-go/issues/6489">#6489</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/fho"><code>@​fho</code></a></li>
</ul>
</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>codes: clarify that only codes defined by this package are valid and that users should not cast other values to <code>codes.Code</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6701">#6701</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/297d8ddeb0d5834b47f40a5bd624aa0c2cfb9c7a"><code>297d8dd</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6841">#6841</a> to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6847">#6847</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3580447e0cc2b9fb1c2f005b182d172c673fc0c6"><code>3580447</code></a> Change version to 1.60.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6792">#6792</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/71e67a93f46639f053cc83cd29e74d2a0248468e"><code>71e67a9</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6834">#6834</a> to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6839">#6839</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/cb6581dd1a407e1679498e9b304ae2000da7dd92"><code>cb6581d</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6804">#6804</a> and dependencies to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6838">#6838</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/dd39cdbddcfbc1ad1cf04910d8fba2b7201469ec"><code>dd39cdb</code></a> credentials: if not set, restrict to TLS v1.2+ and CipherSuites per RFC7540 (...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8645f95509d6c5d17a54621407f3ca717d4f8620"><code>8645f95</code></a> resolver: remove ClientConn.NewServiceConfig (<a href="https://redirect.github.com/grpc/grpc-go/issues/6784">#6784</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8b17a4dbc328e8ef7f9e5094ab5fe8a78efccbb8"><code>8b17a4d</code></a> vet: various cleanups (<a href="https://redirect.github.com/grpc/grpc-go/issues/6780">#6780</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/591c48187c4ba075d14a0ca6e69572a60662af92"><code>591c481</code></a> internal/transport: Add LocalAddr to http2Client.getPeer() (<a href="https://redirect.github.com/grpc/grpc-go/issues/6779">#6779</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/eb46b7d427ee19c821e43dfd034447f8b3a28e7a"><code>eb46b7d</code></a> github: set top-level read-only workflow permissions (<a href="https://redirect.github.com/grpc/grpc-go/issues/6775">#6775</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/be1d1c10a930fa0e91fc4bcd01963035011e2466"><code>be1d1c1</code></a> security/advancedtls: FileWatcher CRL provider initialization enhancement (<a href="https://redirect.github.com/grpc/grpc-go/issues/6">#6</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.59.0...v1.60.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.59.0&new-version=1.60.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-12 14:59:01 +0000 UTC
    </div>
</div>

