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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/530" class=".btn">#530</a>
            </td>
            <td>
                <b>
                    Bump github.com/quic-go/quic-go from 0.38.1 to 0.38.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/quic-go/quic-go](https://github.com/quic-go/quic-go) from 0.38.1 to 0.38.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/quic-go/quic-go/releases">github.com/quic-go/quic-go's releases</a>.</em></p>
<blockquote>
<h2>v0.38.2</h2>
<p>This release contains fixes for a resource exhaustion attack on QUIC's path validation logic (CVE-2023-49295), see <a href="https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation">https://seemann.io/posts/2023-12-18-exploiting-quics-path-validation</a> for details:</p>
<ul>
<li>limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/pull/4199">quic-go/quic-go#4199</a>)</li>
<li>don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/pull/4200">quic-go/quic-go#4200</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/quic-go/quic-go/commit/9aaefe19fc3dc8c8917cc87e6128bb56d9e9e6cc"><code>9aaefe1</code></a> don't retransmit PATH_CHALLENGE and PATH_RESPONSE frames (<a href="https://redirect.github.com/quic-go/quic-go/issues/4200">#4200</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/17fc98c2d81dbe685c19702dc694a9d606ac56dc"><code>17fc98c</code></a> limit the number of queued PATH_RESPONSE frames to 256 (<a href="https://redirect.github.com/quic-go/quic-go/issues/4199">#4199</a>)</li>
<li>See full diff in <a href="https://github.com/quic-go/quic-go/compare/v0.38.1...v0.38.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/quic-go/quic-go&package-manager=go_modules&previous-version=0.38.1&new-version=0.38.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-01-10 15:11:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/529" class=".btn">#529</a>
            </td>
            <td>
                <b>
                    remove kvs from ttxdb
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
        Created At 2024-01-10 14:29:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/528" class=".btn">#528</a>
            </td>
            <td>
                <b>
                    Refactored wallet registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                Extracted kvs functionality to be wallet specific
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 16:50:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.7.7 to 1.7.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.7.7 to 1.7.11.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/releases">github.com/containerd/containerd's releases</a>.</em></p>
<blockquote>
<h2>containerd 1.7.11</h2>
<p>Welcome to the v1.7.11 release of containerd!</p>
<p>The eleventh patch release for containerd 1.7 contains various fixes and updates including
one security issue.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix Windows default path overwrite issue</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9440">#9440</a>)</li>
<li><strong>Update push to always inherit distribution sources from parent</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9452">#9452</a>)</li>
<li><strong>Update shim to use net dial for gRPC shim sockets</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9458">#9458</a>)</li>
<li><strong>Fix otel version incompatibility</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9483">#9483</a>)</li>
<li><strong>Fix Windows snapshotter blocking snapshot GC on remove failure</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9482">#9482</a>)</li>
<li><strong>Mask <code>/sys/devices/virtual/powercap</code> path in runtime spec and deny in default apparmor profile</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-7ww5-4wqc-m92c">GHSA-7ww5-4wqc-m92c</a>)</li>
</ul>
<h3>Deprecation Warnings</h3>
<ul>
<li><strong>Emit deprecation warning for AUFS snapshotter</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9436">#9436</a>)</li>
<li><strong>Emit deprecation warning for v1 runtime</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9450">#9450</a>)</li>
<li><strong>Emit deprecation warning for deprecated CRI configs</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9469">#9469</a>)</li>
<li><strong>Emit deprecation warning for CRI v1alpha1 usage</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9479">#9479</a>)</li>
<li><strong>Emit deprecation warning for CRIU config in CRI</strong> (<a href="https://redirect.github.com/containerd/containerd/pull/9481">#9481</a>)</li>
</ul>
<p>See the changelog for complete list of changes</p>
<p>Please try out the release binaries and report any issues at
<a href="https://github.com/containerd/containerd/issues">https://github.com/containerd/containerd/issues</a>.</p>
<h3>Contributors</h3>
<ul>
<li>Samuel Karp</li>
<li>Derek McGowan</li>
<li>Phil Estes</li>
<li>Bjorn Neergaard</li>
<li>Danny Canter</li>
<li>Sebastiaan van Stijn</li>
<li>ruiwen-zhao</li>
<li>Akihiro Suda</li>
<li>Amit Barve</li>
<li>Charity Kathure</li>
<li>Maksym Pavlenko</li>
<li>Milas Bowman</li>
<li>Paweł Gronowski</li>
<li>Wei Fu</li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>[release/1.7] Prepare release notes for v1.7.11 (<a href="https://redirect.github.com/containerd/containerd/pull/9491">#9491</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/64b8a811b07ba6288238eefc14d898ee0b5b99ba"><code>64b8a81</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9491">#9491</a> from dmcgowan/prepare-1.7.11</li>
<li><a href="https://github.com/containerd/containerd/commit/ea5a4778aa63b3bee0225ec368d4cd2af7dcd238"><code>ea5a477</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9352">#9352</a> from thaJeztah/1.7_update_golang_1.20.11</li>
<li><a href="https://github.com/containerd/containerd/commit/67d356cb3095f3e8f8ad7d36f9a733fea1e7e28c"><code>67d356c</code></a> Merge pull request from GHSA-7ww5-4wqc-m92c</li>
<li><a href="https://github.com/containerd/containerd/commit/dfae68bc3e614a091d0a468c9026da370e3de0d9"><code>dfae68b</code></a> Prepare release notes for v1.7.11</li>
<li><a href="https://github.com/containerd/containerd/commit/de6d8a8fc60851adbfc1d7c9567799357f288e5c"><code>de6d8a8</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9482">#9482</a> from ambarve/sn_cleanup_1.7</li>
<li><a href="https://github.com/containerd/containerd/commit/ed7c6895bd3b33ccc7cfbc8cbd43f6a31333328a"><code>ed7c689</code></a> Don't block snapshot garbage collection on Remove failures</li>
<li><a href="https://github.com/containerd/containerd/commit/467de562c108d074d81dd81d42150f98a6608eae"><code>467de56</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9481">#9481</a> from ruiwen-zhao/cri-u</li>
<li><a href="https://github.com/containerd/containerd/commit/d94f8ffeb057a89dd363fa220b24454cf88f0780"><code>d94f8ff</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9483">#9483</a> from dmcgowan/backport-1.7-fix-otel-http</li>
<li><a href="https://github.com/containerd/containerd/commit/1fdefdd2242fcf704a11f1d6b5149e056ce98ed3"><code>1fdefdd</code></a> Add warning for CRIU config usage</li>
<li><a href="https://github.com/containerd/containerd/commit/8e0689938a47e582ebefc5709b405fce3badd835"><code>8e06899</code></a> Merge pull request <a href="https://redirect.github.com/containerd/containerd/issues/9479">#9479</a> from ruiwen-zhao/cri-api-warning</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.7.7...v1.7.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.7.7&new-version=1.7.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-01-08 13:34:29 +0000 UTC
    </div>
</div>

