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
                PR <a href="https://github.com/hyperledger-labs/perun-eth-contracts/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    ⬆️ Bump apollo-server-core from 3.9.0 to 3.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [apollo-server-core](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core) from 3.9.0 to 3.11.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apollographql/apollo-server/blob/apollo-server-core@3.11.0/CHANGELOG.md">apollo-server-core's changelog</a>.</em></p>
<blockquote>
<h2>v3.11.0</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong>: The cache control plugin no longer sets the <code>cache-control</code> HTTP response header if the operation is part of a batched HTTP request. Previously, it would set the header to a value describing the cache policy of only one of the operations in the request, which could lead to data being unintentionally cached by proxies or clients. This bug was introduced in v3.0.0 and this fix restores the behavior of Apollo Server 2. (In Apollo Server 4 (specifically, <code>@apollo/server@4.1.0</code> or newer), the features work properly together, setting the header based on the combined cache policy of all operations.) This could theoretically have led to data tagged as uncacheable being cached and potentially served to different users. More details are available at the <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-8r69-3cvp-wxc3">security advisory</a>.</li>
<li><code>apollo-server-core</code>: New field <code>GraphQLRequestContext.requestIsBatched</code> available to plugins.</li>
</ul>
<h2>v3.10.4</h2>
<ul>
<li><code>apollo-server-core</code>: Manage memory more efficiently in the usage reporting plugin by allowing large objects to be garbage collected more quickly. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7106">#7106</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/7106">apollographql/apollo-server#7106</a>)</li>
<li><code>apollo-server-core</code>: The usage reporting plugin now defaults to a 30 second timeout for each attempt to send reports to Apollo Server instead of no timeout; the timeout can be adjusted with the new <code>requestTimeoutMs</code> option to <code>ApolloServerPluginUsageReporting</code>. (Apollo's servers already enforced a 30 second timeout, so this is unlikely to break any existing use cases.) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7106">#7106</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/7106">apollographql/apollo-server#7106</a>)</li>
</ul>
<h2>v3.10.3</h2>
<ul>
<li><code>apollo-server-core</code>: Fix memory leak in usage reporting plugin. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6983">#6983</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/6983">apollographql/apollo-server#6983</a>) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6999">#6999</a>](<a href="https://github.com/apollographql/apollo-server/%5BIssue">https://github.com/apollographql/apollo-server/[Issue</a> <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6983">#6983</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/6983)pull/6999">apollographql/apollo-server#6983</a>)</li>
</ul>
<h2>v3.10.2</h2>
<ul>
<li><code>apollo-server-fastify</code>: Use <code>return reply.send</code> in handlers to match the pattern encouraged by Fastify 4 (although <a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/6576#issuecomment-1159249244"><code>apollo-server-fastify@3</code> only works with Fastify 3</a>). [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6798">#6798</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6798">apollographql/apollo-server#6798</a>)</li>
<li><code>apollo-datasource-rest@3.7.0</code>: Add option <code>memoizeGetRequests</code> to disable GET cache [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6650">#6650</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6650">apollographql/apollo-server#6650</a>) and [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6834">#6834</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6834">apollographql/apollo-server#6834</a>)</li>
</ul>
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
<li><a href="https://github.com/apollographql/apollo-server/commit/538151b9f30dfc91036eef2f8f65fbf7922d861e"><code>538151b</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/69be2f75d05c7044086a869d915b965ada033850"><code>69be2f7</code></a> Merge pull request from GHSA-8r69-3cvp-wxc3</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/40fcd3d1a0b5f0d9887c6c2e2f731a90eebfa238"><code>40fcd3d</code></a> Backport <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7107">#7107</a> (docs: document new usage reporting option)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/f519e1d7de8564259eb1c8c1c7523669bd9ad815"><code>f519e1d</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/8ca2c1184ea48ca8c3bfc7227c6dc0524375eea3"><code>8ca2c11</code></a> Backport usage reporting improvements <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7101">#7101</a> to AS3 (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7106">#7106</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/985c0795579a1d39e7b78edce1c9e2e7c8facf82"><code>985c079</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/cd31e33ede4262b475fd6ccca4fa06e98f87d434"><code>cd31e33</code></a> usage reporting: fix memory leak (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7000">#7000</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/ca928e4bcc5aa1e0ccfb297298cf25c3d280abb1"><code>ca928e4</code></a> Upgrade <code>typescript</code> version and resolve &quot;unconstrained generic&quot; errors (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6940">#6940</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/40ed23fbb5dd620902d7c31bcc1e26e098990041"><code>40ed23f</code></a> chore(deps): update dependency uuid to v9 (main) (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6883">#6883</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/f6c5c9fec04c222aa15272b90d203ddc3fe64857"><code>f6c5c9f</code></a> Release</li>
<li>Additional commits viewable in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server-core@3.11.0/packages/apollo-server-core">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=apollo-server-core&package-manager=npm_and_yarn&previous-version=3.9.0&new-version=3.11.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-02 19:08:45 +0000 UTC
    </div>
</div>

