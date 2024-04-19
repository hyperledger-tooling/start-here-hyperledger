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
                PR <a href="https://github.com/hyperledger/iroha-java/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    Bump org.gradle.toolchains.foojay-resolver-convention from 0.5.0 to 0.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps org.gradle.toolchains.foojay-resolver-convention from 0.5.0 to 0.8.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.gradle.toolchains.foojay-resolver-convention&package-manager=gradle&previous-version=0.5.0&new-version=0.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-19 11:36:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    Bump gradle/gradle-build-action from 2.3.3 to 3.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [gradle/gradle-build-action](https://github.com/gradle/gradle-build-action) from 2.3.3 to 3.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gradle/gradle-build-action/releases">gradle/gradle-build-action's releases</a>.</em></p>
<blockquote>
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
<pre><code>uses: gradle/actions/setup-gradle@v3
</code></pre>
<p>See the <a href="https://github.com/gradle/actions/tree/main/setup-gradle">setup-gradle documentation</a> for up-to-date documentation for <code>gradle/actions/setup-gradle</code>.</p>
</blockquote>
<p>For release details, see <a href="https://github.com/gradle/actions/releases/tag/v3.3.0">https://github.com/gradle/actions/releases/tag/v3.3.0</a></p>
<h2>v3.2.1</h2>
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
<li><a href="https://github.com/gradle/gradle-build-action/commit/e2097ccd7e8ed48671dc068ac4efa86d25745b39"><code>e2097cc</code></a> Bump to use v3.3.1</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8baac4c8ef753599f92eeb509c246d09d6250fa6"><code>8baac4c</code></a> Map setup-gradle outputs back to gradle-build-action</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/595fa85721f407447040bb9c9976254d88ad793d"><code>595fa85</code></a> Run quick-check on main</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/f02f491d0d40a7ae88c67d3eaf2f3aa55c60a27b"><code>f02f491</code></a> Update action.yml for setup-gradle@v3.3.0</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/cb6e43f18001186272630908bb44a8246d3df780"><code>cb6e43f</code></a> Emit correct deprecation warnings in setup-gradle</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/bdf99f9dada2506e990bac6de8ec5e3de34a04f1"><code>bdf99f9</code></a> Update action.yml for v3.2.1</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/fe59895742b4f984530980e4f693943577526b61"><code>fe59895</code></a> Disable dependabot for this repo</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/928891f9d83ac8e366d29011d0d8406343d1e19b"><code>928891f</code></a> Update action.yml for v3.2.0</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/942d5e1456472d289f4b112fd3b62244067bac9c"><code>942d5e1</code></a> Bump Gradle Wrapper from 8.6 to 8.7 in /.github/workflow-samples</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/2bd30acc50398ddb4c24deba4f10013f9672b8ef"><code>2bd30ac</code></a> Bump org.junit.jupiter:junit-jupiter</li>
<li>Additional commits viewable in <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v3.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gradle/gradle-build-action&package-manager=github_actions&previous-version=2.3.3&new-version=3.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-19 11:36:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    Bump com.github.docker-java:docker-java from 3.3.0 to 3.3.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [com.github.docker-java:docker-java](https://github.com/docker-java/docker-java) from 3.3.0 to 3.3.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker-java/docker-java/releases">com.github.docker-java:docker-java's releases</a>.</em></p>
<blockquote>
<h2>3.3.6</h2>
<h2>Changes</h2>
<ul>
<li>Test against Java 21 <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2304">#2304</a>)</li>
<li>Update actions/checkout and actions/setup-java version to v4 <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2309">#2309</a>)</li>
</ul>
<h2>📈 Enhancements</h2>
<ul>
<li>Add <code>Runtimes</code> to <code>Info</code> response <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2311">#2311</a>)</li>
</ul>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Remove exclusion and fix httpclient5 compatibility <a href="https://github.com/Sineaggi"><code>@​Sineaggi</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2294">#2294</a>)</li>
<li>If BuildImage fails but logs something about success, don't succeed <a href="https://github.com/niloc132"><code>@​niloc132</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2305">#2305</a>)</li>
</ul>
<h2>3.3.5</h2>
<h2>Changes</h2>
<ul>
<li>Ignore LogSwarmObjectIT#testLogsCmd <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2280">#2280</a>)</li>
</ul>
<h2>📈 Enhancements</h2>
<ul>
<li>Add missing states in ServiceUpdateState <a href="https://github.com/Nowheresly"><code>@​Nowheresly</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2292">#2292</a>)</li>
<li>Add StartInterval to health check since it will be supported by the 1.44 docker API <a href="https://github.com/henri-tremblay"><code>@​henri-tremblay</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2244">#2244</a>)</li>
</ul>
<h2>🧰 Maintenance</h2>
<ul>
<li>Enable japicmp in docker-java-api module <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2279">#2279</a>)</li>
</ul>
<h2>3.3.4</h2>
<h2>Changes</h2>
<ul>
<li>Bump org.testcontainers:testcontainers from 1.16.3 to 1.19.1 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2218">#2218</a>)</li>
<li>Bump com.github.siom79.japicmp:japicmp-maven-plugin from 0.15.4 to 0.18.2 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2226">#2226</a>)</li>
<li>Add units (nanoseconds) to HealthCheck. <a href="https://github.com/SLG"><code>@​SLG</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2187">#2187</a>)</li>
<li>Disable CopyArchiveToContainerCmdIT#copyFileWithUIDGID <a href="https://github.com/eddumelendez"><code>@​eddumelendez</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2228">#2228</a>)</li>
<li>Bump assertj-core from 3.22.0 to 3.24.2 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2051">#2051</a>)</li>
<li>Bump jna from 5.12.1 to 5.13.0 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2047">#2047</a>)</li>
<li>Bump commons-io from 2.6 to 2.13.0 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2153">#2153</a>)</li>
<li>Bump org.junit.jupiter:junit-jupiter from 5.7.2 to 5.10.0 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2163">#2163</a>)</li>
<li>Bump org.bouncycastle:bcpkix-jdk18on from 1.75 to 1.76 <a href="https://github.com/dependabot"><code>@​dependabot</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2169">#2169</a>)</li>
</ul>
<h2>📈 Enhancements</h2>
<ul>
<li>Add signal query argument for Restart Container command <a href="https://github.com/dmmax"><code>@​dmmax</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2186">#2186</a>)</li>
<li>Implemented the <code>SizeRw</code> field in the <code>InspectContainerResponse</code> class. <a href="https://github.com/LarsSven"><code>@​LarsSven</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2216">#2216</a>)</li>
</ul>
<h2>🧰 Maintenance</h2>
<ul>
<li>Improve assertions <a href="https://github.com/Sineaggi"><code>@​Sineaggi</code></a> (<a href="https://redirect.github.com/docker-java/docker-java/issues/2189">#2189</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker-java/docker-java/commit/b29527510d9f7c16b30b138ae4a2f6703d88bb01"><code>b295275</code></a> Add <code>Runtimes</code> to <code>Info</code> response (<a href="https://redirect.github.com/docker-java/docker-java/issues/2311">#2311</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/4f6c5937983ff4ae7cc82bead44afe3afee4d0ed"><code>4f6c593</code></a> Test against Java 21 (<a href="https://redirect.github.com/docker-java/docker-java/issues/2304">#2304</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/3514b3ba9c6d938e2a0435ad8d84905cb1cdfed1"><code>3514b3b</code></a> Remove exclusion and fix httpclient5 compatibility (<a href="https://redirect.github.com/docker-java/docker-java/issues/2294">#2294</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/4d8c436d6cbe312be22b157c3ebdb6eb973140ae"><code>4d8c436</code></a> If BuildImage fails but logs something about success, don't succeed (<a href="https://redirect.github.com/docker-java/docker-java/issues/2305">#2305</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/129f7868a0463bad09f74dcfb26391b224be6784"><code>129f786</code></a> Update actions/checkout and actions/setup-java version to v4 (<a href="https://redirect.github.com/docker-java/docker-java/issues/2309">#2309</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/1bac81fa0afdae18d30bd62b1ba666375ee20147"><code>1bac81f</code></a> Add missing states in ServiceUpdateState (<a href="https://redirect.github.com/docker-java/docker-java/issues/2292">#2292</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/7957a142809184817483aaebd2eb03398f0e6394"><code>7957a14</code></a> Add StartInterval to health check since it will be supported by the 1.44 dock...</li>
<li><a href="https://github.com/docker-java/docker-java/commit/1c6fcdbce655bc60c5fe291465809934b1b4ac76"><code>1c6fcdb</code></a> Enable japicmp in docker-java-api module (<a href="https://redirect.github.com/docker-java/docker-java/issues/2279">#2279</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/b56497a01b50aaacb73cb34aa8de9f2d2fb0f780"><code>b56497a</code></a> Ignore LogSwarmObjectIT#testLogsCmd (<a href="https://redirect.github.com/docker-java/docker-java/issues/2280">#2280</a>)</li>
<li><a href="https://github.com/docker-java/docker-java/commit/84d7750d7f290c66f0ae18c88ab92a3cde2c804d"><code>84d7750</code></a> Use long rather than int for sizeRw and sizeRootFs (<a href="https://redirect.github.com/docker-java/docker-java/issues/2230">#2230</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/docker-java/docker-java/compare/3.3.0...3.3.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.github.docker-java:docker-java&package-manager=gradle&previous-version=3.3.0&new-version=3.3.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-19 11:36:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    Bump actions/cache from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/cache](https://github.com/actions/cache) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/releases">actions/cache's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update action to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li>feat: save-always flag by <a href="https://github.com/to-s"><code>@​to-s</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li><a href="https://github.com/to-s"><code>@​to-s</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v4.0.0">https://github.com/actions/cache/compare/v3...v4.0.0</a></p>
<h2>v3.3.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Cache v3.3.3 by <a href="https://github.com/robherley"><code>@​robherley</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/robherley"><code>@​robherley</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.3">https://github.com/actions/cache/compare/v3...v3.3.3</a></p>
<h2>v3.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed readme with new segment timeout values by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1133">actions/cache#1133</a></li>
<li>Readme fixes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1134">actions/cache#1134</a></li>
<li>Updated description of the lookup-only input for main action by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1130">actions/cache#1130</a></li>
<li>Change two new actions mention as quoted text by <a href="https://github.com/bishal-pdMSFT"><code>@​bishal-pdMSFT</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1131">actions/cache#1131</a></li>
<li>Update Cross-OS Caching tips by <a href="https://github.com/pdotl"><code>@​pdotl</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1122">actions/cache#1122</a></li>
<li>Bazel example (Take <a href="https://redirect.github.com/actions/cache/issues/2">#2</a>️⃣) by <a href="https://github.com/vorburger"><code>@​vorburger</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li>Remove actions to add new PRs and issues to a project board by <a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li>Consume latest toolkit and fix dangling promise bug by <a href="https://github.com/chkimes"><code>@​chkimes</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li>Bump action version to 3.3.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vorburger"><code>@​vorburger</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li><a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li><a href="https://github.com/chkimes"><code>@​chkimes</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li><a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.2">https://github.com/actions/cache/compare/v3...v3.3.2</a></p>
<h2>v3.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Reduced download segment size to 128 MB and timeout to 10 minutes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1129">actions/cache#1129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.1">https://github.com/actions/cache/compare/v3...v3.3.1</a></p>
<h2>v3.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bug: Permission is missing in cache delete example by <a href="https://github.com/kotokaze"><code>@​kotokaze</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1123">actions/cache#1123</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/blob/main/RELEASES.md">actions/cache's changelog</a>.</em></p>
<blockquote>
<h1>Releases</h1>
<h3>4.0.2</h3>
<ul>
<li>Fixed restore <code>fail-on-cache-miss</code> not working.</li>
</ul>
<h3>4.0.1</h3>
<ul>
<li>Updated <code>isGhes</code> check</li>
</ul>
<h3>4.0.0</h3>
<ul>
<li>Updated minimum runner version support from node 12 -&gt; node 20</li>
</ul>
<h3>3.3.3</h3>
<ul>
<li>Updates <code>@​actions/cache</code> to v3.2.3 to fix accidental mutated path arguments to <code>getCacheVersion</code> <a href="https://redirect.github.com/actions/toolkit/pull/1378">actions/toolkit#1378</a></li>
<li>Additional audit fixes of npm package(s)</li>
</ul>
<h3>3.3.2</h3>
<ul>
<li>Fixes bug with Azure SDK causing blob downloads to get stuck.</li>
</ul>
<h3>3.3.1</h3>
<ul>
<li>Reduced segment size to 128MB and segment timeout to 10 minutes to fail fast in case the cache download is stuck.</li>
</ul>
<h3>3.3.0</h3>
<ul>
<li>Added option to lookup cache without downloading it.</li>
</ul>
<h3>3.2.6</h3>
<ul>
<li>Fix zstd not being used after zstd version upgrade to 1.5.4 on hosted runners.</li>
</ul>
<h3>3.2.5</h3>
<ul>
<li>Added fix to prevent from setting MYSYS environment variable globally.</li>
</ul>
<h3>3.2.4</h3>
<ul>
<li>Added option to fail job on cache miss.</li>
</ul>
<h3>3.2.3</h3>
<ul>
<li>Support cross os caching on Windows as an opt-in feature.</li>
<li>Fix issue with symlink restoration on Windows for cross-os caches.</li>
</ul>
<h3>3.2.2</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/cache/commit/0c45773b623bea8c8e75f6c82b208c3cf94ea4f9"><code>0c45773</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1327">#1327</a> from cdce8p/fix-fail-on-cache-miss</li>
<li><a href="https://github.com/actions/cache/commit/8a55f839aa4b4578e47bdc8a52828637cbb9a454"><code>8a55f83</code></a> Add test case for process exit</li>
<li><a href="https://github.com/actions/cache/commit/3884cace147bdf9307fcc52a277f421af7b30798"><code>3884cac</code></a> Bump version</li>
<li><a href="https://github.com/actions/cache/commit/e29dad3e36390db18fc19fb666cb1302f4929002"><code>e29dad3</code></a> Fix fail-on-cache-miss not working</li>
<li><a href="https://github.com/actions/cache/commit/ab5e6d0c87105b4c9c2047343972218f562e4319"><code>ab5e6d0</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1341">#1341</a> from bethanyj28/main</li>
<li><a href="https://github.com/actions/cache/commit/89c7d86c71006451e399dfcc588eed8e392e0dcf"><code>89c7d86</code></a> licensed cache</li>
<li><a href="https://github.com/actions/cache/commit/d2c84da363007d814e47d50565ba3794c1a84c56"><code>d2c84da</code></a> update <code>@​actions/cache</code></li>
<li><a href="https://github.com/actions/cache/commit/37e7d4eb166540050942d75a6e40742cbfc92f65"><code>37e7d4e</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1340">#1340</a> from actions/bethanyj28/update-publish-flow</li>
<li><a href="https://github.com/actions/cache/commit/a18323f50430a57f9094db3ce508dc1e3a25d4a2"><code>a18323f</code></a> add release action</li>
<li><a href="https://github.com/actions/cache/commit/a2ed59d39b352305bdd2f628719a53b2cc4f9613"><code>a2ed59d</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1305">#1305</a> from actions/yacaovsnc/update_examples</li>
<li>Additional commits viewable in <a href="https://github.com/actions/cache/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/cache&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-19 11:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    feature: update Iroha image version, recompiled executor and nft smart contract, added test for trigger metadata update event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update Iroha image version, recompiled executor and nft smart contract, added test for trigger metadata update event
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 09:56:33 +0000 UTC
    </div>
</div>

