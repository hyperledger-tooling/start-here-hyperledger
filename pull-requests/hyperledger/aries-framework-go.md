---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3116" class=".btn">#3116</a>
            </td>
            <td>
                <b>
                    feat: didcomm v2 peer did integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - DID rotation command can now rotate to a freshly-made peer DID
- OOBv2 inviter creates connection on inbound invitation response
- present-proof controller API can take connection ID instead of DIDs
- BDD tests have better handling of connection IDs, using BDDContext

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 09:59:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3115" class=".btn">#3115</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 2.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 2.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Fix logic of error handling for npm warning and uncaught exception</h2>
<p>In scope of this release we fix logic of error handling related to caching (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/358">actions/setup-node#358</a>) and (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/359">actions/setup-node#359</a>).</p>
<p>In the previous behaviour we relied on <code>stderr</code> output to throw error. The warning messages from package managers can be written to the stderr's output. For now the action will throw an error only if exit code differs from zero. Besides, we add logic to сatch and log unhandled exceptions.</p>
<h2>Adding Node.js version file support</h2>
<p>In scope of this release we add the <code>node-version-file</code> input and update <code>actions/cache</code> dependency to the latest version.</p>
<h2>Adding Node.js version file support</h2>
<p>The new input (<code>node-version-file</code>) provides functionality to specify the path to the file containing Node.js's version with such behaviour:</p>
<ul>
<li>If the file does not exist the action will throw an error.</li>
<li>If you specify both <code>node-version</code> and <code>node-version-file</code> inputs, the action will use value from the <code>node-version</code> input and throw the following warning: <code>Both node-version and node-version-file inputs are specified, only node-version will be used</code>.</li>
<li>For now the action does not support all of the variety of values for Node.js version files. The action can handle values according to the <a href="https://github.com/actions/setup-node#supported-version-syntax">documentation</a> and values with <code>v</code> prefix (<code>v14</code>)</li>
</ul>
<pre lang="yaml"><code>steps:
  - uses: actions/checkout@v2
  - name: Setup node from node version file
    uses: actions/setup-node@v2
    with:
      node-version-file: '.nvmrc'
  - run: npm install
  - run: npm test
</code></pre>
<h2>Update actions/cache dependency to 1.0.8 version.</h2>
<p>We updated actions/cache dependency to the latest version (1.0.8). For more information please refer to the <a href="https://github.com/actions/toolkit/blob/main/packages/cache/RELEASES.md">toolkit/cache</a>.</p>
<h2>Add &quot;cache-hit&quot; output</h2>
<p>This release introduces a new output: <code>cache-hit</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a>).</p>
<p>The <code>cache-hit</code> output contains boolean value indicating that an exact match was found for the key. It shows that the action uses already existing cache or not. The output is available only if cache is enabled.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/1f8c6b94b26d0feae1e387ca63ccbdc44d27b561"><code>1f8c6b9</code></a> Pass to warning uncaught exceptions (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/359">#359</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/9a74eb4e6473f91fbde564f97c2662fd1dc4875c"><code>9a74eb4</code></a> Throw error only if exit code is note zero.  (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/358">#358</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/04c56d2f954f1e4c69436aa54cfef261a018f458"><code>04c56d2</code></a> update cache to 1.0.8 (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/367">#367</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/d08cf222111d5c1d21b3cd4b958937f818d10d9a"><code>d08cf22</code></a> Adding Node.js version file support (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/338">#338</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/360ab8b75b056fc18d368ee27a78d34e29c0b2d9"><code>360ab8b</code></a> Fix typo in the <code>bug_report</code> template (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/353">#353</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/fd4bd829f2dd6b6c1420bd94a93449c54612ffc2"><code>fd4bd82</code></a> Add issue and pull request templates (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/344">#344</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/a4b8ed2f4e9dd97eeae325f6967ce23d5478bd53"><code>a4b8ed2</code></a> Update dependencies (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/346">#346</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/270253e841af726300e85d718a5f606959b2903c"><code>270253e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a> from WtfJoke/addCacheHitOutPut</li>
<li><a href="https://github.com/actions/setup-node/commit/d1178716dbbe024f9d459612c22072517a781faa"><code>d117871</code></a> Add 'cache-hit' as output</li>
<li><a href="https://github.com/actions/setup-node/commit/041bafb67276a76a9cc88cd8a4e99165e9eb287d"><code>041bafb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/322">#322</a> from brcrista/brcrista/check-dist</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v2.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=2.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 08:17:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3114" class=".btn">#3114</a>
            </td>
            <td>
                <b>
                    fix: unnoticed bdd test error in didcommv2 implicit connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 08:10:25 +0000 UTC
    </div>
</div>

