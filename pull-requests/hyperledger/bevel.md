---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2094" class=".btn">#2094</a>
            </td>
            <td>
                <b>
                    Bump express from 4.16.4 to 4.17.3 in /examples/supplychain-app/fabric/express_nodeJs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.16.4 to 4.17.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.17.3</h2>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
<li>deps: negotiator@0.6.3</li>
</ul>
</li>
<li>deps: body-parser@1.19.2
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7</li>
<li>deps: raw-body@2.4.3</li>
</ul>
</li>
<li>deps: cookie@0.4.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>pref: remove unnecessary regexp for trust proxy</li>
</ul>
<h2>4.17.2</h2>
<ul>
<li>Fix handling of <code>undefined</code> in <code>res.jsonp</code></li>
<li>Fix handling of <code>undefined</code> when <code>&quot;json escape&quot;</code> is enabled</li>
<li>Fix incorrect middleware execution with unanchored <code>RegExp</code>s</li>
<li>Fix <code>res.jsonp(obj, status)</code> deprecation message</li>
<li>Fix typo in <code>res.is</code> JSDoc</li>
<li>deps: body-parser@1.19.1
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</li>
<li>deps: content-disposition@0.5.4
<ul>
<li>deps: safe-buffer@5.2.1</li>
</ul>
</li>
<li>deps: cookie@0.4.1
<ul>
<li>Fix <code>maxAge</code> option to reject invalid values</li>
</ul>
</li>
<li>deps: proxy-addr@~2.0.7
<ul>
<li>Use <code>req.socket</code> over deprecated <code>req.connection</code></li>
<li>deps: forwarded@0.2.0</li>
<li>deps: ipaddr.js@1.9.1</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: send@0.17.2
<ul>
<li>deps: http-errors@1.8.1</li>
<li>deps: ms@2.1.3</li>
<li>pref: ignore empty http tokens</li>
</ul>
</li>
<li>deps: serve-static@1.14.2
<ul>
<li>deps: send@0.17.2</li>
</ul>
</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
<h2>4.17.1</h2>
<ul>
<li>Revert &quot;Improve error message for <code>null</code>/<code>undefined</code> to <code>res.status</code>&quot;</li>
</ul>
<h2>4.17.0</h2>
<ul>
<li>Add <code>express.raw</code> to parse bodies into <code>Buffer</code></li>
<li>Add <code>express.text</code> to parse bodies into string</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.17.3 / 2022-02-16</h1>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
<li>deps: negotiator@0.6.3</li>
</ul>
</li>
<li>deps: body-parser@1.19.2
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7</li>
<li>deps: raw-body@2.4.3</li>
</ul>
</li>
<li>deps: cookie@0.4.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>pref: remove unnecessary regexp for trust proxy</li>
</ul>
<h1>4.17.2 / 2021-12-16</h1>
<ul>
<li>Fix handling of <code>undefined</code> in <code>res.jsonp</code></li>
<li>Fix handling of <code>undefined</code> when <code>&quot;json escape&quot;</code> is enabled</li>
<li>Fix incorrect middleware execution with unanchored <code>RegExp</code>s</li>
<li>Fix <code>res.jsonp(obj, status)</code> deprecation message</li>
<li>Fix typo in <code>res.is</code> JSDoc</li>
<li>deps: body-parser@1.19.1
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</li>
<li>deps: content-disposition@0.5.4
<ul>
<li>deps: safe-buffer@5.2.1</li>
</ul>
</li>
<li>deps: cookie@0.4.1
<ul>
<li>Fix <code>maxAge</code> option to reject invalid values</li>
</ul>
</li>
<li>deps: proxy-addr@~2.0.7
<ul>
<li>Use <code>req.socket</code> over deprecated <code>req.connection</code></li>
<li>deps: forwarded@0.2.0</li>
<li>deps: ipaddr.js@1.9.1</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: send@0.17.2
<ul>
<li>deps: http-errors@1.8.1</li>
<li>deps: ms@2.1.3</li>
<li>pref: ignore empty http tokens</li>
</ul>
</li>
<li>deps: serve-static@1.14.2
<ul>
<li>deps: send@0.17.2</li>
</ul>
</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
<h1>4.17.1 / 2019-05-25</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/3d7fce56a35f4f73fa437866cd1401587a212334"><code>3d7fce5</code></a> 4.17.3</li>
<li><a href="https://github.com/expressjs/express/commit/f9063712e01979588818b0756851053b5ee43d09"><code>f906371</code></a> build: update example dependencies</li>
<li><a href="https://github.com/expressjs/express/commit/6381bc6317ec8ffbf830e2d16677e4b5af37cc08"><code>6381bc6</code></a> deps: qs@6.9.7</li>
<li><a href="https://github.com/expressjs/express/commit/a00786309641731661edb4d826a6919330887ca7"><code>a007863</code></a> deps: body-parser@1.19.2</li>
<li><a href="https://github.com/expressjs/express/commit/e98f5848a0a496c0977a2d1734067b77f69de360"><code>e98f584</code></a> Revert &quot;build: use minimatch@3.0.4 for Node.js &lt; 4&quot;</li>
<li><a href="https://github.com/expressjs/express/commit/a65913776d0b16837364ee66caa1a7f38a9997c0"><code>a659137</code></a> tests: use strict mode</li>
<li><a href="https://github.com/expressjs/express/commit/a39e409cf3739ef9c9b597a9680813a34c3931c2"><code>a39e409</code></a> tests: prevent leaking changes to NODE_ENV</li>
<li><a href="https://github.com/expressjs/express/commit/82de4de5ab92e8237d713285104e4b8452927352"><code>82de4de</code></a> examples: fix path traversal in downloads example</li>
<li><a href="https://github.com/expressjs/express/commit/12310c52947ee159f7ecd63d125243cdca891135"><code>12310c5</code></a> build: use nyc for test coverage</li>
<li><a href="https://github.com/expressjs/express/commit/884657d54665f323c236055d6e3d3e85d96e5f08"><code>884657d</code></a> examples: remove bitwise syntax for includes check</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.16.4...4.17.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.16.4&new-version=4.17.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 12:27:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2093" class=".btn">#2093</a>
            </td>
            <td>
                <b>
                    [besu] refactoring charts to removing dependency on external tools and artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: adityajoshi12 <adityaprakashjoshi1@gmail.com>

**Changelog**
- Updated the charts to remove dependency of tools like jq, curl and openssl
- Added utility binaries to apline container image

 

**Reviewed by**
@developer_github_id

 

**Linked issue**
#2073 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 12:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2092" class=".btn">#2092</a>
            </td>
            <td>
                <b>
                    Bump express from 4.16.4 to 4.17.3 in /examples/supplychain-app/corda/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.16.4 to 4.17.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.17.3</h2>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
<li>deps: negotiator@0.6.3</li>
</ul>
</li>
<li>deps: body-parser@1.19.2
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7</li>
<li>deps: raw-body@2.4.3</li>
</ul>
</li>
<li>deps: cookie@0.4.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>pref: remove unnecessary regexp for trust proxy</li>
</ul>
<h2>4.17.2</h2>
<ul>
<li>Fix handling of <code>undefined</code> in <code>res.jsonp</code></li>
<li>Fix handling of <code>undefined</code> when <code>&quot;json escape&quot;</code> is enabled</li>
<li>Fix incorrect middleware execution with unanchored <code>RegExp</code>s</li>
<li>Fix <code>res.jsonp(obj, status)</code> deprecation message</li>
<li>Fix typo in <code>res.is</code> JSDoc</li>
<li>deps: body-parser@1.19.1
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</li>
<li>deps: content-disposition@0.5.4
<ul>
<li>deps: safe-buffer@5.2.1</li>
</ul>
</li>
<li>deps: cookie@0.4.1
<ul>
<li>Fix <code>maxAge</code> option to reject invalid values</li>
</ul>
</li>
<li>deps: proxy-addr@~2.0.7
<ul>
<li>Use <code>req.socket</code> over deprecated <code>req.connection</code></li>
<li>deps: forwarded@0.2.0</li>
<li>deps: ipaddr.js@1.9.1</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: send@0.17.2
<ul>
<li>deps: http-errors@1.8.1</li>
<li>deps: ms@2.1.3</li>
<li>pref: ignore empty http tokens</li>
</ul>
</li>
<li>deps: serve-static@1.14.2
<ul>
<li>deps: send@0.17.2</li>
</ul>
</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
<h2>4.17.1</h2>
<ul>
<li>Revert &quot;Improve error message for <code>null</code>/<code>undefined</code> to <code>res.status</code>&quot;</li>
</ul>
<h2>4.17.0</h2>
<ul>
<li>Add <code>express.raw</code> to parse bodies into <code>Buffer</code></li>
<li>Add <code>express.text</code> to parse bodies into string</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.17.3 / 2022-02-16</h1>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
<li>deps: negotiator@0.6.3</li>
</ul>
</li>
<li>deps: body-parser@1.19.2
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7</li>
<li>deps: raw-body@2.4.3</li>
</ul>
</li>
<li>deps: cookie@0.4.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>pref: remove unnecessary regexp for trust proxy</li>
</ul>
<h1>4.17.2 / 2021-12-16</h1>
<ul>
<li>Fix handling of <code>undefined</code> in <code>res.jsonp</code></li>
<li>Fix handling of <code>undefined</code> when <code>&quot;json escape&quot;</code> is enabled</li>
<li>Fix incorrect middleware execution with unanchored <code>RegExp</code>s</li>
<li>Fix <code>res.jsonp(obj, status)</code> deprecation message</li>
<li>Fix typo in <code>res.is</code> JSDoc</li>
<li>deps: body-parser@1.19.1
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</li>
<li>deps: content-disposition@0.5.4
<ul>
<li>deps: safe-buffer@5.2.1</li>
</ul>
</li>
<li>deps: cookie@0.4.1
<ul>
<li>Fix <code>maxAge</code> option to reject invalid values</li>
</ul>
</li>
<li>deps: proxy-addr@~2.0.7
<ul>
<li>Use <code>req.socket</code> over deprecated <code>req.connection</code></li>
<li>deps: forwarded@0.2.0</li>
<li>deps: ipaddr.js@1.9.1</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: send@0.17.2
<ul>
<li>deps: http-errors@1.8.1</li>
<li>deps: ms@2.1.3</li>
<li>pref: ignore empty http tokens</li>
</ul>
</li>
<li>deps: serve-static@1.14.2
<ul>
<li>deps: send@0.17.2</li>
</ul>
</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
<h1>4.17.1 / 2019-05-25</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/3d7fce56a35f4f73fa437866cd1401587a212334"><code>3d7fce5</code></a> 4.17.3</li>
<li><a href="https://github.com/expressjs/express/commit/f9063712e01979588818b0756851053b5ee43d09"><code>f906371</code></a> build: update example dependencies</li>
<li><a href="https://github.com/expressjs/express/commit/6381bc6317ec8ffbf830e2d16677e4b5af37cc08"><code>6381bc6</code></a> deps: qs@6.9.7</li>
<li><a href="https://github.com/expressjs/express/commit/a00786309641731661edb4d826a6919330887ca7"><code>a007863</code></a> deps: body-parser@1.19.2</li>
<li><a href="https://github.com/expressjs/express/commit/e98f5848a0a496c0977a2d1734067b77f69de360"><code>e98f584</code></a> Revert &quot;build: use minimatch@3.0.4 for Node.js &lt; 4&quot;</li>
<li><a href="https://github.com/expressjs/express/commit/a65913776d0b16837364ee66caa1a7f38a9997c0"><code>a659137</code></a> tests: use strict mode</li>
<li><a href="https://github.com/expressjs/express/commit/a39e409cf3739ef9c9b597a9680813a34c3931c2"><code>a39e409</code></a> tests: prevent leaking changes to NODE_ENV</li>
<li><a href="https://github.com/expressjs/express/commit/82de4de5ab92e8237d713285104e4b8452927352"><code>82de4de</code></a> examples: fix path traversal in downloads example</li>
<li><a href="https://github.com/expressjs/express/commit/12310c52947ee159f7ecd63d125243cdca891135"><code>12310c5</code></a> build: use nyc for test coverage</li>
<li><a href="https://github.com/expressjs/express/commit/884657d54665f323c236055d6e3d3e85d96e5f08"><code>884657d</code></a> examples: remove bitwise syntax for includes check</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.16.4...4.17.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.16.4&new-version=4.17.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 06:52:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2091" class=".btn">#2091</a>
            </td>
            <td>
                <b>
                    Bump qs, body-parser and express in /examples/supplychain-app/corda/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) to 6.11.0 and updates ancestor dependencies [qs](https://github.com/ljharb/qs), [body-parser](https://github.com/expressjs/body-parser) and [express](https://github.com/expressjs/express). These dependencies need to be updated together.

Updates `qs` from 6.5.2 to 6.11.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.11.0</strong></h2>
<ul>
<li>[New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/442">#442</a>)</li>
<li>[readme] fix version badge</li>
</ul>
<h2><strong>6.10.5</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/434">#434</a>)</li>
</ul>
<h2><strong>6.10.4</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/441">#441</a>)</li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[actions] reuse common workflows</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.2</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: actually fix cyclic references (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/426">#426</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[actions] update codecov uploader</li>
<li>[actions] update workflows</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>object-inspect</code>, <code>safe-publish-latest</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.1</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: avoid exception on repeated object values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/402">#402</a>)</li>
</ul>
<h2><strong>6.10.0</strong></h2>
<ul>
<li>[New] <code>stringify</code>: throw on cycles, instead of an infinite loop (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/395">#395</a>, <a href="https://github-redirect.dependabot.com/ljharb/qs/issues/394">#394</a>, <a href="https://github-redirect.dependabot.com/ljharb/qs/issues/393">#393</a>)</li>
<li>[New] <code>parse</code>: add <code>allowSparse</code> option for collapsing arrays with missing indices (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/312">#312</a>)</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] only run <code>npm run dist</code> in publish, not install</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbols</code>, <code>tape</code></li>
<li>[Tests] fix tests on node v0.6</li>
<li>[Tests] use <code>ljharb/actions/node/install</code> instead of <code>ljharb/actions/node/run</code></li>
<li>[Tests] Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
</ul>
<h2><strong>6.9.7</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/56763c12ec4fbf723333cbb32371cbd386c33cbb"><code>56763c1</code></a> v6.11.0</li>
<li><a href="https://github.com/ljharb/qs/commit/ddd3e293b801df7a06cb7f2746462a6ca1dd3fb2"><code>ddd3e29</code></a> [readme] fix version badge</li>
<li><a href="https://github.com/ljharb/qs/commit/c31347299f34afca90e8b5ff793eb4d0f77cfa56"><code>c313472</code></a> [New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option</li>
<li><a href="https://github.com/ljharb/qs/commit/95bc0185e157d400da4f43f1fcf1c7f008fd847e"><code>95bc018</code></a> v6.10.5</li>
<li><a href="https://github.com/ljharb/qs/commit/0e903c0a9092618756b0962f1b80655ac0da436a"><code>0e903c0</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit `[...</li>
<li><a href="https://github.com/ljharb/qs/commit/ba9703c0340dfdeb73cb4387d6ab32c37768aa5b"><code>ba9703c</code></a> v6.10.4</li>
<li><a href="https://github.com/ljharb/qs/commit/4e440195c7647f21c20bb76340774cb3a0cb6eac"><code>4e44019</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a s...</li>
<li><a href="https://github.com/ljharb/qs/commit/113b990ed23ae8d6f670eb879e16ed105cd9081b"><code>113b990</code></a> [Dev Deps] update <code>object-inspect</code></li>
<li><a href="https://github.com/ljharb/qs/commit/c77f38f7174b9f10e8937e0f601fa1e6f0373b33"><code>c77f38f</code></a> [Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>tape</code></li>
<li><a href="https://github.com/ljharb/qs/commit/2cf45b2dcd31a6d5c7fc16f33c7148fade0eef1e"><code>2cf45b2</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.11.0">compare view</a></li>
</ul>
</details>
<br />

Updates `body-parser` from 1.18.3 to 1.20.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/releases">body-parser's releases</a>.</em></p>
<blockquote>
<h2>1.20.0</h2>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h2>1.19.2</h2>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h2>1.19.1</h2>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
<h2>1.19.0</h2>
<ul>
<li>deps: bytes@3.1.0
<ul>
<li>Add petabyte (<code>pb</code>) support</li>
</ul>
</li>
<li>deps: http-errors@1.7.2
<ul>
<li>Set constructor name when possible</li>
<li>deps: setprototypeof@1.1.1</li>
<li>deps: statuses@'&gt;= 1.5.0 &lt; 2'</li>
</ul>
</li>
<li>deps: iconv-lite@0.4.24
<ul>
<li>Added encoding MIK</li>
</ul>
</li>
<li>deps: qs@6.7.0
<ul>
<li>Fix parsing array brackets after index</li>
</ul>
</li>
<li>deps: raw-body@2.4.0
<ul>
<li>deps: bytes@3.1.0</li>
<li>deps: http-errors@1.7.2</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/blob/master/HISTORY.md">body-parser's changelog</a>.</em></p>
<blockquote>
<h1>1.20.1 / 2022-10-06</h1>
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
<h1>1.20.0 / 2022-04-02</h1>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h1>1.19.2 / 2022-02-15</h1>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h1>1.19.1 / 2021-12-10</h1>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
<h1>1.19.0 / 2019-04-25</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/body-parser/commit/830bdfbee021d540a742de857dcbd43f40563a02"><code>830bdfb</code></a> 1.20.1</li>
<li><a href="https://github.com/expressjs/body-parser/commit/ecad1ccf9eefe61a4ba5b8354d914e262eba7648"><code>ecad1cc</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/03b93cf9f11c201631a8cefa09df08feb6f2bb00"><code>03b93cf</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/2c611fcda0fe54043eb8c914f1fde412ba9432c0"><code>2c611fc</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/body-parser/commit/f199e94b115de00feae7ae5559638c0c52019b2e"><code>f199e94</code></a> perf: remove unnecessary object clone</li>
<li><a href="https://github.com/expressjs/body-parser/commit/0123e12d6b6db1bdb66b271b2822b5070096dc32"><code>0123e12</code></a> build: Node.js@18.9</li>
<li><a href="https://github.com/expressjs/body-parser/commit/de1e6c2b390244e486f235151d8e6b9646f2122f"><code>de1e6c2</code></a> build: Node.js@16.17</li>
<li><a href="https://github.com/expressjs/body-parser/commit/477ff13b9c608800cc25331e0de6da6cd4970ee3"><code>477ff13</code></a> build: eslint-plugin-import@2.26.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/40c3fff30b0d88763e89f1a41ed76d2cf8aa1b14"><code>40c3fff</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/4aa84b70c298354e902edfc4a85ddfdc9fa905c8"><code>4aa84b7</code></a> build: supertest@6.2.4</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/body-parser/compare/1.18.3...1.20.1">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.16.4 to 4.18.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.18.2</h2>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h2>4.18.1</h2>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h2>4.18.0</h2>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0
<ul>
<li>Fix emitted 416 error missing headers property</li>
<li>Limit the headers removed for 304 response</li>
<li>deps: depd@2.0.0</li>
<li>deps: destroy@1.2.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.18.2 / 2022-10-08</h1>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h1>4.18.1 / 2022-04-29</h1>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h1>4.18.0 / 2022-04-25</h1>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/8368dc178af16b91b576c4c1d135f701a0007e5d"><code>8368dc1</code></a> 4.18.2</li>
<li><a href="https://github.com/expressjs/express/commit/61f40491222dbede653b9938e6a4676f187aab44"><code>61f4049</code></a> docs: replace Freenode with Libera Chat</li>
<li><a href="https://github.com/expressjs/express/commit/bb7907b932afe3a19236a642f6054b6c8f7349a0"><code>bb7907b</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/express/commit/f56ce73186e885a938bfdb3d3d1005a58e6ae12b"><code>f56ce73</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/express/commit/24b3dc551670ac4fb0cd5a2bd5ef643c9525e60f"><code>24b3dc5</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/express/commit/689d175b8b39d8860b81d723233fb83d15201827"><code>689d175</code></a> deps: body-parser@1.20.1</li>
<li><a href="https://github.com/expressjs/express/commit/340be0f79afb9b3176afb76235aa7f92acbd5050"><code>340be0f</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/express/commit/33e8dc303af9277f8a7e4f46abfdcb5e72f6797b"><code>33e8dc3</code></a> docs: use Node.js name style</li>
<li><a href="https://github.com/expressjs/express/commit/644f6464b9f61cbafa8f880636b1aa5237d95bad"><code>644f646</code></a> build: supertest@6.2.4</li>
<li><a href="https://github.com/expressjs/express/commit/ecd7572f1e920b7a512452b8d9806ae617a99c54"><code>ecd7572</code></a> build: Node.js@14.20</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.16.4...4.18.2">compare view</a></li>
</ul>
</details>
<br />


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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 06:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2089" class=".btn">#2089</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /examples/supplychain-app/besu/express_nodeJS
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 03:03:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2088" class=".btn">#2088</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /examples/supplychain-app/supplychain-frontend
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 02:44:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2087" class=".btn">#2087</a>
            </td>
            <td>
                <b>
                    Bump qs from 6.5.2 to 6.5.3 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) from 6.5.2 to 6.5.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.5.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix]<code> </code>utils.merge`: avoid a crash with a null target and a truthy non-array source</li>
<li>[Fix] correctly parse nested arrays</li>
<li>[Fix] <code>stringify</code>: fix a crash with <code>strictNullHandling</code> and a custom <code>filter</code>/<code>serializeDate</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/279">#279</a>)</li>
<li>[Fix] <code>utils</code>: <code>merge</code>: fix crash when <code>source</code> is a truthy primitive &amp; no options are provided</li>
<li>[Fix] when <code>parseArrays</code> is false, properly handle keys ending in <code>[]</code></li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and an array source</li>
<li>[Refactor] <code>utils</code>: reduce observable [[Get]]s</li>
<li>[Refactor] use cached <code>Array.isArray</code></li>
<li>[Refactor] <code>stringify</code>: Avoid arr = arr.concat(...), push to the existing instance (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/269">#269</a>)</li>
<li>[Refactor] <code>parse</code>: only need to reassign the var once</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li>[Docs] Clarify the need for &quot;arrayLimit&quot; option</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] add FUNDING.yml</li>
<li>[actions] backport actions from main</li>
<li>[Tests] always use <code>String(x)</code> over <code>x.toString()</code></li>
<li>[Tests] remove nonexistent tape option</li>
<li>[Dev Deps] backport from main</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/298bfa55d6db00ddea78dd0333509aadf9bb3077"><code>298bfa5</code></a> v6.5.3</li>
<li><a href="https://github.com/ljharb/qs/commit/ed0f5dcbef4b168a8ae299d78b1e4a2e9b1baf1f"><code>ed0f5dc</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/691e739cfa40cd42604dc05a54e6154371a429ab"><code>691e739</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/1072d57d38a690e1ad7616dced44390bffedcbb2"><code>1072d57</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/12ac1c403aaa04d1a34844f514ed9f9abfb76e64"><code>12ac1c4</code></a> [meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/0338716b09fdbd4711823eeb0a14e556a2498e7a"><code>0338716</code></a> [actions] backport actions from main</li>
<li><a href="https://github.com/ljharb/qs/commit/5639c20ce0a7c1332200a3181339331483e5a3a1"><code>5639c20</code></a> Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li><a href="https://github.com/ljharb/qs/commit/51b8a0b1b213596dd1702b837f5e7dec2229793d"><code>51b8a0b</code></a> add FUNDING.yml</li>
<li><a href="https://github.com/ljharb/qs/commit/45f675936e742d92fac8d4dae5cfc385c576a977"><code>45f6759</code></a> [Fix] fix for an impossible situation: when the formatter is called with a no...</li>
<li><a href="https://github.com/ljharb/qs/commit/f814a7f8f2af059f8158f7e4b2bf8b46aeb62cd3"><code>f814a7f</code></a> [Dev Deps] backport from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.5.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=qs&package-manager=npm_and_yarn&previous-version=6.5.2&new-version=6.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 15:50:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2084" class=".btn">#2084</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /examples/supplychain-app/quorum/smartContracts
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 22:17:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2083" class=".btn">#2083</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /platforms/r3-corda/images/networkmap/website
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 17:25:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2082" class=".btn">#2082</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /examples/supplychain-app/quorum/express_nodeJS
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 10:53:13 +0000 UTC
    </div>
</div>

