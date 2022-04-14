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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3220" class=".btn">#3220</a>
            </td>
            <td>
                <b>
                    docs: [readme-text] replace digital-hub with encrypted-data-vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Rolson Quadras <rolson.quadras@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 17:04:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3218" class=".btn">#3218</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 3.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 3.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Update actions/cache version to 2.0.2</h2>
<p>In scope of this release we updated <code>actions/cache</code> package as the new version contains fixes related to GHES 3.5 (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/460">actions/setup-node#460</a>)</p>
<h2>Add caching support on GHES 3.5</h2>
<p>In scope of this release we added <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/452">support for caching from GHES 3.5</a> and fixed download issue for files &gt; 2GB during restore. Besides, we updated <code>actions/cache</code> dependency to 2.0.0 version.</p>
<h2>v3.0.0</h2>
<p>In scope of this release we changed version of the runtime Node.js for the setup-node action and updated package-lock.json file to  v2.</p>
<h3>Breaking Changes</h3>
<ul>
<li>With the update to Node 16 in <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/414">actions/setup-node#414</a>, all scripts will now be run with Node 16 rather than Node 12.</li>
<li>We removed deprecated <code>version</code> input (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/424">actions/setup-node#424</a>). Please use <code>node-version</code> input instead.</li>
</ul>
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
<li><a href="https://github.com/actions/setup-node/commit/56337c425554a6be30cdef71bf441f15be286854"><code>56337c4</code></a> Updated <code>@​actions/cache</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/460">#460</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/76d3665dc084409ba9e6c467009338cf86e9dd5f"><code>76d3665</code></a> Convert CONDUCT to CODE_OF_CONDUCT.md (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/391">#391</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/5b52f097d36d4b0b2f94ed6de710023fbb8b2236"><code>5b52f09</code></a> Bump <code>actions/checkout@v3</code> within advanced usage examples documentation (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/456">#456</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/75716637dc8cd06e88621003df6357fdcee67772"><code>7571663</code></a> Bump to <code>actions/checkout@v3</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/437">#437</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/546fd45825c7f5d63e19e4595c08c16d66bcbad9"><code>546fd45</code></a> Updated documentation/workflows to use <code>actions/setup-node@v3</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/433">#433</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/bacd6b4b3ac3127b28a1e1920c23bf1c2cadbb85"><code>bacd6b4</code></a> Caching on GHES (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/452">#452</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/bed538bd04a773f1616efba082915a7638d8eb5f"><code>bed538b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/448">#448</a> from actions/dependabot/npm_and_yarn/minimist-1.2.6</li>
<li><a href="https://github.com/actions/setup-node/commit/f3e93d1b9dbf0ec44d17b09dea3d0446dd7d25d7"><code>f3e93d1</code></a> Bump minimist from 1.2.5 to 1.2.6</li>
<li><a href="https://github.com/actions/setup-node/commit/ed960c9656f8a2da28b0133d2bba0c7b6f2728a1"><code>ed960c9</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/440">#440</a> from actions/joshmgross/service-codeowners</li>
<li><a href="https://github.com/actions/setup-node/commit/77f43a440004389e5ec966078985f6a3153df1da"><code>77f43a4</code></a> Update CODEOWNERS to actions-service</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v3.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-12 11:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3217" class=".btn">#3217</a>
            </td>
            <td>
                <b>
                    chore: rename operationRequest to operation
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
        Created At 2022-04-11 20:30:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3216" class=".btn">#3216</a>
            </td>
            <td>
                <b>
                    docs: Updated storage interface documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the documentation for the Put method to indicate that in the set of tags used on a single Put call, those tags must have unique tag names. The reason for this is because several of our major storage implementations in aries-framework-go-ext have this implementation, so this note was added to help ensure consistent behaviour.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 17:28:39 +0000 UTC
    </div>
</div>

