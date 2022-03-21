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
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Bump actions/cache from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [actions/cache](https://github.com/actions/cache) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/releases">actions/cache's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>
<p>This change adds a minimum runner version(node12 -&gt; node16), which can break users using an out-of-date/fork of the runner. This would be most commonly affecting users on GHES 3.3 or before, as those runners do not support node16 actions and they can use actions from github.com via <a href="https://docs.github.com/en/enterprise-server@3.0/admin/github-actions/managing-access-to-actions-from-githubcom/enabling-automatic-access-to-githubcom-actions-using-github-connect">github connect</a> or manually copying the repo to their GHES instance.</p>
</li>
<li>
<p>Few dependencies and cache action usage examples have also been updated.</p>
</li>
</ul>
<h2>v2.1.7</h2>
<p>Support 10GB cache upload using the latest version <code>1.0.8</code> of <a href="https://www.npmjs.com/package/@actions/cache"><code>@actions/cache</code> </a></p>
<h2>v2.1.6</h2>
<ul>
<li>Catch unhandled &quot;bad file descriptor&quot; errors that sometimes occurs when the cache server returns non-successful response (<a href="https://github-redirect.dependabot.com/actions/cache/pull/596">actions/cache#596</a>)</li>
</ul>
<h2>v2.1.5</h2>
<ul>
<li>Fix permissions error seen when extracting caches with GNU tar that were previously created using BSD tar (<a href="https://github-redirect.dependabot.com/actions/cache/issues/527">actions/cache#527</a>)</li>
</ul>
<h2>v2.1.4</h2>
<ul>
<li>Make caching more verbose <a href="https://github-redirect.dependabot.com/actions/toolkit/pull/650">#650</a></li>
<li>Use GNU tar on macOS if available <a href="https://github-redirect.dependabot.com/actions/toolkit/pull/701">#701</a></li>
</ul>
<h2>v2.1.3</h2>
<ul>
<li>Upgrades <code>@actions/core</code> to v1.2.6 for <a href="https://github.com/advisories/GHSA-mfwh-5m23-j46w">CVE-2020-15228</a>. This action was not using the affected methods.</li>
<li>Fix error handling in <code>uploadChunk</code> where 400-level errors were not being detected and handled correctly</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Adds input to limit the chunk upload size, useful for self-hosted runners with slower upload speeds</li>
<li>No-op when executing on GHES</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>Update <code>@actions/cache</code> package to <code>v1.0.2</code> which allows cache action to use posix format when taring files.</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>Replaces the <code>http-client</code> with the Azure Storage SDK for NodeJS when downloading cache content from Azure.  This should help improve download performance and reliability as the SDK downloads files in 4 MB chunks, which can be parallelized and retried independently</li>
<li>Display download progress and speed</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/cache/commit/4b0cf6cc4619e737324ddfcec08fff2413359514"><code>4b0cf6c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/cache/issues/769">#769</a> from actions/users/ashwinsangem/bump_major_version</li>
<li><a href="https://github.com/actions/cache/commit/60c606a2b4c5358e11c2ca7b4694e59049d008d1"><code>60c606a</code></a> Update licensed files</li>
<li><a href="https://github.com/actions/cache/commit/b6e9a919a7da3606e9b2db756823ee1c39c7b48d"><code>b6e9a91</code></a> Revert &quot;Updated to the latest version.&quot;</li>
<li><a href="https://github.com/actions/cache/commit/c8425035834f98c304ecf92f5d50f41d433885c1"><code>c842503</code></a> Updated to the latest version.</li>
<li><a href="https://github.com/actions/cache/commit/2b7da2a62c3af9fa2692cd8d2d117da76faf31ac"><code>2b7da2a</code></a> Bumped up to a major version.</li>
<li><a href="https://github.com/actions/cache/commit/deae296ab340574da1ec86242984dfc91f0a7b81"><code>deae296</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/cache/issues/651">#651</a> from magnetikonline/fix-golang-windows-example</li>
<li><a href="https://github.com/actions/cache/commit/c7c46bcb6db3c571021a3a2dc2d2557b512ecace"><code>c7c46bc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/cache/issues/707">#707</a> from duxtland/main</li>
<li><a href="https://github.com/actions/cache/commit/6535c5fb5fe2870754afba7bd4e514867ac9cb98"><code>6535c5f</code></a> Regenerated <code>examples.md</code> TOC</li>
<li><a href="https://github.com/actions/cache/commit/3fdafa472e0db16435add384585aa138ffdd16d3"><code>3fdafa4</code></a> Update GitHub Actions status badge markdown in <code>README.md</code></li>
<li><a href="https://github.com/actions/cache/commit/341e6d75d9826beb2fa659263d862f6aec63a064"><code>341e6d7</code></a> Merge branch 'actions:main' into fix-golang-windows-example</li>
<li>Additional commits viewable in <a href="https://github.com/actions/cache/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/cache&package-manager=github_actions&previous-version=2&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-21 14:26:19 +0000 UTC
    </div>
</div>

