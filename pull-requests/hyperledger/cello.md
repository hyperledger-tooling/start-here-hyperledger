---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Bump undefsafe from 2.0.2 to 2.0.5 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undefsafe](https://github.com/remy/undefsafe) from 2.0.2 to 2.0.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remy/undefsafe/releases">undefsafe's releases</a>.</em></p>
<blockquote>
<h2>v2.0.5</h2>
<h2><a href="https://github.com/remy/undefsafe/compare/v2.0.4...v2.0.5">2.0.5</a> (2021-10-17)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove debug and add tests (<a href="https://github.com/remy/undefsafe/commit/58fc47439a3bb2cd1cccdaeb8777561a325fba1c">58fc474</a>), closes <a href="https://github-redirect.dependabot.com/remy/undefsafe/issues/12">#12</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remy/undefsafe/commit/5d3fa3460e6716ed85dd3d41f4973fcd0896493d"><code>5d3fa34</code></a> chore: adding semver release</li>
<li><a href="https://github.com/remy/undefsafe/commit/58fc47439a3bb2cd1cccdaeb8777561a325fba1c"><code>58fc474</code></a> fix: remove debug and add tests</li>
<li><a href="https://github.com/remy/undefsafe/commit/f272681b3a50e2c4cbb6a8533795e1453382c822"><code>f272681</code></a> fix: prevent changes in prototype chain</li>
<li><a href="https://github.com/remy/undefsafe/commit/f4959541af2a607258ce197e7a07b79e6e8a8356"><code>f495954</code></a> chore: prettier changes</li>
<li>See full diff in <a href="https://github.com/remy/undefsafe/compare/v2.0.2...v2.0.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undefsafe&package-manager=npm_and_yarn&previous-version=2.0.2&new-version=2.0.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 09:53:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Remove hardcode for publishing ports of HLF nodes. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since we are using the docker network instead, mapping ports from hosts
is no longer necessary here. I remove these lines of code in this pr.

Fix #377 

Signed-off-by: Yuanmao Zhu <yuanmao@ualberta.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 19:57:15 +0000 UTC
    </div>
</div>

