---
layout: default
title: perun-eth-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-contracts
---

# perun-eth-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-contracts/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    ⬆️ Bump apollo-server-core from 3.9.0 to 3.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [apollo-server-core](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core) from 3.9.0 to 3.10.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apollographql/apollo-server/blob/main/CHANGELOG.md">apollo-server-core's changelog</a>.</em></p>
<blockquote>
<h2>v3.10.1</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong>: The default landing page contained HTML to display a sample <code>curl</code> command which is made visible if the full landing page bundle could not be fetched from Apollo's CDN. The server's URL is directly interpolated into this command inside the browser from <code>window.location.href</code>. On some older browsers such as IE11, this value is not URI-encoded. On such browsers, opening a malicious URL pointing at an Apollo Router could cause execution of attacker-controlled JavaScript. In this release, the fallback page does not display a <code>curl</code> command. More details are available at the <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-2fvv-qxrq-7jq6">security advisory</a>.</li>
<li>Improve error message when both a graph ref and a graph variant are specified. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6709">#6709</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6709">apollographql/apollo-server#6709</a>)</li>
<li>Fix the TypeScript declaration of the <code>fieldLevelInstrumentation</code> option to <code>ApolloServerPluginUsageReporting</code> to show that the function may return a number in addition to a boolean. This now matches the implementation and docs. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6763">#6763</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6763">apollographql/apollo-server#6763</a>)</li>
</ul>
<h2>v3.10.0</h2>
<ul>
<li>Add <code>document</code>, <code>variables</code>, <code>headers</code> as an option in the <code>ApolloServerPluginLandingPageLocalDefault</code> plugins. The embedded version of Apollo Sandbox can now use these options as an initial state. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6628">#6628</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6628">apollographql/apollo-server#6628</a>)</li>
<li>Add <code>generateCacheKey</code> to <code>ApolloServerPluginResponseCache</code> to allow for custom cache keys. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6655">#6655</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6655">apollographql/apollo-server#6655</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/e6097d614c9ac6887b359529cf27c1bd1a5de59c"><code>e6097d6</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/68a439b6e3af9edc8a2480092f2d49f058be1e64"><code>68a439b</code></a> Merge pull request from GHSA-2fvv-qxrq-7jq6</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/6140880d54e5299a193eb42c02bf279fd0f0f9c5"><code>6140880</code></a> Usage reporting: fix TS declaration of fieldLevelInstrumentation (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6763">#6763</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/bd499754e595a2c2b0e53a2e08d10427d4433ea7"><code>bd49975</code></a> Update error message when graph ref and variant are specified (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6709">#6709</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/4041aaed6d616ee4b06fced0af482c73b6f752be"><code>4041aae</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/e9ae0f28d11d2fdfc5abd5048c85acf70de21592"><code>e9ae0f2</code></a> fix: &quot;without going through&quot; typo (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6661">#6661</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/07639bb35e5994ff58fedc64d59b4ef2e1598a21"><code>07639bb</code></a> NEBULA-1385: Add <code>initialState</code> to embeddable sandbox based on config (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6628">#6628</a>)</li>
<li>See full diff in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server-core@3.10.1/packages/apollo-server-core">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=apollo-server-core&package-manager=npm_and_yarn&previous-version=3.9.0&new-version=3.10.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/perun-eth-contracts/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 19:44:42 +0000 UTC
    </div>
</div>

