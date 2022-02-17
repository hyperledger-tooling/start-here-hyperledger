---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Update proto files and generated python files to support Iroha 1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">iroha1</span>
            </td>
            <td>
                New features were added to https://github.com/hyperledger/iroha in version Iroha 1.4, which modified protobuf files. Thats why client libraries should be updated.

Features which modified protobuf files:
1. Syncing nodes: https://github.com/hyperledger/iroha/pull/1648/
2. Health check: https://github.com/hyperledger/iroha/pull/1735
_____________
- commit 1: I've updated proto files with attached script: https://github.com/hyperledger/iroha-python/blob/main/scripts/download-schema.py
- commit 2: I've generated python files from proto with attached script: https://github.com/hyperledger/iroha-python/blob/main/scripts/compile-proto.py
_____________
Signed-off-by: Grzegorz Bazior <g.bazior@yodiss.pl>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 13:45:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Bump protobuf from 3.12.2 to 3.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobuf](https://github.com/protocolbuffers/protobuf) from 3.12.2 to 3.15.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.15.0</h2>
<h1>Protocol Compiler</h1>
<ul>
<li>Optional fields for proto3 are enabled by default, and no longer require
the --experimental_allow_proto3_optional flag.</li>
</ul>
<h1>C++</h1>
<ul>
<li>MessageDifferencer: fixed bug when using custom ignore with multiple
unknown fields</li>
<li>Use init_seg in MSVC to push initialization to an earlier phase.</li>
<li>Runtime no longer triggers -Wsign-compare warnings.</li>
<li>Fixed -Wtautological-constant-out-of-range-compare warning.</li>
<li>DynamicCastToGenerated works for nullptr input for even if RTTI is disabled</li>
<li>Arena is refactored and optimized.</li>
<li>Clarified/specified that the exact value of Arena::SpaceAllocated() is an
implementation detail users must not rely on. It should not be used in
unit tests.</li>
<li>Change the signature of Any::PackFrom() to return false on error.</li>
<li>Add fast reflection getter API for strings.</li>
<li>Constant initialize the global message instances</li>
<li>Avoid potential for missed wakeup in UnknownFieldSet</li>
<li>Now Proto3 Oneof fields have &quot;has&quot; methods for checking their presence in
C++.</li>
<li>Bugfix for NVCC</li>
<li>Return early in _InternalSerialize for empty maps.</li>
<li>Adding functionality for outputting map key values in proto path logging
output (does not affect comparison logic) and stop printing 'value' in the
path. The modified print functionality is in the
MessageDifferencer::StreamReporter.</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8129">protocolbuffers/protobuf#8129</a></li>
<li>Ensure that null char symbol, package and file names do not result in a
crash.</li>
<li>Constant initialize the global message instances</li>
<li>Pretty print 'max' instead of numeric values in reserved ranges.</li>
<li>Removed remaining instances of std::is_pod, which is deprecated in C++20.</li>
<li>Changes to reduce code size for unknown field handling by making uncommon
cases out of line.</li>
<li>Fix std::is_pod deprecated in C++20 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/7180">#7180</a>)</li>
<li>Fix some -Wunused-parameter warnings (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8053">#8053</a>)</li>
<li>Fix detecting file as directory on zOS issue <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8051">#8051</a> (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8052">#8052</a>)</li>
<li>Don't include sys/param.h for _BYTE_ORDER (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8106">#8106</a>)</li>
<li>remove CMAKE_THREAD_LIBS_INIT from pkgconfig CFLAGS (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8154">#8154</a>)</li>
<li>Fix TextFormatMapTest.DynamicMessage issue#5136 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8159">#8159</a>)</li>
<li>Fix for compiler warning issue#8145 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8160">#8160</a>)</li>
<li>fix: support deprecated enums for GCC &lt; 6 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8164">#8164</a>)</li>
<li>Fix some warning when compiling with Visual Studio 2019 on x64 target (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8125">#8125</a>)</li>
</ul>
<h1>Python</h1>
<ul>
<li>Provided an override for the reverse() method that will reverse the internal
collection directly instead of using the other methods of the BaseContainer.</li>
<li>MessageFactory.CreateProtoype can be overridden to customize class creation.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/ae50d9b9902526efd6c7a1907d09739f959c6297"><code>ae50d9b</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/8260126500f073894c38b2211d383442eb7e58d5"><code>8260126</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/c741c4660443da46bfaf6c96fd1f01e743f97b56"><code>c741c46</code></a> Resovled issue in the .pb.cc files</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/eef276412ec417e2f0563c1c51d59a968cb2a6db"><code>eef2764</code></a> Resolved an issue where NO_DESTROY and CONSTINIT were in incorrect order</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/0040102e6f001724194d9c4c6bcd5effcec52bf1"><code>0040102</code></a> Updated collect_all_artifacts.sh for Ubuntu Xenial</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/26cb6a7a6d7973657f09fc44b201287c046da62e"><code>26cb6a7</code></a> Delete root-owned files in Kokoro builds</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/1e924efa90b476d23157426ad1eb17301bc4df41"><code>1e924ef</code></a> Update port_def.inc</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/9a80cf12254dec1af833d9fb78a80673dce45dc4"><code>9a80cf1</code></a> Update coded_stream.h</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/a97c4f4f2c9e5ffce0db787268414eb141194c62"><code>a97c4f4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8276">#8276</a> from haberman/php-warning</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/44cd75d2153fab614480517e40ee4c10cb153716"><code>44cd75d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8282">#8282</a> from haberman/changelog</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.12.2...v3.15.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobuf&package-manager=pip&previous-version=3.12.2&new-version=3.15.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 02:52:38 +0000 UTC
    </div>
</div>

