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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    join orderer issue fix on without system channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
<!--- Describe your changes in detail, including motivation. -->
Issue fix channel creation fail on join orderer

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 15:28:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Fix for Channel UI change from Grid to List view
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
<!--- Describe your changes in detail, including motivation. -->
- Handle error while switching channel UI from Grid to List view.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 05:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    Sync and update fabric operator apis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement

#### Description
Sync the deployer code up to dated with the fabric-operator API changes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 15:11:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    bump release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
increment release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 22:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 20.10.12+incompatible to 20.10.27+incompatible in /packages/fabric-deployer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 20.10.12+incompatible to 20.10.27+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v20.10.27</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A20.10.27">docker/cli, 20.10.27 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A20.10.27">moby/moby, 20.10.27 milestone</a></li>
</ul>
<h3>Bug Fixes and Enhancements</h3>
<ul>
<li>Fix dockerd-rootless-setuptools.sh when user name contains a backslash. <a href="https://redirect.github.com/moby/moby/pull/46424">moby/moby#46424</a></li>
<li>Add <code>IP_NF_MANGLE</code> to check-config.sh to the &quot;generally required&quot; list in check-config.sh because it is required by Swarm. <a href="https://redirect.github.com/moby/moby/pull/46674">moby/moby#46674</a></li>
<li>Fix a deadlock in libnetwork which could prevent containers from starting. <a href="https://redirect.github.com/moby/moby/pull/46693">moby/moby#46693</a></li>
<li>Write overlay2 layer metadata atomically. <a href="https://redirect.github.com/moby/moby/pull/46705">moby/moby#46705</a></li>
<li>Support building with Go 1.20. <a href="https://redirect.github.com/moby/moby/pull/46694">moby/moby#46694</a> <a href="https://redirect.github.com/moby/moby/pull/46695">moby/moby#46695</a> <a href="https://redirect.github.com/moby/moby/pull/46696">moby/moby#46696</a></li>
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update to go1.20.10, golang/org/x/net v0.17.0. <a href="https://redirect.github.com/moby/moby/pull/46692">moby/moby#46692</a></li>
</ul>
<h3>Security</h3>
<ul>
<li>Deny containers access to <code>/sys/devices/virtual/powercap</code> by default. This change hardens against <a href="https://scout.docker.com/v/CVE-2020-8694">CVE-2020-8694</a>, <a href="https://scout.docker.com/v/CVE-2020-8695">CVE-2020-8695</a>, and <a href="https://scout.docker.com/v/CVE-2020-12912">CVE-2020-12912</a>, and an attack known as <a href="https://platypusattack.com/">the PLATYPUS attack</a>. For more details, see <a href="https://github.com/moby/moby/security/advisories/GHSA-jq35-85cj-fj4p">advisory</a>, <a href="https://github.com/moby/moby/commit/81ebe71275768629689a23bc3bca34b3b374a6a6">commit</a>.</li>
</ul>
<h2>v20.10.26</h2>
<h2>20.10.26</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A20.10.26">docker/cli, 20.10.26 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A20.10.26">moby/moby, 20.10.26 milestone</a></li>
</ul>
<h3>Bug Fixes and Enhancements</h3>
<ul>
<li>Support filesystems which do not support extended file attributes with the VFS graph driver. <a href="https://redirect.github.com/moby/moby/pull/45466">moby/moby#45466</a></li>
<li>Fix AppArmor profile docker-default <code>/proc/sys</code> rule. <a href="https://redirect.github.com/moby/moby/pull/45716">moby/moby#45716</a></li>
<li>seccomp: always allow <code>name_to_handle_at(2)</code>. <a href="https://redirect.github.com/moby/moby/pull/45835">moby/moby#45835</a></li>
<li>Fix an issue which prevented volumes mounted to a live-restored container from being removed. <a href="https://redirect.github.com/moby/moby/pull/45840">moby/moby#45840</a></li>
<li>client: resolve an incompatibility with Go 1.20.6, Go 1.20.7, Go 1.19.11 and Go 1.19.12. <a href="https://redirect.github.com/moby/moby/pull/45972">moby/moby#45972</a></li>
<li>windows: fix <code>--register-service</code> when executed from within binary directory. <a href="https://redirect.github.com/moby/moby/pull/46217">moby/moby#46217</a></li>
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update Go to 1.19.12. <a href="https://redirect.github.com/moby/moby/pull/46142">moby/moby#46142</a></li>
<li>Update containerd to v1.6.22. <a href="https://redirect.github.com/moby/moby/pull/46105">moby/moby#46105</a></li>
<li>Update runc to v1.1.8. <a href="https://redirect.github.com/moby/moby/pull/46031">moby/moby#46031</a></li>
<li>Delete Upstart init scripts and clean up sysvinit. <a href="https://redirect.github.com/moby/moby/pull/46047">moby/moby#46047</a></li>
</ul>
<h2>v20.10.25</h2>
<h2>Bug fixes and enhancements</h2>
<ul>
<li>Fix log loss with the AWSLogs log driver <a href="https://redirect.github.com/moby/moby/pull/45349">moby/moby#45349</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/81ebe71275768629689a23bc3bca34b3b374a6a6"><code>81ebe71</code></a> Merge pull request from GHSA-jq35-85cj-fj4p</li>
<li><a href="https://github.com/moby/moby/commit/fb636657a7a322bd5da4270c4d95f037576570b3"><code>fb63665</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46705">#46705</a> from thaJeztah/20.10_backport_atomic-layer-data-write</li>
<li><a href="https://github.com/moby/moby/commit/b967d897586ca3e3e8dcd96d9b5712b5ac02bc9f"><code>b967d89</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46692">#46692</a> from corhere/backport-20.10/update-x-net-v0.17</li>
<li><a href="https://github.com/moby/moby/commit/2c22bd52808f1c15d8efcdfb8c960f778c439a37"><code>2c22bd5</code></a> vendor: golang.org/x/net v0.17.0</li>
<li><a href="https://github.com/moby/moby/commit/d862c21eb2a806ab72069664f6ba5a75006fc843"><code>d862c21</code></a> Update to go1.20.10</li>
<li><a href="https://github.com/moby/moby/commit/cb47414f4187aff09c3d49ac93f7a15411c49d11"><code>cb47414</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46696">#46696</a> from corhere/backport-20.10/go1.20-enablement</li>
<li><a href="https://github.com/moby/moby/commit/ea4eb7398c8adea7610ea9b0123cf19dad9a7817"><code>ea4eb73</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/46695">#46695</a> from corhere/backport-20.10/safer-fileinfo</li>
<li><a href="https://github.com/moby/moby/commit/6c523aabaec55e36c0b53f4b03844b377869ce91"><code>6c523aa</code></a> hack: fix suppressing Xattrs lint errors</li>
<li><a href="https://github.com/moby/moby/commit/31b837499c2cd62bdd3d4cdfeaf83903dbc27f6b"><code>31b8374</code></a> pkg/archive: audit gosec file-traversal lints</li>
<li><a href="https://github.com/moby/moby/commit/8e4485536ba493508afd894beb9f7c2bdbf4df99"><code>8e44855</code></a> Remove local fork of archive/tar package</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v20.10.12...v20.10.27">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=20.10.12+incompatible&new-version=20.10.27+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-06 19:25:25 +0000 UTC
    </div>
</div>

