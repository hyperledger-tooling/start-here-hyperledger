---
layout: default
title: microfab
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/microfab
---

# microfab <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/microfab){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 24.0.9+incompatible to 25.0.6+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 24.0.9+incompatible to 25.0.6+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v25.0.6</h2>
<h2>25.0.6</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A25.0.6">docker/cli, 25.0.6 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A25.0.6">moby/moby, 25.0.6 milestone</a></li>
<li>Deprecated and removed features, see <a href="https://github.com/docker/cli/blob/v25.0.6/docs/deprecated.md">Deprecated Features</a>.</li>
<li>Changes to the Engine API, see <a href="https://github.com/moby/moby/blob/v25.0.6/docs/api/version-history.md">API version history</a>.</li>
</ul>
<h3>Security</h3>
<p>This release contains a fix for <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-41110">CVE-2024-41110</a> / <a href="https://github.com/moby/moby/security/advisories/GHSA-v23v-6jw2-98fq">GHSA-v23v-6jw2-98fq</a> that impacted setups using <a href="https://docs.docker.com/engine/extend/plugins_authorization/">authorization plugins (AuthZ)</a> for access control.</p>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>[25.0] remove erroneous <code>platform</code> from image <code>config</code> OCI descriptor in <code>docker save</code> output. <a href="https://redirect.github.com/moby/moby/pull/47695">moby/moby#47695</a></li>
<li>[25.0 backport] Fix a nil dereference when getting image history for images having layers without the <code>Created</code> value set. <a href="https://redirect.github.com/moby/moby/pull/47759">moby/moby#47759</a></li>
<li>[25.0 backport] apparmor: Allow confined runc to kill containers. <a href="https://redirect.github.com/moby/moby/pull/47830">moby/moby#47830</a></li>
<li>[25.0 backport] Fix an issue where rapidly promoting a Swarm node after another node was demoted could cause the promoted node to fail its promotion. <a href="https://redirect.github.com/moby/moby/pull/47869">moby/moby#47869</a></li>
<li>[25.0 backport] don't depend on containerd platform.Parse to return a typed error. <a href="https://redirect.github.com/moby/moby/pull/47890">moby/moby#47890</a></li>
<li>[25.0 backport] builder/mobyexporter: Add missing nil check <a href="https://redirect.github.com/moby/moby/pull/47987">moby/moby#47987</a></li>
</ul>
<h3>Packaging updates</h3>
<ul>
<li>Update AWS SDK Go v2 to v1.24.1 for AWS CloudWatch logging driver. <a href="https://redirect.github.com/moby/moby/pull/47724">moby/moby#47724</a></li>
<li>Update Go runtime to 1.21.12, which contains security fixes for <a href="https://github.com/advisories/GHSA-hw49-2p59-3mhj">CVE-2024-24791</a> <a href="https://redirect.github.com/moby/moby/pull/48146">moby/moby#48146</a></li>
<li>Update Containerd (static binaries only) to <a href="https://github.com/containerd/containerd/releases/tag/v1.7.20">v1.7.20</a>. <a href="https://redirect.github.com/moby/moby/pull/48199">moby/moby#48199</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/moby/moby/compare/v25.0.5...v25.0.6">https://github.com/moby/moby/compare/v25.0.5...v25.0.6</a></p>
<h2>v25.0.5</h2>
<h2>25.0.5</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A25.0.5">docker/cli, 25.0.5 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A25.0.5">moby/moby, 25.0.5 milestone</a></li>
<li>Deprecated and removed features, see <a href="https://github.com/docker/cli/blob/v25.0.5/docs/deprecated.md">Deprecated Features</a>.</li>
<li>Changes to the Engine API, see <a href="https://github.com/moby/moby/blob/v25.0.5/docs/api/version-history.md">API version history</a>.</li>
</ul>
<h3>Security</h3>
<p>This release contains a security fix for <a href="https://github.com/moby/moby/security/advisories/GHSA-mq39-4gv4-mvpx">CVE-2024-29018</a>, a potential data exfiltration from 'internal' networks via authoritative DNS servers.</p>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>
<p><a href="https://github.com/moby/moby/security/advisories/GHSA-mq39-4gv4-mvpx">CVE-2024-29018</a>: Do not forward requests to external DNS servers for a container that is only connected to an 'internal' network. Previously, requests were forwarded if the host's DNS server was running on a loopback address, like systemd's 127.0.0.53. <a href="https://redirect.github.com/moby/moby/pull/47589">moby/moby#47589</a></p>
</li>
<li>
<p>plugin: fix mounting /etc/hosts when running in UserNS. <a href="https://redirect.github.com/moby/moby/pull/47588">moby/moby#47588</a></p>
</li>
<li>
<p>rootless: fix <code>open /etc/docker/plugins: permission denied</code>. <a href="https://redirect.github.com/moby/moby/pull/47587">moby/moby#47587</a></p>
</li>
<li>
<p>Fix multiple parallel <code>docker build</code> runs leaking disk space. <a href="https://redirect.github.com/moby/moby/pull/47527">moby/moby#47527</a></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/b08a51fe16eed67de3861c03b363ba403643b12e"><code>b08a51f</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/48231">#48231</a> from austinvazquez/backport-vendor-otel-v0.46.1-to-...</li>
<li><a href="https://github.com/moby/moby/commit/d151b0f87f9673f206b477c90db25956e1704ba5"><code>d151b0f</code></a> vendor: OTEL v0.46.1 / v1.21.0</li>
<li><a href="https://github.com/moby/moby/commit/c6ba9a5124603357bfc4a64971cbb9708180f06e"><code>c6ba9a5</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/48225">#48225</a> from austinvazquez/backport-workflow-artifact-reten...</li>
<li><a href="https://github.com/moby/moby/commit/4673a3ca2c37ae30270a29c281ccd9477107dcee"><code>4673a3c</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/48227">#48227</a> from austinvazquez/backport-backport-branch-check-t...</li>
<li><a href="https://github.com/moby/moby/commit/30f89081028ce6fb1b49a71c02c156dacbe9aa62"><code>30f8908</code></a> github/ci: Check if backport is opened against the expected branch</li>
<li><a href="https://github.com/moby/moby/commit/7454d6a2e672b0b977aaa14463c9aeb53acd06af"><code>7454d6a</code></a> ci: update workflow artifacts retention</li>
<li><a href="https://github.com/moby/moby/commit/65cc597cea28cdc25bea3b8a86384b4251872919"><code>65cc597</code></a> Merge commit from fork</li>
<li><a href="https://github.com/moby/moby/commit/b722836927669b414569c42f096869cd800b59a6"><code>b722836</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/48199">#48199</a> from austinvazquez/update-containerd-binary-to-1.7.20</li>
<li><a href="https://github.com/moby/moby/commit/e8ecb9c76d97579ebbf3f9d3ef770d08ac303809"><code>e8ecb9c</code></a> update containerd binary to v1.7.20</li>
<li><a href="https://github.com/moby/moby/commit/e6cae1f2373d4ff37499570e67f23b2cebb7a043"><code>e6cae1f</code></a> update containerd binary to v1.7.19</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v24.0.9...v25.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=24.0.9+incompatible&new-version=25.0.6+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/microfab/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-08-01 17:18:44 +0000 UTC
    </div>
</div>

