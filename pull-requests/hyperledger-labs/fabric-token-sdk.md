---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    Update FSC dependencies
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
        Created At 2024-03-26 12:50:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    simpler token transaction flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The goal of this PR is to remove the need to distributed the fabric envelope to the participant nodes of a transaction.
It is enough that each node receives the token request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 14:04:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/583" class=".btn">#583</a>
            </td>
            <td>
                <b>
                    shared wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 08:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/582" class=".btn">#582</a>
            </td>
            <td>
                <b>
                    Delete tokens: move nilcheck and simplify the call used by HTLC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the nilcheck to make sure it gets used (Delete does not fail if the token doesn't exist).

When running two replicas of Token SDK, one instance will delete the token from the database and notify its mailman. A current limitation is that the mailman of the second replica will not be notified (if tok turns out to be nil we don't post the event). This is not new in this PR, but we should consider it when working on the statelessness of the Token SDK instance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 14:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/581" class=".btn">#581</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 24.0.7+incompatible to 24.0.9+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 24.0.7+incompatible to 24.0.9+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v24.0.9</h2>
<h2>24.0.9</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A24.0.9">docker/cli, 24.0.9 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A24.0.9">moby/moby, 24.0.9 milestone</a></li>
</ul>
<h2>Security</h2>
<p>This release contains security fixes for the following CVEs affecting Docker Engine and its components.</p>
<table>
<thead>
<tr>
<th>CVE</th>
<th>Component</th>
<th>Fix version</th>
<th>Severity</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://scout.docker.com/v/CVE-2024-21626">CVE-2024-21626</a></td>
<td>runc</td>
<td>1.1.12</td>
<td>High, CVSS 8.6</td>
</tr>
<tr>
<td><a href="https://scout.docker.com/v/CVE-2024-24557">CVE-2024-24557</a></td>
<td>Docker Engine</td>
<td>24.0.9</td>
<td>Medium, CVSS 6.9</td>
</tr>
</tbody>
</table>
<blockquote>
<p><strong>Important</strong> ⚠️</p>
<p>Note that this release of Docker Engine doesn't include fixes for the following known vulnerabilities in BuildKit:</p>
<ul>
<li><a href="https://scout.docker.com/v/CVE-2024-23651">CVE-2024-23651</a></li>
<li><a href="https://scout.docker.com/v/CVE-2024-23652">CVE-2024-23652</a></li>
<li><a href="https://scout.docker.com/v/CVE-2024-23653">CVE-2024-23653</a></li>
<li><a href="https://scout.docker.com/v/CVE-2024-23650">CVE-2024-23650</a></li>
</ul>
<p>To address these vulnerabilities, upgrade to <a href="https://github.com/docker/docker/blob/HEAD/25.0.md#2502">Docker Engine v25.0.2</a>.</p>
</blockquote>
<p>For more information about the security issues addressed in this release, and the unaddressed vulnerabilities in BuildKit, refer to the
<a href="https://www.docker.com/blog/docker-security-advisory-multiple-vulnerabilities-in-runc-buildkit-and-moby/">blog post</a>. For details about each vulnerability, see the relevant security advisory:</p>
<ul>
<li><a href="https://github.com/opencontainers/runc/security/advisories/GHSA-xr7r-f8xq-vfvv">CVE-2024-21626</a></li>
<li><a href="https://github.com/moby/moby/security/advisories/GHSA-xw73-rw38-6vjc">CVE-2024-24557</a></li>
</ul>
<h3>Packaging updates</h3>
<ul>
<li>Upgrade runc to <a href="https://github.com/opencontainers/runc/releases/tag/v1.1.12">v1.1.12</a>. <a href="https://redirect.github.com/moby/moby/pull/47269">moby/moby#47269</a></li>
<li>Upgrade containerd to <a href="https://github.com/containerd/containerd/releases/tag/v1.7.13">v1.7.13</a> (static binaries only). <a href="https://redirect.github.com/moby/moby/pull/47280">moby/moby#47280</a></li>
</ul>
<h2>v24.0.8</h2>
<h2>24.0.8</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A24.0.8">docker/cli, 24.0.8 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A24.0.8">moby/moby, 24.0.8 milestone</a></li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Live restore: Containers with auto remove (<code>docker run --rm</code>) are no longer forcibly removed on engine restart. <a href="https://redirect.github.com/moby/moby/pull/46869">moby/moby#46857</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/fca702de7f71362c8d103073c7e4a1d0a467fadd"><code>fca702d</code></a> Merge pull request from GHSA-xw73-rw38-6vjc</li>
<li><a href="https://github.com/moby/moby/commit/f78a7726d747847e443a5a5a4b4ad8ab31d87d78"><code>f78a772</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47281">#47281</a> from thaJeztah/24.0_backport_bump_containerd_binary...</li>
<li><a href="https://github.com/moby/moby/commit/61afffeeb3d4264db7a697ca8bd3d25824bee182"><code>61afffe</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47270">#47270</a> from thaJeztah/24.0_backport_bump_runc_binary_1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/b38e74c4e095d584e21576e9cc43a355446e5b71"><code>b38e74c</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47276">#47276</a> from thaJeztah/24.0_backport_bump_runc_1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/dac56638adccd215bae6cc23146f29e4697e1e98"><code>dac5663</code></a> update containerd binary to v1.7.13</li>
<li><a href="https://github.com/moby/moby/commit/20e1af361628a31afd1af58d25cd6ea4e495669f"><code>20e1af3</code></a> vendor: github.com/opencontainers/runc v1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/858919d39968c687de3afb0a0a3a212d60ef2a99"><code>858919d</code></a> update runc binary to v1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/141ad39e38a9a44b7487933d74815863c2c588e6"><code>141ad39</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47266">#47266</a> from vvoland/ci-fix-makeps1-templatefail-24</li>
<li><a href="https://github.com/moby/moby/commit/db968c672bcd6eeed09a0ad35cac843a5ffe7e48"><code>db968c6</code></a> hack/make.ps1: Fix go list pattern</li>
<li><a href="https://github.com/moby/moby/commit/61c51fbb5aeb648eb5f97704b8c75be3ccf1c9a0"><code>61c51fb</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47221">#47221</a> from vvoland/pkg-pools-close-noop-24</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v24.0.7...v24.0.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=24.0.7+incompatible&new-version=24.0.9+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-20 17:29:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/580" class=".btn">#580</a>
            </td>
            <td>
                <b>
                    register wallets dynamically
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                remove reloading, the driver must be instantiated with the given public params and the wallets can be loaded immediately.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-20 16:04:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/579" class=".btn">#579</a>
            </td>
            <td>
                <b>
                    Query improvements
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
        Created At 2024-03-20 10:24:12 +0000 UTC
    </div>
</div>

