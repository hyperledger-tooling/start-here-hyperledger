---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    The user logs in through the front page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *The user logins through the front page，and get token.

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-03 13:48:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    fix #264: fix swagger api doc loading error.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                failed to load swagger api definition, fixed it by removing undefined fields and serailizers.

Close #264

Signed-off-by: Yuanmao Zhu <zhu.yuanmao18@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 19:35:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    Debug the registration part of the front end
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                You can register an organization to the backend through the front page；

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 09:55:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 3.3.0 to 3.3.2 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 3.3.0 to 3.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>3.3.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>prevent DoS (OOM) via massive packets (<a href="https://github-redirect.dependabot.com/Automattic/socket.io-parser/issues/95">#95</a>) (<a href="https://github.com/Automattic/socket.io-parser/commit/89197a05c43b18cc4569fd178d56e7bb8f403865">89197a0</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/Automattic/socket.io-parser/compare/3.3.1...3.3.2">https://github.com/Automattic/socket.io-parser/compare/3.3.1...3.3.2</a></li>
</ul>
<h2>3.3.1</h2>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/3.3.0...3.3.1">https://github.com/socketio/socket.io-parser/compare/3.3.0...3.3.1</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/3.3.2/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/Automattic/socket.io-parser/compare/3.3.1...3.3.2">3.3.2</a> (2021-01-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>prevent DoS (OOM) via massive packets (<a href="https://github-redirect.dependabot.com/Automattic/socket.io-parser/issues/95">#95</a>) (<a href="https://github.com/Automattic/socket.io-parser/commit/89197a05c43b18cc4569fd178d56e7bb8f403865">89197a0</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/3.3.0...3.3.1">3.3.1</a> (2020-09-30)</h2>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/3b0a3925fd9f765228e5d06e4a0cc90d81a60d0e"><code>3b0a392</code></a> chore(release): 3.3.2</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/89197a05c43b18cc4569fd178d56e7bb8f403865"><code>89197a0</code></a> fix: prevent DoS (OOM) via massive packets (<a href="https://github-redirect.dependabot.com/socketio/socket.io-parser/issues/95">#95</a>)</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/25ca624b0d9eddc54a0dbaecc535cdf400722169"><code>25ca624</code></a> chore(release): 3.3.1</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b51b39b78d85841a5659778917f240d407fdbce1"><code>b51b39b</code></a> test: use Node.js 10 for the browser tests</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/4184e465344c7ebd1d586e35a53bfad1ab5cfcea"><code>4184e46</code></a> chore: bump component-emitter dependency</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/3.3.0...3.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=3.3.0&new-version=3.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 18:42:01 +0000 UTC
    </div>
</div>

