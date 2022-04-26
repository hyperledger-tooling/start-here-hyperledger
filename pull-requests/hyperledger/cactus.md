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
                PR <a href="https://github.com/hyperledger/cactus/pull/1992" class=".btn">#1992</a>
            </td>
            <td>
                <b>
                    ci(connector-besu): include endpoints in fuzzer tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed

ci(connector-besu): include endpoints in fuzzer tests 


    Primary Changes
    --------------
    1. Updated the git workflow to include the besu connector plugin endpoint
    2. Added the task to run Besu all-in-one image
       as a valid ws endpoint is required for connector to initialize
    3. Updated the besu connector plugin README.md for minor fixes

Fixes #1949

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 10:03:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1991" class=".btn">#1991</a>
            </td>
            <td>
                <b>
                    docs(maintainers): add Rama and Sandeep
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 03:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1990" class=".btn">#1990</a>
            </td>
            <td>
                <b>
                    ci: bump NodeJS v14 and v16 minor versions to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Fixes #1980

Signed-off-by: aldousalvarez <aldousss.alvarez@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 02:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1989" class=".btn">#1989</a>
            </td>
            <td>
                <b>
                    ci: add yaml workflow file for semantic-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1987

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 21:03:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1988" class=".btn">#1988</a>
            </td>
            <td>
                <b>
                    test: jestify jwt socketio endpoint authorization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                packages/cactus-cmd-api-server/src/test/typescript/integration/jwt-socketio-endpoint-authorization.test.ts; WIP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 12:45:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1986" class=".btn">#1986</a>
            </td>
            <td>
                <b>
                    docs(readme): replaced rocketchat link with discord link in README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Since the migration from RocketChat to Discord we had our chat platform
link in the readme outdated and basically dead. This change remedies that.

Fixes: #1937

Signed-off-by: Emerson Shoichet-Bartus <emersonfieldstone@gmail.com>
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 17:13:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1985" class=".btn">#1985</a>
            </td>
            <td>
                <b>
                    build(deps): bump convict from 6.0.0 to 6.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [convict](https://github.com/mozilla/node-convict) from 6.0.0 to 6.2.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mozilla/node-convict/blob/master/CHANGELOG.md">convict's changelog</a>.</em></p>
<blockquote>
<h2>[6.2.2] - 2022-03-27</h2>
<h3>Fixed</h3>
<ul>
<li>More complete fix for prototype pollution vulnerability first addressed in
<a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/384">#384</a> (Marc-Aurèle Darche <a href="https://github.com/madarche"><code>@​madarche</code></a>)</li>
</ul>
<h2>[6.2.1] - 2021-10-20</h2>
<h3>Fixed</h3>
<ul>
<li>Fix misspelling of the word optional in the error message <a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/397">#397</a> (Dan Allen <a href="https://github.com/mojavelinux"><code>@​mojavelinux</code></a>))</li>
</ul>
<h2>[6.2.0] - 2021-05-21</h2>
<h3>Changed</h3>
<ul>
<li>Update dependency: validator <code>^11.1.0</code> → <code>^13.6.0</code> (<a href="https://github-redirect.dependabot.com/mozilla/node-convict/pull/390">#390</a>)</li>
<li>Update dependency: parser <code>^18.1.3</code> → <code>^20.2.7</code> (<a href="https://github-redirect.dependabot.com/mozilla/node-convict/pull/390">#390</a>)</li>
<li>Update dependency: moment <code>^2.24.0</code> → <code>^2.29.1</code> (<a href="https://github-redirect.dependabot.com/mozilla/node-convict/pull/390">#390</a>)</li>
</ul>
<h2>[6.1.0] - 2021-05-03</h2>
<h3>Added</h3>
<ul>
<li>Add new &quot;nullable&quot; option to allow &quot;null&quot; additionally to any format <a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/386">#386</a> (maxwrlr)</li>
</ul>
<h2>[6.0.1] - 2021-03-11</h2>
<h3>Fixed</h3>
<ul>
<li>Fix prototype pollution vulnerability <a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/384">#384</a> (arjunshibu, Jamie Slome)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mozilla/node-convict/commit/4da12f88f77a3a4c1d61fee3bc5d16194892802d"><code>4da12f8</code></a> v6.2.2</li>
<li><a href="https://github.com/mozilla/node-convict/commit/8ad66b5268831674e021cbfa6101143d6af187aa"><code>8ad66b5</code></a> Update CHANGELOG</li>
<li><a href="https://github.com/mozilla/node-convict/commit/3b86be087d8f14681a9c889d45da7fe3ad9cd880"><code>3b86be0</code></a> More complete fix against prototype pollution</li>
<li><a href="https://github.com/mozilla/node-convict/commit/e3173b13c25b5f340f1f231b6c65c3c7c69030a6"><code>e3173b1</code></a> Clearer variable name</li>
<li><a href="https://github.com/mozilla/node-convict/commit/5eb1314f85346760a3c31cb14510f2f0af11d0d3"><code>5eb1314</code></a> v6.2.1</li>
<li><a href="https://github.com/mozilla/node-convict/commit/5ad62d6365ffe37d0457ed5caaac96d88168264f"><code>5ad62d6</code></a> Update CHANGELOG</li>
<li><a href="https://github.com/mozilla/node-convict/commit/c6820864857adea0c025adfbb2b1f62b0318885b"><code>c682086</code></a> fix misspelling of the word optional in the error message (<a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/397">#397</a>)</li>
<li><a href="https://github.com/mozilla/node-convict/commit/bdd8a4e55a236c2ccb2a2d6062c9ac3ddec34af6"><code>bdd8a4e</code></a> v6.2.0</li>
<li><a href="https://github.com/mozilla/node-convict/commit/f69307793c415485c8afd7e00a2b5a64b62b74c9"><code>f693077</code></a> Provide working links in the CHANGELOG</li>
<li><a href="https://github.com/mozilla/node-convict/commit/d90f2f8f80eb0e404a621e77e6302d6213ffa3ff"><code>d90f2f8</code></a> Update CHANGELOG</li>
<li>Additional commits viewable in <a href="https://github.com/mozilla/node-convict/compare/v6.0.0...v6.2.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~madarche">madarche</a>, a new releaser for convict since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=convict&package-manager=npm_and_yarn&previous-version=6.0.0&new-version=6.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-20 21:09:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1984" class=".btn">#1984</a>
            </td>
            <td>
                <b>
                    refactor(discounted-cartrade): use cactus-verifier-client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sample app discounted-cartrade is currently using Verifier interface from cactus-cmd-socket-server.
Replace it with VerifierFactory from cactus-verifier-client package that
can work with all cactus connectors.

Related: #1982
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 14:51:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1983" class=".btn">#1983</a>
            </td>
            <td>
                <b>
                    refactor(electricity-trade): use cactus-verifier-client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sample app electricity-trade is currently using Verifier interface from cactus-cmd-socket-server.
Replace it with VerifierFactory from cactus-verifier-client package that
can work with all cactus connectors.

Related: #1982
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 12:24:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1981" class=".btn">#1981</a>
            </td>
            <td>
                <b>
                    Zondervancalvez/issue1876
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
        Created At 2022-04-20 07:35:50 +0000 UTC
    </div>
</div>

