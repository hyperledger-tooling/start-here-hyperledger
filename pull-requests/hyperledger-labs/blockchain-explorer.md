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
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    purge functionality based on blockcount and time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:

Now explorer database is saving each transaction that is committed on to the ledger making replica copies of ledger. When number of transactions increases there is a chance of outage of postgres database. In order to address this we would keep only the recent data in database and provide a query back mechanism to read back from the blockchain for any of the purged data.

Implementation

Based on BLOCKCOUNT
Based on TIME
We can set the purgeMode attribute in config.json file and according to the purge mode, it enables purging from database.
If it is based on blockcount (mention the number of blocks as blockCount value in config.json) ,it will retain those many blocks in the database and the rest of the records would be purged.
If it is based on time (mention the number of days as daysToPurge value in config.json) then it will keep those many days of records in the database according to the daystoPurge provided in the config file.
If the purgeMode attribute is set to "NONE", then purging won't happen and it will retain the complete data as of ledger.

All the audit records of deletion is saved to explorer_audit_table which is further used for the sync process.

Why is this needed?
Explorer creates duplicate copy of complete ledger data in postgres which can be of larger number and can lead to database storage outage.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #332 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
NONE
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
        Created At 2023-03-01 12:29:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    added Prometheus metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This PR has changes to add support for prometheus metrics.

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
        Created At 2023-03-01 06:50:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/sys from 0.0.0-20200212091648-12a6c2dcc1e4 to 0.1.0 in /app/platform/fabric/e2e-test/specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/sys](https://github.com/golang/sys) from 0.0.0-20200212091648-12a6c2dcc1e4 to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/sys/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/sys&package-manager=go_modules&previous-version=0.0.0-20200212091648-12a6c2dcc1e4&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-25 04:34:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Bump sequelize from 6.12.2 to 6.29.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [sequelize](https://github.com/sequelize/sequelize) from 6.12.2 to 6.29.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sequelize/sequelize/releases">sequelize's releases</a>.</em></p>
<blockquote>
<h2>v6.29.0</h2>
<h1><a href="https://github.com/sequelize/sequelize/compare/v6.28.2...v6.29.0">6.29.0</a> (2023-02-23)</h1>
<h3>Features</h3>
<ul>
<li>throw an error if attribute includes parentheses (fixes CVE-2023-22578) (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15710">#15710</a>) (<a href="https://github.com/sequelize/sequelize/commit/d3f5b5a65e297f4b6861e6a6ce335a9830b28781">d3f5b5a</a>)</li>
</ul>
<h2>v6.28.2</h2>
<h2><a href="https://github.com/sequelize/sequelize/compare/v6.28.1...v6.28.2">6.28.2</a> (2023-02-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>accept undefined in where (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15703">#15703</a>) (<a href="https://github.com/sequelize/sequelize/commit/13f2e89f8b6147897e3e43f01487de51aebcde87">13f2e89</a>)</li>
</ul>
<h2>v6.28.1</h2>
<h2><a href="https://github.com/sequelize/sequelize/compare/v6.28.0...v6.28.1">6.28.1</a> (2023-02-21)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>throw if where receives an invalid value (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15699">#15699</a>) (<a href="https://github.com/sequelize/sequelize/commit/d9e0728f2c2c5ae319f337c78091e1081440595d">d9e0728</a>)</li>
<li>update moment-timezone version (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15685">#15685</a>) (<a href="https://github.com/sequelize/sequelize/commit/48d619379108320831c9c6a0ec42bfda6586fec5">48d6193</a>)</li>
</ul>
<h2>v6.28.0</h2>
<h1><a href="https://github.com/sequelize/sequelize/compare/v6.27.0...v6.28.0">6.28.0</a> (2022-12-20)</h1>
<h3>Features</h3>
<ul>
<li><strong>types:</strong> use retry-as-promised types for retry options to match documentation  (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15484">#15484</a>) (<a href="https://github.com/sequelize/sequelize/commit/fd4afa6a89c111c6d6d0c94f0b98bf421b5357b6">fd4afa6</a>)</li>
</ul>
<h2>v6.27.0</h2>
<h1><a href="https://github.com/sequelize/sequelize/compare/v6.26.0...v6.27.0">6.27.0</a> (2022-12-12)</h1>
<h3>Features</h3>
<ul>
<li>add support for bigints (backport of <a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/14485">#14485</a>) (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15413">#15413</a>) (<a href="https://github.com/sequelize/sequelize/commit/1247c01265743e4bdbd6d91a51cf64cd9d1e6617">1247c01</a>)</li>
</ul>
<h2>v6.26.0</h2>
<h1><a href="https://github.com/sequelize/sequelize/compare/v6.25.8...v6.26.0">6.26.0</a> (2022-11-29)</h1>
<h3>Features</h3>
<ul>
<li><strong>postgres:</strong> add support for lock_timeout [<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15345">#15345</a>] (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15355">#15355</a>) (<a href="https://github.com/sequelize/sequelize/commit/94beace4ca666765ec9c84a3f7ef0e826e09699d">94beace</a>)</li>
</ul>
<h2>v6.25.8</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sequelize/sequelize/commit/d3f5b5a65e297f4b6861e6a6ce335a9830b28781"><code>d3f5b5a</code></a> feat: throw an error if attribute includes parentheses (fixes CVE-2023-22578)...</li>
<li><a href="https://github.com/sequelize/sequelize/commit/53bd9b78c18992765a5a078e3d759199c4de69a7"><code>53bd9b7</code></a> meta: fix null test getWhereConditions (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15705">#15705</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/13f2e89f8b6147897e3e43f01487de51aebcde87"><code>13f2e89</code></a> fix: accept undefined in where (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15703">#15703</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/d9e0728f2c2c5ae319f337c78091e1081440595d"><code>d9e0728</code></a> fix: throw if where receives an invalid value (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15699">#15699</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/48d619379108320831c9c6a0ec42bfda6586fec5"><code>48d6193</code></a> fix: update moment-timezone version (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15685">#15685</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/fd4afa6a89c111c6d6d0c94f0b98bf421b5357b6"><code>fd4afa6</code></a> feat(types): use retry-as-promised types for retry options to match documenta...</li>
<li><a href="https://github.com/sequelize/sequelize/commit/1247c01265743e4bdbd6d91a51cf64cd9d1e6617"><code>1247c01</code></a> feat: add support for bigints (backport of <a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/14485">#14485</a>) (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15413">#15413</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/94beace4ca666765ec9c84a3f7ef0e826e09699d"><code>94beace</code></a> feat(postgres): add support for lock_timeout <a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15345">#15345</a> (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15355">#15355</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/7885000a70eb451100fa8f54d45361887241521c"><code>7885000</code></a> fix(oracle): remove hardcoded maxRows value (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15323">#15323</a>)</li>
<li><a href="https://github.com/sequelize/sequelize/commit/bc39fd69919e0af0cb0732ca9bfe3e60691c778a"><code>bc39fd6</code></a> fix: fix parameters not being replaced when after $$ strings (<a href="https://github-redirect.dependabot.com/sequelize/sequelize/issues/15307">#15307</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/sequelize/sequelize/compare/v6.12.2...v6.29.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~sdepold">sdepold</a>, a new releaser for sequelize since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sequelize&package-manager=npm_and_yarn&previous-version=6.12.2&new-version=6.29.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-25 00:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/357" class=".btn">#357</a>
            </td>
            <td>
                <b>
                    Added search functonality to dashboard so user can search with Txn ha…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …sh/Block no from there itself

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
The feature facilitates user to search data using a block number/transaction id. The Search field is provided in the dashboard screen. A modal with the appropriate data will be displayed in response to user input.
It provisions user for a quick data search pertaining to specific block or transaction.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #345 

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
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-24 08:19:41 +0000 UTC
    </div>
</div>

