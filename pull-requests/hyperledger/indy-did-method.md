---
layout: default
title: indy-did-method
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-did-method
---

# indy-did-method <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-did-method){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Update readme with specup instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

Can’t assign you as reviewers, but please take a look @domwoe @l-wegner 

Thanks!

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 22:13:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Cleanup editors list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Cleanup editors list

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 21:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Testing rendering -- adding some editors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Tweak to get GHA to run
- Testing rendering -- adding some editors

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:56:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Tweak to get GHA to run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Update GHA to publish to gh-pages branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In theory, should address #8 . Publishing will go to the gh-pages branch, and gh-pages publishing will trigger on that.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:46:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Updates to render the spec into the /docs dir
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates to make the Spec Up render into the /docs dir. From there we will publish using gh-pages.

More updates probably needed, but this gets us started.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:52:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Bump axios from 0.21.1 to 0.21.2
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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:19:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Initial spec based on HackMD document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Transferred spec from [collaborative HackMD document](https://hackmd.io/@icZC4epNSnqBbYE0hJYseA/S1eUS2BQw#Indy-DID-Method) to Spec-Up.
* ToDos have been transferred as well
* Comments have not been transferred.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 14:48:20 +0000 UTC
    </div>
</div>

