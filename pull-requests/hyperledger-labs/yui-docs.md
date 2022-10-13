---
layout: default
title: yui-docs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-docs
---

# yui-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Bump apollo-server from 2.25.2 to 2.26.0 in /contracts/minitoken/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [apollo-server](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server) from 2.25.2 to 2.26.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apollographql/apollo-server/blob/apollo-server@2.26.0/CHANGELOG.md">apollo-server's changelog</a>.</em></p>
<blockquote>
<h2>v2.26.0</h2>
<ul>
<li>Backport [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5537">#5537</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5537">apollographql/apollo-server#5537</a>) from Apollo Server 3. This fixes a TypeScript declaration relating to the Fetch API. We believe this will make it possible to use Apollo Server 2 with Apollo Gateway 0.52.0. (This change does not provide any functionality other than hopefully fixing some TypeScript builds, so if it turns out that this breaks your TypeScript build instead, just don't take the upgrade. We encourage you to upgrade to actively supported Apollo major versions instead.) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/6829">#6829</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6829">apollographql/apollo-server#6829</a>)</li>
</ul>
<h2>v2.25.4</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong>: If your server does not explicitly enable <code>graphql-upload</code> support via the <code>uploads</code> option to <code>new ApolloServer</code> and your schema does not use the <code>Upload</code> scalar (other than in its own definition), Apollo Server will not process the <code>multipart/form-data</code> requests sent by <code>graphql-upload</code> clients. This fixes a Cross-Site Request Forgery (CSRF) vulnerability where origins could cause browsers to execute mutations using a user's cookies even when those origins are not allowed by your CORS policy. If you <em>do</em> use uploads in your server, the vulnerability still exists with this version; you should instead upgrade to Apollo Server v3.7 and enable the CSRF prevention feature. (The AS3.7 CSRF prevention feature also protects against other forms of CSRF such as timing attacks against read-only query operations.) See <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-2p3c-p3qw-69r4">advisory GHSA-2p3c-p3qw-69r4</a> for more details.</li>
</ul>
<h2>v2.25.3</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong> <code>apollo-server-core</code>: Update default version of the GraphQL Playground React app loaded from the CDN to be <code>@apollographql/graphql-playground-react@1.7.42</code>. This patches an XSS vulnerability. Note that if you are pinning the Playground React app version in your app with <code>new ApolloServer({playground: {version: 'some version'}})</code>, you will need to update the specified version to 1.7.42 or later to avoid this vulnerability. If you disable GraphQL Playground with <code>new ApolloServer({playground: false})</code>, this vulnerability does not affect you. See <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-qm7x-rc44-rrqw">advisory GHSA-qm7x-rc44-rrqw</a> for more details.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/91de501bb389c07ccfc5e684811153267b91e9ac"><code>91de501</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/ae444b2916deb2fa37dbd8fa091201235dc2ec6d"><code>ae444b2</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/a725306525a99650af46effb72ae9afe780ed88b"><code>a725306</code></a> Release</li>
<li>See full diff in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server@2.26.0/packages/apollo-server">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=apollo-server&package-manager=npm_and_yarn&previous-version=2.25.2&new-version=2.26.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 19:18:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Bump apollo-server from 2.25.2 to 2.26.0 in /samples/minitoken-besu-ethereum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [apollo-server](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server) from 2.25.2 to 2.26.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apollographql/apollo-server/blob/apollo-server@2.26.0/CHANGELOG.md">apollo-server's changelog</a>.</em></p>
<blockquote>
<h2>v2.26.0</h2>
<ul>
<li>Backport [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5537">#5537</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5537">apollographql/apollo-server#5537</a>) from Apollo Server 3. This fixes a TypeScript declaration relating to the Fetch API. We believe this will make it possible to use Apollo Server 2 with Apollo Gateway 0.52.0. (This change does not provide any functionality other than hopefully fixing some TypeScript builds, so if it turns out that this breaks your TypeScript build instead, just don't take the upgrade. We encourage you to upgrade to actively supported Apollo major versions instead.) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/6829">#6829</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6829">apollographql/apollo-server#6829</a>)</li>
</ul>
<h2>v2.25.4</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong>: If your server does not explicitly enable <code>graphql-upload</code> support via the <code>uploads</code> option to <code>new ApolloServer</code> and your schema does not use the <code>Upload</code> scalar (other than in its own definition), Apollo Server will not process the <code>multipart/form-data</code> requests sent by <code>graphql-upload</code> clients. This fixes a Cross-Site Request Forgery (CSRF) vulnerability where origins could cause browsers to execute mutations using a user's cookies even when those origins are not allowed by your CORS policy. If you <em>do</em> use uploads in your server, the vulnerability still exists with this version; you should instead upgrade to Apollo Server v3.7 and enable the CSRF prevention feature. (The AS3.7 CSRF prevention feature also protects against other forms of CSRF such as timing attacks against read-only query operations.) See <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-2p3c-p3qw-69r4">advisory GHSA-2p3c-p3qw-69r4</a> for more details.</li>
</ul>
<h2>v2.25.3</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong> <code>apollo-server-core</code>: Update default version of the GraphQL Playground React app loaded from the CDN to be <code>@apollographql/graphql-playground-react@1.7.42</code>. This patches an XSS vulnerability. Note that if you are pinning the Playground React app version in your app with <code>new ApolloServer({playground: {version: 'some version'}})</code>, you will need to update the specified version to 1.7.42 or later to avoid this vulnerability. If you disable GraphQL Playground with <code>new ApolloServer({playground: false})</code>, this vulnerability does not affect you. See <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-qm7x-rc44-rrqw">advisory GHSA-qm7x-rc44-rrqw</a> for more details.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/91de501bb389c07ccfc5e684811153267b91e9ac"><code>91de501</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/ae444b2916deb2fa37dbd8fa091201235dc2ec6d"><code>ae444b2</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/a725306525a99650af46effb72ae9afe780ed88b"><code>a725306</code></a> Release</li>
<li>See full diff in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server@2.26.0/packages/apollo-server">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=apollo-server&package-manager=npm_and_yarn&previous-version=2.25.2&new-version=2.26.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 19:18:27 +0000 UTC
    </div>
</div>

