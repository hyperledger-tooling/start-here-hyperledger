---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Bump github.com/hyperledger/fabric-protos-go from 0.3.0 to 0.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/hyperledger/fabric-protos-go](https://github.com/hyperledger/fabric-protos-go) from 0.3.0 to 0.3.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/70e28b46d1b86eb038ede16050eff87dff58094c"><code>70e28b4</code></a> Extend lifecycle protos to query all approved chaincode definitions</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/212400245d309cf319fd0734ac18d60783d3a746"><code>2124002</code></a> Extend lifecycle protos to checkcommitreadiness to provide discrepancy details</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/b03edb47a905a20294e668e937d2035659852564"><code>b03edb4</code></a> system channel cleanup - make HeaderType_ORDERER_TRANSACTION deprecated (<a href="https://redirect.github.com/hyperledger/fabric-protos-go/issues/184">#184</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/8f302041c2e296480a3755906f72f5aab9bcc3ba"><code>8f30204</code></a> Bump Go to 1.19 (<a href="https://redirect.github.com/hyperledger/fabric-protos-go/issues/178">#178</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/8b7f1c52afc671f1e64c3c18bf192078facaace2"><code>8b7f1c5</code></a> Update Go bindings build</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-protos-go/compare/v0.3.0...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/hyperledger/fabric-protos-go&package-manager=go_modules&previous-version=0.3.0&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-25 04:54:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.54.0 to 1.60.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.54.0 to 1.60.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release v1.60.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>server: fix two bugs that could lead to panics at shutdown when using <a href="https://pkg.go.dev/google.golang.org/grpc#NumStreamWorkers">NumStreamWorkers</a> (experimental feature).</li>
</ul>
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
<h2>Release 1.58.3</h2>
<h1>Security</h1>
<ul>
<li>
<p>server: prohibit more than MaxConcurrentStreams handlers from running at once (CVE-2023-44487)</p>
<p>In addition to this change, applications should ensure they do not leave running tasks behind related to the RPC before returning from method handlers, or should enforce appropriate limits on any such work.</p>
</li>
</ul>
<h2>Release 1.58.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>
<p>balancer/weighted_round_robin: fix ticker leak on update</p>
<p>A new ticker is created every time there is an update of addresses or configuration, but was not properly stopped.  This change stops the ticker when it is no longer needed.</p>
</li>
</ul>
<h2>Release 1.58.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpc: fix a bug that was decrementing active RPC count too early for streaming RPCs; leading to channel moving to IDLE even though it had open streams</li>
<li>grpc: fix a bug where transports were not being closed upon channel entering IDLE</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dbbcf59957fec0bd58063224cbf105b3b3698d4e"><code>dbbcf59</code></a> Update version.go to 1.60.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6865">#6865</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6e384cfd437a759b6c21af9496c4e32bd890af2e"><code>6e384cf</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6856">#6856</a> to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6864">#6864</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6430548ff97b036ffaea26b9381252b46352d385"><code>6430548</code></a> Change version to 1.60.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6793">#6793</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/297d8ddeb0d5834b47f40a5bd624aa0c2cfb9c7a"><code>297d8dd</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6841">#6841</a> to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6847">#6847</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3580447e0cc2b9fb1c2f005b182d172c673fc0c6"><code>3580447</code></a> Change version to 1.60.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6792">#6792</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/71e67a93f46639f053cc83cd29e74d2a0248468e"><code>71e67a9</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6834">#6834</a> to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6839">#6839</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/cb6581dd1a407e1679498e9b304ae2000da7dd92"><code>cb6581d</code></a> Cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6804">#6804</a> and dependencies to v1.60.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6838">#6838</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/dd39cdbddcfbc1ad1cf04910d8fba2b7201469ec"><code>dd39cdb</code></a> credentials: if not set, restrict to TLS v1.2+ and CipherSuites per RFC7540 (...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8645f95509d6c5d17a54621407f3ca717d4f8620"><code>8645f95</code></a> resolver: remove ClientConn.NewServiceConfig (<a href="https://redirect.github.com/grpc/grpc-go/issues/6784">#6784</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8b17a4dbc328e8ef7f9e5094ab5fe8a78efccbb8"><code>8b17a4d</code></a> vet: various cleanups (<a href="https://redirect.github.com/grpc/grpc-go/issues/6780">#6780</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.54.0...v1.60.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.54.0&new-version=1.60.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-19 04:27:07 +0000 UTC
    </div>
</div>

