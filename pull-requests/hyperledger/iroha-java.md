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
                PR <a href="https://github.com/hyperledger/iroha-java/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Bump gradle/gradle-build-action from 2.3.3 to 2.11.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [gradle/gradle-build-action](https://github.com/gradle/gradle-build-action) from 2.3.3 to 2.11.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gradle/gradle-build-action/releases">gradle/gradle-build-action's releases</a>.</em></p>
<blockquote>
<h2>v2.11.1</h2>
<p>This patch release fixes an issue that prevented the <code>gradle-build-action</code> from executing with Gradle 1.12, and improves error reporting for dependency submission failures.</p>
<h3>Changelog</h3>
<ul>
<li>[FIX] Poor error reporting for dependency-submission failure <a href="https://redirect.github.com/gradle/gradle-build-action/issues/1008">#1008</a></li>
<li>[FIX] Error with gradle-build-action v2.11.0 and Gradle 1.12: unable to resolve class PluginManager <a href="https://redirect.github.com/gradle/gradle-build-action/issues/1007">#1007</a></li>
</ul>
<p><strong>Full-changelog</strong>: <a href="https://github.com/gradle/gradle-build-action/compare/v2.11.0...v2.11.1">https://github.com/gradle/gradle-build-action/compare/v2.11.0...v2.11.1</a></p>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gradle/gradle-build-action/commit/982da8e78c05368c70dac0351bb82647a9e9a5d2"><code>982da8e</code></a> Attempt to make init-script compatible with Gradle 1.12</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/a0fc8606d24d4f5b643362f5342396929b656e05"><code>a0fc860</code></a> Build outputs</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/a1980784de3397bb0ae047a357871ec28d15395a"><code>a198078</code></a> Improve reporting for dependency-graph failure</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/f95e9c74599bc49122b76ecfe1306f0034f87266"><code>f95e9c7</code></a> Clarify dependency-graph example</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8cbcb9948b5892387aed077daf6f90e1f0ba5b27"><code>8cbcb99</code></a> Plugin repository URL is configurable</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/a71aff6a12dc717483196ae40080f41808faea40"><code>a71aff6</code></a> Handle failure in cache-cleanup</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/77699bae74fcfcf7dbe2095af457475d9cb6e9f4"><code>77699ba</code></a> Handle failure writing build-results file</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/dc5927259fdde73189c645eb5874c73b80ed8d5f"><code>dc59272</code></a> Merge branch 'dd/dependency-updates'</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/4f0075d967f5e96afd7bb359e1fd6161ad68e322"><code>4f0075d</code></a> Clarify docs for dedicated workflow</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/e1f9864a520782a0a40b9e595c69efea82417765"><code>e1f9864</code></a> Bumps the npm-dependencies group with 5 updates:</li>
<li>Additional commits viewable in <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v2.11.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gradle/gradle-build-action&package-manager=github_actions&previous-version=2.3.3&new-version=2.11.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-12-25 05:38:44 +0000 UTC
    </div>
</div>

