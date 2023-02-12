---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/376" class=".btn">#376</a>
            </td>
            <td>
                <b>
                    Bump cacheable-request and nodemon in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [cacheable-request](https://github.com/jaredwray/cacheable-request). It's no longer used after updating ancestor dependency [nodemon](https://github.com/remy/nodemon). These dependencies need to be updated together.

Removes `cacheable-request`

Updates `nodemon` from 2.0.18 to 2.0.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remy/nodemon/releases">nodemon's releases</a>.</em></p>
<blockquote>
<h2>v2.0.20</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.19...v2.0.20">2.0.20</a> (2022-09-16)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove postinstall script (<a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0">e099e91</a>)</li>
</ul>
<h2>v2.0.19</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.19">2.0.19</a> (2022-07-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Replace update notifier with simplified deps (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2033">#2033</a>) (<a href="https://github.com/remy/nodemon/commit/176c4a6bed989fe94f103c905e5eee341d26794d">176c4a6</a>), closes <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1961">#1961</a> <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2028">#2028</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0"><code>e099e91</code></a> fix: remove postinstall script</li>
<li><a href="https://github.com/remy/nodemon/commit/05de353d4de1a7e1f2aa2c9bf641c3fe2d652122"><code>05de353</code></a> chore: supports</li>
<li><a href="https://github.com/remy/nodemon/commit/876d60c8a241f13376f1b32f853d48ae77ec69a4"><code>876d60c</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/188f2d3cdc960fce5d7413e1326da76bd5be780c"><code>188f2d3</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/a1ad44a876df74be742c64af5640b300c302b977"><code>a1ad44a</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/8abd3fc9daff813199042c26a1e8aa5691a5ab37"><code>8abd3fc</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/30c80f8a4eee379fa2ebad95b81c42ef11670829"><code>30c80f8</code></a> chore: add unused files to .npmignore (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2055">#2055</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/3dd38deb4a97a52608aac148200b48d844df0a66"><code>3dd38de</code></a> docs: added link on banner (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1944">#1944</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/fb51359dde4b4ad6081f6c2690d1052fc8f5fcaf"><code>fb51359</code></a> docs: add important note about ignore rules</li>
<li><a href="https://github.com/remy/nodemon/commit/8fe7d770d06305e5e7a4aa4ab4783d4b2c5eaac8"><code>8fe7d77</code></a> chore: supporters</li>
<li>Additional commits viewable in <a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.20">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 06:07:31 +0000 UTC
    </div>
</div>

