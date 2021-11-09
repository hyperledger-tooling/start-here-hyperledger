---
layout: default
title: burrow
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/burrow
---

# burrow <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/burrow){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1523" class=".btn">#1523</a>
            </td>
            <td>
                <b>
                    Bump apollo-server from 2.21.1 to 2.25.3 in /vent/test/eth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [apollo-server](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server) from 2.21.1 to 2.25.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/apollographql/apollo-server/blob/main/CHANGELOG.md">apollo-server's changelog</a>.</em></p>
<blockquote>
<h2>v2.25.3</h2>
<ul>
<li>⚠️ <strong>SECURITY</strong> <code>apollo-server-core</code>: Update default version of the GraphQL Playground React app loaded from the CDN to be <code>@apollographql/graphql-playground-react@1.7.42</code>. This patches an XSS vulnerability. Note that if you are pinning the Playground React app version in your app with <code>new ApolloServer({playground: {version: 'some version'}})</code>, you will need to update the specified version to 1.7.42 or later to avoid this vulnerability. If you disable GraphQL Playground with <code>new ApolloServer({playground: false})</code>, this vulnerability does not affect you. See <a href="https://github.com/apollographql/apollo-server/security/advisories/GHSA-qm7x-rc44-rrqw">advisory GHSA-qm7x-rc44-rrqw</a> for more details.</li>
</ul>
<h2>v2.25.2</h2>
<ul>
<li><code>apollo-server-express</code>: Update dependencies on <code>@types/express</code> and <code>@types/express-serve-static-core</code>. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5352">#5352</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5352">apollographql/apollo-server#5352</a>)</li>
</ul>
<h2>v2.25.1</h2>
<ul>
<li><code>apollo-server-core</code>, <code>apollo-server-express</code>: Upgrade <code>subscriptions-transport-ws</code> dependency and remove unneeded runtime dependency on <code>ws</code>. This should enable you to install Apollo Server without depending on versions of <code>ws</code> vulnerable to <a href="https://www.npmjs.com/advisories/1748">CVE-2021-32640</a>. Note that the superficial integration of the unmaintained <code>subscriptions-transport-ws</code> package will be removed in Apollo Server 3; you can also avoid this vulnerability by disabling the built-in subscription support with <code>new ApolloServer({subscriptions: false})</code> and using a maintained package such as <code>graphql-ws</code> instead. (Instead of taking this upgrade, you can also upgrade <code>ws</code> to <code>5.2.3</code>, which was just released.)</li>
</ul>
<h2>v2.25.0</h2>
<ul>
<li><code>apollo-server-core</code>: You may now specify your Studio graph as a graph ref (<code>id@variant</code>) via the <code>APOLLO_GRAPH_REF</code> environment variable or <code>new ApolloServer({apollo: {graphRef}})</code> instead of specifying graph ID and graph variant separately. The <code>apollo</code> object passed to plugin <code>serverWillStart</code> and to gateway <code>load</code> now contains a <code>graphRef</code> field.</li>
<li><code>apollo-server-core</code>: Fix a race condition where schema reporting could lead to a delay at process shutdown. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5222">#5222</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5222">apollographql/apollo-server#5222</a>)</li>
<li><code>apollo-server-core</code>: Allow the Fetch API implementation to be overridden for the schema reporting and usage reporting plugins via a new <code>fetcher</code> option. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5179">#5179</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5179">apollographql/apollo-server#5179</a>)</li>
<li><code>apollo-server-core</code>: The <code>server.executeOperation</code> method (designed for testing) can now take its <code>query</code> as a <code>DocumentNode</code> (eg, a <code>gql</code>-tagged string) in addition to as a string. (This matches the behavior of the <code>apollo-server-testing</code> <code>createTestClient</code> function which is now deprecated.) We now recommend this method instead of <code>apollo-server-testing</code> in our docs. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/4952">#4952</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/4952">apollographql/apollo-server#4952</a>)</li>
<li><code>apollo-server-testing</code>: Replace README with a deprecation notice explaining how to use <code>server.executeOperation</code> instead. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/4952">#4952</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/4952">apollographql/apollo-server#4952</a>)</li>
</ul>
<h2>v2.24.1</h2>
<ul>
<li><code>apollo-server-core</code>: Fix a typo that could lead to TypeScript compilation when combined with a recent version of <code>@types/node</code>. (This bug had no runtime effect.) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5149">#5149</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5149">apollographql/apollo-server#5149</a>)</li>
</ul>
<h2>v2.24.0</h2>
<ul>
<li><code>apollo-server-core</code>: Apollo Studio usage reporting uses a more efficient format which sends fewer detailed traces to Apollo's server. This change should not have a major effect on the experience of using Apollo Studio. This also fixes a bug in all prior versions where all operations were reported to Studio as &quot;uncached&quot;. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/4142">#4142</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/4142">apollographql/apollo-server#4142</a>)</li>
</ul>
<h2>v2.23.0</h2>
<ul>
<li><code>apollo-server-core</code>: Add optional argument to <code>ApolloServer.executeOperation</code> allowing the caller to manually specify an argument to the <code>config</code> function analogous to that provided by integration packages. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/4166">#4166</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/4166">apollographql/apollo-server#4166</a>) [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/2886">#2886</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/2886">apollographql/apollo-server#2886</a>)</li>
<li><code>apollo-server-cache-redis@1.4.0</code>: New <code>BaseRedisCache</code> class which takes an <code>ioredis</code>-compatible Redis client as an argument. The existing classes <code>RedisCache</code> and <code>RedisClusterCache</code> (which pass their arguments to <code>ioredis</code> constructors) are now implemented in terms of this class. This allows you to use any of the <code>ioredis</code> constructor forms rather than just the ones recognized by our classes. This also fixes a long-standing bug where the Redis cache implementations returned a number from <code>delete()</code>; it now returns a number, matching what the <code>KeyValueCache</code> interface and the TypeScript types expect. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5034">#5034</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5034">apollographql/apollo-server#5034</a>) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5088">#5088</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5088">apollographql/apollo-server#5088</a>) [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/4870">#4870</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/4870">apollographql/apollo-server#4870</a>) [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5006">#5006</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/5006">apollographql/apollo-server#5006</a>)</li>
<li><code>apollo-server-core</code>: Fix type for <code>formatResponse</code> function. It never is called with a <code>null</code> argument, and is allowed to return <code>null</code>. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5009">#5009</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/5009">apollographql/apollo-server#5009</a>) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5089">#5089</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5089">apollographql/apollo-server#5089</a>)</li>
<li><code>apollo-server-lambda</code>: Fix regression in v2.21.2 where thrown errors were replaced by throwing the JS Error class itself. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5085">#5085</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5085">apollographql/apollo-server#5085</a>)</li>
<li><code>apollo-server-core</code>: If a client sends a variable of the wrong type, this is now reported as an error with an <code>extensions.code</code> of <code>BAD_USER_INPUT</code> rather than <code>INTERNAL_SERVER_ERROR</code>. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5091">#5091</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5091">apollographql/apollo-server#5091</a>) [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/3498">#3498</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/3498">apollographql/apollo-server#3498</a>)</li>
<li><code>apollo-server-lambda</code>: Explicitly support API Gateway <code>payloadFormatVersion</code> 2.0. Previously some codepaths did appropriate checks to partially support 2.0 and other codepaths could lead to errors like <code>event.path.endsWith is not a function</code> (especially since v2.21.1). Note that this changes the TypeScript typing of the <code>onHealthCheck</code> callback passed to <code>createHandler</code> to indicate that it can receive either type of event. If you are using TypeScript and care about having a precise typing for the argument to your <code>onHealthCheck</code> callback, you should determine which payload format you want to support and write <code>new ApolloServer&lt;APIGatewayProxyEvent&gt;(...)</code> or <code>new ApolloServer&lt;APIGatewayProxyEventV2&gt;(...)</code> (importing these types from <code>aws-lambda</code>), or differentiate between the two formats by checking to see if <code>'path' in event</code>. [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5084">#5084</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/5084">apollographql/apollo-server#5084</a>) [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5016">#5016</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/5016">apollographql/apollo-server#5016</a>)</li>
</ul>
<h2>v2.22.2</h2>
<ul>
<li><code>apollo-server-core</code>: Fix a regression in v2.22.0 where combining <code>apollo-server-core</code> v2.22 with an older version of an integration package could lead to startup errors like <code>called start() with surprising state invoking serverWillStart</code>. The fix involves changing the semantics of the protected <code>willStart</code> method (which is left in only for backwards compatibility). [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5065">#5065</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/5065">apollographql/apollo-server#5065</a>) [Issue <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5066">#5066</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/issues/5066">apollographql/apollo-server#5066</a>) [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5073">#5073</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5073">apollographql/apollo-server#5073</a>)</li>
</ul>
<h2>v2.22.1</h2>
<ul>
<li><code>apollo-server-core</code>: Fix a regression in v2.22.0 where startup errors could be thrown as part of the GraphQL response instead of redacted in one edge case. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5064">#5064</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/5064">apollographql/apollo-server#5064</a>)</li>
</ul>
<h2>v2.22.0</h2>
<ul>
<li>Improve startup error handling by ensuring that your server has loaded its schema and executed its <code>serverWillStart</code> handlers successfully before starting an HTTP server. If you're using the <code>apollo-server</code> package, no code changes are necessary. If you're using an integration such as <code>apollo-server-express</code> that is not a &quot;serverless framework&quot;, you can insert <a href="https://www.apollographql.com/docs/apollo-server/api/apollo-server/#start"><code>await server.start()</code></a> between <code>server = new ApolloServer()</code> and <code>server.applyMiddleware</code>. (If you don't call <code>server.start()</code> yourself, your server will still work, but the previous behavior of starting a web server that may fail to load its schema still applies.) The serverless framework integrations (Lambda, Azure Functions, and Cloud Functions) do not support this functionality. While the protected method <code>willStart</code> still exists for backwards compatibility, you should replace calls to it with <code>start</code> or the new protected method <code>ensureStarting</code>. [PR <a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/4981">#4981</a>](<a href="https://github-redirect.dependabot.com/apollographql/apollo-server/pull/4981">apollographql/apollo-server#4981</a>)</li>
</ul>
<h2>v2.21.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/a725306525a99650af46effb72ae9afe780ed88b"><code>a725306</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/70a431212bd2d07d68c962cb5ded63ecc6a21963"><code>70a4312</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/f47c11d3f40f87797c5a615af0bd0225fb18fda8"><code>f47c11d</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/42983b06a381aee6333fd11d5af7bd7fa0d549ec"><code>42983b0</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/19572d7b36f01768faf2b2e9b1fbd18638ef7397"><code>19572d7</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/c8c07483f914a18c07cce6435dcc8816fa795c34"><code>c8c0748</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/df92f399bb5106a496b414c7e9984f6da97c7c55"><code>df92f39</code></a> docs: replace spectrum with community forum (<a href="https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server/issues/5228">#5228</a>)</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/9e1bf7df8ce856f62e851a9cf268508eb574e32c"><code>9e1bf7d</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/f2349d0e10633ee79bed152f682e53730175d59b"><code>f2349d0</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/4e5f03e2b071c2a049836dd14f072f161a0ccd12"><code>4e5f03e</code></a> Release</li>
<li>Additional commits viewable in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server@2.25.3/packages/apollo-server">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=apollo-server&package-manager=npm_and_yarn&previous-version=2.21.1&new-version=2.25.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/burrow/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 18:41:52 +0000 UTC
    </div>
</div>

