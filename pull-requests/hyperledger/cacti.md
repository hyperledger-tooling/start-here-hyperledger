---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2384" class=".btn">#2384</a>
            </td>
            <td>
                <b>
                    feat(relay): configurable db_open retry mechanism added and in driver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added two env variables in driver and config variables in relay to configure retry mechanism while opening database:
1. Max number of retries
2. Backoff time in milli seconds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 11:19:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2382" class=".btn">#2382</a>
            </td>
            <td>
                <b>
                    chore(docs): fix dci-lint failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 18:24:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2381" class=".btn">#2381</a>
            </td>
            <td>
                <b>
                    fix(iroha2-connector): fix flaky tests to solve #2370 and #2373
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use waitForCommit for all transactions used in test suites to prevent spurious CI test failures.

Closes: #2370
Closes: #2373
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 13:19:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2380" class=".btn">#2380</a>
            </td>
            <td>
                <b>
                    fix(custom-gitguardian): error invalid token header #2379
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: 2379

related to: #2313 and #1996
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 03:54:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2374" class=".btn">#2374</a>
            </td>
            <td>
                <b>
                    build(deps): bump @sideway/formula from 3.0.0 to 3.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@sideway/formula](https://github.com/sideway/formula) from 3.0.0 to 3.0.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hapijs/formula/commit/5b44c1bffc38135616fb91d5ad46eaf64f03d23b"><code>5b44c1b</code></a> 3.0.1</li>
<li><a href="https://github.com/hapijs/formula/commit/9fbc20a02d75ae809c37a610a57802cd1b41b3fe"><code>9fbc20a</code></a> chore: better number regex</li>
<li><a href="https://github.com/hapijs/formula/commit/41ae98e0421913b100886adb0107a25d552d9e1a"><code>41ae98e</code></a> Cleanup</li>
<li><a href="https://github.com/hapijs/formula/commit/c59f35ec401e18cead10e0cedfb44291517610b1"><code>c59f35e</code></a> Move to Sideway</li>
<li>See full diff in <a href="https://github.com/sideway/formula/compare/v3.0.0...v3.0.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~marsup">marsup</a>, a new releaser for <code>@​sideway/formula</code> since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@sideway/formula&package-manager=npm_and_yarn&previous-version=3.0.0&new-version=3.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 20:51:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2372" class=".btn">#2372</a>
            </td>
            <td>
                <b>
                    build(deps): upgrade lerna-lite from v1.4.0 to v1.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The upgrade is necessary in order to address this
server side request forgery vulnerability:

https://github.com/hyperledger/cacti/security/dependabot/240

CVE-2022-2900

Fixes #2371
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 01:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2369" class=".btn">#2369</a>
            </td>
            <td>
                <b>
                    refactor(workflows): use 4vcpu runner for weaver data sharing workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to resolve data sharing worklow failing for abritrary reasons.
Additionally rename weaver workflows jobs, so as to uniquely identify them by their name.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 16:56:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2368" class=".btn">#2368</a>
            </td>
            <td>
                <b>
                    chore(ci): update deprecated GitHub API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use current version of GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 15:50:36 +0000 UTC
    </div>
</div>

