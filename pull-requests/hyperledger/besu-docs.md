---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    doc update transaction call object parameters for EIP-1559
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

<!-- A clear and concise description of what this PR changes in the documentation. -->

Add two parameters to transaction call object for EIP-1559 transactions.

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #698 

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

https://hyperledger-besu--708.org.readthedocs.build/en/708/Reference/API-Objects/#transaction-call-object

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 05:04:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/706" class=".btn">#706</a>
            </td>
            <td>
                <b>
                    update guidance around remote connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [ ] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [ ] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [ ] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [ ] you fixed all the issues raised by the tests, if any.
- [ ] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

<!-- A clear and concise description of what this PR changes in the documentation. -->

Update guidance around limiting remote connections.

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #409 

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [ ] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 19:39:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/705" class=".btn">#705</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.20 to 4.17.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.20 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li>See full diff in <a href="https://github.com/lodash/lodash/compare/4.17.20...4.17.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.20&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/besu-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 00:51:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/704" class=".btn">#704</a>
            </td>
            <td>
                <b>
                    Bump hosted-git-info from 2.8.8 to 2.8.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [hosted-git-info](https://github.com/npm/hosted-git-info) from 2.8.8 to 2.8.9.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/hosted-git-info/blob/v2.8.9/CHANGELOG.md">hosted-git-info's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/hosted-git-info/compare/v2.8.8...v2.8.9">2.8.9</a> (2021-04-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>backport regex fix from <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/76">#76</a> (<a href="https://github.com/npm/hosted-git-info/commit/29adfe5">29adfe5</a>), closes <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/84">#84</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/hosted-git-info/commit/8d4b3697d79bcd89cdb36d1db165e3696c783a01"><code>8d4b369</code></a> chore(release): 2.8.9</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/29adfe5ef789784c861b2cdeb15051ec2ba651a7"><code>29adfe5</code></a> fix: backport regex fix from <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/76">#76</a></li>
<li>See full diff in <a href="https://github.com/npm/hosted-git-info/compare/v2.8.8...v2.8.9">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~nlf">nlf</a>, a new releaser for hosted-git-info since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hosted-git-info&package-manager=npm_and_yarn&previous-version=2.8.8&new-version=2.8.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/besu-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 00:51:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    Alphabetize API methods and edit for consistency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [ ] you fixed all the issues raised by the tests, if any.
- [ ] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

<!-- A clear and concise description of what this PR changes in the documentation. -->

- alphabetize API methods
- edit parameters/results styles across APIs for consistency
- no changes to the examples

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #363 

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 02:36:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    Add a step-by-step flow to illustrate nonce validation.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [ ] you fixed all the issues raised by the tests, if any.
- [ ] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

Add a step-by-step flow to illustrate nonce validation.

## Issue fixed

Fixes #403 

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 21:30:22 +0000 UTC
    </div>
</div>

