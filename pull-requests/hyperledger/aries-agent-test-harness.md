---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    [#624] Add support for excludes in feature/scenario display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 14:08:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    [#622] Respect bash exit code from a test run for command chaining
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 08:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    Bump express from 4.17.1 to 4.17.3 in /aries-backchannels/verity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.17.1 to 4.17.3.
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
</blockquote>
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.17.1...4.17.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.17.1&new-version=4.17.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 21:43:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    Upgrade actions to latest versions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Wade Barnes <wade@neoterictech.ca>

This PR upgrades the GitHub Actions used to eliminate a number of deprecation warning, however it does not eliminate them all.  The `the-coding-turtle/ga-file-list` action does not have a release that fixes the node.js 12 warning and it also contains the older `set-output` syntax.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 21:21:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Test/multi cred proof rev 605
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 16:58:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Bump qs from 6.5.2 to 6.5.3 in /aries-backchannels/verity
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
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and a truthy non-array source</li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 00:58:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    [#612] Condensed view for feature/scenario display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 14:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    [#609] Upgrade to universalresolver/driver-did-sov:0.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 10:39:04 +0000 UTC
    </div>
</div>

