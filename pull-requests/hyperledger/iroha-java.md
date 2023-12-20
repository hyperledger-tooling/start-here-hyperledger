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
                PR <a href="https://github.com/hyperledger/iroha-java/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    Bump gradle/gradle-build-action from 2.3.3 to 2.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [gradle/gradle-build-action](https://github.com/gradle/gradle-build-action) from 2.3.3 to 2.11.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gradle/gradle-build-action/releases">gradle/gradle-build-action's releases</a>.</em></p>
<blockquote>
<h2>v2.11.0</h2>
<p>In addition to a number of dependency updates, this release:</p>
<ul>
<li>Allows a custom Plugin Repository to be specified when resolving the <a href="https://plugins.gradle.org/plugin/org.gradle.github-dependency-graph-gradle-plugin">github-dependency-graph-gradle-plugin</a>. See <a href="https://github.com/gradle/gradle-build-action#using-a-custom-plugin-repository">the documentation</a> for details.</li>
<li>Brings increased resilience when failures occur collecting build results or cleaning the Gradle User Home. Such failures should no longer prevent the caching of Gradle User Home or lead to build failures.</li>
</ul>
<h3>Changelog</h3>
<ul>
<li>[NEW] Allow a custom plugin repository to be used to resolve dependency-graph plugin <a href="https://redirect.github.com/gradle/gradle-build-action/issues/933">#933</a></li>
<li>[FIX] Cache entries and Job Summary not written on cache-cleanup failure <a href="https://redirect.github.com/gradle/gradle-build-action/issues/990">#990</a> <a href="https://redirect.github.com/gradle/gradle-build-action/issues/858">#858</a></li>
<li>[FIX] Failure to write build results file should not cause overall build to fail <a href="https://redirect.github.com/gradle/gradle-build-action/issues/866">#866</a></li>
</ul>
<p><strong>Full-changelog</strong>: <a href="https://github.com/gradle/gradle-build-action/compare/v2.10.0...v2.11.0">https://github.com/gradle/gradle-build-action/compare/v2.10.0...v2.11.0</a></p>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8cbcb9948b5892387aed077daf6f90e1f0ba5b27"><code>8cbcb99</code></a> Plugin repository URL is configurable</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/a71aff6a12dc717483196ae40080f41808faea40"><code>a71aff6</code></a> Handle failure in cache-cleanup</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/77699bae74fcfcf7dbe2095af457475d9cb6e9f4"><code>77699ba</code></a> Handle failure writing build-results file</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/dc5927259fdde73189c645eb5874c73b80ed8d5f"><code>dc59272</code></a> Merge branch 'dd/dependency-updates'</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/4f0075d967f5e96afd7bb359e1fd6161ad68e322"><code>4f0075d</code></a> Clarify docs for dedicated workflow</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/e1f9864a520782a0a40b9e595c69efea82417765"><code>e1f9864</code></a> Bumps the npm-dependencies group with 5 updates:</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/76d5a9b4755519a89d3dc8f7824b605c78cd7be5"><code>76d5a9b</code></a> Bump the github-actions group with 2 updates</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/39d8c6d06e2a0574353b820fe0958a4168fa8a5f"><code>39d8c6d</code></a> Bump from Gradle 8.4 to Gradle 8.5</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/0280eb7de5ad3fb0deb50017b8ce842980b4789a"><code>0280eb7</code></a> docs: upload build reports even when build failed</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/87a9a15658c426a54dd469d4fc7dc1a73ca9d4a6"><code>87a9a15</code></a> Use 1.0.0 release of dependency graph plugin</li>
<li>Additional commits viewable in <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v2.11.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gradle/gradle-build-action&package-manager=github_actions&previous-version=2.3.3&new-version=2.11.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-18 05:20:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    Bump actions/upload-artifact from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>The release of upload-artifact@v4 and download-artifact@v4 are major changes to the backend architecture of Artifacts. They have numerous performance and behavioral improvements.</p>
<p>For more information, see the <a href="https://github.com/actions/toolkit/tree/main/packages/artifact"><code>@​actions/artifact</code></a> documentation.</p>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vmjoseph"><code>@​vmjoseph</code></a> made their first contribution in <a href="https://redirect.github.com/actions/upload-artifact/pull/464">actions/upload-artifact#464</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v4.0.0">https://github.com/actions/upload-artifact/compare/v3...v4.0.0</a></p>
<h2>v3.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(github): remove trailing whitespaces by <a href="https://github.com/ljmf00"><code>@​ljmf00</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/313">actions/upload-artifact#313</a></li>
<li>Bump <code>@​actions/artifact</code> version to v1.1.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/436">actions/upload-artifact#436</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v3.1.3">https://github.com/actions/upload-artifact/compare/v3...v3.1.3</a></p>
<h2>v3.1.2</h2>
<ul>
<li>Update all <code>@actions/*</code> NPM packages to their latest versions- <a href="https://redirect.github.com/actions/upload-artifact/issues/374">#374</a></li>
<li>Update all dev dependencies to their most recent versions - <a href="https://redirect.github.com/actions/upload-artifact/issues/375">#375</a></li>
</ul>
<h2>v3.1.1</h2>
<ul>
<li>Update actions/core package to latest version to remove <code>set-output</code> deprecation warning <a href="https://redirect.github.com/actions/upload-artifact/issues/351">#351</a></li>
</ul>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​actions/artifact</code> to v1.1.0 (<a href="https://redirect.github.com/actions/upload-artifact/pull/327">actions/upload-artifact#327</a>)
<ul>
<li>Adds checksum headers on artifact upload (<a href="https://redirect.github.com/actions/toolkit/pull/1095">actions/toolkit#1095</a>) (<a href="https://redirect.github.com/actions/toolkit/pull/1063">actions/toolkit#1063</a>)</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/c7d193f32edcb7bfad88892161225aeda64e9392"><code>c7d193f</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/466">#466</a> from actions/v4-beta</li>
<li><a href="https://github.com/actions/upload-artifact/commit/13131bb095770b4070a7477c3cd2d96e1c16d9f4"><code>13131bb</code></a> licensed cache</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4a6c273b9834f66a1d05c170dc3f80f9cdb9def1"><code>4a6c273</code></a> Merge branch 'main' into v4-beta</li>
<li><a href="https://github.com/actions/upload-artifact/commit/f391bb91a3d3118aeca171c365bb319ece276b37"><code>f391bb9</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/465">#465</a> from actions/robherley/v4-documentation</li>
<li><a href="https://github.com/actions/upload-artifact/commit/9653d03c4b74c32144e02dae644fea70e079d4b3"><code>9653d03</code></a> Apply suggestions from code review</li>
<li><a href="https://github.com/actions/upload-artifact/commit/875b63076402f25ef9d52c294c86ba4f97810575"><code>875b630</code></a> add limitations section</li>
<li><a href="https://github.com/actions/upload-artifact/commit/ecb21463e93740a6be75c3116242169bfdbcb15a"><code>ecb2146</code></a> add compression example</li>
<li><a href="https://github.com/actions/upload-artifact/commit/5e7604f84a055838f64ed68bb9904751523081ae"><code>5e7604f</code></a> trim some repeated info</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d6437d07581fe318a364512e6cf6b1dca6b4f92c"><code>d6437d0</code></a> naming</li>
<li><a href="https://github.com/actions/upload-artifact/commit/1b561557037b4957d7d184e9aac02bec86c771eb"><code>1b56155</code></a> s/v4-beta/v4/g</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/upload-artifact&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-18 05:20:42 +0000 UTC
    </div>
</div>

