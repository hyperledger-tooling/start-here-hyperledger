---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4582" class=".btn">#4582</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.6.18 to 1.6.26
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.6.18 to 1.6.26.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/releases">github.com/containerd/containerd's releases</a>.</em></p>
<blockquote>
<h2>containerd 1.6.26</h2>
<p>Welcome to the v1.6.26 release of containerd!</p>
<p>The twenty-sixth patch release for containerd 1.6 contains various fixes and updates.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix windows default path overwrite issue</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9441">#9441</a>)</li>
<li><strong>Update push to inherit distribution sources from parent</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9453">#9453</a>)</li>
<li><strong>Mask <code>/sys/devices/virtual/powercap</code> path in runtime spec and deny in default apparmor profile</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-7ww5-4wqc-m92c">GHSA-7ww5-4wqc-m92c</a>)</li>
</ul>
<h3>Deprecation Warnings</h3>
<ul>
<li><strong>Emit deprecation warning for AUFS snapshotter usage</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9448">#9448</a>)</li>
<li><strong>Emit deprecation warning for v1 runtime usage</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9468">#9468</a>)</li>
<li><strong>Emit deprecation warning for CRI v1alpha1 usage</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9468">#9468</a>)</li>
</ul>
<p>See the changelog for complete list of changes</p>
<p>Please try out the release binaries and report any issues at
<a href="https://github.com/containerd/containerd/issues">https://github.com/containerd/containerd/issues</a>.</p>
<h3>Contributors</h3>
<ul>
<li>Samuel Karp</li>
<li>Derek McGowan</li>
<li>Kohei Tokunaga</li>
<li>Phil Estes</li>
<li>Bjorn Neergaard</li>
<li>Sebastiaan van Stijn</li>
<li>Brian Goff</li>
<li>Charity Kathure</li>
<li>Kazuyoshi Kato</li>
<li>Milas Bowman</li>
<li>Wei Fu</li>
<li>ruiwen-zhao</li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>[release/1.6] Prepare release notes for v1.6.26 (<a href="https://redirect.github.com/containerd/containerd/pull/9490">#9490</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/ac5c5d3e03ab3c5b8103a1c0bd9931389f7a8fcf"><code>ac5c5d3e0</code></a> Prepare release notes for v1.6.26</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-7ww5-4wqc-m92c">GHSA-7ww5-4wqc-m92c</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/02f07fe1994a3ddda3626c1ede2e32bc82b8e426"><code>02f07fe19</code></a> contrib/apparmor: deny /sys/devices/virtual/powercap</li>
<li><a href="https://github.com/containerd/containerd/commit/c94577e78d2924ddeb90d1601e31b50ee3acac48"><code>c94577e78</code></a> oci/spec: deny /sys/devices/virtual/powercap</li>
</ul>
</li>
<li>[release/1.6] update to go1.20.12, test go1.21.5 (<a href="https://redirect.github.com/containerd/containerd/pull/9472">#9472</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/7cbdfc92ef38f789f1a2773fa6fac405d361a6cc"><code>7cbdfc92e</code></a> update to go1.20.12, test go1.21.5</li>
<li><a href="https://github.com/containerd/containerd/commit/024b1cce6b27f10e00bb9bde33a5fe9563545f8d"><code>024b1cce6</code></a> update to go1.20.11, test go1.21.4</li>
</ul>
</li>
<li>[release/1.6] Add cri-api v1alpha2 usage warning to all api calls (<a href="https://redirect.github.com/containerd/containerd/pull/9484">#9484</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/3dd1e886e55dd695541fdcd67420c2888645a495"><code>3dd1e88</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9490">#9490</a> from dmcgowan/prepare-1.6.26</li>
<li><a href="https://github.com/containerd/containerd/commit/746b910f05855c8bfdb4415a1c0f958b234910e5"><code>746b910</code></a> Merge pull request from GHSA-7ww5-4wqc-m92c</li>
<li><a href="https://github.com/containerd/containerd/commit/ac5c5d3e03ab3c5b8103a1c0bd9931389f7a8fcf"><code>ac5c5d3</code></a> Prepare release notes for v1.6.26</li>
<li><a href="https://github.com/containerd/containerd/commit/e7ca005043f6974536c3f8e0da42f93b5bdc2879"><code>e7ca005</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9472">#9472</a> from thaJeztah/1.6_update_golang_1.20.12</li>
<li><a href="https://github.com/containerd/containerd/commit/7cbdfc92ef38f789f1a2773fa6fac405d361a6cc"><code>7cbdfc9</code></a> update to go1.20.12, test go1.21.5</li>
<li><a href="https://github.com/containerd/containerd/commit/024b1cce6b27f10e00bb9bde33a5fe9563545f8d"><code>024b1cc</code></a> update to go1.20.11, test go1.21.4</li>
<li><a href="https://github.com/containerd/containerd/commit/2e404598e7da93f4ad8b13bb6119441a5e3c83b0"><code>2e40459</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9484">#9484</a> from ruiwen-zhao/cri-api-warning-1.6</li>
<li><a href="https://github.com/containerd/containerd/commit/64e56bfde95828660971673d20952f275cc2c0ba"><code>64e56bf</code></a> Add cri-api v1alpha2 usage warning to all api calls</li>
<li><a href="https://github.com/containerd/containerd/commit/c566b7d46668de23d2881eb86ce1b76ca23c8a75"><code>c566b7d</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9468">#9468</a> from samuelkarp/deprecation-warning-runtime-1.6</li>
<li><a href="https://github.com/containerd/containerd/commit/efefd3bf334b5df0e97bff0be61ba906a9b3b528"><code>efefd3b</code></a> tasks: emit warning for runc v1 runtime</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.6.18...v1.6.26">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.6.18&new-version=1.6.26)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 21:26:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4581" class=".btn">#4581</a>
            </td>
            <td>
                <b>
                    Check error in the same line
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I20200cff6e7ea6f4bc508e13ea96a24d39de74f2

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset follows Go style to check error immediately after calling the method in the same line.


#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 19:04:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4580" class=".btn">#4580</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/crypto from 0.14.0 to 0.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.14.0 to 0.17.0.
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
<li>Additional commits viewable in <a href="https://github.com/golang/crypto/compare/v0.14.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.14.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 23:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4579" class=".btn">#4579</a>
            </td>
            <td>
                <b>
                    Add doc links to chaincode access control (backport #4576)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4576 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 14:53:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4578" class=".btn">#4578</a>
            </td>
            <td>
                <b>
                    Directly check the return error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I1138688b89200c6bcb0b18f854c46f03815ad15d

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset simplifies the code by directly checking the return error,
    which follows the Go style.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 22:41:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4577" class=".btn">#4577</a>
            </td>
            <td>
                <b>
                    Private data purge test improvements - release-2.5 backport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport private data purge test improvements to release-2.5.
This should resolve the flake failures in release-2.5 branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 19:14:18 +0000 UTC
    </div>
</div>

