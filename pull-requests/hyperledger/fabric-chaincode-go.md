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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.48.0 to 1.49.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.48.0 to 1.49.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
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
<li>xds/xdsclient: NACK endpoint resources with zero weight (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5560">#5560</a>)</li>
<li>xds/xdsclient: fix bug that would reset resource version information after ADS stream restart (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5422">#5422</a>)</li>
<li>xds/xdsclient: fix goroutine leaks when load reporting is enabled (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5505">#5505</a>)</li>
<li>xds/ringhash: fix config update processing to recreate ring and picker when min/max ring size changes (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5557">#5557</a>)</li>
<li>xds/ringhash: avoid recreating subChannels when update doesn't change address weight information (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5431">#5431</a>)</li>
<li>xds/priority: fix bug which could cause priority LB to block all traffic after a config update (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5549">#5549</a>)</li>
<li>xds: fix bug when environment variable <code>GRPC_EXPERIMENTAL_ENABLE_OUTLIER_DETECTION</code> is set to true (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5537">#5537</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/1c29e075ab1c83a455cf942dd148c467a879800a"><code>1c29e07</code></a> Change version to 1.49.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5583">#5583</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8e5a84e6b2dec2a96d0b780eeb93cbfd4928086e"><code>8e5a84e</code></a> xds/resolver: generate channel ID randomly (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5603">#5603</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/92cee3440fed794a84394c42046b6b61c07af705"><code>92cee34</code></a> gcp/observability: Add logging filters for logging, tracing, and metrics API ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c7fe135d124ebd51e6a9728d1e55c7bebc85407e"><code>c7fe135</code></a> O11Y: Added support for custom tags (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5565">#5565</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/7981af402b2327512c001f8c8eb92b5034ec8ad4"><code>7981af4</code></a> test/kokoro: add missing image tagging to the xDS interop url map buildscript...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6f34b7ad1546ea084ed79f4b1db6ba5e61c2d8c4"><code>6f34b7a</code></a> xdsclient: NACK endpoint resource if load_balancing_weight is specified and i...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/f9409d385fbaa24c04d2c634aafe974f4f13a042"><code>f9409d3</code></a> ringhash: handle config updates properly (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5557">#5557</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/946dde008f3d66634ab1ae4624a44efb10aa5be6"><code>946dde0</code></a> xdsclient: NACK endpoint resources with zero weight (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5560">#5560</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/b89f49b0ffe3a1ebdf037e7e42dc99ca6a90c8a5"><code>b89f49b</code></a> xdsclient: deflake Test/LDSWatch_PartialValid (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5552">#5552</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/9bc72deba4d2107740084b05f415a766a62c6e06"><code>9bc72de</code></a> grpc: remove mentions of WithBalancerName from comments (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5555">#5555</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.48.0...v1.49.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.48.0&new-version=1.49.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-08-24 04:34:34 +0000 UTC
    </div>
</div>

