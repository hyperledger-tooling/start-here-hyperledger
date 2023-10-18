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
                PR <a href="https://github.com/hyperledger/cacti/pull/2782" class=".btn">#2782</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/sdks/fabric/go-sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-11 23:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/core/network/fabric-interop-cc/libs/assetexchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-11 23:36:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2775" class=".btn">#2775</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/core/network/fabric-interop-cc/libs/utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-11 23:35:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2774" class=".btn">#2774</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/common/protos-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-11 23:35:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2773" class=".btn">#2773</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/samples/fabric/simplestatewithacl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-11 23:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2772" class=".btn">#2772</a>
            </td>
            <td>
                <b>
                    build(deps): bump golang.org/x/net from 0.8.0 to 0.17.0 in /weaver/samples/fabric/go-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.8.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.8.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.8.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-11 23:35:09 +0000 UTC
    </div>
</div>

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

