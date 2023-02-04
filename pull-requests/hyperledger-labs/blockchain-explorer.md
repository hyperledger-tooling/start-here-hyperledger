---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/343" class=".btn">#343</a>
            </td>
            <td>
                <b>
                    Bump http-cache-semantics from 4.1.0 to 4.1.1 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [http-cache-semantics](https://github.com/kornelski/http-cache-semantics) from 4.1.0 to 4.1.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kornelski/http-cache-semantics/commit/24496504352199caf360d1b4d4a01efdc8a7249e"><code>2449650</code></a> Update mocha</li>
<li><a href="https://github.com/kornelski/http-cache-semantics/commit/560b2d8ef452bbba20ffed69dc155d63ac757b74"><code>560b2d8</code></a> Don't use regex to trim whitespace</li>
<li><a href="https://github.com/kornelski/http-cache-semantics/commit/b1bdb92638426fab978f31e1330b6833015cabf0"><code>b1bdb92</code></a> Remove linting package zoo</li>
<li><a href="https://github.com/kornelski/http-cache-semantics/commit/c20dc7eeca608339143857953ee7ed9343fe6d3d"><code>c20dc7e</code></a> Cache 308</li>
<li>See full diff in <a href="https://github.com/kornelski/http-cache-semantics/compare/v4.1.0...v4.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=http-cache-semantics&package-manager=npm_and_yarn&previous-version=4.1.0&new-version=4.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-04 14:05:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    BE-340 Display health status of peers and orderers - FrontEnd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                …ity of peers and orderers

Signed-off-by: saksham1203 <saksham.s1203@gmail.com>

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This feature enables the explorer to indicate the health status of peers and orderers that are online or offline.
The status can be indicated with red being offline, green being online, green with flickering - fetching status.
As of now the explorer is not showing the status of peers/orderers that are part of HLF-Network. With this new feature enablement, we could display the health status of peers/orderers in the explorer dashboard.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #340 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
yes
```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->

![peer status](https://user-images.githubusercontent.com/72246428/215970360-2f8e6a84-8846-484d-ba5b-d35f7f3851e6.png "peer status").

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 06:43:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Purge data in explorer based on a parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Abhay Kishore <abhay.kishore@walmart.com>

#### What this PR does / why we need it: 
It will purge the old data present in explorer db based on the parameter `blockCount`.`blockCount` property can be defined in `config.json`.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note

```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 09:40:01 +0000 UTC
    </div>
</div>

