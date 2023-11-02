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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    fix: FSC panics when provided with a malformed identity certificate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 09:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 20.10.24+incompatible to 24.0.7+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 20.10.24+incompatible to 24.0.7+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v24.0.7</h2>
<h2>24.0.7</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A24.0.7">docker/cli, 24.0.7 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A24.0.7">moby/moby, 24.0.7 milestone</a></li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Write overlay2 layer metadata atomically. <a href="https://redirect.github.com/moby/moby/pull/46703">moby/moby#46703</a></li>
<li>Fix &quot;Rootful-in-Rootless&quot; Docker-in-Docker on systemd version 250 and later. <a href="https://redirect.github.com/moby/moby/pull/46626">moby/moby#46626</a></li>
<li>Fix <code>dockerd-rootless-setuptools.sh</code> when username contains a backslash. <a href="https://redirect.github.com/moby/moby/pull/46407">moby/moby#46407</a></li>
<li>Fix a bug that would prevent network sandboxes to be fully deleted when stopping containers with no network attachments and when <code>dockerd --bridge=none</code> is used. <a href="https://redirect.github.com/moby/moby/pull/46702">moby/moby#46702</a></li>
<li>Fix a bug where cancelling an API request could interrupt container restart. <a href="https://redirect.github.com/moby/moby/pull/46697">moby/moby#46697</a></li>
<li>Fix an issue where containers would fail to start when providing <code>--ip-range</code> with a range larger than the subnet. <a href="https://redirect.github.com/docker/for-mac/issues/6870">docker/for-mac#6870</a></li>
<li>Fix data corruption with zstd output. <a href="https://redirect.github.com/moby/moby/pull/46709">moby/moby#46709</a></li>
<li>Fix the conditions under which the container's MAC address is applied. <a href="https://redirect.github.com/moby/moby/pull/46478">moby/moby#46478</a></li>
<li>Improve the performance of the stats collector. <a href="https://redirect.github.com/moby/moby/pull/46448">moby/moby#46448</a></li>
<li>Fix an issue with source policy rules ending up in the wrong order. <a href="https://redirect.github.com/moby/moby/pull/46441">moby/moby#46441</a></li>
</ul>
<h3>Packaging updates</h3>
<ul>
<li>Add support for Fedora 39 and Ubuntu 23.10. <a href="https://redirect.github.com/docker/docker-ce-packaging/pull/940">docker/docker-ce-packaging#940</a>, <a href="https://redirect.github.com/docker/docker-ce-packaging/pull/955">docker/docker-ce-packaging#955</a></li>
<li>Fix <code>docker.socket</code> not getting disabled when uninstalling the <code>docker-ce</code> RPM package. <a href="https://redirect.github.com/docker/docker-ce-packaging/pull/852">docker/docker-ce-packaging#852</a></li>
<li>Upgrade Go to <code>go1.20.10</code>. <a href="https://redirect.github.com/docker/docker-ce-packaging/pull/951">docker/docker-ce-packaging#951</a></li>
<li>Upgrade containerd to <code>v1.7.6</code> (static binaries only). <a href="https://redirect.github.com/moby/moby/pull/46103">moby/moby#46103</a></li>
<li>Upgrade the <code>containerd.io</code> package to <a href="https://github.com/containerd/containerd/releases/tag/v1.6.24"><code>v1.6.24</code></a>.</li>
</ul>
<h3>Security</h3>
<ul>
<li>Deny containers access to <code>/sys/devices/virtual/powercap</code> by default. This change hardens against <a href="https://scout.docker.com/v/CVE-2020-8694">CVE-2020-8694</a>, <a href="https://scout.docker.com/v/CVE-2020-8695">CVE-2020-8695</a>, and <a href="https://scout.docker.com/v/CVE-2020-12912">CVE-2020-12912</a>, and an attack known as <a href="https://platypusattack.com/">the PLATYPUS attack</a>. For more details, see <a href="https://github.com/moby/moby/security/advisories/GHSA-jq35-85cj-fj4p">advisory</a>, <a href="https://github.com/moby/moby/commit/c9ccbfad11a60e703e91b6cca4f48927828c7e35">commit</a>.</li>
</ul>
<h2>v24.0.6</h2>
<h2>24.0.6</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A24.0.6">docker/cli, 24.0.6 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A24.0.6">moby/moby, 24.0.6 milestone</a></li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>containerd storage backend: Fix <code>docker ps</code> failing when a container image is no longer present in the content store. <a href="https://redirect.github.com/moby/moby/pull/46095">moby/moby#46095</a></li>
<li>containerd storage backend: Fix <code>docker ps -s -a</code> and <code>docker container prune</code> failing when a container image config is no longer present in the content store. <a href="https://redirect.github.com/moby/moby/pull/46097">moby/moby#46097</a></li>
<li>containerd storage backend: Fix <code>docker inspect</code> failing when a container image config is no longer (or was never) present in the content store. <a href="https://redirect.github.com/moby/moby/pull/46244">moby/moby#46244</a></li>
<li>containerd storage backend: Fix diff and export with the <code>overlayfs</code> snapshotter by using reference-counted rootfs mounts. <a href="https://redirect.github.com/moby/moby/pull/46266">moby/moby#46266</a></li>
<li>containerd storage backend: Fix a misleading error message when the image platforms available locally do not match the desired platform. <a href="https://redirect.github.com/moby/moby/pull/46300">moby/moby#46300</a></li>
<li>containerd storage backend: Fix the <code>FROM scratch</code> Dockerfile instruction with the classic builder. <a href="https://redirect.github.com/moby/moby/pull/46302">moby/moby#46302</a></li>
<li>containerd storage backend: Fix <code>mismatched image rootfs and manifest layers</code> errors with the classic builder. <a href="https://redirect.github.com/moby/moby/pull/46310">moby/moby#46310</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/311b9ff0aa93aa55880e1e5f8871c4fb69583426"><code>311b9ff</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46697">#46697</a> from thaJeztah/24.0_backport_restart_nocancel</li>
<li><a href="https://github.com/moby/moby/commit/af608045eef0b87f31a24d21fb7af80de76134aa"><code>af60804</code></a> Merge pull request from GHSA-jq35-85cj-fj4p</li>
<li><a href="https://github.com/moby/moby/commit/3cf363e1ee33fe00dbedfdb7d6caf299990d5568"><code>3cf363e</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46709">#46709</a> from thaJeztah/24.0_backport_bump_compress</li>
<li><a href="https://github.com/moby/moby/commit/05d7386665793b7f8398eb80b4e85adff5486035"><code>05d7386</code></a> daemon: daemon.containerRestart: don't cancel restart on context cancel</li>
<li><a href="https://github.com/moby/moby/commit/649c9440f28c7334ee5c9f17889448a81dcc8729"><code>649c944</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46703">#46703</a> from thaJeztah/24.0_backport_atomic-layer-data-write</li>
<li><a href="https://github.com/moby/moby/commit/9b20b1a5fe0919a79cc15f6a3f331f2cdae0a37a"><code>9b20b1a</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46702">#46702</a> from thaJeztah/24.0_backport_releaseNetwork_Network...</li>
<li><a href="https://github.com/moby/moby/commit/dd37b0b960ec4d3da0ca2efe78fa47484d4c6380"><code>dd37b0b</code></a> vendor: github.com/klauspost/compress v1.17.2</li>
<li><a href="https://github.com/moby/moby/commit/7058c0d24da8ac9267e52224b6a3beaa24ce5e9f"><code>7058c0d</code></a> vendor: github.com/klauspost/compress v1.16.5</li>
<li><a href="https://github.com/moby/moby/commit/57bd38858262922b86ceea37770536ff535fa2af"><code>57bd388</code></a> daemon: overlay2: Write layer metadata atomically</li>
<li><a href="https://github.com/moby/moby/commit/05d95fd5038a8a56ff69294a3bdd33b2d2769ba3"><code>05d95fd</code></a> daemon: release sandbox even when NetworkDisabled</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v20.10.24...v24.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=20.10.24+incompatible&new-version=24.0.7+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-30 15:37:23 +0000 UTC
    </div>
</div>

