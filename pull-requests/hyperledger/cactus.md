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
                PR <a href="https://github.com/hyperledger/cactus/pull/2194" class=".btn">#2194</a>
            </td>
            <td>
                <b>
                    build: fix release automation - try #2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A second attempt at fixing the release automation.

The missing piece was that some of the Indy SDK dependencies
were not installed by default and we forgot to run the ci.sh
script to take care of that within this workflow action.

With this fix now we have an additional step in the action which
takes care of installing the OS level build dependencies for
the project.

Fixes #1951
Fixes #2069
Fixes #2175

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 22:34:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2193" class=".btn">#2193</a>
            </td>
            <td>
                <b>
                    build(deps): bump loader-utils from 1.4.0 to 1.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [loader-utils](https://github.com/webpack/loader-utils) from 1.4.0 to 1.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/releases">loader-utils's releases</a>.</em></p>
<blockquote>
<h2>v1.4.1</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v1.4.1">1.4.1</a> (2022-11-07)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>security problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/220">#220</a>) (<a href="https://github.com/webpack/loader-utils/commit/4504e34c4796a5836ef70458327351675aed48a5">4504e34</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/blob/v1.4.1/CHANGELOG.md">loader-utils's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v1.4.1">1.4.1</a> (2022-11-07)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>security problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/220">#220</a>) (<a href="https://github.com/webpack/loader-utils/commit/4504e34c4796a5836ef70458327351675aed48a5">4504e34</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/loader-utils/commit/8f082b39f6903929f30fe29dab34f4d9c7ef070a"><code>8f082b3</code></a> chore(release): 1.4.1</li>
<li><a href="https://github.com/webpack/loader-utils/commit/4504e34c4796a5836ef70458327351675aed48a5"><code>4504e34</code></a> fix: security problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/220">#220</a>)</li>
<li>See full diff in <a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v1.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=loader-utils&package-manager=npm_and_yarn&previous-version=1.4.0&new-version=1.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-09 01:57:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2192" class=".btn">#2192</a>
            </td>
            <td>
                <b>
                    docs(odap-plugin): update odap plugin doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the merge of  #2154 this is the update of the README file

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 17:27:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2190" class=".btn">#2190</a>
            </td>
            <td>
                <b>
                    test(verifier-client): add stress test and fix a memory leak
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a new package `@hyperledger/cactus-test-verifier-client` for verifier-client stress and
  functional tests that involve multiple packages.
- Add stress test for verifier-client that reports memory usage of repeated operation
  on `cactus-plugin-ledger-connector-go-ethereum-socketio` connector plugin.
- Fix a memory leak in `SocketIOApiClient` - free socket listeners when they are no longer needed.
- Fix `cactus-plugin-ledger-connector-go-ethereum-socketio` - use single a web3 connection
  (with keep-alive/reconnect) instead of spawning new one for each request.
  Previous solution was causing connection issues in stress testing.

Depends on: https://github.com/hyperledger/cactus/pull/2089
Closes: https://github.com/hyperledger/cactus/issues/2189

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

-------------

Please review only the last commit, the others are dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 16:34:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2188" class=".btn">#2188</a>
            </td>
            <td>
                <b>
                    ci(github): upgrade actions/checkout to v3.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Project-wide search and replace for all occurrences of the
checkout GH workflow action so that it is at the current
latest stable release version which is v3.1.0

Fixes #2187

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 00:15:22 +0000 UTC
    </div>
</div>

