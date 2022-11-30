---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2222" class=".btn">#2222</a>
            </td>
            <td>
                <b>
                    fix(test-tooling): substrate test ledger fails if WS_PORT not specified
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docker expects environment variables passed to the container
to be strings.
The null coalescing code was making it so that if the test case
did not pass in a custom WS_PORT  env var, then it would default
to using a value for the port that was a number not a string.
This would crash the serialization logic within docker that was
trying to apply the environment variables to the container when
starting it.

Switching the type of 9944 default WS port to "9944" (string) fixes it.
Also specifying explicitly the `wsPort` variable's type to be
string so that the next time someone tries to make this mistake
the compiler will slap their hands right away.

Fixes #2213

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 18:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2221" class=".btn">#2221</a>
            </td>
            <td>
                <b>
                    build(deps): bump socket.io-parser from 3.3.2 to 3.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 3.3.2 to 3.3.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>3.3.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/Automattic/socket.io-parser/commit/fb21e422fc193b34347395a33e0f625bebc09983">fb21e42</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/Automattic/socket.io-parser/compare/3.3.2...3.3.3">https://github.com/Automattic/socket.io-parser/compare/3.3.2...3.3.3</a></li>
<li>Branch: <a href="https://github.com/socketio/socket.io-parser/tree/3.3.x">3.3.x</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/main/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/Automattic/socket.io-parser/compare/3.3.2...3.3.3">3.3.3</a> (2022-11-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/Automattic/socket.io-parser/commit/fb21e422fc193b34347395a33e0f625bebc09983">fb21e42</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/3.4.1...3.4.2">3.4.2</a> (2022-11-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/socketio/socket.io-parser/commit/04d23cecafe1b859fb03e0cbf6ba3b74dff56d14">04d23ce</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.0...4.2.1">4.2.1</a> (2022-06-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/socketio/socket.io-parser/commit/b5d0cb7dc56a0601a09b056beaeeb0e43b160050">b5d0cb7</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.0.4...4.0.5">4.0.5</a> (2022-06-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/socketio/socket.io-parser/commit/b559f050ee02bd90bd853b9823f8de7fa94a80d4">b559f05</a>)</li>
</ul>
<h1><a href="https://github.com/socketio/socket.io-parser/compare/4.1.2...4.2.0">4.2.0</a> (2022-04-17)</h1>
<h3>Features</h3>
<ul>
<li>allow the usage of custom replacer and reviver (<a href="https://github-redirect.dependabot.com/socketio/socket.io-parser/issues/112">#112</a>) (<a href="https://github.com/socketio/socket.io-parser/commit/b08bc1a93e8e3194b776c8a0bdedee1e29333680">b08bc1a</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.1.1...4.1.2">4.1.2</a> (2022-02-17)</h2>
<h3>Bug Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/cd11e38e1a3e2146617bc586f86512605607b212"><code>cd11e38</code></a> chore(release): 3.3.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/fb21e422fc193b34347395a33e0f625bebc09983"><code>fb21e42</code></a> fix: check the format of the index of each attachment</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/3.3.2...3.3.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=3.3.2&new-version=3.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 19:54:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2219" class=".btn">#2219</a>
            </td>
            <td>
                <b>
                    chore: update settings to rename
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 20:16:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2218" class=".btn">#2218</a>
            </td>
            <td>
                <b>
                    ci: set username and email for NPM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Semantic PR to version 5

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 16:14:53 +0000 UTC
    </div>
</div>

