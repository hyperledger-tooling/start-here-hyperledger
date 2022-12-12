---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/347" class=".btn">#347</a>
            </td>
            <td>
                <b>
                    Bump apollo-server-core from 3.6.7 to 3.11.1 in /samples/besu/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [apollo-server-core](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core) from 3.6.7 to 3.11.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apollographql/apollo-server/blob/apollo-server-core@3.11.1/CHANGELOG.md">apollo-server-core's changelog</a>.</em></p>
<blockquote>
<h2>v3.11.1</h2>
<ul>
<li><code>apollo-server-core</code>: Follow-up to v3.11.0: make <code>GraphQLRequestContext.requestIsBatched</code> optional for better compatibility with older versions of <code>@apollo/gateway</code>.</li>
</ul>
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
<h2>v3.9.0</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong> <code>apollo-server-core</code>: The default configuration of Apollo Server is vulnerable to denial of service attacks via memory exhaustion. If you do not currently specify the <code>cache</code> option to <code>new ApolloServer()</code>, we strongly recommend you specify <code>cache: 'bounded'</code>, which replaces the default in-memory unbounded cache with a 30MB in-memory cache, or disable automatic persisted queries with <code>persistedQueries: false</code>. Apollo Server now logs a warning in production if you do not configure the cache or disable APQs. See <a href="https://www.apollographql.com/docs/apollo-server/performance/cache-backends#ensuring-a-bounded-cache">the docs</a> for more details.</li>
<li>The <code>apollo-server-caching</code> package is no longer published. The TypeScript types <code>KeyValueCache</code> and <code>KeyValueCacheSetOptions</code> and the classes <code>PrefixingKeyValueCache</code> and <code>InMemoryLRUCache</code> can be imported from <code>@apollo/utils.keyvaluecache</code> instead. The first three exports are identical; <code>InMemoryLRUCache</code> is based on <code>lru-cache</code> v7 instead of v6, and no longer supports creating unbounded caches (which was the default behavior for <code>apollo-server-caching</code>'s <code>InMemoryLRUCache</code>). [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6522">#6522</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6522">apollographql/apollo-server#6522</a>)</li>
<li>The <code>apollo-server-cache-redis</code> and <code>apollo-server-cache-memcached</code> packages are no longer published (though previous versions continue to work). We recommend that users of these packages migrate to <code>@apollo/utils.keyvadapter</code>, which lets you connect to Redis, Memcached, or any other backend supported by the <a href="https://www.npmjs.com/package/keyv">Keyv</a> project. See <a href="https://www.apollographql.com/docs/apollo-server/performance/cache-backends">the new cache backend docs</a> for more details. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6541">#6541</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6541">apollographql/apollo-server#6541</a>)</li>
<li>Avoid unhandled rejection errors if the end hook from a <code>parsingDidStart</code> plugin method rejects. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6567">#6567</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6567">apollographql/apollo-server#6567</a>) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6559">#6559</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6559">apollographql/apollo-server#6559</a>)</li>
</ul>
<h2>v3.8.2</h2>
<ul>
<li><code>apollo-server-core</code>: Fix usage reporting plugin &quot;willResolveField called after stopTiming!&quot; error caused by a race condition related to null bubbling. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/4472">#4472</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/4472">apollographql/apollo-server#4472</a>) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6398">#6398</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/6398">apollographql/apollo-server#6398</a>)</li>
</ul>
<h2>v3.8.1</h2>
<ul>
<li>This is a patch release strictly for republishing over what appears to be a hiccup in NPMs service. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6469">#6469</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/6469">apollographql/apollo-server#6469</a>)</li>
</ul>
<h2>v3.8.0</h2>
<ul>
<li>Add <code>embed</code> as an option in the <code>ApolloServerPluginLandingPageLocalDefault</code> and <code>ApolloServerPluginLandingPageProductionDefault</code> plugins. If you pass the <code>embed</code> option to <code>ApolloServerPluginLandingPageLocalDefault</code>, the Apollo Studio Sandbox will be embedded on your Apollo Server endpoint. If you pass the <code>embed</code> option to <code>ApolloServerPluginLandingPageProductionDefault</code>, the Apollo Studio embedded Explorer will be embedded on your Apollo Server endpoint. In both cases, users can use the embedded app to run GraphQL operations without any special CORS setup.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/6247d96ba90de6fa9b45995dcab72758c99aab78"><code>6247d96</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/538151b9f30dfc91036eef2f8f65fbf7922d861e"><code>538151b</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/69be2f75d05c7044086a869d915b965ada033850"><code>69be2f7</code></a> Merge pull request from GHSA-8r69-3cvp-wxc3</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/40fcd3d1a0b5f0d9887c6c2e2f731a90eebfa238"><code>40fcd3d</code></a> Backport <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7107">#7107</a> (docs: document new usage reporting option)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/f519e1d7de8564259eb1c8c1c7523669bd9ad815"><code>f519e1d</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/8ca2c1184ea48ca8c3bfc7227c6dc0524375eea3"><code>8ca2c11</code></a> Backport usage reporting improvements <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7101">#7101</a> to AS3 (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7106">#7106</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/985c0795579a1d39e7b78edce1c9e2e7c8facf82"><code>985c079</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/cd31e33ede4262b475fd6ccca4fa06e98f87d434"><code>cd31e33</code></a> usage reporting: fix memory leak (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/7000">#7000</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/ca928e4bcc5aa1e0ccfb297298cf25c3d280abb1"><code>ca928e4</code></a> Upgrade <code>typescript</code> version and resolve &quot;unconstrained generic&quot; errors (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6940">#6940</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/40ed23fbb5dd620902d7c31bcc1e26e098990041"><code>40ed23f</code></a> chore(deps): update dependency uuid to v9 (main) (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core/issues/6883">#6883</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server-core@3.11.1/packages/apollo-server-core">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=apollo-server-core&package-manager=npm_and_yarn&previous-version=3.6.7&new-version=3.11.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 11:45:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/346" class=".btn">#346</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /samples/besu/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [decode-uri-component](https://github.com/SamVerschueren/decode-uri-component) from 0.2.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/SamVerschueren/decode-uri-component/releases">decode-uri-component's releases</a>.</em></p>
<blockquote>
<h2>v0.2.2</h2>
<ul>
<li>Prevent overwriting previously decoded tokens  980e0bf</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2</a></p>
<h2>v0.2.1</h2>
<ul>
<li>Switch to GitHub workflows  76abc93</li>
<li>Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a>  746ca5d</li>
<li>Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)  486d7e2</li>
<li>Tidelift tasks  a650457</li>
<li>Meta tweaks  66e1c28</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a0eea469d26eb0df668b081672cdb9581feb78eb"><code>a0eea46</code></a> 0.2.2</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/980e0bf09b64d94f1aa79012f895816c30ffd152"><code>980e0bf</code></a> Prevent overwriting previously decoded tokens</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/3c8a373dd4837e89b3f970e01295dd03e1405a33"><code>3c8a373</code></a> 0.2.1</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/76abc939783fe3900fadb7d384a74d324d5557f3"><code>76abc93</code></a> Switch to GitHub workflows</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/746ca5dcb6667c5d364e782d53c542830e4c10b9"><code>746ca5d</code></a> Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a></li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/486d7e26d3a8c0fbe860fb651fe1bc98c2f2be30"><code>486d7e2</code></a> Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a65045724e6234acef87f31da499d4807b20b134"><code>a650457</code></a> Tidelift tasks</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/66e1c2834c0e189201cb65196ec3101372459b02"><code>66e1c28</code></a> Meta tweaks</li>
<li>See full diff in <a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=decode-uri-component&package-manager=npm_and_yarn&previous-version=0.2.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 11:45:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/345" class=".btn">#345</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.6.0 to 4.7.3 in /samples/besu/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.6.0 to 4.7.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.3</h2>
<p>:warning: This is a patch for a high severity issue. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4h98-2769-gh6h">visit the security advisory</a>.</p>
<h3>Breaking changes</h3>
<ul>
<li><code>ECDSA</code>: <code>recover(bytes32,bytes)</code> and <code>tryRecover(bytes32,bytes)</code> no longer accept compact signatures to prevent malleability. Compact signature support remains available using <code>recover(bytes32,bytes32,bytes32)</code> and <code>tryRecover(bytes32,bytes32,bytes32)</code>.</li>
</ul>
<h2>v4.7.2</h2>
<p>:warning: This is a patch for three issues, including a high severity issue in <code>GovernorVotesQuorumFraction</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-xrc4-737v-9q75">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-7grf-83vw-6f5x">2</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9j3m-g383-29qr">3</a>).</p>
<ol>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
</ol>
<h2>v4.7.1</h2>
<p>:warning: This is a patch for a medium severity issue affecting <code>SignatureChecker</code> and a high severity issue affecting <code>ERC165Checker</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4g63-c64m-25w9">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-qh9x-gcfh-pcrw">2</a>).</p>
<ul>
<li><code>SignatureChecker</code>: Fix an issue that causes <code>isValidSignatureNow</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
<li><code>ERC165Checker</code>: Fix an issue that causes <code>supportsInterface</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
</ul>
<h2>v4.7.0</h2>
<ul>
<li><code>TimelockController</code>: Migrate <code>_call</code> to <code>_execute</code> and allow inheritance and overriding similar to <code>Governor</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3317">#3317</a>)</li>
<li><code>CrossChainEnabledPolygonChild</code>: replace the <code>require</code> statement with the custom error <code>NotCrossChainCall</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3380">#3380</a>)</li>
<li><code>ERC20FlashMint</code>: Add customizable flash fee receiver. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3327">#3327</a>)</li>
<li><code>ERC4626</code>: add an extension of <code>ERC20</code> that implements the ERC4626 Tokenized Vault Standard. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>SafeERC20</code>: add <code>safePermit</code> as mitigation against phantom permit functions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3280">#3280</a>)</li>
<li><code>Math</code>: add a <code>mulDiv</code> function that can round the result either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>Math</code>: Add a <code>sqrt</code> function to compute square roots of integers, rounding either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3242">#3242</a>)</li>
<li><code>Strings</code>: add a new overloaded function <code>toHexString</code> that converts an <code>address</code> with fixed length of 20 bytes to its not checksummed ASCII <code>string</code> hexadecimal representation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3403">#3403</a>)</li>
<li><code>EnumerableMap</code>: add new <code>UintToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3338">#3338</a>)</li>
<li><code>EnumerableMap</code>: add new <code>Bytes32ToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3416">#3416</a>)</li>
<li><code>SafeCast</code>: add support for many more types, using procedural code generation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3245">#3245</a>)</li>
<li><code>MerkleProof</code>: add <code>multiProofVerify</code> to prove multiple values are part of a Merkle tree. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3276">#3276</a>)</li>
<li><code>MerkleProof</code>: add calldata versions of the functions to avoid copying input arrays to memory and save gas. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3200">#3200</a>)</li>
<li><code>ERC721</code>, <code>ERC1155</code>: simplified revert reasons. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3254">#3254</a>, (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3438">#3438</a>))</li>
<li><code>ERC721</code>: removed redundant require statement. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3434">#3434</a>)</li>
<li><code>PaymentSplitter</code>: add <code>releasable</code> getters. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3350">#3350</a>)</li>
<li><code>Initializable</code>: refactored implementation of modifiers for easier understanding. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3450">#3450</a>)</li>
<li><code>Proxies</code>: remove runtime check of ERC1967 storage slots. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3455">#3455</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>Initializable</code>: functions decorated with the modifier <code>reinitializer(1)</code> may no longer invoke each other.</li>
</ul>
<h2>v4.7.0-rc.0</h2>
<p>This prerelease is now available for open review! Let us know your feedback and if you find any security issues.</p>
<p>We have a <a href="https://immunefi.com/bounty/openzeppelin/">bug bounty</a> with rewards of up to USD $25,000 and a special POAP for submitting a valid issue.</p>
<p>See the <a href="https://forum.openzeppelin.com/t/release-candidate-for-contracts-4-7-open-review-period/29443">announcement</a> for more details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.7.3</h2>
<h3>Breaking changes</h3>
<ul>
<li><code>ECDSA</code>: <code>recover(bytes32,bytes)</code> and <code>tryRecover(bytes32,bytes)</code> no longer accept compact signatures to prevent malleability. Compact signature support remains available using <code>recover(bytes32,bytes32,bytes32)</code> and <code>tryRecover(bytes32,bytes32,bytes32)</code>.</li>
</ul>
<h2>4.7.2</h2>
<ul>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
</ul>
<h2>4.7.1</h2>
<ul>
<li><code>SignatureChecker</code>: Fix an issue that causes <code>isValidSignatureNow</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
<li><code>ERC165Checker</code>: Fix an issue that causes <code>supportsInterface</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
</ul>
<h2>4.7.0 (2022-06-29)</h2>
<ul>
<li><code>TimelockController</code>: Migrate <code>_call</code> to <code>_execute</code> and allow inheritance and overriding similar to <code>Governor</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3317">#3317</a>)</li>
<li><code>CrossChainEnabledPolygonChild</code>: replace the <code>require</code> statement with the custom error <code>NotCrossChainCall</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3380">#3380</a>)</li>
<li><code>ERC20FlashMint</code>: Add customizable flash fee receiver. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3327">#3327</a>)</li>
<li><code>ERC4626</code>: add an extension of <code>ERC20</code> that implements the ERC4626 Tokenized Vault Standard. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>SafeERC20</code>: add <code>safePermit</code> as mitigation against phantom permit functions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3280">#3280</a>)</li>
<li><code>Math</code>: add a <code>mulDiv</code> function that can round the result either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>Math</code>: Add a <code>sqrt</code> function to compute square roots of integers, rounding either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3242">#3242</a>)</li>
<li><code>Strings</code>: add a new overloaded function <code>toHexString</code> that converts an <code>address</code> with fixed length of 20 bytes to its not checksummed ASCII <code>string</code> hexadecimal representation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3403">#3403</a>)</li>
<li><code>EnumerableMap</code>: add new <code>UintToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3338">#3338</a>)</li>
<li><code>EnumerableMap</code>: add new <code>Bytes32ToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3416">#3416</a>)</li>
<li><code>SafeCast</code>: add support for many more types, using procedural code generation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3245">#3245</a>)</li>
<li><code>MerkleProof</code>: add <code>multiProofVerify</code> to prove multiple values are part of a Merkle tree. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3276">#3276</a>)</li>
<li><code>MerkleProof</code>: add calldata versions of the functions to avoid copying input arrays to memory and save gas. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3200">#3200</a>)</li>
<li><code>ERC721</code>, <code>ERC1155</code>: simplified revert reasons. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3254">#3254</a>, (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3438">#3438</a>))</li>
<li><code>ERC721</code>: removed redundant require statement. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3434">#3434</a>)</li>
<li><code>PaymentSplitter</code>: add <code>releasable</code> getters. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3350">#3350</a>)</li>
<li><code>Initializable</code>: refactored implementation of modifiers for easier understanding. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3450">#3450</a>)</li>
<li><code>Proxies</code>: remove runtime check of ERC1967 storage slots. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3455">#3455</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>Initializable</code>: functions decorated with the modifier <code>reinitializer(1)</code> may no longer invoke each other.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ecd2ca2cd7cac116f7a37d0e474bbb3d7d5e1c4d"><code>ecd2ca2</code></a> 4.7.3</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e1878ace8c2908b85d39f9925c68c6f738cf3325"><code>e1878ac</code></a> Fix ECDSA signature malleability (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3610">#3610</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/64e48203cecad94f02de9891ecdeed4d629c6dae"><code>64e4820</code></a> 4.7.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/b66fe1606a173f2b78694567b543d480cb39cfe4"><code>b66fe16</code></a> Update changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8fb5f5774e3e8cfc10699f58749d8a34ec9d3e86"><code>8fb5f57</code></a> Avoid returnbomb in ERC165Checker (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3587">#3587</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/67b2572c6a050563990637f5017af8eeda111b21"><code>67b2572</code></a> Keep track of historical quorum values (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3561">#3561</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4337192dc02b64785885787e80126f93ee3f2659"><code>4337192</code></a> Fix arbitrum L1 to L2 crosschain call detection (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3578">#3578</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/41c7b25a65f636feaef7f0dc932ec4c44baa12f3"><code>41c7b25</code></a> Fix error in documentation and typo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3567">#3567</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e15862f2893f024e0872f0f1abcf275c4b436834"><code>e15862f</code></a> Remove test for feature not in 4.7</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/3b8b4ba82c880c31cd3b96dd5e15741d7e26658e"><code>3b8b4ba</code></a> 4.7.1</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.6.0...v4.7.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.6.0&new-version=4.7.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 11:44:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Fixing Miscellaneous Structure and Policy Issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes #140 , #288 , #297 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 06:43:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Besu Simplestate Application Contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                SimpleState Contract for Besu network with functions: 
1. `get(key)`: returns value stored at key.
2. `set(key, value)`: sets "value" at key "key".

Added besu-cli commands to test the simplestate:
1. `./bin/besu-cli state set --network=network1 <key> <value>`
2. `./bin/besu-cli state get --network=network1 <key>`

Closes #226 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 18:31:58 +0000 UTC
    </div>
</div>

