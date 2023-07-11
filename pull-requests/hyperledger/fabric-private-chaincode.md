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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/713" class=".btn">#713</a>
            </td>
            <td>
                <b>
                    Resolves #693, upgrade ego to v1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                What this PR does / why we need it:
Upgrade ego to v1.2, current ego version is v1.0

Which issue(s) this PR fixes:

Fixes https://github.com/hyperledger/fabric-private-chaincode/issues/693

Special notes for your reviewer:
Successfully build docker-dev in local

can build local dev and test ego using the code below
```
cd $FPC_PATH/utils/docker
make build-dev
make run-dev
```

Here is the result:
```
root@docker-desktop:/project/src/github.com/hyperledger/fabric-private-chaincode# ego
EGo v1.2.0 (f272b3f4430c819530e33ef5ff6c930b3dd2afa0)
Manage and run EGo enclaves.
...
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 20:39:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/712" class=".btn">#712</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 23.0.2+incompatible to 23.0.3+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 23.0.2+incompatible to 23.0.3+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v23.0.3</h2>
<h2>23.0.3</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Due to an issue with CentOS 9 Stream's package repositories, packages for
CentOS 9 are currently unavailable. Packages for CentOS 9 may be added later,
or as part of the next (23.0.4) patch release.</p>
</blockquote>
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
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update containerd to <a href="https://github.com/containerd/containerd/releases/tag/v1.6.20">v1.6.20</a>.</li>
<li>Update runc to <a href="https://github.com/opencontainers/runc/releases/tag/v1.1.5">v1.1.5</a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/59118bff500fc0d95d0560a9788735a8d89568ce"><code>59118bf</code></a> Merge pull request from GHSA-232p-vwff-86mp</li>
<li><a href="https://github.com/moby/moby/commit/b87f7f18b82fbb647b5142c6e5459a88a7652d02"><code>b87f7f1</code></a> libnet/d/overlay: insert the input-drop rule</li>
<li><a href="https://github.com/moby/moby/commit/98cbcb8003b7cf8da35fb5d05f5babbe142ab7c8"><code>98cbcb8</code></a> libnet/d/overlay: add BPF-powered VNI matcher</li>
<li><a href="https://github.com/moby/moby/commit/5c5fac237425c4bf79d2f048c1850f855f0182aa"><code>5c5fac2</code></a> libnet/d/overlay: extract VNI match rule builder</li>
<li><a href="https://github.com/moby/moby/commit/c492a22287557860831a7c4f523b8e53692bb822"><code>c492a22</code></a> libn/d/overlay: enforce encryption on sandbox init</li>
<li><a href="https://github.com/moby/moby/commit/018edb02849100de701d6ab6fb932ffb68843e4b"><code>018edb0</code></a> libnet/d/overlay: document some encryption code</li>
<li>See full diff in <a href="https://github.com/docker/docker/compare/v23.0.2...v23.0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=23.0.2+incompatible&new-version=23.0.3+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-07-10 12:52:04 +0000 UTC
    </div>
</div>

