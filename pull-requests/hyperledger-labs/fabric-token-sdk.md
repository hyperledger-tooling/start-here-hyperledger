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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/distribution from 2.8.1+incompatible to 2.8.2+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/distribution](https://github.com/docker/distribution) from 2.8.1+incompatible to 2.8.2+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/distribution/releases">github.com/docker/distribution's releases</a>.</em></p>
<blockquote>
<h2>v2.8.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Revert registry/client: set <code>Accept: identity</code> header when getting layers by <a href="https://github.com/ndeloof"><code>@​ndeloof</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3783">distribution/distribution#3783</a></li>
<li>Parse <code>http</code> forbidden as denied by <a href="https://github.com/vvoland"><code>@​vvoland</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3914">distribution/distribution#3914</a></li>
<li>Fix <a href="https://www.cve.org/CVERecord?id=CVE-2022-28391">CVE-2022-28391</a> by bumping alpine from 3.14 to 3.16 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> (<a href="https://redirect.github.com/distribution/distribution/pull/3650">#3650</a>)</li>
<li>Fix <a href="https://www.cve.org/CVERecord?id=CVE-2023-2253">CVE-2023-2253</a> runaway allocation on /v2/_catalog  by <a href="https://github.com/josegomezr"><code>@​josegomezr</code></a> <a href="https://github.com/distribution/distribution/commit/521ea3d973cb0c7089ebbcdd4ccadc34be941f54"><code>521ea3d9</code></a></li>
<li>Fix panic in inmemory driver by <a href="https://github.com/wy65701436"><code>@​wy65701436</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3815">distribution/distribution#3815</a></li>
<li>bump up golang version (alternative) by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3903">distribution/distribution#3903</a></li>
<li>Dockerfile: update xx to v1.2.1 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3907">distribution/distribution#3907</a></li>
<li>update to go1.19.9 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3908">distribution/distribution#3908</a></li>
<li>Add code to handle pagination of parts. Fixes max layer size of 10GB bug by <a href="https://github.com/DavidSpek"><code>@​DavidSpek</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3893">distribution/distribution#3893</a></li>
<li>Dockerfile: fix filenames of artifacts by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3911">distribution/distribution#3911</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/distribution/distribution/compare/v2.8.1...v2.8.2">https://github.com/distribution/distribution/compare/v2.8.1...v2.8.2</a></p>
<h2>v2.8.2-beta.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix <a href="https://www.cve.org/CVERecord?id=CVE-2022-28391">CVE-2022-28391</a> by bumping alpine from 3.14 to 3.16 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> (<a href="https://redirect.github.com/distribution/distribution/pull/3650">#3650</a>)</li>
<li>Fix <a href="https://www.cve.org/CVERecord?id=CVE-2023-2253">CVE-2023-2253</a> runaway allocation on /v2/_catalog  by <a href="https://github.com/josegomezr"><code>@​josegomezr</code></a> <a href="https://github.com/distribution/distribution/commit/521ea3d973cb0c7089ebbcdd4ccadc34be941f54"><code>521ea3d9</code></a></li>
<li>Fix panic in inmemory driver by <a href="https://github.com/wy65701436"><code>@​wy65701436</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3815">distribution/distribution#3815</a></li>
<li>bump up golang version (alternative) by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3903">distribution/distribution#3903</a></li>
<li>Dockerfile: update xx to v1.2.1 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3907">distribution/distribution#3907</a></li>
<li>update to go1.19.9 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3908">distribution/distribution#3908</a></li>
<li>Add code to handle pagination of parts. Fixes max layer size of 10GB bug by <a href="https://github.com/DavidSpek"><code>@​DavidSpek</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3893">distribution/distribution#3893</a></li>
<li>Dockerfile: fix filenames of artifacts by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3911">distribution/distribution#3911</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/distribution/distribution/compare/v2.8.1...v2.8.2-beta.2">https://github.com/distribution/distribution/compare/v2.8.1...v2.8.2-beta.2</a></p>
<h2>v2.8.2-beta.1</h2>
<h3><strong>NOTE: This is a pre-release that does not contain any artifacts!</strong></h3>
<h2>What's Changed</h2>
<ul>
<li>Fix runaway allocation on /v2/_catalog by <a href="https://github.com/josegomezr"><code>@​josegomezr</code></a> <a href="https://github.com/distribution/distribution/commit/521ea3d973cb0c7089ebbcdd4ccadc34be941f54"><code>521ea3d9</code></a></li>
<li>Fix CVE-2022-28391 by bumping alpine from 3.14 to 3.16 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3650">distribution/distribution#3650</a></li>
<li>Fix panic in inmemory driver by <a href="https://github.com/wy65701436"><code>@​wy65701436</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3815">distribution/distribution#3815</a></li>
<li>bump up golang version (alternative) by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3903">distribution/distribution#3903</a></li>
<li>Dockerfile: update xx to v1.2.1 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3907">distribution/distribution#3907</a></li>
<li>update to go1.19.9 by <a href="https://github.com/thaJeztah"><code>@​thaJeztah</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3908">distribution/distribution#3908</a></li>
<li>Add code to handle pagination of parts. Fixes max layer size of 10GB bug by <a href="https://github.com/DavidSpek"><code>@​DavidSpek</code></a> in <a href="https://redirect.github.com/distribution/distribution/pull/3893">distribution/distribution#3893</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/distribution/distribution/compare/v2.8.1...v2.8.2-beta.1">https://github.com/distribution/distribution/compare/v2.8.1...v2.8.2-beta.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/distribution/distribution/commit/7c354a4b40feeea21d7eeae4de91c8ff7951e672"><code>7c354a4</code></a> Merge pull request <a href="https://redirect.github.com/docker/distribution/issues/3915">#3915</a> from distribution/2.8.2-release-notes</li>
<li><a href="https://github.com/distribution/distribution/commit/a173a9c625cdc84498580e4f486b36d4c9859065"><code>a173a9c</code></a> Add v2.8.2 release notes</li>
<li><a href="https://github.com/distribution/distribution/commit/4894d35ecc831b114d86cd3795573e5f4f306ea7"><code>4894d35</code></a> Merge pull request <a href="https://redirect.github.com/docker/distribution/issues/3914">#3914</a> from vvoland/handle-forbidden-28</li>
<li><a href="https://github.com/distribution/distribution/commit/f067f66d3de1fd82d6bf139d15130ff59d3db7e1"><code>f067f66</code></a> Merge pull request <a href="https://redirect.github.com/docker/distribution/issues/3783">#3783</a> from ndeloof/accept-encoding-28</li>
<li><a href="https://github.com/distribution/distribution/commit/483ad69da3e3fb9ac885962d50834ff8619733a2"><code>483ad69</code></a> registry/errors: Parse http forbidden as denied</li>
<li><a href="https://github.com/distribution/distribution/commit/2b0f84df21e062bd0cc3676557c6bee4cbb9e9bc"><code>2b0f84d</code></a> Revert &quot;registry/client: set Accept: identity header when getting layers&quot;</li>
<li><a href="https://github.com/distribution/distribution/commit/320d6a141f17d11c44f98fd975b2368705e27971"><code>320d6a1</code></a> Merge pull request <a href="https://redirect.github.com/docker/distribution/issues/3912">#3912</a> from distribution/2.8.2-beta.2-release-notes</li>
<li><a href="https://github.com/distribution/distribution/commit/5f3ca1b2fb6109705d729816e7260a6966d2b42d"><code>5f3ca1b</code></a> Add release notes for 2.8.2-beta.2 release</li>
<li><a href="https://github.com/distribution/distribution/commit/cb840f63b3b27cce503aee5e3291750f3cd90c1c"><code>cb840f6</code></a> Merge pull request <a href="https://redirect.github.com/docker/distribution/issues/3911">#3911</a> from thaJeztah/2.8_backport_fix_releaser_filenames</li>
<li><a href="https://github.com/distribution/distribution/commit/e884644fff38a5bf601a2272f434ee2b01dd2b17"><code>e884644</code></a> Dockerfile: fix filenames of artifacts</li>
<li>Additional commits viewable in <a href="https://github.com/docker/distribution/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/distribution&package-manager=go_modules&previous-version=2.8.1+incompatible&new-version=2.8.2+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 20:50:39 +0000 UTC
    </div>
</div>

