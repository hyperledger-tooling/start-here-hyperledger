---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    Bump gradle/gradle-build-action from 2.3.3 to 3.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [gradle/gradle-build-action](https://github.com/gradle/gradle-build-action) from 2.3.3 to 3.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gradle/gradle-build-action/releases">gradle/gradle-build-action's releases</a>.</em></p>
<blockquote>
<h2>v3.3.2</h2>
<blockquote>
<p>[!IMPORTANT]
As of <code>v3</code> this action has been superceded by <code>gradle/actions/setup-gradle</code>.
Any workflow that uses <code>gradle/gradle-build-action@v3</code> will transparently delegate to <code>gradle/actions/setup-gradle@v3</code>.</p>
<p>Users are encouraged to update their workflows, replacing:</p>
<pre><code>uses: gradle/gradle-build-action@v3
</code></pre>
<p>with</p>
<pre><code>uses: gradle/actions/setup-gradle@v3
</code></pre>
<p>See the <a href="https://github.com/gradle/actions/tree/main/setup-gradle">setup-gradle documentation</a> for up-to-date documentation for <code>gradle/actions/setup-gradle</code>.</p>
</blockquote>
<p>For release details, see <a href="https://github.com/gradle/actions/releases/tag/v3.3.2">https://github.com/gradle/actions/releases/tag/v3.3.2</a></p>
<h2>v3.3.1</h2>
<blockquote>
<p>[!IMPORTANT]
As of <code>v3</code> this action has been superceded by <code>gradle/actions/setup-gradle</code>.
Any workflow that uses <code>gradle/gradle-build-action@v3</code> will transparently delegate to <code>gradle/actions/setup-gradle@v3</code>.</p>
<p>Users are encouraged to update their workflows, replacing:</p>
<pre><code>uses: gradle/gradle-build-action@v3
</code></pre>
<p>with</p>
<pre><code>uses: gradle/actions/setup-gradle@v3
</code></pre>
<p>See the <a href="https://github.com/gradle/actions/tree/main/setup-gradle">setup-gradle documentation</a> for up-to-date documentation for <code>gradle/actions/setup-gradle</code>.</p>
</blockquote>
<p>For release details, see <a href="https://github.com/gradle/actions/releases/tag/v3.3.1">https://github.com/gradle/actions/releases/tag/v3.3.1</a></p>
<h2>v3.3.0</h2>
<blockquote>
<p>[!IMPORTANT]
As of <code>v3</code> this action has been superceded by <code>gradle/actions/setup-gradle</code>.
Any workflow that uses <code>gradle/gradle-build-action@v3</code> will transparently delegate to <code>gradle/actions/setup-gradle@v3</code>.</p>
<p>Users are encouraged to update their workflows, replacing:</p>
<pre><code>uses: gradle/gradle-build-action@v3
</code></pre>
<p>with</p>
<pre><code></code></pre>
</blockquote>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gradle/gradle-build-action/commit/4c39dd82cd5e1ec7c6fa0173bb41b4b6bb3b86ff"><code>4c39dd8</code></a> Bump to v3.3.2</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/e2097ccd7e8ed48671dc068ac4efa86d25745b39"><code>e2097cc</code></a> Bump to use v3.3.1</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8baac4c8ef753599f92eeb509c246d09d6250fa6"><code>8baac4c</code></a> Map setup-gradle outputs back to gradle-build-action</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/595fa85721f407447040bb9c9976254d88ad793d"><code>595fa85</code></a> Run quick-check on main</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/f02f491d0d40a7ae88c67d3eaf2f3aa55c60a27b"><code>f02f491</code></a> Update action.yml for setup-gradle@v3.3.0</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/cb6e43f18001186272630908bb44a8246d3df780"><code>cb6e43f</code></a> Emit correct deprecation warnings in setup-gradle</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/bdf99f9dada2506e990bac6de8ec5e3de34a04f1"><code>bdf99f9</code></a> Update action.yml for v3.2.1</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/fe59895742b4f984530980e4f693943577526b61"><code>fe59895</code></a> Disable dependabot for this repo</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/928891f9d83ac8e366d29011d0d8406343d1e19b"><code>928891f</code></a> Update action.yml for v3.2.0</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/942d5e1456472d289f4b112fd3b62244067bac9c"><code>942d5e1</code></a> Bump Gradle Wrapper from 8.6 to 8.7 in /.github/workflow-samples</li>
<li>Additional commits viewable in <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v3.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gradle/gradle-build-action&package-manager=github_actions&previous-version=2.3.3&new-version=3.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 05:59:18 +0000 UTC
    </div>
</div>

