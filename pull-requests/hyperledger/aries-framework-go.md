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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3080" class=".btn">#3080</a>
            </td>
            <td>
                <b>
                    fix: don't set recipientKeys and routingKeys if empty
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
        Created At 2021-12-01 16:37:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3079" class=".btn">#3079</a>
            </td>
            <td>
                <b>
                    refactor: change webkms to fit refactored kms service, add bdd tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Change format of remote kms api calls to correspond to changes in kms service api

**Description:**
Make changes to webkms and remote crytro to work with new version of kms service.
Add bdd tests for webkms and remote crypto.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 14:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3077" class=".btn">#3077</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 2.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 2.5.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
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
<li><a href="https://github.com/actions/setup-node/commit/04c56d2f954f1e4c69436aa54cfef261a018f458"><code>04c56d2</code></a> update cache to 1.0.8 (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/367">#367</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/d08cf222111d5c1d21b3cd4b958937f818d10d9a"><code>d08cf22</code></a> Adding Node.js version file support (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/338">#338</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/360ab8b75b056fc18d368ee27a78d34e29c0b2d9"><code>360ab8b</code></a> Fix typo in the <code>bug_report</code> template (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/353">#353</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/fd4bd829f2dd6b6c1420bd94a93449c54612ffc2"><code>fd4bd82</code></a> Add issue and pull request templates (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/344">#344</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/a4b8ed2f4e9dd97eeae325f6967ce23d5478bd53"><code>a4b8ed2</code></a> Update dependencies (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/346">#346</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/270253e841af726300e85d718a5f606959b2903c"><code>270253e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a> from WtfJoke/addCacheHitOutPut</li>
<li><a href="https://github.com/actions/setup-node/commit/d1178716dbbe024f9d459612c22072517a781faa"><code>d117871</code></a> Add 'cache-hit' as output</li>
<li><a href="https://github.com/actions/setup-node/commit/041bafb67276a76a9cc88cd8a4e99165e9eb287d"><code>041bafb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/322">#322</a> from brcrista/brcrista/check-dist</li>
<li><a href="https://github.com/actions/setup-node/commit/996306e892eb8e97c8cfe8226ee043ae86a8f377"><code>996306e</code></a> rm <strong>tests</strong>/verify-no-unstaged-changes.sh</li>
<li><a href="https://github.com/actions/setup-node/commit/85d412253086d787de7add5f46dcf5964224c032"><code>85d4122</code></a> Fix triggers in licensed.yml</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v2.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=2.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-30 08:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3076" class=".btn">#3076</a>
            </td>
            <td>
                <b>
                    feat: Credential Fulfillment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added a library that allows you to parse Credential Fulfillment objects and resolve VCs from them based on an Issue Credential Message's attachment. This Credential Fulfillment implementation is based on the specification at https://identity.foundation/credential-manifest/#credential-fulfillment.

- Refactored the CredentialManifest.ResolveOutputDescriptors method to take in a *verifiable.Credential object instead of a []byte, in order to make the expected type more explicit.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 03:19:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    feat: command controllers for wallet issuance flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added JS, REST command controllers for wallet issuance interfaces.
- Part of  #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 21:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3074" class=".btn">#3074</a>
            </td>
            <td>
                <b>
                    feat: WACI issuance flow interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                based on [WACI Issuance in Universal
Wallet](https://github.com/w3c-ccg/universal-wallet-interop-spec/issues/101)

- added propose credential interface
- added request credential interface
- added tests
- Closes #3073

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 16:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3072" class=".btn">#3072</a>
            </td>
            <td>
                <b>
                    feat: connectionRecord in OOBV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change includes ConnectionRecord creation in OOBV2 and requires invitation attachment messages to include `from`
header representing the sender's DID.


Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 15:24:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3071" class=".btn">#3071</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.64.4 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.64.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.64.4</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix tagged template literal evaluation</li>
<li>fix ModuleFederation with ESM</li>
<li>fix outputModule with intial splitChunks</li>
</ul>
<h1>Performance</h1>
<ul>
<li>upgrade watchpack for faster watcher updating</li>
<li>track file and directory timestamps separately in watchpack and webpack</li>
</ul>
<h1>Developer Experience</h1>
<ul>
<li>show origin of singleton shared module in mismatch warning</li>
</ul>
<h2>v5.64.3</h2>
<h1>Performance</h1>
<ul>
<li>allow to use pre-compiled schema when <code>Infinity</code> is used in configuration</li>
<li>allow to use pre-compiled schema for configuration arrays</li>
</ul>
<h2>v5.64.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>avoid double initial compilation due to invalid dependencies with managedPaths</li>
</ul>
<h2>v5.64.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix regexp in managedPaths to exclude additional slash</li>
<li>make module.accept errorHandler optional in typings</li>
<li>correctly create an async chunk when using a <code>require(...).property</code> in <code>require.ensure</code></li>
<li>fix cleaning of symlinks in <code>output.clean: true</code></li>
<li>fix change detection with <code>unsafeCache</code> within <code>managedPaths</code> (node_modules)</li>
<li>bump webpack-sources for Stack Overflow bugfix</li>
</ul>
<h2>v5.64.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>asyncChunks: boolean</code> option to disable creation of async chunks</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix ProfilingPlugin for <code>experiments.backCompat: false</code></li>
</ul>
<h1>Performance</h1>
<ul>
<li>avoid running regexp twice over the file list</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/d3cd4cb6e38338237fe722d4b7feae2244c425c5"><code>d3cd4cb</code></a> 5.64.4</li>
<li><a href="https://github.com/webpack/webpack/commit/4f9fafc73e46b1b08fa0d3e7551b5ab6b94d1441"><code>4f9fafc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14829">#14829</a> from webpack/bugfix/split-chunks-esm</li>
<li><a href="https://github.com/webpack/webpack/commit/093eadfdb45c3e94bab7057971debba093cb39a9"><code>093eadf</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14827">#14827</a> from webpack/bugfix/mf-module</li>
<li><a href="https://github.com/webpack/webpack/commit/c69e37c39d12c8e3c761c883069d89f90cac817c"><code>c69e37c</code></a> fix outputModule with initial splitChunks</li>
<li><a href="https://github.com/webpack/webpack/commit/041287ff589701f288d6baafe150002529317ca9"><code>041287f</code></a> fix test problem</li>
<li><a href="https://github.com/webpack/webpack/commit/c3691df74064ec2a591b3c0beefe3565f84cb71b"><code>c3691df</code></a> fix CI problems</li>
<li><a href="https://github.com/webpack/webpack/commit/d91248711b63818a4e935294dec290a760fcca5d"><code>d912487</code></a> fix and test module federation with ESM</li>
<li><a href="https://github.com/webpack/webpack/commit/ac9a2c87ed732adaf9dfe307c7690c43609d06a2"><code>ac9a2c8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14782">#14782</a> from tanhauhau/tanhauhau/show-which-container-loade...</li>
<li><a href="https://github.com/webpack/webpack/commit/ce0f0b3a164591da1b8edcee038b9e81d0bf4909"><code>ce0f0b3</code></a> update test case</li>
<li><a href="https://github.com/webpack/webpack/commit/68c4a2a0a9a9c12c55e2ba2a5273dd26958e4027"><code>68c4a2a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14728">#14728</a> from markjm/markjm/context-timestamps</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.64.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.64.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-26 08:14:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3070" class=".btn">#3070</a>
            </td>
            <td>
                <b>
                    wip: merge present proof v2/v3 client APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 03:34:51 +0000 UTC
    </div>
</div>

