---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/518" class=".btn">#518</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.6.18 to 1.6.26
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-smart-client/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 21:26:38 +0000 UTC
    </div>
</div>

