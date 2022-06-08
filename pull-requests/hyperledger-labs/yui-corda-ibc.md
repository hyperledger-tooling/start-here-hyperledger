---
layout: default
title: yui-corda-ibc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-corda-ibc
---

# yui-corda-ibc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-corda-ibc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    build(deps): bump tokio from 1.9.0 to 1.13.1 in /rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.9.0 to 1.13.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.13.1</h2>
<h1>1.13.1 (November 15, 2021)</h1>
<p>This release fixes a data race when sending and receiving on a
closed <code>oneshot</code> channel (<a href="https://rustsec.org/advisories/RUSTSEC-2021-0124.html">RUSTSEC-2021-0124</a>).</p>
<h3>Fixed</h3>
<ul>
<li>sync: fix a data race between <code>oneshot::Sender::send</code> and awaiting a
<code>oneshot::Receiver</code> when the oneshot has been closed (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4226">#4226</a>)</li>
</ul>
<h2>Tokio v1.13.0</h2>
<h1>1.13.0 (October 29, 2021)</h1>
<h3>Fixed</h3>
<ul>
<li>sync: fix <code>Notify</code> to clone the waker before locking its waiter list (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4129">#4129</a>)</li>
<li>tokio: add riscv32 to non atomic64 architectures (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4185">#4185</a>)</li>
</ul>
<h3>Added</h3>
<ul>
<li>net: add <code>poll_{recv,send}_ready</code> methods to <code>udp</code> and <code>uds_datagram</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4131">#4131</a>)</li>
<li>net: add <code>try_*</code>, <code>readable</code>, <code>writable</code>, <code>ready</code>, and <code>peer_addr</code> methods to split halves (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4120">#4120</a>)</li>
<li>sync: add <code>blocking_lock</code> to <code>Mutex</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4130">#4130</a>)</li>
<li>sync: add <code>watch::Sender::send_replace</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3962">#3962</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4195">#4195</a>)</li>
<li>sync: expand <code>Debug</code> for <code>Mutex&lt;T&gt;</code> impl to unsized <code>T</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4134">#4134</a>)</li>
<li>tracing: instrument time::Sleep (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4072">#4072</a>)</li>
<li>tracing: use structured location fields for spawned tasks (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4128">#4128</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>io: add assert in <code>copy_bidirectional</code> that <code>poll_write</code> is sensible (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4125">#4125</a>)</li>
<li>macros: use qualified syntax when polling in <code>select!</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4192">#4192</a>)</li>
<li>runtime: handle <code>block_on</code> wakeups better (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4157">#4157</a>)</li>
<li>task: allocate callback on heap immediately in debug mode (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4203">#4203</a>)</li>
<li>tokio: assert platform-minimum requirements at build time (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3797">#3797</a>)</li>
</ul>
<h3>Documented</h3>
<ul>
<li>docs: conversion of doc comments to indicative mood (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4174">#4174</a>)</li>
<li>docs: add returning on the first error example for <code>try_join!</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4133">#4133</a>)</li>
<li>docs: fixing broken links in <code>tokio/src/lib.rs</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4132">#4132</a>)</li>
<li>signal: add example with background listener (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4171">#4171</a>)</li>
<li>sync: add more oneshot examples (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4153">#4153</a>)</li>
<li>time: document <code>Interval::tick</code> cancel safety (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4152">#4152</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3797">#3797</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3797">tokio-rs/tokio#3797</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3962">#3962</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3962">tokio-rs/tokio#3962</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/2a3c803dd1c487868eabcef547066952cc07624e"><code>2a3c803</code></a> chore: prepare Tokio v1.13.1 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4235">#4235</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/7d8de50482a077349db721c7cad3034b093a0083"><code>7d8de50</code></a> oneshot: document UnsafeCell invariants  (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4229">#4229</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/ab0e60ddeaf1b617ed4990901d2410ef810f1a61"><code>ab0e60d</code></a> sync: fix racy <code>UnsafeCell</code> access on a closed oneshot (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4226">#4226</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/ac89d8926d0c06eeb62936b0843a5278cd98ade0"><code>ac89d89</code></a> chore: prepare Tokio v1.13.0 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4196">#4196</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/e184205421e7a5e6d397805adb516e661819240c"><code>e184205</code></a> chore: prepare tokio-macros 1.6.0 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4197">#4197</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/44a1aad8df43bef416ac91dfc4b9b5614c3d34fd"><code>44a1aad</code></a> task: allocate callback on heap immediately in debug mode (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4203">#4203</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/75c07770bfbfea4e5fd914af819c741ed9c3fc36"><code>75c0777</code></a> sync: make <code>watch::send_replace</code> infallible (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4195">#4195</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/268ed5e73e39c907e0252791cf58daa41980b61b"><code>268ed5e</code></a> task: add more tips + links to <code>spawn_blocking</code> docs (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4150">#4150</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/0c68b89452c6b978002aefe1b3daa391f2125616"><code>0c68b89</code></a> codec: update stream impl for Framed to return <code>None</code> after <code>Err</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4166">#4166</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/827694a9e368b0d339a5b9eeb4fc0fb3c3e7df26"><code>827694a</code></a> ci: fix nightly version for cirrus ci (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4200">#4200</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.9.0...tokio-1.13.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.9.0&new-version=1.13.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-corda-ibc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:48:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    build(deps): bump prost-types from 0.7.0 to 0.8.0 in /rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [prost-types](https://github.com/tokio-rs/prost) from 0.7.0 to 0.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/prost/releases">prost-types's releases</a>.</em></p>
<blockquote>
<h2>v0.8.0</h2>
<p><em>PROST!</em> is a <a href="https://developers.google.com/protocol-buffers/">Protocol Buffers</a> implementation for the <a href="https://www.rust-lang.org/">Rust Language</a>. <code>prost</code> generates simple, idiomatic Rust code from <code>proto2</code> and <code>proto3</code> files.</p>
<p><em>NOTE: This version contains a security fix for <code>prost-types</code> and is recommend that you upgrade to it from &lt;0.7.</em></p>
<p><code>prost</code> 0.8.0 includes breaking changes:</p>
<ul>
<li><code>Timestamp</code>'s <code>From</code> implementation for converting into <code>SystemTime</code> has been converted to a fallible <code>TryFrom</code> implementation.</li>
<li><code>prost-build</code>'s <code>compile_protos</code> now takes <code>impl AsRef&lt;Path&gt;</code> to allow each parameter to use its own generic type.</li>
<li>Bundled <code>protoc</code> version bumped to <code>3.15.8</code></li>
</ul>
<p>As well as many new (non-breaking) changes:</p>
<ul>
<li><a href="https://github.com/pluth"><code>@​pluth</code></a> enabled zero-copy support for <code>Bytes</code> based fields.</li>
<li><a href="https://github.com/sfackler"><code>@​sfackler</code></a> for fixing message optionals and oneofs in <code>prost-build</code>.</li>
<li><a href="https://github.com/rubdos"><code>@​rubdos</code></a> for adding the ability to encode prost messages directly to a <code>Vec&lt;u8&gt;</code>.</li>
</ul>
<p>and numerous smaller fixes. Many thanks to the generous contributors who have helped out since 0.7:</p>
<ul>
<li><a href="https://github.com/dfreese"><code>@​dfreese</code></a></li>
<li><a href="https://github.com/carols10cents"><code>@​carols10cents</code></a></li>
<li><a href="https://github.com/pluth"><code>@​pluth</code></a></li>
<li><a href="https://github.com/jfornoff"><code>@​jfornoff</code></a></li>
<li><a href="https://github.com/sphw"><code>@​sphw</code></a></li>
<li><a href="https://github.com/bpowers"><code>@​bpowers</code></a></li>
<li><a href="https://github.com/sfackler"><code>@​sfackler</code></a></li>
<li><a href="https://github.com/koushiro"><code>@​koushiro</code></a></li>
<li><a href="https://github.com/dbrgn"><code>@​dbrgn</code></a></li>
<li><a href="https://github.com/argv-minus-one"><code>@​argv-minus-one</code></a></li>
<li><a href="https://github.com/nagisa"><code>@​nagisa</code></a></li>
<li><a href="https://github.com/evanj"><code>@​evanj</code></a></li>
<li><a href="https://github.com/aquarhead"><code>@​aquarhead</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/prost/commit/998f288fe09a2e457fe23b54f61b1f106c608fb2"><code>998f288</code></a> release 0.8.0</li>
<li><a href="https://github.com/tokio-rs/prost/commit/edb1464b71528286a6ce74278af05f19c3e0e820"><code>edb1464</code></a> derive: Fix unstable fn name collision warning (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/499">#499</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/4ae66ccca65c3c348c577860bca0df0df821516d"><code>4ae66cc</code></a> Remove path type generic for better ergonomic (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/496">#496</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/5d93c55426d9c219fb1fb065adfa8fd3e43833a1"><code>5d93c55</code></a> Bundled protoc only if the interpreter exists (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/459">#459</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/fdc319c8f118f91cbc73752a30238273204dabc8"><code>fdc319c</code></a> prost-build lib.rs: Minor doc comment edits (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/498">#498</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/d8cb390d606638e0bb24208a56996b680e9d21b4"><code>d8cb390</code></a> Add encode to Vec&lt;u8&gt; (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/378">#378</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/59f2a7311dd6540696bfd0145f5281ce495f4385"><code>59f2a73</code></a> Fix <a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/438">#438</a>: Check for overflow in <code>Duration</code> and <code>Timestamp</code> processing (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/439">#439</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/0833d467bd55ee7ff427e0484fc299366ad9ab7d"><code>0833d46</code></a> Add afl fuzz tests (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/272">#272</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/c8691b701a5e2e542e52122a73af1f696c437a09"><code>c8691b7</code></a> Update repository &amp; author references to tokio-rs (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/489">#489</a>)</li>
<li><a href="https://github.com/tokio-rs/prost/commit/6cf97ea422b09d98de34643c4dda2d4f8b7e23e6"><code>6cf97ea</code></a> Update outdated dependencies (<a href="https://github-redirect.dependabot.com/tokio-rs/prost/issues/474">#474</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/prost/compare/v0.7.0...v0.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prost-types&package-manager=cargo&previous-version=0.7.0&new-version=0.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-corda-ibc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 19:25:58 +0000 UTC
    </div>
</div>

