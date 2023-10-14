---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.7.0 to 0.17.0 in /packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/fixtures/go/asset-transfer-private-data/chaincode-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.7.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.7.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.7.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 21:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2761" class=".btn">#2761</a>
            </td>
            <td>
                <b>
                    docs(README): updated README files to reflect recent documentation upgrades
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated README files to add current info and update links to point to the newly published integrated documentation (https://hyperledger.github.io/cacti/)
- Added a blog entries section to the documentation website.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 21:11:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2756" class=".btn">#2756</a>
            </td>
            <td>
                <b>
                    build(deps): bump webpki from 0.22.1 to 0.22.4 in /weaver/common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [webpki](https://github.com/briansmith/webpki) from 0.22.1 to 0.22.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/briansmith/webpki/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpki&package-manager=cargo&previous-version=0.22.1&new-version=0.22.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 02:47:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): add runtime type validation to HTTP verbs pulled from OAS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                This addresses the shortcomings of the linter fix provided in #2751, which
uses unchecked casts to the linter warnings go away.
With the fix of #2751, at runtime, the possibility of a crash is still there
exactly as before, but it has silenced the linter about calling that
possibility out.

We now use a type guard to check the type of the object before casting it
and therefore ensure that at runtime the cast will not produce a crash.

[skip ci]

Depends on #2751
Depends on #2754

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 17:59:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2754" class=".btn">#2754</a>
            </td>
            <td>
                <b>
                    feat(common): add express http verb method name string literal type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Also ships with a user-defined typescript type-guard so that we can
ensure at runtime that the string literal value is indeed one of the
valid ExpressJS HTTP verb method names.
2. The primary use-case for this is checking at runtime the HTTP verb
name of OpenAPI specifications that are being loaded into the API.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 17:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2753" class=".btn">#2753</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add json-rpc proxy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add proxy endpoint handling. Requests sent to this endpoint will be passed directly to the ethereum node.
- Add test to verify that proxy is working.
- Update README of ethereum connector.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 12:21:11 +0000 UTC
    </div>
</div>

