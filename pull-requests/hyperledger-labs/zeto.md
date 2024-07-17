---
layout: default
title: zeto
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/zeto
---

# zeto <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/zeto){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Initial sparse merkle tree impl; missing proof generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:49:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/crypto from 0.7.0 to 0.17.0 in /zkp/golang
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.7.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/crypto/commit/9d2ee975ef9fe627bf0a6f01c1f69e8ef1d4f05d"><code>9d2ee97</code></a> ssh: implement strict KEX protocol changes</li>
<li><a href="https://github.com/golang/crypto/commit/4e5a26183ecb4f9a0f85c8f8dbe7982885435436"><code>4e5a261</code></a> ssh: close net.Conn on all NewServerConn errors</li>
<li><a href="https://github.com/golang/crypto/commit/152cdb1503ebc13bc0fbb68f92ee189ebf9e3d00"><code>152cdb1</code></a> x509roots/fallback: update bundle</li>
<li><a href="https://github.com/golang/crypto/commit/fdfe1f8531a1adcc300c8eba98cb372044826d62"><code>fdfe1f8</code></a> ssh: defer channel window adjustment</li>
<li><a href="https://github.com/golang/crypto/commit/b8ffc16e10063067bac0e15c6d7f7995937503ce"><code>b8ffc16</code></a> blake2b: drop Go 1.6, Go 1.8 compatibility</li>
<li><a href="https://github.com/golang/crypto/commit/7e6fbd82c804e1760feb603fe21caecb0af0a124"><code>7e6fbd8</code></a> ssh: wrap errors from client handshake</li>
<li><a href="https://github.com/golang/crypto/commit/bda2f3f5cfce3f27039acccd823693f6d67c2a74"><code>bda2f3f</code></a> argon2: avoid clobbering BP</li>
<li><a href="https://github.com/golang/crypto/commit/325b735346247f48971d2b37d24dd180a35f391f"><code>325b735</code></a> ssh/test: skip TestSSHCLIAuth on Windows</li>
<li><a href="https://github.com/golang/crypto/commit/1eadac50a566dfaa1b603ca15e8ad3cbd1c77b20"><code>1eadac5</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/crypto/commit/b2d7c26edb17864f117d8b0ee73c1843bcc6090f"><code>b2d7c26</code></a> ssh: add (*Client).DialContext method</li>
<li>Additional commits viewable in <a href="https://github.com/golang/crypto/compare/v0.7.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.7.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/zeto/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 15:18:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    zeto-js should make no assumptions about environment variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exported functions in this library should only expose the pre-compiled WASM circuits that ship with the library. Because key generation is done separately, key loading should be handled by the client and not by the library.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-11 18:19:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    update readme with details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add details
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-11 05:59:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Add Makefile to generate all proving keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run "make keys" in zkp folder.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-10 19:59:15 +0000 UTC
    </div>
</div>

