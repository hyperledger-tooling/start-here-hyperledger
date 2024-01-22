---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    Bump commonmarker from 0.23.6 to 0.23.10 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [commonmarker](https://github.com/gjtorikian/commonmarker) from 0.23.6 to 0.23.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gjtorikian/commonmarker/releases">commonmarker's releases</a>.</em></p>
<blockquote>
<h2>v0.23.10</h2>
<h2>What's Changed</h2>
<ul>
<li>Update to 0.29.0.gfm.13 by <a href="https://github.com/anticomputer"><code>@​anticomputer</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/247">gjtorikian/commonmarker#247</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.9...v0.23.10">https://github.com/gjtorikian/commonmarker/compare/v0.23.9...v0.23.10</a></p>
<h2>v0.23.9</h2>
<h2>What's Changed</h2>
<ul>
<li>Update to 0.29.0.gfm.11 by <a href="https://github.com/anticomputer"><code>@​anticomputer</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/236">gjtorikian/commonmarker#236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.8...v0.23.9">https://github.com/gjtorikian/commonmarker/compare/v0.23.8...v0.23.9</a></p>
<h2>v0.23.8</h2>
<h2>What's Changed</h2>
<ul>
<li>Update cmark-upstream to <code>0.29.0.gfm.9</code> by <a href="https://github.com/smockle"><code>@​smockle</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/227">gjtorikian/commonmarker#227</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/smockle"><code>@​smockle</code></a> made their first contribution in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/227">gjtorikian/commonmarker#227</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.7...v0.23.8">https://github.com/gjtorikian/commonmarker/compare/v0.23.7...v0.23.8</a></p>
<h2>v0.23.7</h2>
<h2>What's Changed</h2>
<ul>
<li>C API stable test by <a href="https://github.com/gjtorikian"><code>@​gjtorikian</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/201">gjtorikian/commonmarker#201</a></li>
<li>Update to 29.0.gfm.7 by <a href="https://github.com/anticomputer"><code>@​anticomputer</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/224">gjtorikian/commonmarker#224</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7">https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7</a></p>
<h2>v0.23.7.pre1</h2>
<h2>What's Changed</h2>
<ul>
<li>C API stable test by <a href="https://github.com/gjtorikian"><code>@​gjtorikian</code></a> in <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/201">gjtorikian/commonmarker#201</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7.pre1">https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.7.pre1</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/gjtorikian/commonmarker/blob/v0.23.10/CHANGELOG.md">commonmarker's changelog</a>.</em></p>
<blockquote>
<h2>[v0.23.10] (2023-07-31)</h2>
<ul>
<li>Update GFM release to <a href="https://github.com/github/cmark-gfm/releases/tag/0.29.0.gfm.12"><code>0.29.0.gfm.12</code></a> and <a href="https://github.com/github/cmark-gfm/releases/tag/0.29.0.gfm.13"><code>0.29.0.gfm.13</code></a>, thereby <a href="https://github.com/github/cmark-gfm/security/advisories/GHSA-w4qg-3vf7-m9x5">fixing a polynomial time complexity security vulnerability</a>.</li>
<li>Of note to users of this library, GFM releases <code>0.29.0.gfm.12</code> and <code>0.29.0.gfm.13</code> also:
<ul>
<li>Normalized marker row vs. delimiter row nomenclature (<a href="https://redirect.github.com/github/cmark-gfm/pull/273">#273</a>)</li>
<li>Exposed CMARK_NODE_FOOTNOTE_DEFINITION literal value (<a href="https://redirect.github.com/github/cmark-gfm/pull/336">#336</a>)</li>
</ul>
</li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v0.23.4">v0.23.4</a> (2022-03-03)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.2...v0.23.4">Full Changelog</a></p>
<p><strong>Fixed bugs:</strong></p>
<ul>
<li><code>#render_html</code> way slower than <code>#render_doc.to_html</code> <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/141">#141</a></li>
</ul>
<p><strong>Closed issues:</strong></p>
<ul>
<li>allow keeping text content of unknown tags <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/169">#169</a></li>
<li>STRIKETHROUGH_DOUBLE_TILDE not working <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/168">#168</a></li>
<li>Allow disabling 4-space code blocks <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/167">#167</a></li>
<li>tables with escaped pipes are not recognized <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/166">#166</a></li>
</ul>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>CI: Drop a duplicate 'bundle install' <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/173">#173</a> (<a href="https://github.com/olleolleolle">olleolleolle</a>)</li>
<li>CI: Drop duplicate bundle install <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/172">#172</a> (<a href="https://github.com/olleolleolle">olleolleolle</a>)</li>
<li>Fixup benchmark and speedup a little, fixes <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/141">#141</a> <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/171">#171</a> (<a href="https://github.com/ojab">ojab</a>)</li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v0.23.2">v0.23.2</a> (2021-09-17)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.1...v0.23.2">Full Changelog</a></p>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>Update GFM release to <code>0.29.0.gfm.2</code> <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/148">#148</a> (<a href="https://github.com/phillmv">phillmv</a>)</li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v0.23.1">v0.23.1</a> (2021-09-03)</h2>
<p><a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.0...v0.23.1">Full Changelog</a></p>
<p><strong>Closed issues:</strong></p>
<ul>
<li>Incorrect processing of list and next block of code <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/146">#146</a></li>
</ul>
<p><strong>Merged pull requests:</strong></p>
<ul>
<li>Normalize parse and render options <a href="https://redirect.github.com/gjtorikian/commonmarker/pull/145">#145</a> (<a href="https://github.com/phillmv">phillmv</a>)</li>
</ul>
<h2><a href="https://github.com/gjtorikian/commonmarker/tree/v0.23.0">v0.23.0</a> (2021-08-30)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/db8cd377b54541f7fd484d168b7682a282a680f7"><code>db8cd37</code></a> Merge pull request <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/247">#247</a> from anticomputer/update-to-0.29.0.gfm.13</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/e1e450c381e1fac5021a08bdc5f72bbac9cf6038"><code>e1e450c</code></a> :gem: release 0.23.10</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/08b7c4b96c2835edcc2f14e978f758f6ac58b158"><code>08b7c4b</code></a> Update cmark-upstream to <a href="https://github.com/github/cmark-gfm/commit/587a12bb5">https://github.com/github/cmark-gfm/commit/587a12bb5</a>...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/d0e81e2392861ad3f6f27e895080cdfc6a8e72e7"><code>d0e81e2</code></a> I've used this version of the update_submodules script for several releases, ...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/42cfc90251353f9fceda91b884d0ded8d3da0bcf"><code>42cfc90</code></a> Merge pull request <a href="https://redirect.github.com/gjtorikian/commonmarker/issues/236">#236</a> from anticomputer/update-to-0.29.0.gfm.10</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/d793fbf45106f17c1eb721293bcc8d098bd999dc"><code>d793fbf</code></a> Update cmark-upstream to <a href="https://github.com/github/cmark-gfm/commit/1e230827a">https://github.com/github/cmark-gfm/commit/1e230827a</a>...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/4e4588f2e0d34a21eeb79ec53459d248fdf56b39"><code>4e4588f</code></a> Update Makefile for export header consolidation</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/2eb8ca8f2f4463448806663d72218cdcc0a9f38c"><code>2eb8ca8</code></a> Update cmark-upstream to <a href="https://github.com/github/cmark-gfm/commit/c8dcdc71c">https://github.com/github/cmark-gfm/commit/c8dcdc71c</a>...</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/bbb49db7223d71ad9366309c358c7c09a4e1c5a8"><code>bbb49db</code></a> HtmlRenderer: don't nest &lt;strong&gt;</li>
<li><a href="https://github.com/gjtorikian/commonmarker/commit/f303e6bae7d83c76f3a929fa9e59ae2e3ac27081"><code>f303e6b</code></a> :gem: release 0.23.9</li>
<li>Additional commits viewable in <a href="https://github.com/gjtorikian/commonmarker/compare/v0.23.6...v0.23.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=commonmarker&package-manager=bundler&previous-version=0.23.6&new-version=0.23.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-21 21:36:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.57.0 to 1.57.1 in /bindings/go-apiv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-21 21:35:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.14.0 to 0.17.0 in /bindings/go-apiv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.14.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.14.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.14.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-protos/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-21 21:35:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Release v0.3.3 commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release v0.3.3 commit

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-21 21:34:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc v1.56.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                +       github.com/golang/protobuf v1.5.3
+       google.golang.org/grpc v1.56.3
+       google.golang.org/protobuf v1.32.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-21 21:18:46 +0000 UTC
    </div>
</div>

