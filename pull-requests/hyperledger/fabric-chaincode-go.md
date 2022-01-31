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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/38" class=".btn">#38</a>
            </td>
            <td>
                <b>
                    Bump github.com/golang/protobuf from 1.3.2 to 1.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/golang/protobuf](https://github.com/golang/protobuf) from 1.3.2 to 1.5.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/golang/protobuf/releases">github.com/golang/protobuf's releases</a>.</em></p>
<blockquote>
<h2>v1.5.2</h2>
<p>Notable changes:</p>
<ul>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1306">#1306</a>) all: deprecate the module</li>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1300">#1300</a>) jsonpb: restore previous behavior for handling nulls and JSONPBUnmarshaler</li>
</ul>
<h2>v1.5.1</h2>
<p>Notable changes:</p>
<ul>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1293">#1293</a>) all: depend on <a href="https://github.com/protocolbuffers/protobuf-go/releases/tag/v1.26.0">google.golang.org/protobuf@v1.26.0</a></li>
</ul>
<h2>v1.5.0</h2>
<ul>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.5-overview">Overview</a></li>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.5-notable-changes">Notable changes</a></li>
</ul>
<h1>Overview <!-- raw HTML omitted --><!-- raw HTML omitted --></h1>
<p>This marks the <a href="https://pkg.go.dev/github.com/golang/protobuf/ptypes"><code>ptypes</code></a> package as deprecated and upgrades the dependency on <code>google.golang.org/protobuf</code> to a pre-release version of v1.26.0. A subsequent patch release will update the dependency to <a href="https://github.com/protocolbuffers/protobuf-go/releases/tag/v1.26.0">v1.26.0</a> proper.</p>
<h1>Notable changes <!-- raw HTML omitted --><!-- raw HTML omitted --></h1>
<ul>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1217">#1217</a>) ptypes: deprecate the package</li>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1214">#1214</a>) rely on protodesc.ToFileDescriptorProto</li>
</ul>
<h2>v1.4.3</h2>
<p>Notable changes:</p>
<ul>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1221">#1221</a>) jsonpb: Fix marshaling of Duration</li>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1210">#1210</a>) proto: convert integer to rune before converting to string</li>
</ul>
<h2>v1.4.2</h2>
<p>Notable changes:</p>
<ul>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1131">#1131</a>) all: upgrade to google.golang.org/protobuf@v1.23.0</li>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1125">#1125</a>) jsonpb: fix a confusing error message</li>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1129">#1129</a>) proto: make InternalMessageInfo functional</li>
</ul>
<h2>v1.4.1</h2>
<p>Notable changes:</p>
<ul>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1114">#1114</a>) all: upgrade to google.golang.org/protobuf@v1.22.0</li>
<li>(<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1113">#1113</a>) protoc-gen-go/grpc: make identical to v1.3.5</li>
</ul>
<h2>v1.4.0</h2>
<ul>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.4-overview">Overview</a>
<ul>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.4-backwards-compatibility">Backwards compatibility</a></li>
</ul>
</li>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.4-notable-changes">Notable changes</a>
<ul>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.4-wire-serialization">Wire serialization</a></li>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.4-json-text-serialization">JSON and text serialization</a></li>
<li><a href="https://github.com/golang/protobuf/blob/HEAD/#v1.4-well-known-types">Well-known types</a></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/protobuf/commit/ae97035608a719c7a1c1c41bed0ae0744bdb0c6f"><code>ae97035</code></a> all: deprecate the module (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1306">#1306</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/af940030a2b77f37337632168f18403433e21e61"><code>af94003</code></a> jsonpb: restore previous behavior for handling nulls and JSONPBUnmarshaler (#...</li>
<li><a href="https://github.com/golang/protobuf/commit/a36a1a1c346d5cb6951b9440755adb530334f910"><code>a36a1a1</code></a> all: depend on google.golang.org/protobuf@v1.26.0 (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1293">#1293</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/f746d3b8ecd31eac7c04a954f3905d46b09f8114"><code>f746d3b</code></a> all: depend on google.golang.org/protobuf@v1.26.0-rc.1 (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1292">#1292</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/78b1f09b4310f9ee5c9a07dca51bf007b82c83ea"><code>78b1f09</code></a> Switch from Travis-CI to GitHub actions (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1286">#1286</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/acacf8158c9a307051c92dc233966e8324facd45"><code>acacf81</code></a> all: rely on protodesc.ToFileDescriptorProto (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1214">#1214</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/eccd77d6ffe33de3bca6050a06c4e8294783de69"><code>eccd77d</code></a> ptypes: deprecate the package (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1217">#1217</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/4846b58453b3708320bdb524f25cc5a1d9cda4d4"><code>4846b58</code></a> jsonpb: Fix marshaling of Duration (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1221">#1221</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/91c84e0db17890c2bb64280a6d660e73e4237fd1"><code>91c84e0</code></a> travis.yml: update tested versions of Go (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1211">#1211</a>)</li>
<li><a href="https://github.com/golang/protobuf/commit/3860b2764ff25e103fbe1db40f22248fe7a6dc20"><code>3860b27</code></a> proto: convert integer to rune before converting to string (<a href="https://github-redirect.dependabot.com/golang/protobuf/issues/1210">#1210</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/golang/protobuf/compare/v1.3.2...v1.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/golang/protobuf&package-manager=go_modules&previous-version=1.3.2&new-version=1.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-31 13:26:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.23.0 to 1.44.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.23.0 to 1.44.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.44.0</h2>
<h1>New Features</h1>
<ul>
<li>balancer: add RLS load balancing policy (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5046">#5046</a>)</li>
<li>xds: add RLS Cluster Specifier Plugin (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5004">#5004</a>)</li>
<li>insecure: remove experimental notice (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5069">#5069</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>internal/balancergroup: eliminate race in exitIdle (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5012">#5012</a>)</li>
<li>authz: fix regex expression match (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5035">#5035</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>grpc: minor improvement on WithInsecure() document (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5068">#5068</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/shitian-ni"><code>@​shitian-ni</code></a></li>
</ul>
</li>
<li>attributes: document that some value types (e.g. <code>map</code>s) must implement Equal (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5109">#5109</a>)</li>
<li>dialoptions.go: Fix WithBlock godoc (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5073">#5073</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/sgreene570"><code>@​sgreene570</code></a></li>
</ul>
</li>
<li>grpclog.DepthLoggerV2: Correct comment: formats like fmt.Println (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5038">#5038</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/evanj"><code>@​evanj</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.43.0</h2>
<h1>API Changes</h1>
<ul>
<li>grpc: stabilize <code>WithConnectParams</code> <code>DialOption</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4915">#4915</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/hypnoglow"><code>@​hypnoglow</code></a></li>
</ul>
</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>status: support wrapped errors in <code>FromContextError</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4977">#4977</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/bestbeforetoday"><code>@​bestbeforetoday</code></a></li>
</ul>
</li>
<li>config: remove the environment variable to disable retry support (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4922">#4922</a>)</li>
</ul>
<h1>New Features</h1>
<ul>
<li>balancer: new field <code>Authority</code> in <code>BuildOptions</code> for server name to use in the authentication handshake with a remote load balancer (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4969">#4969</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>xds/resolver: fix possible <code>ClientConn</code> leak upon resolver initialization failure (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4900">#4900</a>)</li>
<li>client: fix <code>nil</code> panic in rare race conditions with the pick first LB policy (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4971">#4971</a>)</li>
<li>xds: improve RPC error messages when xDS connection errors occur (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5032">#5032</a>, <a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5054">#5054</a>)</li>
<li>transport: do not create stream object in the face of illegal stream IDs (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4873">#4873</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/uds5501"><code>@​uds5501</code></a></li>
</ul>
</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>client: clarify errors to indicate whether compressed or uncompressed messages exceeded size limits (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4918">#4918</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/uds5501"><code>@​uds5501</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.42.0</h2>
<h1>Behavior Changes</h1>
<ul>
<li>grpc: Dial(&quot;unix://relative-path&quot;) no longer works (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4817">#4817</a>)
<ul>
<li>use &quot;unix://absolute-path&quot; or &quot;unix:relative-path&quot; instead in accordance with <a href="https://github.com/grpc/grpc/blob/master/doc/naming.md#name-syntax">our documentation</a></li>
</ul>
</li>
<li>xds/csds: use new field <code>GenericXdsConfig</code> instead of <code>PerXdsConfig</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4898">#4898</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/b4c5e24c7373b22c6c38d68379c39ecdc616a968"><code>b4c5e24</code></a> Change version to 1.44.1-dev (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5121">#5121</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/da8e0b8fa35c185b30da2fe706ce9535b918239f"><code>da8e0b8</code></a> Change version to 1.44.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5120">#5120</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/77b478d768e7e75234406b53471844a0a8d6faf4"><code>77b478d</code></a> xds/federation: e2e tests (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5103">#5103</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/907a202a615d3b2de857e4302cf6032004d65aee"><code>907a202</code></a> attributes: document that some value types (e.g. <code>map</code>s) must implement Equal...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2fb1ac854b2037b408121870f0dcc81474ca483b"><code>2fb1ac8</code></a> test: fix potential goroutine leak in TestUpdateAddresses_RetryFromFirstAddr ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/afded7231d0083fb7e9fcccc768ecbf56c271626"><code>afded72</code></a> xds/federation: update xdsclient to support multi authority (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5042">#5042</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/b069440926d58e0a6fa6c59b01638a6948f9e6f3"><code>b069440</code></a> credentials/google: use grpctest.Tester for tests in this package (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5098">#5098</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/fbaf7c55821070944bb0ce342ba3c54cc521c6fe"><code>fbaf7c5</code></a> authz: update representation of allow authenticated in SDK (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5052">#5052</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/344b93a285883f2da713622d5064ad4b4512e63e"><code>344b93a</code></a> testdata: use SHA256 as signing algorithm in testdata certs (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5074">#5074</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4d58dd98db75e180ebf67cce127db5068ff7ab3e"><code>4d58dd9</code></a> dialoptions.go: Fix WithBlock godoc (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5073">#5073</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.23.0...v1.44.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.23.0&new-version=1.44.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-31 13:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Enable dependabot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 11:54:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Update github.com/stretchr/testify
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves vulnerability in gopkg.in/yaml.v2

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 11:53:56 +0000 UTC
    </div>
</div>

