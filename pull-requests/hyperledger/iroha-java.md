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
                PR <a href="https://github.com/hyperledger/iroha-java/pull/386" class=".btn">#386</a>
            </td>
            <td>
                <b>
                    Bump gradle/gradle-build-action from 2.3.3 to 2.4.2 in /.github/workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [gradle/gradle-build-action](https://github.com/gradle/gradle-build-action) from 2.3.3 to 2.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gradle/gradle-build-action/releases">gradle/gradle-build-action's releases</a>.</em></p>
<blockquote>
<h2>v2.4.2</h2>
<p>This release disables the save/restore of configuration-cache data, since this functionality has been shown to be problematic.
Gradle 8.1 has made changes to this functionality which will require a more comprehensive rework of the action before we can re-enable this.</p>
<h2>v2.4.1</h2>
<p>This patch release updates a number of dependencies, including <code>xmljs</code> which was reported to have a security vulnerability (<a href="https://nvd.nist.gov/vuln/detail/CVE-2023-0842">https://nvd.nist.gov/vuln/detail/CVE-2023-0842</a>).
There is no evidence that this vulnerability affected the <code>gradle-build-action</code>.</p>
<p><strong>Full changelog</strong>: <a href="https://github.com/gradle/gradle-build-action/compare/v2.4.0...v2.4.1">https://github.com/gradle/gradle-build-action/compare/v2.4.0...v2.4.1</a></p>
<h2>v2.4.0</h2>
<h2>What's new</h2>
<p>The <code>v.2.4.0</code> release contains various library updates and fixes to fully support Gradle 8.</p>
<p>Notable changes:</p>
<ul>
<li>Update to <code>@actions/cache: 3.1.3</code> should improve cache save/restore performance on Windows by using gnu tar and zstd when available.</li>
<li>Fix caching of extracted JDK toolchains for Gradle 7.6+ (e4446473950007d0d0323adeed9f992824618be9)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v2.4.0">https://github.com/gradle/gradle-build-action/compare/v2.3.3...v2.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gradle/gradle-build-action/commit/749f47bda3e44aa060e82d7b3ef7e40d953bd629"><code>749f47b</code></a> Update README.md for changes in release</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/eb126d771e2fad56aea2b224b1764ca712b41ce9"><code>eb126d7</code></a> Update for Gradle 8.1 release</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/5056fa9d50478a14af3c9925c12ca02318659d3e"><code>5056fa9</code></a> Patch <code>@​azure/logger</code> to address CodeQL violations</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/8a0051ffb29295bbf97779cf17b74f44cae97fdf"><code>8a0051f</code></a> Specify current Gradle version via ASDF</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/4f87177da051d58a8dc3ec108795fc0637008161"><code>4f87177</code></a> Build outputs</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/ff6294699860ad3ec1ac4b1cf1c535495ea623d5"><code>ff62946</code></a> Update development dependencies</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/2eddd207d622bc55228cd4943b0116075ed768ea"><code>2eddd20</code></a> Bump xml2js, <code>@​azure/ms-rest-js</code> and <code>@​azure/core-http</code></li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/887e0bda35d667c5e52556fedb21d18fe62fca93"><code>887e0bd</code></a> Fix typo (<a href="https://redirect.github.com/gradle/gradle-build-action/issues/655">#655</a>)</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/dac0b87334f7d76ec53693bb72cf7fe06c9515be"><code>dac0b87</code></a> Bump <code>@​typescript-eslint/parser</code> from 5.56.0 to 5.57.0 (<a href="https://redirect.github.com/gradle/gradle-build-action/issues/654">#654</a>)</li>
<li><a href="https://github.com/gradle/gradle-build-action/commit/a8f0f0d523dc65b8b1c498d552cb13949dfbc8c9"><code>a8f0f0d</code></a> NPM dependency updates</li>
<li>Additional commits viewable in <a href="https://github.com/gradle/gradle-build-action/compare/v2.3.3...v2.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gradle/gradle-build-action&package-manager=github_actions&previous-version=2.3.3&new-version=2.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 12:17:33 +0000 UTC
    </div>
</div>

