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
                PR <a href="https://github.com/hyperledger/cacti/pull/2310" class=".btn">#2310</a>
            </td>
            <td>
                <b>
                    feat(quorum-connector): add script for checking connection status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Simple script will check ledger connection by getting block through the connector.

Closes: #2309
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 13:59:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2307" class=".btn">#2307</a>
            </td>
            <td>
                <b>
                    fix: cannot read config eslint-config-prettier/@typescript-eslint.js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For now the ./weaver/ folder has been ignored by the root ESLint config.
This is a temporary fix given that ultimately we should be linting the
entire codebase.

I'll open a follow-up issue to cover the task of turning ESLint back on
for the code under ./weaver/

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 22:39:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2305" class=".btn">#2305</a>
            </td>
            <td>
                <b>
                    docs(maintainers/codeowners): update Sandeep's GH user to sandeepnRES
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Housekeeping of the documents that mention usernames.

Had to skip changing the username in the ./weaver/*.md because of the
newline index corruption problem explained in
https://github.com/hyperledger/cacti/issues/2302

Resolves #2304

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 21:27:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2303" class=".btn">#2303</a>
            </td>
            <td>
                <b>
                    fix(git): broken line endings corrupt git index after weaver merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not yet sure if this will fix the issue, but based on my research this
is the easiest and most probable solution.

Leaving a "paper trail" of the magical git commands that were executed
in order to have an idea in the future on how to fix potential negative
side-effects that might come out of this later (not likely but if it
does happen this should be immensely helpful information)

Without further ado, the list of commands executed to achieve this diff:

git rm --cached -r .

git config core.autocrlf input

git diff --cached --name-only -z | xargs -0 git add

Fixes #2302

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 21:09:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2301" class=".btn">#2301</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/sys from 0.0.0-20200720211630-cb9d2d5c5666 to 0.1.0 in /packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/fixtures/go/asset-transfer-private-data/chaincode-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/sys](https://github.com/golang/sys) from 0.0.0-20200720211630-cb9d2d5c5666 to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/sys/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/sys&package-manager=go_modules&previous-version=0.0.0-20200720211630-cb9d2d5c5666&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-25 06:24:02 +0000 UTC
    </div>
</div>

