---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    non admin didentity message no longer appears on ca details page.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem <Nikhil.Modem@ibm.com>

#### Type of change

- Bug fix
- Improvement (improvement to code, performance, etc)

#### Description
- Non-admin identity message appeared for associated identities of CAs which didn't make sense so took it out.
-  Also moved PageHeader component on CA details page to reflect other pages. This makes the migration banners present better too.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-27 09:41:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    move typescript from dev dep to peer dep
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
move typescript from dev dependency to a peer dependency.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 18:40:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    move ts-loader to peer dep from dev dep
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
`ts-loader` needs to be a peer dependency. moved from dev dependency.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 18:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    clean up dev deps in image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Remove dev deps in image from athena and stitch installations.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 16:08:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Bump parse-path and lerna
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [parse-path](https://github.com/IonicaBizau/parse-path) to 7.0.0 and updates ancestor dependency [lerna](https://github.com/lerna/lerna/tree/HEAD/core/lerna). These dependencies need to be updated together.

Updates `parse-path` from 4.0.3 to 7.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/IonicaBizau/parse-path/releases">parse-path's releases</a>.</em></p>
<blockquote>
<h2>7.0.0</h2>
<p>Add the <code>parse_failed</code> property — whether the input was parsed successfully or not.</p>
<h2>6.0.0</h2>
<h3>parse-path 6.0.0</h3>
<p><strong>Breaking changes</strong></p>
<ul>
<li>The <code>resource</code> property will not contain the <code>port</code> anymore. Added the <code>host</code> property which has the port too.</li>
</ul>
<h2>5.0.0</h2>
<h3><code>parse-path</code> 5.0.0</h3>
<p>:star: This is a major release of <code>parse-path</code>! :star:</p>
<h4>Breaking changes</h4>
<ul>
<li><code>parse-path</code> will not parse <code>git@...</code> ssh URLs anymore. Use <code>parse-url</code> for that.</li>
<li>If the input url has a trailing slash, the trailing slash will be added in the <code>pathname</code> too.</li>
<li>The <code>port</code> field is a string. By default empty.</li>
<li>Added the <code>password</code> field (default: <code>&quot;&quot;</code>)</li>
<li>The resource may contain the <code>port</code> in it (e.g. <code>resource: &quot;domain.com:4200&quot;</code>).</li>
</ul>
<h4>Features</h4>
<ul>
<li>Faster</li>
<li>More secure</li>
<li>Cleaner codebase</li>
</ul>
<p>Any questions, suggestions, contributions are always welcome! :blush:</p>
<h2>4.0.4</h2>
<p>Remove the new line characters.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/c53b17e228fd09e2e072ce0d9c6076cf7bb879da"><code>c53b17e</code></a> Updated docs</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/a0269b12b3f3eb4ce4a1b5a9a6da24832d3d2d8f"><code>a0269b1</code></a> :arrow_up: 7.0.0 :tada:</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/e3ee527ab36be1166f72d1654a5a6e31f18c866a"><code>e3ee527</code></a> :arrow_up: 6.1.0 :tada:</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/4bae19e8e0e6b8566201387c1b1e664a9e87b904"><code>4bae19e</code></a> Add the parse_failed property.</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/3d1525d9ec72f5a1ad67b438bed95dd752ed3413"><code>3d1525d</code></a> Updated docs</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/31f7a332f9c4ce5e1c6448ac5a7b4507cb00deed"><code>31f7a33</code></a> Add the host property</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/02995c6c7ccb3d05180f235b1dc1c3abb710147b"><code>02995c6</code></a> Merge branch 'patch-1' of github.com:viceice/parse-path into new-version</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/cbb46e0e713d747b7851eb98c1c4af1bb1ead238"><code>cbb46e0</code></a> :arrow_up: 6.0.0 :tada:</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/01b23dc123c6f2cdc1357eba22243c7b7324e4ea"><code>01b23dc</code></a> test: add test</li>
<li><a href="https://github.com/IonicaBizau/parse-path/commit/9032ebb45a28deb57fef2928acd72fca25aabbef"><code>9032ebb</code></a> fix: use hostname instead of host</li>
<li>Additional commits viewable in <a href="https://github.com/IonicaBizau/parse-path/compare/4.0.3...7.0.0">compare view</a></li>
</ul>
</details>
<br />

Updates `lerna` from 4.0.0 to 6.0.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/lerna/lerna/releases">lerna's releases</a>.</em></p>
<blockquote>
<h2>v6.0.1</h2>
<h2><a href="https://github.com/lerna/lerna/compare/v6.0.0...v6.0.1">6.0.1</a> (2022-10-14)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>run:</strong> allow for loading of env files to be skipped (<a href="https://github-redirect.dependabot.com/lerna/lerna/issues/3375">#3375</a>) (<a href="https://github.com/lerna/lerna/commit/5dbd904009ede4cc952fc7f8cbafebf6b12d81a1">5dbd904</a>)</li>
</ul>
<h2>v6.0.0</h2>
<h1><a href="https://github.com/lerna/lerna/compare/v6.0.0-alpha.2...v6.0.0">6.0.0</a> (2022-10-12)</h1>
<h3>Super fast, modern task-runner implementation for <code>lerna run</code></h3>
<p>As of version 6.0.0, Lerna will now delegate the implementation details of the <code>lerna run</code> command to the super fast, modern task-runner (powered by Nx) by default.</p>
<p>If for some reason you wish to opt in to the legacy task-runner implementation details (powered by <code>p-map</code> and <code>p-queue</code>), you can do so by setting <code>&quot;useNx&quot;: false</code> in your lerna.json. (Please let us know via a Github issue if you feel the need to do that, however, as in general the new task-runner should just work how you expect it to as a lerna user).</p>
<h3>Interactive configurtion for <code>lerna run</code> caching and task pipelines via the new <code>lerna add-caching</code> command</h3>
<p>When using the modern task-runner implementation described above, the way to get the most out of it is to tell it about the outputs of your various scripts, and also any relationships that exist between them (such as needing to run the <code>build</code> script before the <code>test</code>, for example).</p>
<p>Simply run <code>lerna add-caching</code> and follow the instructions in order to generate all the relevant configuration for your workspace.</p>
<p>You can learn more about the configuration it generates here: <a href="https://lerna.js.org/docs/concepts/task-pipeline-configuration">https://lerna.js.org/docs/concepts/task-pipeline-configuration</a></p>
<h3>Automatic loading of .env files in <code>lerna run</code> with the new task-runner implementation</h3>
<p>By default the modern task runner powered by Nx will automatically load <code>.env</code> files for you. You can set <code>--load-env-files</code> to false if you want to disable this behavior for any reason.</p>
<p>For more details about what <code>.env</code> files will be loaded by default please see: <a href="https://nx.dev/recipes/environment-variables/define-environment-variables">https://nx.dev/recipes/environment-variables/define-environment-variables</a></p>
<h3>Obselete options in <code>lerna run</code> with the new task-runner implementation</h3>
<p>There are certain legacy options for <code>lerna run</code> which are no longer applicable to the modern task-runner. Please see full details about those flags, and the reason behind their obselence, here:</p>
<p><a href="https://lerna.js.org/docs/lerna6-obsolete-options">https://lerna.js.org/docs/lerna6-obsolete-options</a></p>
<h3>New <code>lerna repair</code> command</h3>
<p>When configuration changes over time as new versions of a tool are published it can be tricky to keep up with the changes and sometimes it's possible to miss out on optimizations as a result.</p>
<p>When you run the new command <code>lerna repair</code>, lerna will execute a serious of code migrations/codemods which update your workspace to the latest and greatest best practices for workspace configuration.</p>
<p>The actual codemods which run will be added to over time, but for now one you might see run on your workspace is that it will remove any explicit <code>&quot;useNx&quot;: true</code> references from lerna.json files, because that is no longer necessary and it's cleaner not to have it.</p>
<p>We are really excited about this feature and how we can use it to help users keep their workspaces up to date.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/lerna/lerna/blob/main/core/lerna/CHANGELOG.md">lerna's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/lerna/lerna/compare/v6.0.0...v6.0.1">6.0.1</a> (2022-10-14)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>run:</strong> allow for loading of env files to be skipped (<a href="https://github-redirect.dependabot.com/lerna/lerna/issues/3375">#3375</a>) (<a href="https://github.com/lerna/lerna/commit/5dbd904009ede4cc952fc7f8cbafebf6b12d81a1">5dbd904</a>)</li>
</ul>
<h1><a href="https://github.com/lerna/lerna/compare/v6.0.0-alpha.2...v6.0.0">6.0.0</a> (2022-10-12)</h1>
<p><strong>Note:</strong> Version bump only for package lerna</p>
<h1><a href="https://github.com/lerna/lerna/compare/v6.0.0-alpha.1...v6.0.0-alpha.2">6.0.0-alpha.2</a> (2022-10-12)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>run:</strong> update docs for v6 (<a href="https://github-redirect.dependabot.com/lerna/lerna/issues/3366">#3366</a>) (<a href="https://github.com/lerna/lerna/commit/130f4906bee3e240ea9ad9245dfb0fe208668dae">130f490</a>)</li>
</ul>
<h1><a href="https://github.com/lerna/lerna/compare/v5.6.2...v6.0.0-alpha.1">6.0.0-alpha.1</a> (2022-10-09)</h1>
<h1><a href="https://github.com/lerna/lerna/compare/v5.6.1...v6.0.0-alpha.0">6.0.0-alpha.0</a> (2022-10-07)</h1>
<p><strong>Note:</strong> Version bump only for package lerna</p>
<h2><a href="https://github.com/lerna/lerna/compare/v5.6.1...v5.6.2">5.6.2</a> (2022-10-09)</h2>
<p><strong>Note:</strong> Version bump only for package lerna</p>
<h2><a href="https://github.com/lerna/lerna/compare/v5.6.0...v5.6.1">5.6.1</a> (2022-09-30)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>add-caching:</strong> ensure lerna.json is configured automatically (<a href="https://github.com/lerna/lerna/commit/9677cda7c9e16ae3cc02cd01c7b1087d81095750">9677cda</a>)</li>
</ul>
<h1><a href="https://github.com/lerna/lerna/compare/v5.5.4...v5.6.0">5.6.0</a> (2022-09-29)</h1>
<h3>Features</h3>
<ul>
<li><strong>core:</strong> add add-caching command (<a href="https://github-redirect.dependabot.com/lerna/lerna/issues/3350">#3350</a>) (<a href="https://github.com/lerna/lerna/commit/ef09a06ffc30384194fb120307269f49e4ebc54b">ef09a06</a>)</li>
<li><strong>repair:</strong> add lerna repair command (<a href="https://github-redirect.dependabot.com/lerna/lerna/issues/3314">#3314</a>) (<a href="https://github.com/lerna/lerna/commit/7defab3434687fc8e17f921250846aa279ac3df3">7defab3</a>)</li>
</ul>
<h2><a href="https://github.com/lerna/lerna/compare/v5.5.3...v5.5.4">5.5.4</a> (2022-09-28)</h2>
<p><strong>Note:</strong> Version bump only for package lerna</p>
<h2><a href="https://github.com/lerna/lerna/compare/v5.5.2...v5.5.3">5.5.3</a> (2022-09-28)</h2>
<p><strong>Note:</strong> Version bump only for package lerna</p>
<h2><a href="https://github.com/lerna/lerna/compare/v5.5.1...v5.5.2">5.5.2</a> (2022-09-20)</h2>
<p><strong>Note:</strong> Version bump only for package lerna</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lerna/lerna/commit/4fcefff1b7d982c83b6d68d0a84d7e878ea87449"><code>4fcefff</code></a> chore(release): v6.0.1</li>
<li><a href="https://github.com/lerna/lerna/commit/5dbd904009ede4cc952fc7f8cbafebf6b12d81a1"><code>5dbd904</code></a> fix(run): allow for loading of env files to be skipped (<a href="https://github.com/lerna/lerna/tree/HEAD/core/lerna/issues/3375">#3375</a>)</li>
<li><a href="https://github.com/lerna/lerna/commit/6fa5951a03d3c0c4bd2f154b413cc9a378adc02b"><code>6fa5951</code></a> chore(release): v6.0.0</li>
<li><a href="https://github.com/lerna/lerna/commit/154b93901308cbfd6b803e1f199e9b6d2e362b6f"><code>154b939</code></a> chore(release): v6.0.0-alpha.2</li>
<li><a href="https://github.com/lerna/lerna/commit/130f4906bee3e240ea9ad9245dfb0fe208668dae"><code>130f490</code></a> fix(run): update docs for v6 (<a href="https://github.com/lerna/lerna/tree/HEAD/core/lerna/issues/3366">#3366</a>)</li>
<li><a href="https://github.com/lerna/lerna/commit/8a1660e1e78c39db2f7a080862d93bbde6dd9339"><code>8a1660e</code></a> chore(release): v6.0.0-alpha.1</li>
<li><a href="https://github.com/lerna/lerna/commit/a926c6a648c85a4ea97ef343b3a796bbe0b25d22"><code>a926c6a</code></a> Merge branch 'main' into next</li>
<li><a href="https://github.com/lerna/lerna/commit/04f85a38c72dd043e7e25072c6e29d8a6411b867"><code>04f85a3</code></a> chore(release): v5.6.2</li>
<li><a href="https://github.com/lerna/lerna/commit/84597c511c4503562c641b481a2854137465ba5c"><code>84597c5</code></a> chore(release): v6.0.0-alpha.0</li>
<li><a href="https://github.com/lerna/lerna/commit/8991812096dc874fc7be6ae7130e03c9a660f2c7"><code>8991812</code></a> feat(run)!: legacy task runner implementations no longer used by default (<a href="https://github.com/lerna/lerna/tree/HEAD/core/lerna/issues/3355">#3355</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/lerna/lerna/commits/v6.0.1/core/lerna">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jameshenry">jameshenry</a>, a new releaser for lerna since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 15:38:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    remove npm devDependencies from image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Dev dependencies do not need to be in the image we publish. This PR removes them.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 15:32:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/326" class=".btn">#326</a>
            </td>
            <td>
                <b>
                    don't show the migrated console banner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The new migration banner was left visible, accidentally. It should only show after a console has migrated.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-26 15:08:59 +0000 UTC
    </div>
</div>

