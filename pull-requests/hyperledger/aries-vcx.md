---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/783" class=".btn">#783</a>
            </td>
            <td>
                <b>
                    Avoid misusing peer dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span><span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                We have the following local dependency chain of node modules in the project:

`@hyperledger/vcx-napi-rs` -> `@hyperledger/node-vcx-wrapper` -> `@hyperledger/vcxagent-core`

Currently, we are specifying local node dependencies twice:

* as `devDependencies` (via relative path) for local development, and
* as `peerDependencies` (referring to a previously published version) for publishing.

Moreover:
* `vcxagent-core`, unnecessarily specifies both `node-vcx-wrapper` and `vcx-napi-rs` dependency, and
* since all publish CI jobs run in parallel, both `node-vcx-wrapper` and `vcxagent-core` use the version of a previous release of their dependencies for publishing.

The current approach is obviously not ideal, misuses the concept of a peer dependency and causes version resolution issues when both `node-vcx-wrapper` and `vcxagent-core` (of the same version) are installed in the same package.

This PR eliminates duplicate imports, replaces peer with prod dependencies via a relative path for local development and sets the appropriate version before publishing (which now happens sequentially in the order of dependence).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-26 17:11:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.43 to 0.10.48
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.43 to 0.10.48.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl v0.10.48</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix LibreSSL version checking in openssl/ by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1851">sfackler/rust-openssl#1851</a></li>
<li>Skip a test that hangs on OpenSSL 3.1.0 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1850">sfackler/rust-openssl#1850</a></li>
<li>Improve reliability of some tests by <a href="https://github.com/smoelius"><code>@​smoelius</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1852">sfackler/rust-openssl#1852</a></li>
<li>Fix a series of security issues by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1854">sfackler/rust-openssl#1854</a></li>
<li>Release openssl v0.10.48 and openssl-sys v0.9.83 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1855">sfackler/rust-openssl#1855</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/smoelius"><code>@​smoelius</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1852">sfackler/rust-openssl#1852</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.47...openssl-v0.10.48">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.47...openssl-v0.10.48</a></p>
<h2>openssl v0.10.47</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.46</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.45</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.44</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4ff734fe4c5a22f7346b7b3c47ece4c4c1c01817"><code>4ff734f</code></a> Release openssl v0.10.48 and openssl-sys v0.9.83 (<a href="https://redirect.github.com/sfackler/rust-openssl/issues/1855">#1855</a>)</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/5efceaabd69c540b487f6372be4982cf94884008"><code>5efceaa</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1854">#1854</a> from alex/davids-openssl-of-horrors</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/6ced4f305e44df7ca32e478621bf4840b122f1a3"><code>6ced4f3</code></a> Fix race condition with X509Name creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a7528056c5be6f3fbabc52c2fd02882b208d5939"><code>a752805</code></a> Document the horror show</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/78aa9aa22cfd58ac33d1e19184cec667438fd2a1"><code>78aa9aa</code></a> Always provide an X509V3Context in X509Extension::new because OpenSSL require...</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/332311b597cc444a10d4acaf122ee58bd1bc8ff8"><code>332311b</code></a> Resolve an injection vulnerability in EKU creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/482575bff434f58b80ffea34a9610d0ff265ac1f"><code>482575b</code></a> Resolve an injection vulnerability in SAN creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/690eeb2ac20d47e43f04d8cb43f03d4128946b81"><code>690eeb2</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1852">#1852</a> from smoelius/master</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/e5b6d97ed170f835b56440d79edcd46381a46ebc"><code>e5b6d97</code></a> Improve reliability of some tests</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/319200ab93e252a3c0e127adc1e4c43a90f063a1"><code>319200a</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1851">#1851</a> from alex/libressl-versions</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.43...openssl-v0.10.48">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.43&new-version=0.10.48)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 01:29:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    Add state machines implementation guidelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                Per discussions on the last 2 community calls

https://wiki.hyperledger.org/display/ARIES/2023-03-23+Aries-vcx+community+call
https://wiki.hyperledger.org/display/ARIES/2023-03-16+Aries-vcx+community+call

It will be important to stay aligned on the approach as we are preparing to rewrite state machines with the state pattern.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 15:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/780" class=".btn">#780</a>
            </td>
            <td>
                <b>
                    Bump rmp-serde from 0.13.7 to 1.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [rmp-serde](https://github.com/3Hren/msgpack-rust) from 0.13.7 to 1.1.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/3Hren/msgpack-rust/commits/rmp-serde/v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rmp-serde&package-manager=cargo&previous-version=0.13.7&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 22:23:57 +0000 UTC
    </div>
</div>

