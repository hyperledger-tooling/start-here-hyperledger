---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    Acapy-b-verity test runset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR adds an acapy-b-verity runset for daily execution in GHA. 
A acapy-b-verity project has been added to allure. 
The aries interop reports should be automatically updated upon test completion.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 21:30:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    removal of one revocation test as mobile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Simple fix to remove a mistakenly added Revocation MobileTest in a previous PR. 

This PR closes #330
There is still a failure with the esatus wallet on revocation test `T001.2-HIPE0011`. This test revokes a credential, but since the verifier doesn't include a timestamp in the proof request, that means they don't care if the credential was revoked.  This case is derived from [RFC 0441](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0441-present-proof-best-practices#semantics-of-non-revocation-interval-presence-and-absence) and states the following, 
```
The absence of any non-revocation interval applicable to a requested item signifies that the verifier has no interest in its
credential's non-revocation status.

A revocable or non-revocable credential may satisfy a presentation request with or without a non-revocation interval. 
The presence of a non-revocation interval conveys that if the prover presents a revocable credential, the presentation 
must include proof of non-revocation. Its presence does not convey any restriction on the revocability of the credential to 
present: in many cases the verifier cannot know whether a prover's credential is revocable or not.
```
Depending on how we interpret that section, we may want to talk to esatus about it. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 22:06:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    build(deps): Bump axios from 0.21.1 to 0.21.2 in /aries-backchannels/verity
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 23:06:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    build(deps): Bump tar from 4.4.13 to 4.4.19 in /aries-backchannels/verity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 4.4.13 to 4.4.19.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/9a6faa017ca90538840f3ae2ccdb4550ac3f4dcf"><code>9a6faa0</code></a> 4.4.19</li>
<li><a href="https://github.com/npm/node-tar/commit/70ef812593184cc54ea1bc74c5dae2d22995002d"><code>70ef812</code></a> drop dirCache for symlink on all platforms</li>
<li><a href="https://github.com/npm/node-tar/commit/3e35515c09da615ac268254bed85fe43ee71e2f0"><code>3e35515</code></a> 4.4.18</li>
<li><a href="https://github.com/npm/node-tar/commit/52b09e309bcae0c741a7eb79a17ef36e7828b946"><code>52b09e3</code></a> fix: prevent path escape using drive-relative paths</li>
<li><a href="https://github.com/npm/node-tar/commit/bb93ba243746f705092905da1955ac3b0509ba1e"><code>bb93ba2</code></a> fix: reserve paths properly for unicode, windows</li>
<li><a href="https://github.com/npm/node-tar/commit/2f1bca027286c23e110b8dfc7efc10756fa3db5a"><code>2f1bca0</code></a> fix: prune dirCache properly for unicode, windows</li>
<li><a href="https://github.com/npm/node-tar/commit/9bf70a8cf725c3af5fe2270f1e5d2e06d1559b93"><code>9bf70a8</code></a> 4.4.17</li>
<li><a href="https://github.com/npm/node-tar/commit/6aafff0a8621ba9509b63654bde28762be373d58"><code>6aafff0</code></a> fix: skip extract if linkpath is stripped entirely</li>
<li><a href="https://github.com/npm/node-tar/commit/5c5059a69c2aaaedfe4e9766e102ae9fb79e8255"><code>5c5059a</code></a> fix: reserve paths case-insensitively</li>
<li><a href="https://github.com/npm/node-tar/commit/fd6accba697070560f301604b8f5f7e2995a2a8b"><code>fd6accb</code></a> 4.4.16</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v4.4.13...v4.4.19">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=4.4.13&new-version=4.4.19)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 23:05:47 +0000 UTC
    </div>
</div>

