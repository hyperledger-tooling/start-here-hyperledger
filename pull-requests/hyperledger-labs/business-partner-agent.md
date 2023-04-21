---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/863" class=".btn">#863</a>
            </td>
            <td>
                <b>
                    Bump smartsquaregmbh/delete-old-packages from 0.6.0 to 0.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [smartsquaregmbh/delete-old-packages](https://github.com/smartsquaregmbh/delete-old-packages) from 0.6.0 to 0.7.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/smartsquaregmbh/delete-old-packages/releases">smartsquaregmbh/delete-old-packages's releases</a>.</em></p>
<blockquote>
<h2>v0.7.0</h2>
<h4>:warning: This release includes breaking changes!</h4>
<p>This release features a larger rework of the internal GitHub API usage. Previously, either the REST API or the GraphQL API was used, based on the input parameters. Since the needed functionally has been removed from the GraphQL API, we now exclusively use the REST API. See the updated README for an overview.</p>
<ul>
<li><em>Breaking</em>: The <code>type</code> input is required now.</li>
<li><em>Breaking</em>: Removal of the <code>repo</code>/<code>owner</code> strategy. The API does not support it anymore, all packages need to be either organization or user bound.</li>
<li>Support for rate limiting. Disabled by default for now. Can be enabled via the <code>rate-limit</code> input.</li>
<li>Dependency updates.</li>
</ul>
<p>Big thanks to <a href="https://github.com/prom3theu5"><code>@​prom3theu5</code></a> for implementing these changes!</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/0660d3ee46b6b05c0759824c7d57e3da998ef9a7"><code>0660d3e</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/71ac7c8e99fc3f3e79dd27d22e31562c0718138b"><code>71ac7c8</code></a> Remove unused import</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/b590aa413c25774c2c1c4a72fbd931313800af67"><code>b590aa4</code></a> Remove now unused owner and repo inputs and extend README</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/1026f804270448819ffbff4d5431d93bdb127d61"><code>1026f80</code></a> Bump action version</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/aadf1e6a671b9aa76ab0374b6957b8bc565ecd00"><code>aadf1e6</code></a> Update dependencies</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/7c7a884492a31ee4350db893a6bbb09de01f3ea7"><code>7c7a884</code></a> Formatting</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/3809558deab4f331492adbc12f241bd73568cbb4"><code>3809558</code></a> Build</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/f585a96b75358f951f8924c2a3c47cee70e0e9df"><code>f585a96</code></a> Update to address Comments</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/efcc59aa65ed5f6c8ff4b1e5856388c16ff4bece"><code>efcc59a</code></a> Update src/delete/strategies/organization.delete.strategy.ts</li>
<li><a href="https://github.com/SmartsquareGmbH/delete-old-packages/commit/800adc67017b4f1e8603719eeddabddf2c7d1fb1"><code>800adc6</code></a> Update README.md</li>
<li>Additional commits viewable in <a href="https://github.com/smartsquaregmbh/delete-old-packages/compare/v0.6.0...v0.7.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=smartsquaregmbh/delete-old-packages&package-manager=github_actions&previous-version=0.6.0&new-version=0.7.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 14:08:11 +0000 UTC
    </div>
</div>

