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
                PR <a href="https://github.com/hyperledger/cactus/pull/1896" class=".btn">#1896</a>
            </td>
            <td>
                <b>
                    refactor(cmd-socketio): validators should be configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add the possibility to adjust connector behavior through separate config file.
- Use node-config package for configuration management.
- Add helper classes in validators for easy config entry retrieval.
- Remove obsolete and unnecessary components.
- Adjust sample applications to work in current setup.

Closes: #1895
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

Note - the changes are very similar in all 3 affected ledger connectors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 14:31:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1893" class=".btn">#1893</a>
            </td>
            <td>
                <b>
                    docs: minor tweaks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                -add mention to test running via interface
-explain in more detail the docker requirement
-fix small bug preventing the correct execution of generate-api-server

cc @petermetz 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 14:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1892" class=".btn">#1892</a>
            </td>
            <td>
                <b>
                    test: jestify jwt-unprotected-endpoint-authz-ops-confirm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest

File Path:
packages/cactus-cmd-api-server/src/test/typescript/
integration/jwt-unprotected-endpoint-authz-ops-confirm.test.ts

This is a PARTIAL resolution to issue hyperledger#238

NOT ready to merge, I need to correct the way .toRejects() happens


Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 00:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1891" class=".btn">#1891</a>
            </td>
            <td>
                <b>
                    test(get-single-status-endpoint-invalid): jestify get-single-status-endpoint-invalid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/get-single-status-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 23:20:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1889" class=".btn">#1889</a>
            </td>
            <td>
                <b>
                    Cactus test plugin htlc eth besu erc20/withdraw endpoint invalid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/withdraw-endpoint-invalid-id.test.ts

This is a PARTIAL resolution to issue https://github.com/hyperledger/cactus/issues/238

Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 19:07:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1888" class=".btn">#1888</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump karma from 6.3.14 to 6.3.16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [karma](https://github.com/karma-runner/karma) from 6.3.14 to 6.3.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/karma-runner/karma/releases">karma's releases</a>.</em></p>
<blockquote>
<h2>v6.3.16</h2>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.15...v6.3.16">6.3.16</a> (2022-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> mitigate the &quot;Open Redirect Vulnerability&quot; (<a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d">ff7edbb</a>)</li>
</ul>
<h2>v6.3.15</h2>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.15">6.3.15</a> (2022-02-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>helper:</strong> make mkdirIfNotExists helper resilient to concurrent calls (<a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404">d9dade2</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/karma-runner/karma-coverage/issues/434/issues/issuecomment-1017939333">karma-runner/karma-coverage#434</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/karma-runner/karma/blob/master/CHANGELOG.md">karma's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.15...v6.3.16">6.3.16</a> (2022-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> mitigate the &quot;Open Redirect Vulnerability&quot; (<a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d">ff7edbb</a>)</li>
</ul>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.15">6.3.15</a> (2022-02-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>helper:</strong> make mkdirIfNotExists helper resilient to concurrent calls (<a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404">d9dade2</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/karma-runner/karma-coverage/issues/434/issues/issuecomment-1017939333">karma-runner/karma-coverage#434</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/karma-runner/karma/commit/ab4b32898bcb4e0ba3a1e99835d30c113db3eeeb"><code>ab4b328</code></a> chore(release): 6.3.16 [skip ci]</li>
<li><a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d"><code>ff7edbb</code></a> fix(security): mitigate the &quot;Open Redirect Vulnerability&quot;</li>
<li><a href="https://github.com/karma-runner/karma/commit/c1befa04b32b90f088fefdc0521c6f48cbc510a9"><code>c1befa0</code></a> chore(release): 6.3.15 [skip ci]</li>
<li><a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404"><code>d9dade2</code></a> fix(helper): make mkdirIfNotExists helper resilient to concurrent calls</li>
<li><a href="https://github.com/karma-runner/karma/commit/653c762be4fa464fed5bfa306317b84cc5c28a17"><code>653c762</code></a> ci: prevent duplicate CI tasks on creating a PR</li>
<li>See full diff in <a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=karma&package-manager=npm_and_yarn&previous-version=6.3.14&new-version=6.3.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-02 13:39:37 +0000 UTC
    </div>
</div>

