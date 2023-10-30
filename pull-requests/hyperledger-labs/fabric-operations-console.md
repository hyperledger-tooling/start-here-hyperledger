---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 20.10.12+incompatible to 24.0.7+incompatible in /packages/fabric-deployer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 20.10.12+incompatible to 24.0.7+incompatible.
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
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v20.10.12...v24.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=20.10.12+incompatible&new-version=24.0.7+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-30 15:31:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/548" class=".btn">#548</a>
            </td>
            <td>
                <b>
                    Bump browserify-sign from 4.2.1 to 4.2.2 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [browserify-sign](https://github.com/crypto-browserify/browserify-sign) from 4.2.1 to 4.2.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/browserify/browserify-sign/blob/main/CHANGELOG.md">browserify-sign's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/browserify/browserify-sign/compare/v4.2.1...v4.2.2">v4.2.2</a> - 2023-10-25</h2>
<h3>Fixed</h3>
<ul>
<li>[Tests] log when openssl doesn't support cipher <a href="https://redirect.github.com/browserify/browserify-sign/issues/37"><code>[#37](https://github.com/crypto-browserify/browserify-sign/issues/37)</code></a></li>
</ul>
<h3>Commits</h3>
<ul>
<li>Only apps should have lockfiles <a href="https://github.com/browserify/browserify-sign/commit/09a89959393b3c89fedd4f7f3bafa4fec44371d7"><code>09a8995</code></a></li>
<li>[eslint] switch to eslint <a href="https://github.com/browserify/browserify-sign/commit/83fe46374b819e959d56d2c0b931308f7451a664"><code>83fe463</code></a></li>
<li>[meta] add <code>npmignore</code> and <code>auto-changelog</code> <a href="https://github.com/browserify/browserify-sign/commit/44181838e7dcc4d5d0c568f74312ea28f0bcdfd5"><code>4418183</code></a></li>
<li>[meta] fix package.json indentation <a href="https://github.com/browserify/browserify-sign/commit/9ac5a5eaaac8a11eb70ec2febd13745c8764ae02"><code>9ac5a5e</code></a></li>
<li>[Tests] migrate from travis to github actions <a href="https://github.com/browserify/browserify-sign/commit/d845d855def38e2085d5a21e447a48300f99fa60"><code>d845d85</code></a></li>
<li>[Fix] <code>sign</code>: throw on unsupported padding scheme <a href="https://github.com/browserify/browserify-sign/commit/8767739a4516289568bcce9fed8a3b7e23478de9"><code>8767739</code></a></li>
<li>[Fix] properly check the upper bound for DSA signatures <a href="https://github.com/browserify/browserify-sign/commit/85994cd6348b50f2fd1b73c54e20881416f44a30"><code>85994cd</code></a></li>
<li>[Tests] handle openSSL not supporting a scheme <a href="https://github.com/browserify/browserify-sign/commit/f5f17c27f9824de40b5ce8ebd8502111203fd6af"><code>f5f17c2</code></a></li>
<li>[Deps] update <code>bn.js</code>, <code>browserify-rsa</code>, <code>elliptic</code>, <code>parse-asn1</code>, <code>readable-stream</code>, <code>safe-buffer</code> <a href="https://github.com/browserify/browserify-sign/commit/a67d0eb4ffceabb366b69da69ce9a223e9d5e96b"><code>a67d0eb</code></a></li>
<li>[Dev Deps] update <code>nyc</code>, <code>standard</code>, <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/cc5350b96702fcba930e0662cf763844fd2f59bf"><code>cc5350b</code></a></li>
<li>[Tests] always run coverage; downgrade <code>nyc</code> <a href="https://github.com/browserify/browserify-sign/commit/75ce1d5c49a6591dd13422016c07f8f9cae13371"><code>75ce1d5</code></a></li>
<li>[meta] add <code>safe-publish-latest</code> <a href="https://github.com/browserify/browserify-sign/commit/dcf49ce85a1a66a6fb31689508d916d7894286a9"><code>dcf49ce</code></a></li>
<li>[Tests] add <code>npm run posttest</code> <a href="https://github.com/browserify/browserify-sign/commit/75dd8fd6ce56eb37b12e30807e5f913867b21733"><code>75dd8fd</code></a></li>
<li>[Dev Deps] update <code>tape</code> <a href="https://github.com/browserify/browserify-sign/commit/3aec0386dc8dfba8698be756ec770df863867c84"><code>3aec038</code></a></li>
<li>[Tests] skip unsupported schemes <a href="https://github.com/browserify/browserify-sign/commit/703c83ea72db2f45714fe749c6f04b05243ca9a8"><code>703c83e</code></a></li>
<li>[Tests] node &lt; 6 lacks array <code>includes</code> <a href="https://github.com/browserify/browserify-sign/commit/3aa43cfbc1fdde8481bcdd3bff581574159b869a"><code>3aa43cf</code></a></li>
<li>[Dev Deps] fix eslint range <a href="https://github.com/browserify/browserify-sign/commit/98d4e0d7ff18871b0ca07415f758a610ccf8ebbe"><code>98d4e0d</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/browserify/browserify-sign/commit/4af5a90bf8acd9e76e5671dc0497f6ba71968a2c"><code>4af5a90</code></a> v4.2.2</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/3aec0386dc8dfba8698be756ec770df863867c84"><code>3aec038</code></a> [Dev Deps] update <code>tape</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/85994cd6348b50f2fd1b73c54e20881416f44a30"><code>85994cd</code></a> [Fix] properly check the upper bound for DSA signatures</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/9ac5a5eaaac8a11eb70ec2febd13745c8764ae02"><code>9ac5a5e</code></a> [meta] fix package.json indentation</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/dcf49ce85a1a66a6fb31689508d916d7894286a9"><code>dcf49ce</code></a> [meta] add <code>safe-publish-latest</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/44181838e7dcc4d5d0c568f74312ea28f0bcdfd5"><code>4418183</code></a> [meta] add <code>npmignore</code> and <code>auto-changelog</code></li>
<li><a href="https://github.com/browserify/browserify-sign/commit/8767739a4516289568bcce9fed8a3b7e23478de9"><code>8767739</code></a> [Fix] <code>sign</code>: throw on unsupported padding scheme</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/5f6fb1755917851a40249db7d834da4265ed5950"><code>5f6fb17</code></a> [Tests] log when openssl doesn't support cipher</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/f5f17c27f9824de40b5ce8ebd8502111203fd6af"><code>f5f17c2</code></a> [Tests] handle openSSL not supporting a scheme</li>
<li><a href="https://github.com/browserify/browserify-sign/commit/d845d855def38e2085d5a21e447a48300f99fa60"><code>d845d85</code></a> [Tests] migrate from travis to github actions</li>
<li>Additional commits viewable in <a href="https://github.com/crypto-browserify/browserify-sign/compare/v4.2.1...v4.2.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~ljharb">ljharb</a>, a new releaser for browserify-sign since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=browserify-sign&package-manager=npm_and_yarn&previous-version=4.2.1&new-version=4.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-27 19:18:36 +0000 UTC
    </div>
</div>

