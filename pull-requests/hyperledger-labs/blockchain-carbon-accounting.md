---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/659" class=".btn">#659</a>
            </td>
            <td>
                <b>
                    Fix for frontend issue tokens form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix form conditions to issue tokens:
    - directly to consumers
    - to industry as part of a new or exisiting carbon tracker token

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 19:01:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/658" class=".btn">#658</a>
            </td>
            <td>
                <b>
                    Bump @xmldom/xmldom from 0.7.6 to 0.7.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@xmldom/xmldom](https://github.com/xmldom/xmldom) from 0.7.6 to 0.7.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/releases"><code>@​xmldom/xmldom</code>'s releases</a>.</em></p>
<blockquote>
<h2>0.7.9</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.8...0.7.9">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Properly check nodes before replacement <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/457"><code>[#457](https://github.com/xmldom/xmldom/issues/457)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/455"><code>[#455](https://github.com/xmldom/xmldom/issues/455)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/456"><code>[#456](https://github.com/xmldom/xmldom/issues/456)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/edemaine"><code>@​edemaine</code></a>, <a href="https://github.com/pedro-l9"><code>@​pedro-l9</code></a>, for your contributions</p>
<h2>0.7.8</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.7...0.7.8">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2>0.7.7</h2>
<p><a href="https://github.com/xmldom/xmldom/compare/0.7.6...0.7.7">Commits</a></p>
<h3>Fixed</h3>
<ul>
<li>Security: Prevent inserting DOM nodes when they are not well-formed <a href="https://github.com/xmldom/xmldom/security/advisories/GHSA-crh6-fp67-6883"><code>CVE-2022-39353</code></a>
In case such a DOM would be created, the part that is not well-formed will be transformed into text nodes, in which xml specific characters like <code>&lt;</code> and <code>&gt;</code> are encoded accordingly.
In the upcoming version 0.9.0 those text nodes will no longer be added and an error will be thrown instead.
This change can break your code, if you relied on this behavior, e.g. multiple root elements in the past. We consider it more important to align with the specs that we want to be aligned with, considering the potential security issues that might derive from people not being aware of the difference in behavior.
Related Spec: <a href="https://dom.spec.whatwg.org/#concept-node-ensure-pre-insertion-validity">https://dom.spec.whatwg.org/#concept-node-ensure-pre-insertion-validity</a></li>
</ul>
<p>Thank you, <a href="https://github.com/frumioj"><code>@​frumioj</code></a>, <a href="https://github.com/cjbarth"><code>@​cjbarth</code></a>, <a href="https://github.com/markgollnick"><code>@​markgollnick</code></a> for your contributions</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/xmldom/xmldom/blob/master/CHANGELOG.md"><code>@​xmldom/xmldom</code>'s changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.8...0.7.9">0.7.9</a></h2>
<h3>Fixed</h3>
<ul>
<li>Properly check nodes before replacement <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/457"><code>[#457](https://github.com/xmldom/xmldom/issues/457)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/455"><code>[#455](https://github.com/xmldom/xmldom/issues/455)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/456"><code>[#456](https://github.com/xmldom/xmldom/issues/456)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/edemaine"><code>@​edemaine</code></a>, <a href="https://github.com/pedro-l9"><code>@​pedro-l9</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.5...0.9.0-beta.6">0.9.0-beta.6</a></h2>
<h3>Fixed</h3>
<ul>
<li>Properly check nodes before replacement <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/457"><code>[#457](https://github.com/xmldom/xmldom/issues/457)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/455"><code>[#455](https://github.com/xmldom/xmldom/issues/455)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/456"><code>[#456](https://github.com/xmldom/xmldom/issues/456)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/edemaine"><code>@​edemaine</code></a>, <a href="https://github.com/pedro-l9"><code>@​pedro-l9</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.4...0.9.0-beta.5">0.9.0-beta.5</a></h2>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.8.4...0.8.5">0.8.5</a></h2>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.7.7...0.7.8">0.7.8</a></h2>
<h3>Fixed</h3>
<ul>
<li>fix: Restore ES5 compatibility <a href="https://github-redirect.dependabot.com/xmldom/xmldom/pull/452"><code>[#452](https://github.com/xmldom/xmldom/issues/452)</code></a> / <a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/453"><code>[#453](https://github.com/xmldom/xmldom/issues/453)</code></a></li>
</ul>
<p>Thank you, <a href="https://github.com/fengxinming"><code>@​fengxinming</code></a>, for your contributions</p>
<h2><a href="https://github.com/xmldom/xmldom/compare/0.9.0-beta.3...0.9.0-beta.4">0.9.0-beta.4</a></h2>
<h3>Fixed</h3>
<ul>
<li>Security: Prevent inserting DOM nodes when they are not well-formed <a href="https://github.com/xmldom/xmldom/security/advisories/GHSA-crh6-fp67-6883"><code>CVE-2022-39353</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/xmldom/xmldom/commit/927392f627e8f9cf1ea051612c7996596a904c78"><code>927392f</code></a> 0.7.9</li>
<li><a href="https://github.com/xmldom/xmldom/commit/99cfe62576e563234b928db9305290dfb3a96c03"><code>99cfe62</code></a> fix: Properly check nodes before replacement (<a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/457">#457</a>)</li>
<li><a href="https://github.com/xmldom/xmldom/commit/a627fbcd8b75304abe9142ca963c25ca773685d7"><code>a627fbc</code></a> chore: Preconfigure &quot;patch&quot; version in release script</li>
<li><a href="https://github.com/xmldom/xmldom/commit/0d6e3a132ec6eb32a67cfca327477a2098d4b55c"><code>0d6e3a1</code></a> 0.7.8</li>
<li><a href="https://github.com/xmldom/xmldom/commit/74e25a6763cc6afd0100b82b137f78af649741f8"><code>74e25a6</code></a> fix: Restore ES5 compatibility (<a href="https://github-redirect.dependabot.com/xmldom/xmldom/issues/452">#452</a>)</li>
<li><a href="https://github.com/xmldom/xmldom/commit/fe5b043fd07bbfed7f039b77d0b9e1a1eb832a2a"><code>fe5b043</code></a> 0.7.7</li>
<li><a href="https://github.com/xmldom/xmldom/commit/8a3173dc3bb7edb8619e914b8a2d366cc7cc8401"><code>8a3173d</code></a> docs: Prepare CHANGELOG for 0.7.7</li>
<li><a href="https://github.com/xmldom/xmldom/commit/c02f786216bed70825f9a351c65e61500f51e931"><code>c02f786</code></a> Merge pull request from GHSA-crh6-fp67-6883</li>
<li>See full diff in <a href="https://github.com/xmldom/xmldom/compare/0.7.6...0.7.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@xmldom/xmldom&package-manager=npm_and_yarn&previous-version=0.7.6&new-version=0.7.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 18:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    fix error in react app
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
        Created At 2022-12-05 17:11:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    fix links in READMEs and docuemntation, #655
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
        Created At 2022-12-02 16:33:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/654" class=".btn">#654</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.0.4 to 4.0.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.0.4 to 4.0.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>4.0.5</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/socketio/socket.io-parser/commit/b559f050ee02bd90bd853b9823f8de7fa94a80d4">b559f05</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.0.4...4.0.5">https://github.com/socketio/socket.io-parser/compare/4.0.4...4.0.5</a></li>
<li>Branch: <a href="https://github.com/socketio/socket.io-parser/tree/4.0.x">4.0.x</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/main/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
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
<ul>
<li>allow objects with a null prototype in binary packets (<a href="https://github-redirect.dependabot.com/socketio/socket.io-parser/issues/114">#114</a>) (<a href="https://github.com/socketio/socket.io-parser/commit/7f6b262ac83bdf43c53a7eb02417e56e0cf491c8">7f6b262</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.1.0...4.1.1">4.1.1</a> (2021-10-14)</h2>
<h1><a href="https://github.com/socketio/socket.io-parser/compare/4.0.4...4.1.0">4.1.0</a> (2021-10-11)</h1>
<h3>Features</h3>
<ul>
<li>provide an ESM build with and without debug (<a href="https://github.com/socketio/socket.io-parser/commit/388c616a9221e4341945f8487e729e93a81d2da5">388c616</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/f3329eb5a46b215a3fdf91b6008c56cf177a4124"><code>f3329eb</code></a> chore(release): 4.0.5</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b559f050ee02bd90bd853b9823f8de7fa94a80d4"><code>b559f05</code></a> fix: check the format of the index of each attachment</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/4.0.4...4.0.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.0.4&new-version=4.0.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 19:57:52 +0000 UTC
    </div>
</div>

