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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.53.0 to 1.54.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.53.0 to 1.54.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.54.0</h2>
<h1>Behavior Changes</h1>
<ul>
<li>xds: remove support for xDS v2 transport API (<a href="https://redirect.github.com/grpc/grpc-go/issues/6013">#6013</a>)</li>
</ul>
<h1>New Features</h1>
<ul>
<li>server: expose <code>SetSendCompressor</code> API to set send compressor name (<a href="https://redirect.github.com/grpc/grpc-go/issues/5744">#5744</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/jronak"><code>@​jronak</code></a></li>
</ul>
</li>
<li>xdsclient: include <code>Node</code> proto only in the first discovery request message, to improve performance (<a href="https://redirect.github.com/grpc/grpc-go/issues/6078">#6078</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>metadata: fix validation logic and properly validate metadata appended via <code>AppendToOutgoingContext</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6001">#6001</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/ktalg"><code>@​ktalg</code></a></li>
</ul>
</li>
<li>transport: do not close connections when we encounter I/O errors until after all data is consumed (<a href="https://redirect.github.com/grpc/grpc-go/issues/6110">#6110</a>)</li>
<li>ringhash: ensure addresses are consistently hashed across updates (<a href="https://redirect.github.com/grpc/grpc-go/issues/6066">#6066</a>)</li>
<li>xds/clusterimpl: fix a bug causing unnecessary closing and re-opening of LRS streams (<a href="https://redirect.github.com/grpc/grpc-go/issues/6112">#6112</a>)</li>
<li>xds: NACK route configuration if sum of weights of weighted clusters exceeds uint32_max (<a href="https://redirect.github.com/grpc/grpc-go/issues/6085">#6085</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>resolver: update <code>Resolver.Scheme()</code> docstring to mention requirement of lowercase scheme names (<a href="https://redirect.github.com/grpc/grpc-go/issues/6014">#6014</a>)</li>
<li>resolver: document expected error handling of <code>UpdateState</code> errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/6002">#6002</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/fho"><code>@​fho</code></a></li>
</ul>
</li>
<li>examples: add example for ORCA load reporting (<a href="https://redirect.github.com/grpc/grpc-go/issues/6114">#6114</a>)</li>
<li>examples: add an example to illustrate authorization (authz) support (<a href="https://redirect.github.com/grpc/grpc-go/issues/5920">#5920</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/KenxinKun"><code>@​KenxinKun</code></a></li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/2997e84fd8d18ddb000ac6736129b48b3c9773ec"><code>2997e84</code></a> Change version to 1.54.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6129">#6129</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/b638faff2204da74b93bb4aee28051b15a7a33bd"><code>b638faf</code></a> stats/opencensus: Add message prefix to metrics names (<a href="https://redirect.github.com/grpc/grpc-go/issues/6126">#6126</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c84a5005d97fb43bbc01b7d1484c0e4c844bec4c"><code>c84a500</code></a> credentials/alts: defer ALTS stream creation until handshake time (<a href="https://redirect.github.com/grpc/grpc-go/issues/6077">#6077</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6f44ae89b1ab4e492516fd8f1770ad16451a9f02"><code>6f44ae8</code></a> metadata: add benchmark test for FromIncomingContext and ValueFromIncomingCon...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a1e657ce53ba59e6e4076edaa2c68d398e7f7e4f"><code>a1e657c</code></a> client: log last error on subchannel connectivity change (<a href="https://redirect.github.com/grpc/grpc-go/issues/6109">#6109</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/36fd0a43969cee5d7e0410231f8bee284bf766e7"><code>36fd0a4</code></a> gcp/observability: Add compressed metrics to observability module and synchro...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52ca9571068dd4433b4aed49f303abe0a3776468"><code>52ca957</code></a> xds: make comparison of server configs in bootstrap more reliable (<a href="https://redirect.github.com/grpc/grpc-go/issues/6112">#6112</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/7507ea6bcbef3e25822b2bedccdc923ad1134b59"><code>7507ea6</code></a> gcp/observability: Change logging schema and set queue size limit for logs an...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/16c3b7df7f78df4061703be769832de44216bfc1"><code>16c3b7d</code></a> examples: add example for ORCA load reporting (<a href="https://redirect.github.com/grpc/grpc-go/issues/6114">#6114</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/b458a4f11afbced02ab3db241362c60f75972705"><code>b458a4f</code></a> transport: stop always closing connections when loopy returns (<a href="https://redirect.github.com/grpc/grpc-go/issues/6110">#6110</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.53.0...v1.54.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.53.0&new-version=1.54.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 05:03:49 +0000 UTC
    </div>
</div>

