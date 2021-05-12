---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.0.3 to 1.1.8 in /fabric-protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.0.3 to 1.1.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.1.7</h2>
<ul>
<li>Fix a bug where a client that takes too long to connect can fail to keep the Node process running (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1580">#1580</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.6</h2>
<ul>
<li><code>Channel#watchConnectivityState</code>: handle infinite deadlines correctly (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1553">#1553</a> contributed by <a href="https://github.com/SimonWoolf"><code>@​SimonWoolf</code></a>)</li>
<li>Use correct name for SNI when connecting through a proxy (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1555">#1555</a> contributed by <a href="https://github.com/wkchee"><code>@​wkchee</code></a>)</li>
<li>Preserve the original error code when propagating errors thrown in <code>data</code> event handlers in server call handlers (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1557">#1557</a> contributed by <a href="https://github.com/mad-it"><code>@​mad-it</code></a>)</li>
<li>Fix compatibility issue between <code>ChannelOptions</code> and <code>ClientOptions</code> type definitions (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1559">#1559</a> contributed by <a href="https://github.com/grissius"><code>@​grissius</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.5</h2>
<ul>
<li>Move the dependencies on <code>@grpc/proto-loader</code> and <code>google-auth-library</code> from development dependencies to production dependencies (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1551">#1551</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.4</h2>
<ul>
<li>Clean up calls on the client even when returning a status causes an error to be thrown (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1524">#1524</a>)</li>
<li>Add <code>end(metadata?: Metadata)</code> method overload to streaming server call type definitions (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1525">#1525</a>)</li>
<li>Implement the <code>getPeer</code> method in client and server call classes (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1526">#1526</a>)</li>
<li>Fix an error regarding <code>grpc-tools</code> flags in the README (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1534">#1534</a> contributed by <a href="https://github.com/mavaa"><code>@​mavaa</code></a>)</li>
<li>Move <code>@types/node</code> to a production dependency (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1546">#1546</a>)</li>
<li>Prevent mutation of default headers (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1548">#1548</a> contributed by <a href="https://github.com/richardpringle"><code>@​richardpringle</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.3</h2>
<ul>
<li>Fix handling of unsuccessful TXT record lookups (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1512">#1512</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.2</h2>
<h2><code>@​grpc/grpc-js</code> 1.1.1</h2>
<ul>
<li>Fix how the SNI string is constructed based on the provided target address (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1486">#1486</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.2</h2>
<ul>
<li>Drop connections when failing to use them to start streams, even when those connections appear otherwise healthy (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1494">#1494</a>)</li>
<li>Add the string &quot;Internal server error&quot; to the commonly reported error &quot;Received RST_STREAM with code 2&quot; to clarify what causes that error (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1494">#1494</a>)</li>
<li>Drop the peer dependency on google-auth-library (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1498">#1498</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.1.0</h2>
<ul>
<li>Fix the <code>credentials</code> type definition (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1459">#1459</a> contributed by <a href="https://github.com/greenboxal"><code>@​greenboxal</code></a>)</li>
<li>Export the <code>ClientOptions</code> type (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1465">#1465</a> contributed by <a href="https://github.com/SimenB"><code>@​SimenB</code></a>)</li>
<li>Don't use a global throaway timer for constructing server calls (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1463">#1463</a> contributed by <a href="https://github.com/azban"><code>@​azban</code></a>)</li>
<li>Consistently set <code>servername</code> connection option to support SNI (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1466">#1466</a>)</li>
<li>Don't block in <code>Server#tryShutdown</code> waiting for already-closed sessions to close (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1467">#1467</a>)</li>
<li>Export <code>propagate</code> constants (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1468">#1468</a>)</li>
<li>Add port number to <code>:authority</code> header, but leave it out of <code>service_url</code> passed to metadata generator call credential callbacks (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1478">#1478</a>)</li>
<li>Ensure only one read is pending at a time when handling streams (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1479">#1479</a>)</li>
<li>Add <code>priority</code> and <code>weighted_target</code> load balancing policies internally for use in future features (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1433">#1433</a>, <a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1449">#1449</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.0.5</h2>
<ul>
<li>Add support for <code>grpc.enable_http_proxy</code> channel option to disable connecting through proxies (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1454">#1454</a> contributed by <a href="https://github.com/badsyntax"><code>@​badsyntax</code></a>)</li>
<li>Don't push messages after ending a call (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1436">#1436</a>)</li>
<li>Move google-auth-library to a peer dependency (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1443">#1443</a>)</li>
<li>Properly back off when failing to connect to a server (<a href="https://github-redirect.dependabot.com/grpc/grpc-node/issues/1444">#1444</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/grpc/grpc-node/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.0.3&new-version=1.1.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-sdk-node/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 00:48:19 +0000 UTC
    </div>
</div>

