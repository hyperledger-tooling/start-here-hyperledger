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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.48.0 to 1.50.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.48.0 to 1.50.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.50.1</h2>
<p>New Features</p>
<ul>
<li>gcp/observability: support new configuration defined in public preview user guide</li>
</ul>
<h2>Release 1.50.0</h2>
<h1>Behavior Changes</h1>
<ul>
<li>client: use proper &quot;@&quot; semantics for connecting to abstract unix sockets. (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5678">#5678</a>)
<ul>
<li>This is technically a bug fix; the result is that the address was including a trailing NULL byte, which it should not have.  This may break users creating the socket in Go by prefixing a NULL instead of an &quot;@&quot;, though, so calling it out as a behavior change.</li>
</ul>
<ul>
<li>Special Thanks: <a href="https://github.com/jachor"><code>@​jachor</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>metadata: add experimental <code>ValueFromIncomingContext</code> to more efficiently retrieve a single value (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5596">#5596</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/horpto"><code>@​horpto</code></a></li>
</ul>
</li>
<li>stats: provide peer information in <code>HandleConn</code> context (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5589">#5589</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/feihu-stripe"><code>@​feihu-stripe</code></a></li>
</ul>
</li>
<li>xds: add support for Outlier Detection, enabled by default (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5435">#5435</a>, <a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5673">#5673</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>client: fix deadlock in transport caused by GOAWAY racing with stream creation (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5652">#5652</a>)
<ul>
<li>This should only occur with an HTTP/2 server that does not follow best practices of an advisory GOAWAY (not a grpc-go server).</li>
</ul>
</li>
<li>xds/xdsclient: fix a bug which was causing routes with <code>cluster_specifier_plugin</code> set to be NACKed when GRPC_EXPERIMENTAL_XDS_RLS_LB was off (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5670">#5670</a>)</li>
<li>xds/xdsclient: NACK cluster resource if <code>config_source_specifier</code> in <code>lrs_server</code> is not <code>self</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5613">#5613</a>)</li>
<li>xds/ringhash: fix a bug which sometimes prevents the LB policy from retrying connection attempts (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5601">#5601</a>)</li>
<li>xds/ringhash: do nothing when asked to exit <code>IDLE</code> instead of falling back on the default channel behavior of connecting to all addresses (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5614">#5614</a>)</li>
<li>xds/rls: fix a bug which was causing the channel to be stuck in <code>IDLE</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5656">#5656</a>)</li>
<li>alts: fix a bug which was setting <code>WaitForReady</code> on handshaker service RPCs, thereby delaying fallback when required (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5620">#5620</a>)</li>
<li>gcp/observability: fix End() to cleanup global state correctly (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5623">#5623</a>)</li>
</ul>
<h2>Release 1.49.0</h2>
<h1>New Features</h1>
<ul>
<li>gcp/observability: add support for Environment Variable <code>GRPC_CONFIG_OBSERVABILITY_JSON</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5525">#5525</a>)</li>
<li>gcp/observability: add support for custom tags (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5565">#5565</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>server: reduce log level from Warning to Info for early connection establishment errors (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5524">#5524</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/jpkrohling"><code>@​jpkrohling</code></a></li>
</ul>
</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>client: fix race in flow control that could lead to unexpected EOF errors (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5494">#5494</a>)</li>
<li>client: fix a race that could cause RPCs to time out instead of failing more quickly with UNAVAILABLE (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5503">#5503</a>)</li>
<li>client &amp; server: fix a panic caused by passing a <code>nil</code> stats handler to <code>grpc.WithStatsHandler</code> or <code>grpc.StatsHandler</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5543">#5543</a>)</li>
<li>transport/server: fix a race that could cause a stray header to be sent (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5513">#5513</a>)</li>
<li>balancer: give precedence to <code>IDLE</code> over <code>TRANSIENT_FAILURE</code> when aggregating connectivity state (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5473">#5473</a>)</li>
<li>xds/xdsclient: request correct resource name when user specifies a new style resource name with empty authority (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5488">#5488</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/4c776ec01572d55249df309251900554b46adb41"><code>4c776ec</code></a> Cherry-pick observability changes from master to v1.50.x and update version t...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6576007e5601072d8ddf9a01720851cd12e2b7bc"><code>6576007</code></a> Change version to 1.50.1-dev (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5686">#5686</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c1d7d7acc3d14788d07ded8be9cd74c136084294"><code>c1d7d7a</code></a> Change version to 1.50.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5685">#5685</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/1451c62ccdce325a1f2fdbcc90db89518a36dc06"><code>1451c62</code></a> internal/transport: optimize grpc-message encoding/decoding (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5654">#5654</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/be4b63b1fcab082f7e19b540abfbbaf13958addd"><code>be4b63b</code></a> test: minor test cleanup (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5679">#5679</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d83070ec0d9043f713b6a63e1963c593b447208c"><code>d83070e</code></a> Changed Outlier Detection Env Var to default true (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5673">#5673</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/54521b22e01f52e6e112b33bbca8b2255915dd40"><code>54521b2</code></a> client: remove trailing null from unix abstract socket address (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5678">#5678</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/36e481079b224e01fc3134ba7f1b2717f0c4d4ef"><code>36e4810</code></a> orca: cleanup old code, and get grpc package to use new code (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5627">#5627</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e8866a83edf51f5a5dcd8097c6d4fe4cdef49cdd"><code>e8866a8</code></a> build: harden GitHub Workflow permissions (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5660">#5660</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8458251c6b35036b90788223f67fc9e4396cd32c"><code>8458251</code></a> xdsclient: ignore routes with cluster_specifier_plugin when GRPC_EXPERIMENTAL...</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.48.0...v1.50.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.48.0&new-version=1.50.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-17 04:25:46 +0000 UTC
    </div>
</div>

