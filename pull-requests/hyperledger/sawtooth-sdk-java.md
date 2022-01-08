---
layout: default
title: sawtooth-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-java
---

# sawtooth-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-java/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Bump protobuf-java from 3.6.1 to 3.16.1 in /examples/intkey_java
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobuf-java](https://github.com/protocolbuffers/protobuf) from 3.6.1 to 3.16.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf-java's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.16.1</h2>
<h1>Java</h1>
<ul>
<li>Improve performance characteristics of UnknownFieldSet parsing (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
</ul>
<h2>Protocol Buffers v3.16.0</h2>
<h1>C++</h1>
<ul>
<li>Fix compiler warnings issue found in conformance_test_runner <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8189">#8189</a> (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8190">#8190</a>)</li>
<li>Fix MinGW-w64 build issues. (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8286">#8286</a>)</li>
<li>[Protoc] C++ Resolved an issue where NO_DESTROY and CONSTINIT are in incorrect order (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8296">#8296</a>)</li>
<li>Fix PROTOBUF_CONSTINIT macro redefinition (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8323">#8323</a>)</li>
<li>Delete StringPiecePod (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8353">#8353</a>)</li>
<li>Fix gcc error: comparison of unsigned expression in '&gt;= 0' is always … (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8309">#8309</a>)</li>
<li>Fix cmake install on iOS (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8301">#8301</a>)</li>
<li>Create a CMake option to control whether or not RTTI is enabled (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8347">#8347</a>)</li>
<li>Fix endian.h location on FreeBSD (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8351">#8351</a>)</li>
<li>Refactor util::Status (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8354">#8354</a>)</li>
<li>Make util::Status more similar to absl::Status (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8405">#8405</a>)</li>
<li>Fix -Wsuggest-destructor-override for generated C++ proto classes. (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8408">#8408</a>)</li>
<li>Refactor StatusOr and StringPiece (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8406">#8406</a>)</li>
<li>Refactor uint128 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8416">#8416</a>)</li>
<li>The ::pb namespace is no longer exposed due to conflicts.</li>
<li>Allow MessageDifferencer::TreatAsSet() (and friends) to override previous
calls instead of crashing.</li>
<li>Reduce the size of generated proto headers for protos with <code>string</code> or
<code>bytes</code> fields.</li>
<li>Move arena() operation on uncommon path to out-of-line routine</li>
<li>For iterator-pair function parameter types, take both iterators by value.</li>
<li>Code-space savings and perhaps some modest performance improvements in
RepeatedPtrField.</li>
<li>Eliminate nullptr check from every tag parse.</li>
<li>Remove unused _$name$<em>cached_byte_size</em> fields.</li>
<li>Serialize extension ranges together when not broken by a proto field in the
middle.</li>
<li>Do out-of-line allocation and deallocation of string object in ArenaString.</li>
<li>Streamline ParseContext::ParseMessage<!-- raw HTML omitted --> to avoid code bloat and improve
performance.</li>
<li>New member functions RepeatedField::Assign, RepeatedPtrField::{Add, Assign}.</li>
<li>Fix undefined behavior warning due to innocuous uninitialization of value
on an error path.</li>
<li>Avoid expensive inlined code space for encoding message length for messages
<blockquote>
<p>= 128 bytes and instead do a procedure call to a shared out-of-line routine.</p>
</blockquote>
</li>
<li>util::DefaultFieldComparator will be final in a future version of protobuf.
Subclasses should inherit from SimpleFieldComparator instead.</li>
</ul>
<h1>C#</h1>
<ul>
<li>Add .NET 5 target and improve WriteString performance with SIMD (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8147">#8147</a>)</li>
</ul>
<h1>Java</h1>
<ul>
<li>deps: update JUnit and Truth (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8319">#8319</a>)</li>
<li>Detect invalid overflow of byteLimit and return InvalidProtocolBufferException as documented.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/791a4355c365bd92720160671a7491be168055cb"><code>791a435</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/e8918723cfecb60082f067a98df0a16ffc003b62"><code>e891872</code></a> Update CHANGES.txt for 3.16.1 release</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/f554ccaa514967232cc494cf22947e1c73ca747f"><code>f554cca</code></a> Improve performance of parsing unknown fields in Java (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/2dc747c574b68a808ea4699d26942c8132fe2b09"><code>2dc747c</code></a> Update PHP release notes and update version to 3.16.0 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8573">#8573</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/debc03dfc5d71d7d642dd1c8f7d1c04b36e8a065"><code>debc03d</code></a> Update protobuf version to 3.16.0-rc2 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8556">#8556</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/17b0fb9149109e22d56cfa27f1f17b04508ea726"><code>17b0fb9</code></a> Make update_version.py compatible with Python 3 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8555">#8555</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/4aa425c6c5eb7914582ebd67ab8ecac464bdf271"><code>4aa425c</code></a> Cherry-pick <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8356">#8356</a> into 3.16.x (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8518">#8518</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/e8b78f8208971a28e566198d38e43ad5f49a9009"><code>e8b78f8</code></a> Fixed memory leak of Ruby arena objects. (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8465">#8465</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/7689f00ba8d1e818f2a8e7a4bf24577d9ccd5d84"><code>7689f00</code></a> Update protobuf version (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8448">#8448</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/6099c6505d73681bf98a5c5d8908cb5c3fd1bab9"><code>6099c65</code></a> Updated CHANGES.txt for 3.16.0 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8456">#8456</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.6.1...v3.16.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.protobuf:protobuf-java&package-manager=maven&previous-version=3.6.1&new-version=3.16.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/sawtooth-sdk-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 22:36:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-java/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Bump protobuf-java from 3.6.1 to 3.16.1 in /examples/xo_java
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [protobuf-java](https://github.com/protocolbuffers/protobuf) from 3.6.1 to 3.16.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf-java's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.16.1</h2>
<h1>Java</h1>
<ul>
<li>Improve performance characteristics of UnknownFieldSet parsing (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
</ul>
<h2>Protocol Buffers v3.16.0</h2>
<h1>C++</h1>
<ul>
<li>Fix compiler warnings issue found in conformance_test_runner <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8189">#8189</a> (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8190">#8190</a>)</li>
<li>Fix MinGW-w64 build issues. (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8286">#8286</a>)</li>
<li>[Protoc] C++ Resolved an issue where NO_DESTROY and CONSTINIT are in incorrect order (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8296">#8296</a>)</li>
<li>Fix PROTOBUF_CONSTINIT macro redefinition (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8323">#8323</a>)</li>
<li>Delete StringPiecePod (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8353">#8353</a>)</li>
<li>Fix gcc error: comparison of unsigned expression in '&gt;= 0' is always … (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8309">#8309</a>)</li>
<li>Fix cmake install on iOS (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8301">#8301</a>)</li>
<li>Create a CMake option to control whether or not RTTI is enabled (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8347">#8347</a>)</li>
<li>Fix endian.h location on FreeBSD (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8351">#8351</a>)</li>
<li>Refactor util::Status (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8354">#8354</a>)</li>
<li>Make util::Status more similar to absl::Status (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8405">#8405</a>)</li>
<li>Fix -Wsuggest-destructor-override for generated C++ proto classes. (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8408">#8408</a>)</li>
<li>Refactor StatusOr and StringPiece (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8406">#8406</a>)</li>
<li>Refactor uint128 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8416">#8416</a>)</li>
<li>The ::pb namespace is no longer exposed due to conflicts.</li>
<li>Allow MessageDifferencer::TreatAsSet() (and friends) to override previous
calls instead of crashing.</li>
<li>Reduce the size of generated proto headers for protos with <code>string</code> or
<code>bytes</code> fields.</li>
<li>Move arena() operation on uncommon path to out-of-line routine</li>
<li>For iterator-pair function parameter types, take both iterators by value.</li>
<li>Code-space savings and perhaps some modest performance improvements in
RepeatedPtrField.</li>
<li>Eliminate nullptr check from every tag parse.</li>
<li>Remove unused _$name$<em>cached_byte_size</em> fields.</li>
<li>Serialize extension ranges together when not broken by a proto field in the
middle.</li>
<li>Do out-of-line allocation and deallocation of string object in ArenaString.</li>
<li>Streamline ParseContext::ParseMessage<!-- raw HTML omitted --> to avoid code bloat and improve
performance.</li>
<li>New member functions RepeatedField::Assign, RepeatedPtrField::{Add, Assign}.</li>
<li>Fix undefined behavior warning due to innocuous uninitialization of value
on an error path.</li>
<li>Avoid expensive inlined code space for encoding message length for messages
<blockquote>
<p>= 128 bytes and instead do a procedure call to a shared out-of-line routine.</p>
</blockquote>
</li>
<li>util::DefaultFieldComparator will be final in a future version of protobuf.
Subclasses should inherit from SimpleFieldComparator instead.</li>
</ul>
<h1>C#</h1>
<ul>
<li>Add .NET 5 target and improve WriteString performance with SIMD (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8147">#8147</a>)</li>
</ul>
<h1>Java</h1>
<ul>
<li>deps: update JUnit and Truth (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8319">#8319</a>)</li>
<li>Detect invalid overflow of byteLimit and return InvalidProtocolBufferException as documented.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/791a4355c365bd92720160671a7491be168055cb"><code>791a435</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/e8918723cfecb60082f067a98df0a16ffc003b62"><code>e891872</code></a> Update CHANGES.txt for 3.16.1 release</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/f554ccaa514967232cc494cf22947e1c73ca747f"><code>f554cca</code></a> Improve performance of parsing unknown fields in Java (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/2dc747c574b68a808ea4699d26942c8132fe2b09"><code>2dc747c</code></a> Update PHP release notes and update version to 3.16.0 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8573">#8573</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/debc03dfc5d71d7d642dd1c8f7d1c04b36e8a065"><code>debc03d</code></a> Update protobuf version to 3.16.0-rc2 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8556">#8556</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/17b0fb9149109e22d56cfa27f1f17b04508ea726"><code>17b0fb9</code></a> Make update_version.py compatible with Python 3 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8555">#8555</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/4aa425c6c5eb7914582ebd67ab8ecac464bdf271"><code>4aa425c</code></a> Cherry-pick <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8356">#8356</a> into 3.16.x (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8518">#8518</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/e8b78f8208971a28e566198d38e43ad5f49a9009"><code>e8b78f8</code></a> Fixed memory leak of Ruby arena objects. (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8465">#8465</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/7689f00ba8d1e818f2a8e7a4bf24577d9ccd5d84"><code>7689f00</code></a> Update protobuf version (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8448">#8448</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/6099c6505d73681bf98a5c5d8908cb5c3fd1bab9"><code>6099c65</code></a> Updated CHANGES.txt for 3.16.0 (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/8456">#8456</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.6.1...v3.16.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.protobuf:protobuf-java&package-manager=maven&previous-version=3.6.1&new-version=3.16.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/sawtooth-sdk-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 22:36:00 +0000 UTC
    </div>
</div>

