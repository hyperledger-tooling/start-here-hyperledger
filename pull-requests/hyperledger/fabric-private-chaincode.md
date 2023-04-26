---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/703" class=".btn">#703</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 20.10.7+incompatible to 20.10.24+incompatible in /samples/deployment/fabric-smart-client/the-simple-testing-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 20.10.7+incompatible to 20.10.24+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v20.10.24</h2>
<h2>20.10.24</h2>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Fixed a number of issues that can cause Swarm encrypted overlay networks
to fail to uphold their guarantees, addressing <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28841">CVE-2023-28841</a>,
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28840">CVE-2023-28840</a>, and
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28842">CVE-2023-28842</a>.
<ul>
<li>A lack of kernel support for encrypted overlay networks now reports
as an error.</li>
<li>Encrypted overlay networks are eagerly set up, rather than waiting for
multiple nodes to attach.</li>
<li>Encrypted overlay networks are now usable on Red Hat Enterprise Linux 9
through the use of the <code>xt_bpf</code> kernel module.</li>
<li>Users of Swarm overlay networks should review <a href="https://github.com/moby/moby/security/advisories/GHSA-vwm3-crmr-xfxw">GHSA-vwm3-crmr-xfxw</a>
to ensure that unintentional exposure has not occurred.</li>
</ul>
</li>
<li>Upgrade github.com/containerd/fifo to v1.1.0 to fix a potential panic <a href="https://redirect.github.com/moby/moby/pull/45242">moby/moby#45216</a>.</li>
<li>Fix missing Bash completion for installed cli-plugins <a href="https://redirect.github.com/docker/cli/pull/4091">docker/cli#4091</a>.</li>
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update Go runtime to <a href="https://go.dev/doc/devel/release#go1.19.minor">1.19.7</a>.</li>
<li>Update Docker Buildx to <a href="https://github.com/docker/buildx/releases/tag/v0.10.4">v0.10.4</a>.</li>
<li>Update containerd to <a href="https://github.com/containerd/containerd/releases/tag/v1.6.20">v1.6.20</a>.</li>
<li>Update runc to <a href="https://github.com/opencontainers/runc/releases/tag/v1.1.5">v1.1.5</a>.</li>
</ul>
<h2>v20.10.23</h2>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>
<p>Fix an issue where <code>docker build</code> would fail when using <code>--add-host=host.docker.internal:host-gateway</code>
with BuildKit enabled <a href="https://redirect.github.com/moby/moby/pull/44650">moby/moby#44650</a>.</p>
</li>
<li>
<p>Revert seccomp: block socket calls to <code>AF_VSOCK</code> in default profile <a href="https://redirect.github.com/moby/moby/pull/44712">moby/moby#44712</a>.
This change, while favorable from a security standpoint, caused a change
in behavior for some use-cases. As such, we are reverting it to ensure
stability and compatibility for the affected users.</p>
<p>However, users of <code>AF_VSOCK</code> in containers should recognize that this
(special) address family is not currently namespaced in any version of
the Linux kernel, and may result in unexpected behavior, like containers
communicating directly with host hypervisors.</p>
<p>Future releases, will filter <code>AF_VSOCK</code>. Users who need to allow containers
to communicate over the unnamespaced <code>AF_VSOCK</code> will need to turn off seccomp
confinement or set a custom seccomp profile.</p>
</li>
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update Docker Compose to <a href="https://github.com/docker/compose/releases/tag/v2.15.1">v2.15.1</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/5d6db842238e3c4f5f9fb9ad70ea46b35227d084"><code>5d6db84</code></a> Merge pull request from GHSA-232p-vwff-86mp</li>
<li><a href="https://github.com/moby/moby/commit/d2bc43a75b98887a830501211cc6bc86a59b8cca"><code>d2bc43a</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45242">#45242</a> from neersighted/go1.19.7/20.10</li>
<li><a href="https://github.com/moby/moby/commit/9aa5d55a8ba8725133a6fbb5ac98d1fab341fdc7"><code>9aa5d55</code></a> update to go1.19.7</li>
<li><a href="https://github.com/moby/moby/commit/83679bb638b7d20c913019d62535228e5ed8a1ec"><code>83679bb</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45216">#45216</a> from corhere/backport-20.10/containerd-fifo_v1.1</li>
<li><a href="https://github.com/moby/moby/commit/b4f0442da2d6f432df52ce60d571d512336bcbd9"><code>b4f0442</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45219">#45219</a> from vvoland/test-windows-execstartfails-2010</li>
<li><a href="https://github.com/moby/moby/commit/ba043e86912d47ba760856cab9c34e8b294fe29d"><code>ba043e8</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/44990">#44990</a> from thaJeztah/20.10_backport_update_go1.19</li>
<li><a href="https://github.com/moby/moby/commit/b56fe595050578ced98af6c2deb70f3126cad0f9"><code>b56fe59</code></a> integration-cli: Enable TestExecStartFails on Windows</li>
<li><a href="https://github.com/moby/moby/commit/d9433ee0968c963bc1c993ad408b5da791340175"><code>d9433ee</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45197">#45197</a> from vvoland/integration-restart-race-2010</li>
<li><a href="https://github.com/moby/moby/commit/a9c02c238f403a7a204c909fe5f85fcef13faf75"><code>a9c02c2</code></a> Upgrade containerd/fifo to v1.1.0</li>
<li><a href="https://github.com/moby/moby/commit/bbec6704dcf31a981cec32e2ea95a6c19306a666"><code>bbec670</code></a> [20.10] vendor: libnetwork c5aa85f9b25f0acaec8591ced679cb9fb5b9e32c</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v20.10.7...v20.10.24">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=20.10.7+incompatible&new-version=20.10.24+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-private-chaincode/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 12:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/702" class=".btn">#702</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.0.0-20220225172249-27dd8689420f to 0.7.0 in /samples/deployment/fabric-smart-client/the-simple-testing-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.0.0-20220225172249-27dd8689420f to 0.7.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/net/commits/v0.7.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.0.0-20220225172249-27dd8689420f&new-version=0.7.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-private-chaincode/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 12:25:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/701" class=".btn">#701</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc from 1.0.0-rc93 to 1.1.5 in /samples/deployment/fabric-smart-client/the-simple-testing-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.0-rc93 to 1.1.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/releases">github.com/opencontainers/runc's releases</a>.</em></p>
<blockquote>
<h2>runc 1.1.5 -- &quot;囚われた屈辱は　反撃の嚆矢だ&quot;</h2>
<p>This is the fifth patch release in the 1.1.z series of runc, which fixes
three CVEs found in runc.</p>
<ul>
<li>
<p>CVE-2023-25809 is a vulnerability involving rootless containers where
(under specific configurations), the container would have write access
to the /sys/fs/cgroup/user.slice/... cgroup hierarchy. No other
hierarchies on the host were affected. This vulnerability was
discovered by Akihiro Suda.
<a href="https://github.com/opencontainers/runc/security/advisories/GHSA-m8cg-xc2p-r3fc">https://github.com/opencontainers/runc/security/advisories/GHSA-m8cg-xc2p-r3fc</a></p>
</li>
<li>
<p>CVE-2023-27561 was a regression which effectively re-introduced
CVE-2019-19921. This bug was present from v1.0.0-rc95 to v1.1.4. This
regression was discovered by <a href="https://github.com/Beuc"><code>@​Beuc</code></a>.
<a href="https://github.com/advisories/GHSA-vpvm-3wq2-2wvm">https://github.com/advisories/GHSA-vpvm-3wq2-2wvm</a></p>
</li>
<li>
<p>CVE-2023-28642 is a variant of CVE-2023-27561 and was fixed by the same
patch. This variant of the above vulnerability was reported by Lei
Wang.
<a href="https://github.com/opencontainers/runc/security/advisories/GHSA-g2j6-57v7-gm8c">https://github.com/opencontainers/runc/security/advisories/GHSA-g2j6-57v7-gm8c</a></p>
</li>
</ul>
<p>In addition, the following other fixes are included in this release:</p>
<ul>
<li>Fix the inability to use <code>/dev/null</code> when inside a container. (<a href="https://redirect.github.com/opencontainers/runc/issues/3620">#3620</a>)</li>
<li>Fix changing the ownership of host's <code>/dev/null</code> caused by fd redirection
(a regression in 1.1.1). (<a href="https://redirect.github.com/opencontainers/runc/issues/3674">#3674</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3731">#3731</a>)</li>
<li>Fix rare runc exec/enter unshare error on older kernels, including
CentOS &lt; 7.7. (<a href="https://redirect.github.com/opencontainers/runc/issues/3776">#3776</a>)</li>
<li>nsexec: Check for errors in <code>write_log()</code>. (<a href="https://redirect.github.com/opencontainers/runc/issues/3721">#3721</a>)</li>
</ul>
<h3>Static Linking Notices</h3>
<p>The <code>runc</code> binary distributed with this release are <em>statically linked</em> with
the following <a href="https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html">GNU LGPL-2.1</a> licensed libraries, with <code>runc</code> acting
as a &quot;work that uses the Library&quot;:</p>
<ul>
<li><a href="https://github.com/seccomp/libseccomp">libseccomp</a></li>
</ul>
<p>The versions of these libraries were not modified from their upstream versions,
but in order to comply with the LGPL-2.1 (§6(a)), we have attached the
complete source code for those libraries which (when combined with the attached
runc source code) may be used to exercise your rights under the LGPL-2.1.</p>
<p>However we strongly suggest that you make use of your distribution's packages
or download them from the authoritative upstream sources, especially since
these libraries are related to the security of your containers.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/opencontainers/runc/blob/main/CHANGELOG.md">github.com/opencontainers/runc's changelog</a>.</em></p>
<blockquote>
<h2>[1.1.5] - 2023-03-29</h2>
<blockquote>
<p>囚われた屈辱は
反撃の嚆矢だ</p>
</blockquote>
<h3>Security</h3>
<p>The following CVEs were fixed in this release:</p>
<ul>
<li>
<p><a href="https://github.com/opencontainers/runc/security/advisories/GHSA-m8cg-xc2p-r3fc">CVE-2023-25809</a> is a vulnerability involving rootless containers where
(under specific configurations), the container would have write access to the
<code>/sys/fs/cgroup/user.slice/...</code> cgroup hierarchy. No other hierarchies on the
host were affected. This vulnerability was discovered by Akihiro Suda.</p>
</li>
<li>
<p><a href="https://github.com/advisories/GHSA-vpvm-3wq2-2wvm">CVE-2023-27561</a> was a regression in our protections against tricky <code>/proc</code>
and <code>/sys</code> configurations (where the container mountpoint is a symlink)
causing us to be tricked into incorrectly configuring the container, which
effectively re-introduced <a href="https://github.com/advisories/GHSA-fh74-hm69-rqjw">CVE-2019-19921</a>. This regression was present
from v1.0.0-rc95 to v1.1.4 and was discovered by <a href="https://github.com/Beuc"><code>@​Beuc</code></a>. (<a href="https://redirect.github.com/opencontainers/runc/issues/3785">#3785</a>)</p>
</li>
<li>
<p><a href="https://github.com/opencontainers/runc/security/advisories/GHSA-g2j6-57v7-gm8c">CVE-2023-28642</a> is a different attack vector using the same regression
as in <a href="https://github.com/advisories/GHSA-vpvm-3wq2-2wvm">CVE-2023-27561</a>. This was reported by Lei Wang.</p>
</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix the inability to use <code>/dev/null</code> when inside a container. (<a href="https://redirect.github.com/opencontainers/runc/issues/3620">#3620</a>)</li>
<li>Fix changing the ownership of host's <code>/dev/null</code> caused by fd redirection
(a regression in 1.1.1). (<a href="https://redirect.github.com/opencontainers/runc/issues/3674">#3674</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3731">#3731</a>)</li>
<li>Fix rare runc exec/enter unshare error on older kernels, including
CentOS &lt; 7.7. (<a href="https://redirect.github.com/opencontainers/runc/issues/3776">#3776</a>)</li>
<li>nsexec: Check for errors in <code>write_log()</code>. (<a href="https://redirect.github.com/opencontainers/runc/issues/3721">#3721</a>)</li>
<li>Various CI fixes and updates. (<a href="https://redirect.github.com/opencontainers/runc/issues/3618">#3618</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3630">#3630</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3640">#3640</a>, <a href="https://redirect.github.com/opencontainers/runc/issues/3729">#3729</a>)</li>
</ul>
<h2>[1.1.4] - 2022-08-24</h2>
<blockquote>
<p>If you look for perfection, you'll never be content.</p>
</blockquote>
<h3>Fixed</h3>
<ul>
<li>Fix mounting via wrong proc fd.
When the user and mount namespaces are used, and the bind mount is followed by
the cgroup mount in the spec, the cgroup was mounted using the bind mount's
mount fd. (<a href="https://redirect.github.com/opencontainers/runc/issues/3511">#3511</a>)</li>
<li>Switch <code>kill()</code> in <code>libcontainer/nsenter</code> to <code>sane_kill()</code>. (<a href="https://redirect.github.com/opencontainers/runc/issues/3536">#3536</a>)</li>
<li>Fix &quot;permission denied&quot; error from <code>runc run</code> on <code>noexec</code> fs. (<a href="https://redirect.github.com/opencontainers/runc/issues/3541">#3541</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/opencontainers/runc/commit/f19387a6bec4944c770f7668ab51c4348d9c2f38"><code>f19387a</code></a> VERSION: release v1.1.5</li>
<li><a href="https://github.com/opencontainers/runc/commit/58a9abee210c5a72ab10904f96e0026f684f24e3"><code>58a9abe</code></a> Merge pull request from GHSA-m8cg-xc2p-r3fc</li>
<li><a href="https://github.com/opencontainers/runc/commit/27fb72c7ffdbd509b3c15b2bdb4df3d2192bfe7b"><code>27fb72c</code></a> merge branch 'pr-3776' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/8ec02ea1b14edac85a6e9a2b622ae44e15e11ccd"><code>8ec02ea</code></a> nsexec: retry unshare on EINVAL</li>
<li><a href="https://github.com/opencontainers/runc/commit/059d7730fc102052c90fea52c7b3c6f04fbbc487"><code>059d773</code></a> merge branch 'pr-3785' into release-1.1</li>
<li><a href="https://github.com/opencontainers/runc/commit/0abab45c9b97c113ff2cdc16f3a7388444c3fbec"><code>0abab45</code></a> Prohibit /proc and /sys to be symlinks</li>
<li><a href="https://github.com/opencontainers/runc/commit/0e6b818a2b0d24fdb6697614e5c5f115bbe8e3a5"><code>0e6b818</code></a> rootless: fix /sys/fs/cgroup mounts</li>
<li><a href="https://github.com/opencontainers/runc/commit/c6781d100a73d2dcef84e9376d85fff02235a2ed"><code>c6781d1</code></a> Merge pull request <a href="https://redirect.github.com/opencontainers/runc/issues/3721">#3721</a> from kinvolk/rata/nsfixes-backport</li>
<li><a href="https://github.com/opencontainers/runc/commit/f6e2cd3baf661e1f377088e13084ccb5aadf41e6"><code>f6e2cd3</code></a> nsexec: Check for errors in write_log()</li>
<li><a href="https://github.com/opencontainers/runc/commit/3775df9fcb7828594114866e1df346f44d22ad16"><code>3775df9</code></a> Merge pull request <a href="https://redirect.github.com/opencontainers/runc/issues/3731">#3731</a> from kolyshkin/1.1-fix-dev-null</li>
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.0-rc93...v1.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.0-rc93&new-version=1.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-private-chaincode/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 12:25:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/text from 0.3.7 to 0.3.8 in /samples/deployment/fabric-smart-client/the-simple-testing-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [golang.org/x/text](https://github.com/golang/text) from 0.3.7 to 0.3.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/text/commit/434eadcdbc3b0256971992e8c70027278364c72c"><code>434eadc</code></a> language: reject excessively large Accept-Language strings</li>
<li><a href="https://github.com/golang/text/commit/23407e72ed5b895a2dfd230aec777f4fbe026d6a"><code>23407e7</code></a> go.mod: ignore cyclic dependency for tagging</li>
<li><a href="https://github.com/golang/text/commit/b18d3dd8a4b426ebedcf279b593e85ac4985b9d3"><code>b18d3dd</code></a> secure/precis: replace bytes.Compare with bytes.Equal</li>
<li><a href="https://github.com/golang/text/commit/795e854ff348c9cac4fd0033ce04c417705dd0bb"><code>795e854</code></a> all: replace io/ioutil with io and os package</li>
<li><a href="https://github.com/golang/text/commit/b0ca10ff35f1325c7d0ac7830fe3f036bd72d8f9"><code>b0ca10f</code></a> internal/language: bump script types to uint16 and update registry</li>
<li><a href="https://github.com/golang/text/commit/ba9b0e1d4b03523c708709935fbc961124b6967b"><code>ba9b0e1</code></a> go.mod: update x/tools to HEAD</li>
<li><a href="https://github.com/golang/text/commit/d03b41800055b01e3895b1e047af09733c93bf63"><code>d03b418</code></a> A+C: delete AUTHORS and CONTRIBUTORS</li>
<li><a href="https://github.com/golang/text/commit/b4bca84b03619dba00657375259024a7f8ae6712"><code>b4bca84</code></a> language/display: fix Tag method comment</li>
<li><a href="https://github.com/golang/text/commit/ea49e3e2d5b3f1518081d8bc53ffefc8bc60ecec"><code>ea49e3e</code></a> go.mod: update x/tools to HEAD</li>
<li><a href="https://github.com/golang/text/commit/78819d01d041a94e055bbaa2d95e5e4d49e8f8a0"><code>78819d0</code></a> go.mod: update to golang.org/x/text v0.1.10</li>
<li>Additional commits viewable in <a href="https://github.com/golang/text/compare/v0.3.7...v0.3.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/text&package-manager=go_modules&previous-version=0.3.7&new-version=0.3.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-private-chaincode/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 12:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.5.2 to 1.5.18 in /samples/deployment/fabric-smart-client/the-simple-testing-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.5.2 to 1.5.18.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/releases">github.com/containerd/containerd's releases</a>.</em></p>
<blockquote>
<h2>containerd 1.5.18</h2>
<p>Welcome to the v1.5.18 release of containerd!</p>
<p>The eighteenth patch release for containerd 1.5 includes fixes for CVE-2023-25153 and CVE-2023-25173
along with a security update for Go.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix supplementary groups not being set up properly</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-hmfx-3pcx-653p">GHSA-hmfx-3pcx-653p</a>)</li>
<li><strong>Fix OCI image importer memory exhaustion</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-259w-8hf6-59c2">GHSA-259w-8hf6-59c2</a>)</li>
<li><strong>Update Go to 1.19.6</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/8112">#8112</a>)</li>
</ul>
<p>See the changelog for complete list of changes</p>
<p>Please try out the release binaries and report any issues at
<a href="https://github.com/containerd/containerd/issues">https://github.com/containerd/containerd/issues</a>.</p>
<h3>Contributors</h3>
<ul>
<li>Akihiro Suda</li>
<li>Derek McGowan</li>
<li>Ye Sijun</li>
<li>Samuel Karp</li>
<li>Phil Estes</li>
<li>Swagat Bora</li>
<li>Wei Fu</li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>[release/1.5] Prepare release notes for v1.5.18 (<a href="https://redirect.github.com/containerd/containerd/pull/8117">#8117</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6cb</code></a> Prepare release notes for v1.5.18</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-hmfx-3pcx-653p">GHSA-hmfx-3pcx-653p</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38bf2</code></a> oci: fix additional GIDs</li>
<li><a href="https://github.com/containerd/containerd/commit/3b89da580b76471d6c03cb1fc6c14db6aa23d3db"><code>3b89da580</code></a> oci: fix loop iterator aliasing</li>
<li><a href="https://github.com/containerd/containerd/commit/b07ec6b251bd51f06bc72ef408f31e3f6e6e87f9"><code>b07ec6b25</code></a> oci: skip checking gid for WithAppendAdditionalGroups</li>
<li><a href="https://github.com/containerd/containerd/commit/356672cb56fd5a0eed11e5089ac824c7ab09ffac"><code>356672cb5</code></a> refactor: reduce duplicate code</li>
<li><a href="https://github.com/containerd/containerd/commit/6a7b7617cfbd90009a2e05e0e5eff4ef92028d7b"><code>6a7b7617c</code></a> add WithAdditionalGIDs test</li>
<li><a href="https://github.com/containerd/containerd/commit/832bcf300b1ec29c9b08326aab2d4eafee58dd85"><code>832bcf300</code></a> add WithAppendAdditionalGroups helper</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-259w-8hf6-59c2">GHSA-259w-8hf6-59c2</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/19a347e456f3ab66909edca5351aa6f4ed1be177"><code>19a347e45</code></a> importer: stream oci-layout and manifest.json</li>
</ul>
</li>
<li>[release/1.5] Go 1.19.6 (<a href="https://redirect.github.com/containerd/containerd/pull/8112">#8112</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc243</code></a> Go 1.19.6</li>
</ul>
</li>
<li>[release/1.5] Fix retry logic within devmapper device deactivation (<a href="https://redirect.github.com/containerd/containerd/pull/8089">#8089</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d045d</code></a> Fix retry logic within devmapper device deactivation</li>
</ul>
</li>
<li>[release/1.5] CI: skip some jobs when <code>repo != containerd/containerd</code> (<a href="https://redirect.github.com/containerd/containerd/pull/8084">#8084</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/34451bc66453aad2f911aa8bffa6817061e4a72b"><code>34451bc66</code></a> CI: skip some jobs when <code>repo != containerd/containerd</code></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/blob/main/RELEASES.md">github.com/containerd/containerd's changelog</a>.</em></p>
<blockquote>
<h1>Versioning and Release</h1>
<p>This document details the versioning and release plan for containerd. Stability
is a top goal for this project, and we hope that this document and the processes
it entails will help to achieve that. It covers the release process, versioning
numbering, backporting, API stability and support horizons.</p>
<p>If you rely on containerd, it would be good to spend time understanding the
areas of the API that are and are not supported and how they impact your
project in the future.</p>
<p>This document will be considered a living document. Supported timelines,
backport targets and API stability guarantees will be updated here as they
change.</p>
<p>If there is something that you require or this document leaves out, please
reach out by <a href="https://github.com/containerd/containerd/issues">filing an issue</a>.</p>
<h2>Releases</h2>
<p>Releases of containerd will be versioned using dotted triples, similar to
<a href="http://semver.org/">Semantic Version</a>. For the purposes of this document, we
will refer to the respective components of this triple as
<code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>. The version number may have additional information,
such as alpha, beta and release candidate qualifications. Such releases will be
considered &quot;pre-releases&quot;.</p>
<h3>Major and Minor Releases</h3>
<p>Major and minor releases of containerd will be made from main. Releases of
containerd will be marked with GPG signed tags and announced at
<a href="https://github.com/containerd/containerd/releases">https://github.com/containerd/containerd/releases</a>. The tag will be of the
format <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> and should be made with the command <code>git tag -s v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</p>
<p>After a minor release, a branch will be created, with the format
<code>release/&lt;major&gt;.&lt;minor&gt;</code> from the minor tag. All further patch releases will
be done from that branch. For example, once we release <code>v1.0.0</code>, a branch
<code>release/1.0</code> will be created from that tag. All future patch releases will be
done against that branch.</p>
<h3>Pre-releases</h3>
<p>Pre-releases, such as alphas, betas and release candidates will be conducted
from their source branch. For major and minor releases, these releases will be
done from main. For patch releases, these pre-releases should be done within
the corresponding release branch.</p>
<p>While pre-releases are done to assist in the stabilization process, no
guarantees are provided.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/39bb06f98f17c7a226b10269d325c861585b2389"><code>39bb06f</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8117">#8117</a> from dmcgowan/prepare-v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6</code></a> Prepare release notes for v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/28e461805038a431c0bd1c04f31a438470c24450"><code>28e4618</code></a> Merge pull request from GHSA-hmfx-3pcx-653p</li>
<li><a href="https://github.com/containerd/containerd/commit/959e1cf9602f3b7a71bdca7b6344b40e00504730"><code>959e1cf</code></a> Merge pull request from GHSA-259w-8hf6-59c2</li>
<li><a href="https://github.com/containerd/containerd/commit/b4538c253204b169366b7f3d3f990b47eae7ade0"><code>b4538c2</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8112">#8112</a> from AkihiroSuda/cherrypick-8109-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc2</code></a> Go 1.19.6</li>
<li><a href="https://github.com/containerd/containerd/commit/7c3b24362756e11c841ec7fa4a8aecb8f94e6894"><code>7c3b243</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8089">#8089</a> from swagatbora90/backport-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d04</code></a> Fix retry logic within devmapper device deactivation</li>
<li><a href="https://github.com/containerd/containerd/commit/9e9f4c8ea77d016387bee13eeb773f4a79d6c054"><code>9e9f4c8</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/8084">#8084</a> from AkihiroSuda/ci-skip-on-fork-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38b</code></a> oci: fix additional GIDs</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.5.2...v1.5.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.5.2&new-version=1.5.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-private-chaincode/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 12:25:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    Go support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR brings in experimental support for go-chaincode for FPC.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 11:51:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Remove Ubuntu 18.04 from GH actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes running FPC tests on old ubuntu 18.04.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 11:45:09 +0000 UTC
    </div>
</div>

