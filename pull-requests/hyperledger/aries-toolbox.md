---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jsoneditor from 9.5.2 to 9.5.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jsoneditor](https://github.com/josdejong/jsoneditor) from 9.5.2 to 9.5.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/josdejong/jsoneditor/blob/develop/HISTORY.md">jsoneditor's changelog</a>.</em></p>
<blockquote>
<h2>2021-09-22, version 9.5.6</h2>
<ul>
<li>Fix inefficient regex to replace return characters.</li>
</ul>
<h2>2021-09-01, version 9.5.5</h2>
<ul>
<li>Fix <code>setMode</code> not throwing an exception anymore in case of a parse error
(regression since <code>9.5.4</code>).</li>
</ul>
<h2>2021-08-25, version 9.5.4</h2>
<ul>
<li>Use <code>noreferrer</code> for window.open, see <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1365">#1365</a>. Thanks <a href="https://github.com/rajitbanerjee"><code>@​rajitbanerjee</code></a>.</li>
<li>Fix <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1363">#1363</a>: parsing error contains html characters.</li>
<li>Fix opening the Transform or Sort modal in code mode with invalid JSON
contents not triggering the <code>onError</code> callback (see <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1364">#1364</a>).</li>
<li>Change the default behavior of error handling to open a basic alert instead
of logging the error in the console (see <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1364">#1364</a>).</li>
</ul>
<h2>2021-07-28, version 9.5.3</h2>
<ul>
<li>Fix <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1356">#1356</a>: background of tree mode is transparent instead of white.</li>
<li>Fix <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/473">#473</a>: enum dropdown not working on referenced schemas and templates,
see <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1355">#1355</a>. Thanks <a href="https://github.com/mpccolorado"><code>@​mpccolorado</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/josdejong/jsoneditor/commit/d289517a114a7eccccd80881f40a2b8fd7e31827"><code>d289517</code></a> Publish v9.5.6, update devDependencies</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/6e64f937ef26eb5d894228693ff008f12f7386c6"><code>6e64f93</code></a> Add a SECURITY.md file</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/092e386cf49f2a1450625617da8e0137ed067c3e"><code>092e386</code></a> Fix inefficient regex to replace return characters</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/c33544bf7de6f4af05b58c4072e28bc786fb3f45"><code>c33544b</code></a> publish v9.5.5</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/f5b30462d9034dcd058c2241b6c1d2e4af8fce68"><code>f5b3046</code></a> Fix <code>setMode</code> not throwing an exception anymore in case of a parse error</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/f97e875d676b4fa0dc35721976296904b1356efb"><code>f97e875</code></a> Publish v9.5.4</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/b3b31f28d6b8b0d2e4c1c825acec194e3e8af343"><code>b3b31f2</code></a> Fix opening the Transform or Sort modal in code mode with invalid JSON conten...</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/cbb95ae97b32d0489e43870ed0e9e45d3e5f37bb"><code>cbb95ae</code></a> Change the default behavior of error handling to open a basic alert instead o...</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/883a0c9d4a806fa0291ac0fd4aa489eb655602eb"><code>883a0c9</code></a> Update history</li>
<li><a href="https://github.com/josdejong/jsoneditor/commit/5dbdfe4322008e6b849f2fd025ebdb70c7a1e177"><code>5dbdfe4</code></a> Fix <a href="https://github-redirect.dependabot.com/josdejong/jsoneditor/issues/1363">#1363</a>: parsing error contains html caharacters</li>
<li>Additional commits viewable in <a href="https://github.com/josdejong/jsoneditor/compare/v9.5.2...v9.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsoneditor&package-manager=npm_and_yarn&previous-version=9.5.2&new-version=9.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 17:29:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump axios from 0.21.1 to 0.21.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 18:20:01 +0000 UTC
    </div>
</div>

