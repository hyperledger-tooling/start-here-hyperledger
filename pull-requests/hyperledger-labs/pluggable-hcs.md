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
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/crypto from 0.0.0-20210322153248-0c34fe9e7dc2 to 0.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.0.0-20210322153248-0c34fe9e7dc2 to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/crypto/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.0.0-20210322153248-0c34fe9e7dc2&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 03:16:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pluggable-hcs/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/distribution from 2.7.1+incompatible to 2.8.0+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/docker/distribution](https://github.com/docker/distribution) from 2.7.1+incompatible to 2.8.0+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/distribution/releases">github.com/docker/distribution's releases</a>.</em></p>
<blockquote>
<h2>v2.8.0</h2>
<p>registry 2.8.0</p>
<p>Welcome to the v2.8.0 release of registry!</p>
<p>The 2.8.0 registry release has been a long time overdue.
This is the first step towards the last 2.x release.
No further active development will continue on 2.x branch.
Security vulnerability patches to 2.x might be considered, but
all active development will be focussed on v3 release due in 2022.
This release includes a security vulnerability fix along
with a few minor bug fixes and improvemnts in documentation and CI.</p>
<p>See changelog below for full list of changes.</p>
<h3>Bugfixes</h3>
<ul>
<li>Close the io.ReadCloser from storage driver <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3370">#3370</a></li>
<li>Remove empty Content-Type header <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3297">#3297</a></li>
<li>Make ipfilteredby not required in cloudfront storage middleware <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3088">#3088</a></li>
</ul>
<h3>Features</h3>
<ul>
<li>Add reference.ParseDockerRef utility function <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3002">#3002</a></li>
</ul>
<h3>CI build</h3>
<ul>
<li>First draft of actions based ci <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3347">#3347</a></li>
<li>Fix vndr and check <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3001">#3001</a></li>
<li>Improve code quality by adding linter checks <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3385">#3385</a></li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Add redirect for old URL <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3197">#3197</a></li>
<li>Fix broken table <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3073">#3073</a></li>
<li>Adding deprecated schema v1 instructions <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/2987">#2987</a></li>
<li>Change should to must in v2 spec (<a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3495">#3495</a>)</li>
</ul>
<h3>Storage drivers</h3>
<ul>
<li>S3 Driver: add support for ceph radosgw <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3119">#3119</a></li>
</ul>
<h3>Security</h3>
<ul>
<li>Added flag for user configurable cipher suites <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3384">#3384</a></li>
<li>Address <a href="https://github.com/advisories/GHSA-w73w-5m7g-f7qc">CVE-2020-26160</a> by replacing vulnerable third-party depedency<a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3466">#3466</a></li>
<li>Replace math rand with crypto rand <a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3531">#3531</a></li>
<li>Address <a href="https://github.com/advisories/GHSA-mc8v-mgrf-8f4m">CVE-2021-41190</a> by validating document type before unmarshal <a href="https://github-redirect.dependabot.com/distribution/distribution-ghsa-qq97-vm5h-rrhg/pull/2">GHSA-77vh-xpmg-72qh</a></li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>Prepare for v2.8.0 release (<a href="https://github-redirect.dependabot.com/distribution/distribution/pull/3552">#3552</a>)
<ul>
<li><a href="https://github.com/distribution/distribution/commit/d5d89a46a388a1d35b3b9b9cd60515e45ac3a7d4"><code>d5d89a46</code></a> Make this releaes a beta release first.</li>
<li><a href="https://github.com/distribution/distribution/commit/1ddad0bad8c5e207904d9241ba2fb4557b27e1ed"><code>1ddad0ba</code></a> Apply suggestions from code review</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/distribution/distribution/commit/dcf66392d606f50bf3a9286dcb4bdcdfb7c0e83a"><code>dcf6639</code></a> Update README so the release pipeline works properly.</li>
<li><a href="https://github.com/distribution/distribution/commit/212b38ed225e42676c2a2e478aecc2b2fcc62fc9"><code>212b38e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/distribution/issues/3552">#3552</a> from milosgajdos/v2.8.0-release</li>
<li><a href="https://github.com/distribution/distribution/commit/359b97a75a339af182e960fdabf6ade2e0474629"><code>359b97a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/distribution/issues/3568">#3568</a> from crazy-max/2.8-artifacts</li>
<li><a href="https://github.com/distribution/distribution/commit/d5d89a46a388a1d35b3b9b9cd60515e45ac3a7d4"><code>d5d89a4</code></a> Make this releaes a beta release first.</li>
<li><a href="https://github.com/distribution/distribution/commit/6241e099e14dff2dd85a3bcd31cfcf9942dadc49"><code>6241e09</code></a> [2.8] Release artifacts</li>
<li><a href="https://github.com/distribution/distribution/commit/1840415ca85bc6d70106dccea1c13743e7d3b6fb"><code>1840415</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/docker/distribution/issues/3565">#3565</a> from crazy-max/2.8-gha</li>
<li><a href="https://github.com/distribution/distribution/commit/65ca39e60558bf526de2b1f00bf75b0fdd898071"><code>65ca39e</code></a> release workflow</li>
<li><a href="https://github.com/distribution/distribution/commit/1ddad0bad8c5e207904d9241ba2fb4557b27e1ed"><code>1ddad0b</code></a> Apply suggestions from code review</li>
<li><a href="https://github.com/distribution/distribution/commit/3960a560bbb7a4e483da2d6f83158d18f9ab21f9"><code>3960a56</code></a> Prepare for v2.8.0 release</li>
<li><a href="https://github.com/distribution/distribution/commit/3b7b534569220c840993aad03e3eafe54b923f4d"><code>3b7b534</code></a> Merge pull request from GHSA-qq97-vm5h-rrhg</li>
<li>Additional commits viewable in <a href="https://github.com/docker/distribution/compare/v2.7.1...v2.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/distribution&package-manager=go_modules&previous-version=2.7.1+incompatible&new-version=2.8.0+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/pluggable-hcs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 03:16:30 +0000 UTC
    </div>
</div>

