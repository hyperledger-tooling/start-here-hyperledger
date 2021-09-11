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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2977" class=".btn">#2977</a>
            </td>
            <td>
                <b>
                    feat: support different Accept header values for DIDcomm versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds support for selection of the DIDComm service version based on
the OOB invitation's Accept header.

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 22:30:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2976" class=".btn">#2976</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.21.1 to 0.21.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.21.1 to 0.21.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>v0.21.2</h2>
<h3>0.21.2 (September 4, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Updating axios requests to be delayed by pre-emptive promise creation (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2702">#2702</a>)</li>
<li>Adding &quot;synchronous&quot; and &quot;runWhen&quot; options to interceptors api (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2702">#2702</a>)</li>
<li>Updating of transformResponse (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3377">#3377</a>)</li>
<li>Adding ability to omit User-Agent header (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3703">#3703</a>)</li>
<li>Adding multiple JSON improvements (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3688">#3688</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3763">#3763</a>)</li>
<li>Fixing quadratic runtime and extra memory usage when setting a maxContentLength (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3738">#3738</a>)</li>
<li>Adding parseInt to config.timeout (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3781">#3781</a>)</li>
<li>Adding custom return type support to interceptor (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3783">#3783</a>)</li>
<li>Adding security fix for ReDoS vulnerability (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3980">#3980</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Updating build dev dependancies (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3401">#3401</a>)</li>
<li>Fixing builds running on Travis CI (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3538">#3538</a>)</li>
<li>Updating follow rediect version (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3694">#3694</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3771">#3771</a>)</li>
<li>Updating karma sauce launcher to fix failing sauce tests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3712">#3712</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3717">#3717</a>)</li>
<li>Updating content-type header for application/json to not contain charset field, according do RFC 8259 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2154">#2154</a>)</li>
<li>Fixing tests by bumping karma-sauce-launcher version (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3813">#3813</a>)</li>
<li>Changing testing process from Travis CI to GitHub Actions (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3938">#3938</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Updating documentation around the use of <code>AUTH_TOKEN</code> with multiple domain endpoints (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3539">#3539</a>)</li>
<li>Remove duplication of item in changelog (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3523">#3523</a>)</li>
<li>Fixing gramatical errors (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2642">#2642</a>)</li>
<li>Fixing spelling error (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3567">#3567</a>)</li>
<li>Moving gitpod metion (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2637">#2637</a>)</li>
<li>Adding new axios documentation website link (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3681">#3681</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3707">#3707</a>)</li>
<li>Updating documentation around dispatching requests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3772">#3772</a>)</li>
<li>Adding documentation for the type guard isAxiosError (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3767">#3767</a>)</li>
<li>Adding explanation of cancel token (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3803">#3803</a>)</li>
<li>Updating CI status badge (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3953">#3953</a>)</li>
<li>Fixing errors with JSON documentation (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3936">#3936</a>)</li>
<li>Fixing README typo under Request Config (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3825">#3825</a>)</li>
<li>Adding axios-multi-api to the ecosystem file (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3817">#3817</a>)</li>
<li>Adding SECURITY.md to properly disclose security vulnerabilities (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3981">#3981</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/HEAD/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/SashaKoro">Sasha Korotkov</a></li>
<li><a href="https://github.com/timemachine3030">Daniel Lopretto</a></li>
<li><a href="https://github.com/MikeBishop">Mike Bishop</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
<li><a href="https://github.com/bimbiltu">Mark</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h3>0.21.2 (September 4, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Updating axios requests to be delayed by pre-emptive promise creation (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2702">#2702</a>)</li>
<li>Adding &quot;synchronous&quot; and &quot;runWhen&quot; options to interceptors api (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2702">#2702</a>)</li>
<li>Updating of transformResponse (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3377">#3377</a>)</li>
<li>Adding ability to omit User-Agent header (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3703">#3703</a>)</li>
<li>Adding multiple JSON improvements (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3688">#3688</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3763">#3763</a>)</li>
<li>Fixing quadratic runtime and extra memory usage when setting a maxContentLength (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3738">#3738</a>)</li>
<li>Adding parseInt to config.timeout (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3781">#3781</a>)</li>
<li>Adding custom return type support to interceptor (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3783">#3783</a>)</li>
<li>Adding security fix for ReDoS vulnerability (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3980">#3980</a>)</li>
</ul>
<p>Internal and Tests:</p>
<ul>
<li>Updating build dev dependancies (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3401">#3401</a>)</li>
<li>Fixing builds running on Travis CI (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3538">#3538</a>)</li>
<li>Updating follow rediect version (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3694">#3694</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3771">#3771</a>)</li>
<li>Updating karma sauce launcher to fix failing sauce tests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3712">#3712</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3717">#3717</a>)</li>
<li>Updating content-type header for application/json to not contain charset field, according do RFC 8259 (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2154">#2154</a>)</li>
<li>Fixing tests by bumping karma-sauce-launcher version (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3813">#3813</a>)</li>
<li>Changing testing process from Travis CI to GitHub Actions (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3938">#3938</a>)</li>
</ul>
<p>Documentation:</p>
<ul>
<li>Updating documentation around the use of <code>AUTH_TOKEN</code> with multiple domain endpoints (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3539">#3539</a>)</li>
<li>Remove duplication of item in changelog (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3523">#3523</a>)</li>
<li>Fixing gramatical errors (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2642">#2642</a>)</li>
<li>Fixing spelling error (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3567">#3567</a>)</li>
<li>Moving gitpod metion (<a href="https://github-redirect.dependabot.com/axios/axios/pull/2637">#2637</a>)</li>
<li>Adding new axios documentation website link (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3681">#3681</a>, <a href="https://github-redirect.dependabot.com/axios/axios/pull/3707">#3707</a>)</li>
<li>Updating documentation around dispatching requests (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3772">#3772</a>)</li>
<li>Adding documentation for the type guard isAxiosError (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3767">#3767</a>)</li>
<li>Adding explanation of cancel token (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3803">#3803</a>)</li>
<li>Updating CI status badge (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3953">#3953</a>)</li>
<li>Fixing errors with JSON documentation (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3936">#3936</a>)</li>
<li>Fixing README typo under Request Config (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3825">#3825</a>)</li>
<li>Adding axios-multi-api to the ecosystem file (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3817">#3817</a>)</li>
<li>Adding SECURITY.md to properly disclose security vulnerabilities (<a href="https://github-redirect.dependabot.com/axios/axios/pull/3981">#3981</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/SashaKoro">Sasha Korotkov</a></li>
<li><a href="https://github.com/timemachine3030">Daniel Lopretto</a></li>
<li><a href="https://github.com/MikeBishop">Mike Bishop</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
<li><a href="https://github.com/bimbiltu">Mark</a></li>
<li><a href="https://github.com/piiih">Philipe Gouveia Paixão</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/c0c87610911e1edebc923d0e932fea28cdfddae3"><code>c0c8761</code></a> [Updating] changelog to include links to issues and contributors</li>
<li><a href="https://github.com/axios/axios/commit/619bb465da374bc152f58280bb64c4aae8b78d4c"><code>619bb46</code></a> [Releasing] v0.21.2</li>
<li><a href="https://github.com/axios/axios/commit/82c94555917834770bd1389fc0b4cd9ba35ec3fe"><code>82c9455</code></a> Create SECURITY.md (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3981">#3981</a>)</li>
<li><a href="https://github.com/axios/axios/commit/5b457116e31db0e88fede6c428e969e87f290929"><code>5b45711</code></a> Security fix for ReDoS (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3980">#3980</a>)</li>
<li><a href="https://github.com/axios/axios/commit/5bc9ea24dda14e74def0b8ae9cdb3fa1a0c77773"><code>5bc9ea2</code></a> Update ECOSYSTEM.md (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3817">#3817</a>)</li>
<li><a href="https://github.com/axios/axios/commit/e72813a385c32e4c3eeaeb4fcc4437dd124bbbcf"><code>e72813a</code></a> Fixing README.md  (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3818">#3818</a>)</li>
<li><a href="https://github.com/axios/axios/commit/e10a0270e988a641ba0f01509c4c3ba657afe5a5"><code>e10a027</code></a> Fix README typo under Request Config (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3825">#3825</a>)</li>
<li><a href="https://github.com/axios/axios/commit/e091491127893a476b0223ab72f788c3b30fc082"><code>e091491</code></a> Update README.md (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3936">#3936</a>)</li>
<li><a href="https://github.com/axios/axios/commit/b42fbad57b093bb7214991161c5355bd46b864d0"><code>b42fbad</code></a> Removed un-needed bracket</li>
<li><a href="https://github.com/axios/axios/commit/520c8dccdef92cccbe51ea7cd96ad464c6401914"><code>520c8dc</code></a> Updating CI status badge (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3953">#3953</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.21.1...v0.21.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jasonsaayman">jasonsaayman</a>, a new releaser for axios since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.21.1&new-version=0.21.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 14:35:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2975" class=".btn">#2975</a>
            </td>
            <td>
                <b>
                    test: Present Proof v3 - BDD tests (sdk)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 13:29:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2974" class=".btn">#2974</a>
            </td>
            <td>
                <b>
                    fix: Gets MyDID and TheirDID when kid is KeyAgreement.ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 05:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2972" class=".btn">#2972</a>
            </td>
            <td>
                <b>
                    feat: Present Proof v3 - REST API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 06:54:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2971" class=".btn">#2971</a>
            </td>
            <td>
                <b>
                    feat: Present Proof v3 client implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 06:00:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2970" class=".btn">#2970</a>
            </td>
            <td>
                <b>
                    feat: Present proof v3 service implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 10:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2969" class=".btn">#2969</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.52.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.52.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.52.0</h2>
<h1>Feature</h1>
<ul>
<li><code>experiments.executeModule</code> is enabled by default and the option is removed
<ul>
<li>loaders are now free to use <code>this.importModule</code></li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix generated <code>__WEBPACK_EXTERNAL_MODULE_null__</code>, which leads to merged externals</li>
<li><code>.webpack[...]</code> extension is not part of matching and module name</li>
</ul>
<h2>v5.51.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix crash in FileSystemInfo when errors occur</li>
<li>avoid property access of reserved properties</li>
<li>fix reexports from async modules</li>
<li>automatically close an active watching when closing the compiler</li>
<li>when filenames of other runtimes are referenced that need a full hash, upgrade referencing runtime moduel to full hash mode too
<ul>
<li>fixes a bug where <code>[contenthash]</code> is undefined when using <code>new Worker</code></li>
</ul>
</li>
</ul>
<h2>v5.51.1</h2>
<h1>Bugfixes</h1>
<ul>
<li><code>library: &quot;module&quot;</code> propages top-level-await correctly</li>
<li>fix crash in filesystem snapshotting when trying to snapshot a non-existing directory</li>
<li>fix some context-dependent logic in concatenated modules and source url handling</li>
</ul>
<h2>v5.51.0</h2>
<h1>Bugfixes</h1>
<ul>
<li>correctly keep chunk loading state when the chunk loading logic is HMR updated
<ul>
<li>This fixes some edge cases that e. g. occur when using lazy compilation for entrypoints. It is now able to HMR update that instead of needing a manual reload. Also see fixes in webpack-dev-server@4.</li>
</ul>
</li>
<li>track and resolve symlinks for filesystem snapshotting
<ul>
<li>This fixes some cases of circular <code>yarn link</code>ing of dependencies.</li>
<li>It also fixes some problems when using package managers that use symlinks to deduplicate (e. g. cnpm or pnpm)</li>
</ul>
</li>
<li>pass the resulting module in the callbacks of <code>Compilation.addModuleChain</code> and <code>Compilation.addModuleTree</code></li>
</ul>
<h2>v5.50.0</h2>
<h1>Features</h1>
<ul>
<li>hashbangs (<code>#! ...</code>) are now handled by webpack
<ul>
<li><a href="https://github.com/tc39/proposal-hashbang">https://github.com/tc39/proposal-hashbang</a></li>
</ul>
</li>
</ul>
<h1>Performance</h1>
<ul>
<li>disable cache compression by default as it tend to make performance worse
<ul>
<li>I could still be enabled again for specific scenarios</li>
</ul>
</li>
<li>reduce the number of allocations during cache serialization
<ul>
<li>This improves performance and memory usage</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/4edd3800567f279edd7091af14b3385552a8972f"><code>4edd380</code></a> 5.52.0</li>
<li><a href="https://github.com/webpack/webpack/commit/d05648611aa6f554860a08940c3bf784b499c3a9"><code>d056486</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14134">#14134</a> from webpack/bugfix/webpack-extension</li>
<li><a href="https://github.com/webpack/webpack/commit/a513b1381a6e0248d1b44446a471b0bd6711a9b2"><code>a513b13</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14118">#14118</a> from webpack/bugfix/multiple-module-externals</li>
<li><a href="https://github.com/webpack/webpack/commit/825bbc1b61d562774dbe74ee3a84b4c0920b0a53"><code>825bbc1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14004">#14004</a> from webpack/dependabot/npm_and_yarn/webpack-cli-4.8.0</li>
<li><a href="https://github.com/webpack/webpack/commit/0d25c2f6889e8dd6199eca94e3a69ae5fee28474"><code>0d25c2f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14100">#14100</a> from webpack/dependabot/npm_and_yarn/eslint-plugin-...</li>
<li><a href="https://github.com/webpack/webpack/commit/1220f75bc52ed30e4eaee9f887182414d0b64c2a"><code>1220f75</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14126">#14126</a> from webpack/dependabot/npm_and_yarn/core-js-3.17.2</li>
<li><a href="https://github.com/webpack/webpack/commit/8cc4bda0b3f9b0f3241b4c5e0864239d6a306b14"><code>8cc4bda</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14127">#14127</a> from webpack/dependabot/npm_and_yarn/memfs-3.2.4</li>
<li><a href="https://github.com/webpack/webpack/commit/bc117e1e9782c7a267d97f9079816f77108c0c02"><code>bc117e1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14129">#14129</a> from webpack/dependabot/npm_and_yarn/fork-ts-checke...</li>
<li><a href="https://github.com/webpack/webpack/commit/765101bded6bf9dc9693fac6af18771d11b37eed"><code>765101b</code></a> match resource should not include special <code>.webpack[...]</code> extension</li>
<li><a href="https://github.com/webpack/webpack/commit/2ce5458404fa2db2bf91cec57f91142a2216fbfe"><code>2ce5458</code></a> chore(deps-dev): bump fork-ts-checker-webpack-plugin from 6.3.2 to 6.3.3</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.52.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.52.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-04 07:05:12 +0000 UTC
    </div>
</div>

