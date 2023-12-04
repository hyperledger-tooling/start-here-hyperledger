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
                PR <a href="https://github.com/hyperledger/iroha-java/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    Bump gradle/gradle-build-action from 2.3.3 to 2.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [gradle/gradle-build-action](https://github.com/gradle/gradle-build-action) from 2.3.3 to 2.10.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gradle/gradle-build-action/releases">gradle/gradle-build-action's releases</a>.</em></p>
<blockquote>
<h2>v2.10.0</h2>
<p>This release introduces a new <code>artifact-retention-days</code> parameter, which allows a user to configure how long the generated dependency-graph artifacts are retained by GitHub Actions. Adjusting the retention period can be useful to reduce storage costs associated with these dependency-graph artifacts.</p>
<p>See <a href="https://github.com/gradle/gradle-build-action/tree/v2.10.0#reducing-storage-costs-for-saved-dependency-graph-artifacts">the documentation</a> for more details.</p>
<h3>Changelog</h3>
<ul>
<li>[NEW] Add <code>artifact-retention-days</code> configuration parameter <a href="https://redirect.github.com/gradle/gradle-build-action/issues/903">#903</a></li>
<li>[FIX] Update to <code>v1.0.0</code> of the <a href="https://plugins.gradle.org/plugin/org.gradle.github-dependency-graph-gradle-plugin">github-dependency-graph-gradle-plugin</a></li>
<li>[FIX] Update <code>@babel/traverse</code> to address <a href="https://github.com/gradle/gradle-build-action/security/dependabot/18">reported security vulnerability</a></li>
</ul>
<p><strong>Full-changelog</strong>: <a href="https://github.com/gradle/gradle-build-action/compare/v2.9.0...v2.10.0">https://github.com/gradle/gradle-build-action/compare/v2.9.0...v2.10.0</a></p>
<h2>v2.9.0</h2>
<p>The GitHub <a href="https://github.com/actions/dependency-review-action">dependency-review-action</a> helps you understand dependency changes (and the security impact of these changes) for a pull request.  This release updates the GItHub Dependency Graph support to be compatible with the <code>dependency-review-action</code>.</p>
<p>See <a href="https://github.com/gradle/gradle-build-action#integrating-the-dependency-review-action">the documentation</a> for detailed examples.</p>
<h3>Changelog</h3>
<ul>
<li>[FIX] Use correct SHA for <code>pull-request</code> events <a href="https://redirect.github.com/gradle/gradle-build-action/issues/882">#882</a></li>
<li>[FIX] Avoid generating dependency graph during cache cleanup <a href="https://redirect.github.com/gradle/gradle-build-action/issues/905">#905</a></li>
<li>[NEW] Improve warning on failure to submit dependency graph</li>
<li>[NEW] Compatibility with GitHub <code>dependency-review-action</code> <a href="https://redirect.github.com/gradle/gradle-build-action/issues/879">#879</a></li>
</ul>
<p><strong>Full-changelog</strong>: <a href="https://github.com/gradle/gradle-build-action/compare/v2.8.1...v2.9.0">https://github.com/gradle/gradle-build-action/compare/v2.8.1...v2.9.0</a></p>
<h2>v2.8.1</h2>
<p>Fixes an issue that prevented Dependency Graph submission when running on GitHub Enterprise Server.</p>
<h3>Fixes</h3>
<ul>
<li>Incorrect endpoint used to submit Dependency Graph on GitHub Enterprise <a href="https://redirect.github.com/gradle/gradle-build-action/issues/885">#885</a></li>
</ul>
<h3>Changelog</h3>
<p><a href="https://github.com/gradle/gradle-build-action/compare/v2.8.0...v2.8.1">https://github.com/gradle/gradle-build-action/compare/v2.8.0...v2.8.1</a></p>
<h2>v2.8.0</h2>
<p>The <code>v2.8.0</code> release of the <code>gradle-build-action</code> introduces an easy mechanism to connect to Gradle Enterprise, as well improved support for self-hosted GitHub Actions runners.</p>
<h3>Automatic injection of Gradle Enterprise connectivity</h3>
<p>It is now possible to connect a Gradle build to Gradle Enterprise without changing any of the Gradle project sources. This is achieved through Gradle Enterprise injection, where an init-script will apply the Gradle Enterprise plugin and associated configuration.</p>
<p>This feature can be useful to easily trial Gradle Enterprise on a project, or to centralize Gradle Enterprise configuration for all GitHub Actions workflows in an organization.</p>
<p>See <a href="https://github.com/gradle/gradle-build-action/blob/v2.8.0/README.md#gradle-enterprise-plugin-injection">Gradle Enterprise injection in the README</a> for more info.</p>
<h3>Restore Gradle User Home when directory already exists</h3>
<p>Previously, the Gradle User Home would not be restored if the directory already exists. This wasn't normally an issue with GitHub-hosted runners, but limited the usefulness of the action for persistent, self-hosted runners.</p>
<p>This behaviour has been improved in this release:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gradle/gradle-build-action/commit/87a9a15658c426a54dd469d4fc7dc1a73ca9d4a6"><code>87a9a15</code></a> Use 1.0.0 release of dependency graph plugin</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/375481748bf6d66f045ed675f6ab9387068ab66d"><code>3754817</code></a> Document <code>artifact-retention-days</code></li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/beff1c573c6c87bb3019e1473532b0cf1b787294"><code>beff1c5</code></a> Update dev dependencies</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/21a3ebb55f18705a5107efdf3262ee1e0d8b0578"><code>21a3ebb</code></a> Bump com.fasterxml.jackson.dataformat:jackson-dataformat-smile</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/a5be560235445ae2ff8723c1a2e257667523ca20"><code>a5be560</code></a> Bump the github-actions group with 2 updates</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/9bca466e2722baf9e77b4f929bbe0af18848791f"><code>9bca466</code></a> Make artifact retention configurable</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/f757bcfd86afb75a4bf0a984b0f78fadcbd4314b"><code>f757bcf</code></a> Merge pull request <a href="https://redirect.github.com/gradle/gradle-build-action/issues/951">#951</a> from gradle/dd/v2.9.1</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8b6c211905d84dc9fc3c35be6f002fefea5f6b32"><code>8b6c211</code></a> Bump to RC of github dependency graph plugin</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8db1c7621b81b410d71791e19a472657eedb90c5"><code>8db1c76</code></a> Build outputs</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/6eaacfc06c91de3c8d1c6c5029412a8c6d80122f"><code>6eaacfc</code></a> Update NPM dependencies</li>
<li>Additional commits viewable in <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v2.10.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gradle/gradle-build-action&package-manager=github_actions&previous-version=2.3.3&new-version=2.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-04 06:04:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    Bump actions/setup-java from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-java](https://github.com/actions/setup-java) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-java/releases">actions/setup-java's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>In the scope of this release, the version of the Node.js runtime was updated to 20. The majority of dependencies were updated to the latest versions. From now on, the code for the setup-java will run on Node.js 20 instead of Node.js 16.</p>
<h2>Breaking changes</h2>
<ul>
<li>Update Node.js runtime to version 20 by <a href="https://github.com/aparnajyothi-y"><code>@​aparnajyothi-y</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/558">actions/setup-java#558</a></li>
</ul>
<h2>Non-breaking changes</h2>
<ul>
<li>Adding support for microsoft openjdk 21.0.0 by <a href="https://github.com/ralfstuckert"><code>@​ralfstuckert</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/546">actions/setup-java#546</a></li>
<li>Update <code>@​actions/cache</code> dependency and documentation by <a href="https://github.com/IvanZosimov"><code>@​IvanZosimov</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/549">actions/setup-java#549</a></li>
<li>Implementation of the cache-dependency-path option to control caching dependency by <a href="https://github.com/itchyny"><code>@​itchyny</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/499">actions/setup-java#499</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ralfstuckert"><code>@​ralfstuckert</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/546">actions/setup-java#546</a></li>
<li><a href="https://github.com/itchyny"><code>@​itchyny</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/499">actions/setup-java#499</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v3...v4.0.0">https://github.com/actions/setup-java/compare/v3...v4.0.0</a></p>
<h2>v3.13.0</h2>
<h2>What's changed</h2>
<p>In the scope of this release, support for Dragonwell JDK was added by <a href="https://github.com/Accelerator1996"><code>@​Accelerator1996</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/532">actions/setup-java#532</a></p>
<pre lang="yaml"><code>steps:
 - name: Checkout
   uses: actions/checkout@v3
 - name: Setup-java
   uses: actions/setup-java@v3
   with:
     distribution: 'dragonwell'
     java-version: '17'
</code></pre>
<p>Several inaccuracies were also fixed:</p>
<ul>
<li>Fix XML namespaces wrongly using https by <a href="https://github.com/gnodet"><code>@​gnodet</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/503">actions/setup-java#503</a></li>
<li>Fix typo and remove unintentional(?) word by <a href="https://github.com/CyberFlameGO"><code>@​CyberFlameGO</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/518">actions/setup-java#518</a></li>
<li>Fix usage link within the README.md file by <a href="https://github.com/dassiorleando"><code>@​dassiorleando</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/525">actions/setup-java#525</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/CyberFlameGO"><code>@​CyberFlameGO</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/518">actions/setup-java#518</a></li>
<li><a href="https://github.com/dassiorleando"><code>@​dassiorleando</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/525">actions/setup-java#525</a></li>
<li><a href="https://github.com/gnodet"><code>@​gnodet</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/503">actions/setup-java#503</a></li>
<li><a href="https://github.com/Accelerator1996"><code>@​Accelerator1996</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/532">actions/setup-java#532</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v3...v3.13.0">https://github.com/actions/setup-java/compare/v3...v3.13.0</a></p>
<h2>v3.12.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-java/commit/387ac29b308b003ca37ba93a6cab5eb57c8f5f93"><code>387ac29</code></a> Upgrade Node to v20 (<a href="https://redirect.github.com/actions/setup-java/issues/558">#558</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/9eda6b51cc4f6ee99be3dd5537b85e389e47bda9"><code>9eda6b5</code></a> feat: implement cache-dependency-path option to control caching dependency (#...</li>
<li><a href="https://github.com/actions/setup-java/commit/78078da0cd035d0d177cc2cb696e05d96fba7d11"><code>78078da</code></a> Update <code>@​actions/cache</code> dependency and documentation (<a href="https://redirect.github.com/actions/setup-java/issues/549">#549</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/5caaba646e214abb5c4c808eb8fe13db519ab757"><code>5caaba6</code></a> add support for microsoft openjdk 21.0.0 (<a href="https://redirect.github.com/actions/setup-java/issues/546">#546</a>)</li>
<li>See full diff in <a href="https://github.com/actions/setup-java/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-java&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-04 06:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Bugfixing numeric serialize
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
        Created At 2023-12-01 09:32:14 +0000 UTC
    </div>
</div>

