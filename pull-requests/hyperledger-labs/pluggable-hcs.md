---
layout: default
title: pluggable-hcs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pluggable-hcs
---

# pluggable-hcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pluggable-hcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.26.0 to 2.31.0 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.26.0 to 2.31.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.31.0</h2>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>v2.30.0</h2>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
<h2>v2.29.0</h2>
<h2>2.29.0 (2023-04-26)</h2>
<p><strong>Improvements</strong></p>
<ul>
<li>Requests now defers chunked requests to the urllib3 implementation to improve
standardization. (<a href="https://redirect.github.com/psf/requests/issues/6226">#6226</a>)</li>
<li>Requests relaxes header component requirements to support bytes/str subclasses. (<a href="https://redirect.github.com/psf/requests/issues/6356">#6356</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
<h2>2.30.0 (2023-05-03)</h2>
<p><strong>Dependencies</strong></p>
<ul>
<li>
<p>⚠️ Added support for urllib3 2.0. ⚠️</p>
<p>This may contain minor breaking changes so we advise careful testing and
reviewing <a href="https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html">https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html</a>
prior to upgrading.</p>
<p>Users who wish to stay on urllib3 1.x can pin to <code>urllib3&lt;2</code>.</p>
</li>
</ul>
<h2>2.29.0 (2023-04-26)</h2>
<p><strong>Improvements</strong></p>
<ul>
<li>Requests now defers chunked requests to the urllib3 implementation to improve
standardization. (<a href="https://redirect.github.com/psf/requests/issues/6226">#6226</a>)</li>
<li>Requests relaxes header component requirements to support bytes/str subclasses. (<a href="https://redirect.github.com/psf/requests/issues/6356">#6356</a>)</li>
</ul>
<h2>2.28.2 (2023-01-12)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4"><code>147c851</code></a> v2.31.0</li>
<li><a href="https://github.com/psf/requests/commit/74ea7cf7a6a27a4eeb2ae24e162bcc942a6706d5"><code>74ea7cf</code></a> Merge pull request from GHSA-j8r2-6x86-q33q</li>
<li><a href="https://github.com/psf/requests/commit/302225334678490ec66b3614a9dddb8a02c5f4fe"><code>3022253</code></a> test on pypy 3.8 and pypy 3.9 on windows and macos (<a href="https://redirect.github.com/psf/requests/issues/6424">#6424</a>)</li>
<li><a href="https://github.com/psf/requests/commit/b639e66c816514e40604d46f0088fbceec1a5149"><code>b639e66</code></a> test on py3.12 (<a href="https://redirect.github.com/psf/requests/issues/6448">#6448</a>)</li>
<li><a href="https://github.com/psf/requests/commit/d3d504436ef0c2ac7ec8af13738b04dcc8c694be"><code>d3d5044</code></a> Fixed a small typo (<a href="https://redirect.github.com/psf/requests/issues/6452">#6452</a>)</li>
<li><a href="https://github.com/psf/requests/commit/2ad18e0e10e7d7ecd5384c378f25ec8821a10a29"><code>2ad18e0</code></a> v2.30.0</li>
<li><a href="https://github.com/psf/requests/commit/f2629e9e3c7ce3c3c8c025bcd8db551101cbc773"><code>f2629e9</code></a> Remove strict parameter (<a href="https://redirect.github.com/psf/requests/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/psf/requests/commit/87d63de8739263bbe17034fba2285c79780da7e8"><code>87d63de</code></a> v2.29.0</li>
<li><a href="https://github.com/psf/requests/commit/51716c4ef390136b0d4b800ec7665dd5503e64fc"><code>51716c4</code></a> enable the warnings plugin (<a href="https://redirect.github.com/psf/requests/issues/6416">#6416</a>)</li>
<li><a href="https://github.com/psf/requests/commit/a7da1ab3498b10ec3a3582244c94b2845f8a8e71"><code>a7da1ab</code></a> try on ubuntu 22.04 (<a href="https://redirect.github.com/psf/requests/issues/6418">#6418</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.26.0...v2.31.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.26.0&new-version=2.31.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 20:09:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Archive lab
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
        Created At 2023-05-17 17:29:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 17.12.0-ce-rc1.0.20190628135806-70f67c6240bb+incompatible to 20.10.24+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 17.12.0-ce-rc1.0.20190628135806-70f67c6240bb+incompatible to 20.10.24+incompatible.
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
<li>See full diff in <a href="https://github.com/docker/docker/commits/v20.10.24">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=17.12.0-ce-rc1.0.20190628135806-70f67c6240bb+incompatible&new-version=20.10.24+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:46:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/distribution from 2.8.0+incompatible to 2.8.2+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/docker/distribution](https://github.com/docker/distribution) from 2.8.0+incompatible to 2.8.2+incompatible.
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
<h2>v2.8.1</h2>
<p>Welcome to the v2.8.1 release of registry!</p>
<p>The 2.8.1 registry release fixes the Go module issues that have popped up in the v2.8.0</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/docker/distribution/compare/v2.8.0...v2.8.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/distribution&package-manager=go_modules&previous-version=2.8.0+incompatible&new-version=2.8.2+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc from 1.0.0-rc8 to 1.1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/opencontainers/runc](https://github.com/opencontainers/runc) from 1.0.0-rc8 to 1.1.5.
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
<li>Additional commits viewable in <a href="https://github.com/opencontainers/runc/compare/v1.0.0-rc8...v1.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/opencontainers/runc&package-manager=go_modules&previous-version=1.0.0-rc8&new-version=1.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:45:25 +0000 UTC
    </div>
</div>

