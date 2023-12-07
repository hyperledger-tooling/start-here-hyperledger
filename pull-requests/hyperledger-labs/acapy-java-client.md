---
layout: default
title: acapy-java-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/acapy-java-client
---

# acapy-java-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/acapy-java-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/92" class=".btn">#92</a>
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
        Created At 2023-11-30 14:20:54 +0000 UTC
    </div>
</div>

