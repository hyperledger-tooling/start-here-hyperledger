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
                PR <a href="https://github.com/hyperledger/cello/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    [#248 Add create network page]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                You can create a network by this page

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-30 12:10:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/247" class=".btn">#247</a>
            </td>
            <td>
                <b>
                    Bump ws from 7.4.2 to 7.4.6 in /build_image/dockerhub/v0.9.0/user-dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ws](https://github.com/websockets/ws) from 7.4.2 to 7.4.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>7.4.6</h2>
<h1>Bug fixes</h1>
<ul>
<li>Fixed a ReDoS vulnerability (00c425ec).</li>
</ul>
<p>A specially crafted value of the <code>Sec-Websocket-Protocol</code> header could be used
to significantly slow down a ws server.</p>
<pre lang="js"><code>for (const length of [1000, 2000, 4000, 8000, 16000, 32000]) {
  const value = 'b' + ' '.repeat(length) + 'x';
  const start = process.hrtime.bigint();
<p>value.trim().split(/ *, */);</p>
<p>const end = process.hrtime.bigint();</p>
<p>console.log('length = %d, time = %f ns', length, end - start);
}
</code></pre></p>
<p>The vulnerability was responsibly disclosed along with a fix in private by
<a href="https://github.com/robmcl4">Robert McLaughlin</a> from University of California, Santa Barbara.</p>
<p>In vulnerable versions of ws, the issue can be mitigated by reducing the maximum
allowed length of the request headers using the <a href="https://nodejs.org/api/cli.html#cli_max_http_header_size_size"><code>--max-http-header-size=size</code></a>
and/or the <a href="https://nodejs.org/api/http.html#http_http_createserver_options_requestlistener"><code>maxHeaderSize</code></a> options.</p>
<h2>7.4.5</h2>
<h1>Bug fixes</h1>
<ul>
<li>UTF-8 validation is now done even if <code>utf-8-validate</code> is not installed
(23ba6b29).</li>
<li>Fixed an edge case where <code>websocket.close()</code> and <code>websocket.terminate()</code> did
not close the connection (67e25ff5).</li>
</ul>
<h2>7.4.4</h2>
<h1>Bug fixes</h1>
<ul>
<li>Fixed a bug that could cause the process to crash when using the
permessage-deflate extension (92774377).</li>
</ul>
<h2>7.4.3</h2>
<h1>Bug fixes</h1>
<ul>
<li>The deflate/inflate stream is now reset instead of reinitialized when context
takeover is disabled (<a href="https://github-redirect.dependabot.com/websockets/ws/issues/1840">#1840</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/f5297f7090f6a628832a730187c5b3a06a247f00"><code>f5297f7</code></a> [dist] 7.4.6</li>
<li><a href="https://github.com/websockets/ws/commit/00c425ec77993773d823f018f64a5c44e17023ff"><code>00c425e</code></a> [security] Fix ReDoS vulnerability</li>
<li><a href="https://github.com/websockets/ws/commit/990306d1446faf346c76452409a4c11455690514"><code>990306d</code></a> [lint] Fix prettier error</li>
<li><a href="https://github.com/websockets/ws/commit/32e3a8439b7c8273b44fe1adb5682f529e34d0ba"><code>32e3a84</code></a> [security] Remove reference to Node Security Project</li>
<li><a href="https://github.com/websockets/ws/commit/8c914d18b86a7d1408884d18eeadae0fa41b0bb5"><code>8c914d1</code></a> [minor] Fix nits</li>
<li><a href="https://github.com/websockets/ws/commit/fc7e27d12ad0af90ce05302afc85c292024000b4"><code>fc7e27d</code></a> [ci] Test on node 16</li>
<li><a href="https://github.com/websockets/ws/commit/587c201bfc22c460658ca304d23477fc7ebd2a60"><code>587c201</code></a> [ci] Do not test on node 15</li>
<li><a href="https://github.com/websockets/ws/commit/f67271079755e79a1ac2b40f3f4efb94ca024539"><code>f672710</code></a> [dist] 7.4.5</li>
<li><a href="https://github.com/websockets/ws/commit/67e25ff50230d131d76b1061ca0be5c991df161f"><code>67e25ff</code></a> [fix] Fix case where <code>abortHandshake()</code> does not close the connection</li>
<li><a href="https://github.com/websockets/ws/commit/23ba6b2922f521f2b656891a997ab562b7139dd4"><code>23ba6b2</code></a> [fix] Make UTF-8 validation work even if utf-8-validate is not installed</li>
<li>Additional commits viewable in <a href="https://github.com/websockets/ws/compare/7.4.2...7.4.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ws&package-manager=npm_and_yarn&previous-version=7.4.2&new-version=7.4.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-05-29 23:36:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/246" class=".btn">#246</a>
            </td>
            <td>
                <b>
                    Create organization and create node at the same time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When creating an organization, you can select the number of peers and orderers。
*Create the certificate and configuration file and compress it into a zip file

Signed-off-by: XuHugo <xq-310@163.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 14:53:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/245" class=".btn">#245</a>
            </td>
            <td>
                <b>
                    [#224 Add networklist page]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add network list page,show all blockchian network in this page.

Signed-off-by: fengyang_sy <fengyang.09186@h3c.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 12:29:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    Retire maintainer Tong Li
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tong has been inactive for more than 3 months, and he will focus on
other project, without time to continue the contribution.

Thanks for his past contributions.

Signed-off-by: Baohua Yang <yangbaohua@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 20:32:35 +0000 UTC
    </div>
</div>

