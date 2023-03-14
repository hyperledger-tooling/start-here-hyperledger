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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    enable must gather on migrated consoles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Set `mustgather_enabled` feature flag setting as `true` on migrated consoles.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 18:13:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    Bump webpack from 5.64.4 to 5.76.0 in /packages/stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 5.64.4 to 5.76.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.76.0</h2>
<h2>Bugfixes</h2>
<ul>
<li>Avoid cross-realm object access by <a href="https://github.com/Jack-Works"><code>@​Jack-Works</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16500">webpack/webpack#16500</a></li>
<li>Improve hash performance via conditional initialization by <a href="https://github.com/lvivski"><code>@​lvivski</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16491">webpack/webpack#16491</a></li>
<li>Serialize <code>generatedCode</code> info to fix bug in asset module cache restoration by <a href="https://github.com/ryanwilsonperkin"><code>@​ryanwilsonperkin</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16703">webpack/webpack#16703</a></li>
<li>Improve performance of <code>hashRegExp</code> lookup by <a href="https://github.com/ryanwilsonperkin"><code>@​ryanwilsonperkin</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16759">webpack/webpack#16759</a></li>
</ul>
<h2>Features</h2>
<ul>
<li>add <code>target</code> to <code>LoaderContext</code> type by <a href="https://github.com/askoufis"><code>@​askoufis</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16781">webpack/webpack#16781</a></li>
</ul>
<h2>Security</h2>
<ul>
<li><a href="https://github.com/advisories/GHSA-3rfm-jhwj-7488">CVE-2022-37603</a> fixed by <a href="https://github.com/akhilgkrishnan"><code>@​akhilgkrishnan</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16446">webpack/webpack#16446</a></li>
</ul>
<h2>Repo Changes</h2>
<ul>
<li>Fix HTML5 logo in README by <a href="https://github.com/jakebailey"><code>@​jakebailey</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16614">webpack/webpack#16614</a></li>
<li>Replace TypeScript logo in README by <a href="https://github.com/jakebailey"><code>@​jakebailey</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16613">webpack/webpack#16613</a></li>
<li>Update actions/cache dependencies by <a href="https://github.com/piwysocki"><code>@​piwysocki</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16493">webpack/webpack#16493</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Jack-Works"><code>@​Jack-Works</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16500">webpack/webpack#16500</a></li>
<li><a href="https://github.com/lvivski"><code>@​lvivski</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16491">webpack/webpack#16491</a></li>
<li><a href="https://github.com/jakebailey"><code>@​jakebailey</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16614">webpack/webpack#16614</a></li>
<li><a href="https://github.com/akhilgkrishnan"><code>@​akhilgkrishnan</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16446">webpack/webpack#16446</a></li>
<li><a href="https://github.com/ryanwilsonperkin"><code>@​ryanwilsonperkin</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16703">webpack/webpack#16703</a></li>
<li><a href="https://github.com/piwysocki"><code>@​piwysocki</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16493">webpack/webpack#16493</a></li>
<li><a href="https://github.com/askoufis"><code>@​askoufis</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16781">webpack/webpack#16781</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/webpack/webpack/compare/v5.75.0...v5.76.0">https://github.com/webpack/webpack/compare/v5.75.0...v5.76.0</a></p>
<h2>v5.75.0</h2>
<h1>Bugfixes</h1>
<ul>
<li><code>experiments.*</code> normalize to <code>false</code> when opt-out</li>
<li>avoid <code>NaN%</code></li>
<li>show the correct error when using a conflicting chunk name in code</li>
<li>HMR code tests existance of <code>window</code> before trying to access it</li>
<li>fix <code>eval-nosources-*</code> actually exclude sources</li>
<li>fix race condition where no module is returned from processing module</li>
<li>fix position of standalong semicolon in runtime code</li>
</ul>
<h1>Features</h1>
<ul>
<li>add support for <code>@import</code> to extenal CSS when using experimental CSS in node</li>
<li>add <code>i64</code> support to the deprecated WASM implementation</li>
</ul>
<h1>Developer Experience</h1>
<ul>
<li>expose <code>EnableWasmLoadingPlugin</code></li>
<li>add more typings</li>
<li>generate getters instead of readonly properties in typings to allow overriding them</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/97b1718720c33f1b17302a74c5284b01e02ec001"><code>97b1718</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16781">#16781</a> from askoufis/loader-context-target-type</li>
<li><a href="https://github.com/webpack/webpack/commit/b84efe6224b276bf72e4c5e2f4e76acddfaeef07"><code>b84efe6</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16759">#16759</a> from ryanwilsonperkin/real-content-hash-regex-perf</li>
<li><a href="https://github.com/webpack/webpack/commit/c98e9e001441b165c7ed4845700839730b505833"><code>c98e9e0</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16493">#16493</a> from piwysocki/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/5f34acfbc074da6cc09f48944d7f2b4273ffb3f8"><code>5f34acf</code></a> feat: Add <code>target</code> to <code>LoaderContext</code> type</li>
<li><a href="https://github.com/webpack/webpack/commit/b7fc4d876deb958d7ee81ecc00a312e39a354a44"><code>b7fc4d8</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16703">#16703</a> from ryanwilsonperkin/ryanwilsonperkin/fix-16160</li>
<li><a href="https://github.com/webpack/webpack/commit/63ea82da4d4e4242b6a6285fc937f0684f264fe8"><code>63ea82d</code></a> Merge branch 'webpack:main' into patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/4ba225225b1348c8776ca5b5fe53468519413bc0"><code>4ba2252</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16446">#16446</a> from akhilgkrishnan/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/1acd6350be3d74d4ac70b64cbbc60f27724b618b"><code>1acd635</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16613">#16613</a> from jakebailey/ts-logo</li>
<li><a href="https://github.com/webpack/webpack/commit/302eb37fe19ed7ca60eaf895aca4f9da9dfd7931"><code>302eb37</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16614">#16614</a> from jakebailey/html5-logo</li>
<li><a href="https://github.com/webpack/webpack/commit/cfdb1dfe59b33bf7441b8a8e4fc58d75e4f54cee"><code>cfdb1df</code></a> Improve performance of hashRegExp lookup</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v5.64.4...v5.76.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~evilebottnawi">evilebottnawi</a>, a new releaser for webpack since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=5.64.4&new-version=5.76.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-14 18:12:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    fix password str validation on a dry-run request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- 
#### Description
Fixes password strength validation api if the request was a dry-run and the user does not exist. User does not need to exist for dry-run checks.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 19:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    adding the multi instance warning on migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
Added migration warning text to the migration information panel.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 18:46:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    handle req body size errors correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- bump request limit from 25MB to 100MB for fabric related apis
- adds logs when requests are terminated b/c of their size, actually it will log any body parser failure


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 20:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    Allow saas consoles to test password strength
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The test password strength api should work on saas consoles in prod.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 23:58:50 +0000 UTC
    </div>
</div>

