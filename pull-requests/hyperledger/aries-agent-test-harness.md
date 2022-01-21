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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    further separated crons for less parallel execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This may fix the cancelled jobs in the daily interop test runs. If this does work, that means ultimately we need to move to the matrix model so this doesn't happen again. This current submission is just to prove the crons are/were the problem. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 13:40:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    refactor(dotnet): remove credential proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #356

Tested to work with .NET, still running other tests to make sure I didn't break anything else
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 15:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    fix: sleep is not defined
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes an issue with `sleep` not being defined resulting in all present proof tests to fail (not sure how I missed this, as the tests ran successfully yesterday...)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 14:28:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    fix: rename 0453 to 0454 for present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes #373
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 14:09:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.3 to 1.14.7 in /aries-backchannels/verity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.3 to 1.14.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/6f5029ae1a0fdab4dc25f6379a5ee303c2319070"><code>6f5029a</code></a> Release version 1.14.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/af706bee57de954414c0bde0a9f33e62beea3e52"><code>af706be</code></a> Ignore null headers.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d01ab7a5c5df3617c7a40a03de7af6427fdfac55"><code>d01ab7a</code></a> Release version 1.14.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/40052ea8aa13559becee5795715c1d45b1f0eb76"><code>40052ea</code></a> Make compatible with Node 17.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/86f7572f9365dadc39f85916259b58973819617f"><code>86f7572</code></a> Fix: clear internal timer on request abort to avoid leakage</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2e1eaf0218c5315a2ab27f53964d0535d4dafb51"><code>2e1eaf0</code></a> Keep Authorization header on subdomain redirects.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ad9e82b6277ae2104f7770e9ff1186cc6da29d4"><code>2ad9e82</code></a> Carry over Host header on relative redirects (<a href="https://github-redirect.dependabot.com/follow-redirects/follow-redirects/issues/172">#172</a>)</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/77e2a581e1d1811674b7b74745a9c20a5b939488"><code>77e2a58</code></a> Release version 1.14.4 of the npm package.</li>
<li>Additional commits viewable in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.3...v1.14.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.3&new-version=1.14.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-15 14:20:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    Bump shelljs from 0.8.4 to 0.8.5 in /aries-backchannels/verity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [shelljs](https://github.com/shelljs/shelljs) from 0.8.4 to 0.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/shelljs/shelljs/releases">shelljs's releases</a>.</em></p>
<blockquote>
<h2>v0.8.5</h2>
<p>This was a small security fix for <a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1058">#1058</a>.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/shelljs/shelljs/commit/70668a4555c7d49c4f67d53ea063b899be4d6d40"><code>70668a4</code></a> 0.8.5</li>
<li><a href="https://github.com/shelljs/shelljs/commit/d919d22dd6de385edaa9d90313075a77f74b338c"><code>d919d22</code></a> fix(exec): lockdown file permissions (<a href="https://github-redirect.dependabot.com/shelljs/shelljs/issues/1060">#1060</a>)</li>
<li>See full diff in <a href="https://github.com/shelljs/shelljs/compare/v0.8.4...v0.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=shelljs&package-manager=npm_and_yarn&previous-version=0.8.4&new-version=0.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-15 07:15:04 +0000 UTC
    </div>
</div>

