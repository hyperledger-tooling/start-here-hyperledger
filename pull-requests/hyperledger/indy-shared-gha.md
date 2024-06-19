---
layout: default
title: indy-shared-gha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-shared-gha
---

# indy-shared-gha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-shared-gha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-shared-gha/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Bump docker/build-push-action from 5 to 6 in the all-actions group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 1 update: [docker/build-push-action](https://github.com/docker/build-push-action).

Updates `docker/build-push-action` from 5 to 6
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v6.0.0</h2>
<ul>
<li>Export build record and generate <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">build summary</a> by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1120">docker/build-push-action#1120</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.24.0 to 0.26.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1132">docker/build-push-action#1132</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1136">docker/build-push-action#1136</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1138">docker/build-push-action#1138</a></li>
<li>Bump braces from 3.0.2 to 3.0.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1137">docker/build-push-action#1137</a></li>
</ul>
<blockquote>
<p>[!NOTE]
This major release adds support for generating <a href="https://docs.docker.com/build/ci/github-actions/build-summary/">Build summary</a> and exporting build record for your build. You can disable this feature by setting <a href="https://docs.docker.com/build/ci/github-actions/build-summary/#disable-job-summary"> <code>DOCKER_BUILD_NO_SUMMARY: true</code> environment variable in your workflow</a>.</p>
</blockquote>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0">https://github.com/docker/build-push-action/compare/v5.4.0...v6.0.0</a></p>
<h2>v5.4.0</h2>
<ul>
<li>Show builder information before building by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1128">docker/build-push-action#1128</a></li>
<li>Handle attestations correctly with provenance and sbom inputs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1086">docker/build-push-action#1086</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.24.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1088">docker/build-push-action#1088</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1105">docker/build-push-action#1105</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1121">docker/build-push-action#1121</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1127">docker/build-push-action#1127</a></li>
<li>Bump undici from 5.28.3 to 5.28.4 in <a href="https://redirect.github.com/docker/build-push-action/pull/1090">docker/build-push-action#1090</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0">https://github.com/docker/build-push-action/compare/v5.3.0...v5.4.0</a></p>
<h2>v5.3.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1080">docker/build-push-action#1080</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0">https://github.com/docker/build-push-action/compare/v5.2.0...v5.3.0</a></p>
<h2>v5.2.0</h2>
<ul>
<li>Disable quotes detection for <code>outputs</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1074">docker/build-push-action#1074</a></li>
<li>Warn about ignored inputs by <a href="https://github.com/favonia"><code>@​favonia</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/1019">docker/build-push-action#1019</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.14.0 to 0.18.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/1070">docker/build-push-action#1070</a></li>
<li>Bump undici from 5.26.3 to 5.28.3 in <a href="https://redirect.github.com/docker/build-push-action/pull/1057">docker/build-push-action#1057</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0">https://github.com/docker/build-push-action/compare/v5.1.0...v5.2.0</a></p>
<h2>v5.1.0</h2>
<ul>
<li>Add <code>annotations</code> input by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/992">docker/build-push-action#992</a></li>
<li>Add <code>secret-envs</code> input by <a href="https://github.com/elias-lundgren"><code>@​elias-lundgren</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/980">docker/build-push-action#980</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.17.3 to 7.23.2 in <a href="https://redirect.github.com/docker/build-push-action/pull/991">docker/build-push-action#991</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.13.0-rc.1 to 0.14.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/990">docker/build-push-action#990</a> <a href="https://redirect.github.com/docker/build-push-action/pull/1006">docker/build-push-action#1006</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0">https://github.com/docker/build-push-action/compare/v5.0.0...v5.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/c382f710d39a5bb4e430307530a720f50c2d3318"><code>c382f71</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1120">#1120</a> from crazy-max/build-summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/5a5b70d974381b812e448a9ea8efef0c0781e8a7"><code>5a5b70d</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/dc24cf9e252ee3b05f80a1637b2950c11d305b3d"><code>dc24cf9</code></a> don't generate summary for cloud driver</li>
<li><a href="https://github.com/docker/build-push-action/commit/667cb22c52a8762431790112e70ef7f545dbf2d2"><code>667cb22</code></a> DOCKER_BUILD_NO_SUMMARY env to disable summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/d880b1964b626c7ac1763e83768e139202071136"><code>d880b19</code></a> generate build summary</li>
<li><a href="https://github.com/docker/build-push-action/commit/e51051ad0baf1cdf23788f7f0980f675806b580e"><code>e51051a</code></a> export build record and upload artifact</li>
<li><a href="https://github.com/docker/build-push-action/commit/86c2bd00318427a320d2cee5bbc61251df6f647e"><code>86c2bd0</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1137">#1137</a> from docker/dependabot/npm_and_yarn/braces-3.0.3</li>
<li><a href="https://github.com/docker/build-push-action/commit/268d2b16117932ad41015c96fbc27a7641533625"><code>268d2b1</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1138">#1138</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/2b8dc7f52914dfdd416618a1f33d11277b7d64d2"><code>2b8dc7f</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/840c12be1707e3d7115f8d61da2c8b78442cc538"><code>840c12b</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.25.1 to 0.26.0</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v5...v6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/build-push-action&package-manager=github_actions&previous-version=5&new-version=6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 18:28:42 +0000 UTC
    </div>
</div>

