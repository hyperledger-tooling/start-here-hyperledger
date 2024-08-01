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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    for testing only - pkcs11 on both fsc and fts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This branch is https://github.com/hyperledger-labs/fabric-token-sdk/pull/699
on top of https://github.com/hyperledger-labs/fabric-smart-client/pull/621 so that we can test both changes together.

It is not meant to be merged as is, because the Token SDK should rely on `main` commits on Fabric Smart Client only.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-30 12:45:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 26.1.0+incompatible to 26.1.4+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 26.1.0+incompatible to 26.1.4+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v26.1.4</h2>
<h2>26.1.4</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A26.1.4">docker/cli, 26.1.4 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A26.1.4">moby/moby, 26.1.4 milestone</a></li>
<li>Deprecated and removed features, see <a href="https://github.com/docker/cli/blob/v26.1.4/docs/deprecated.md">Deprecated Features</a>.</li>
<li>Changes to the Engine API, see <a href="https://github.com/moby/moby/blob/v26.1.4/docs/api/version-history.md">API version history</a>.</li>
</ul>
<h3>Security</h3>
<p>This release updates the Go runtime to 1.21.11 which contains security fixes for:</p>
<ul>
<li><a href="https://redirect.github.com/golang/go/issues/66869">CVE-2024-24789</a></li>
<li><a href="https://redirect.github.com/golang/go/issues/67680">CVE-2024-24790</a></li>
<li>A symlink time of check to time of use race condition during directory removal reported by Addison Crump (<a href="https://github.com/addisoncrump"><code>@​addisoncrump</code></a>).</li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Fixed an issue where promoting a node immediately after another node was demoted could cause the promotion to fail. <a href="https://redirect.github.com/moby/moby/pull/47870">moby/moby#47870</a></li>
<li>Prevent the daemon log from being spammed with <code>superfluous response.WriteHeader call ...</code> messages.. <a href="https://redirect.github.com/moby/moby/pull/47843">moby/moby#47843</a></li>
<li>Don't show empty hints when plugins return an empty hook message. <a href="https://redirect.github.com/docker/cli/pull/5083">docker/cli#5083</a></li>
<li>Added <code>ContextType: &quot;moby&quot;</code> to the context list/inspect output to address a compatibility issue with Visual Studio Container Tools. <a href="https://redirect.github.com/docker/cli/pull/5095">docker/cli#5095</a></li>
<li>Fix a compatibility issue with Visual Studio Container Tools. <a href="https://redirect.github.com/docker/cli/pull/5095">docker/cli#5095</a></li>
</ul>
<h3>Packaging updates</h3>
<ul>
<li>Update containerd (static binaries only) to <a href="https://github.com/containerd/containerd/releases/tag/v1.7.17">v1.7.17</a>. <a href="https://redirect.github.com/moby/moby/pull/47841">moby/moby#47841</a></li>
<li><a href="https://redirect.github.com/golang/go/issues/66869">CVE-2024-24789</a>, <a href="https://redirect.github.com/golang/go/issues/67680">CVE-2024-24790</a>: Update Go runtime to 1.21.11. <a href="https://redirect.github.com/moby/moby/pull/47904">moby/moby#47904</a></li>
<li>Update Compose to <a href="https://github.com/docker/compose/releases/tag/v2.27.1">v2.27.1</a>. <a href="https://redirect.github.com/docker/docker-ce-packaging/pull/1022">docker/docker-ce-packages#1022</a></li>
<li>Update Buildx to <a href="https://github.com/docker/buildx/releases/tag/v0.14.1">v0.14.1</a>. <a href="https://redirect.github.com/docker/docker-ce-packaging/pull/1021">docker/docker-ce-packages#1021</a></li>
</ul>
<h2>v26.1.3</h2>
<h2>26.1.3</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A26.1.3">docker/cli, 26.1.3 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A26.1.3">moby/moby, 26.1.3 milestone</a></li>
<li>Deprecated and removed features, see <a href="https://github.com/docker/cli/blob/v26.1.3/docs/deprecated.md">Deprecated Features</a>.</li>
<li>Changes to the Engine API, see <a href="https://github.com/moby/moby/blob/v26.1.3/docs/api/version-history.md">API version history</a>.</li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Fix a regression that prevented the use of DNS servers within a <code>--internal</code> network. <a href="https://redirect.github.com/moby/moby/pull/47832">moby/moby#47832</a></li>
<li>When the internal DNS server's own address is supplied as an external server address, ignore it to avoid unproductive recursion. <a href="https://redirect.github.com/moby/moby/pull/47833">moby/moby#47833</a></li>
</ul>
<h3>Packaging updates</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/de5c9cf0b96e4e172b96db54abababa4a328462f"><code>de5c9cf</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47912">#47912</a> from thaJeztah/26.1_backport_vendor_containerd_1.7.18</li>
<li><a href="https://github.com/moby/moby/commit/c62dcf8ab17bbc61a196047de4e3866e6a16a766"><code>c62dcf8</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47911">#47911</a> from thaJeztah/26.1_backport_bump_containerd_binary...</li>
<li><a href="https://github.com/moby/moby/commit/17315a20ee08bd491eb6a605f11dc02ca0327ee7"><code>17315a2</code></a> vendor: github.com/containerd/containerd v1.7.18</li>
<li><a href="https://github.com/moby/moby/commit/cbd94183abd05880d293f1235707209d7fe593b8"><code>cbd9418</code></a> update containerd binary to v1.7.18</li>
<li><a href="https://github.com/moby/moby/commit/fb9f72aeb6c3d8ada8c88965dd4f12b44cbfea04"><code>fb9f72a</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47904">#47904</a> from thaJeztah/26.1_backport_bump_go1.21.11</li>
<li><a href="https://github.com/moby/moby/commit/3115daaa91e57ab8668c44244642d5a174ae4ad7"><code>3115daa</code></a> update to go1.21.11</li>
<li><a href="https://github.com/moby/moby/commit/2861734174423627ada47d971ae61b639046bdfc"><code>2861734</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47892">#47892</a> from thaJeztah/26.1_backport_api_docs_network_confi...</li>
<li><a href="https://github.com/moby/moby/commit/9c95aea306fc82ffb1e47390578a7c1f21693ae0"><code>9c95aea</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47893">#47893</a> from thaJeztah/26.1_backport_bump_docker_py</li>
<li><a href="https://github.com/moby/moby/commit/3e09e197a7c742b39277495233c918e32a35474f"><code>3e09e19</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47894">#47894</a> from thaJeztah/26.1_backport_vendor_containerd_v1.7.17</li>
<li><a href="https://github.com/moby/moby/commit/65b679ac9c4286778171f21ba51c72ca0aa11fd2"><code>65b679a</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47889">#47889</a> from thaJeztah/26.1_backport_platforms_err_handling</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v26.1.0...v26.1.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=26.1.0+incompatible&new-version=26.1.4+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-30 10:25:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    F cleanup
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
        Created At 2024-07-27 04:58:51 +0000 UTC
    </div>
</div>

