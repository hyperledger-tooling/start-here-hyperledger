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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/791" class=".btn">#791</a>
            </td>
            <td>
                <b>
                    plugin api: updated to artifactory link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Updated maven dependency link

Fixes #787 

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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 05:04:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    [MINOR] Fixed some typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed some typos and updated repo links

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

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 05:00:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/785" class=".btn">#785</a>
            </td>
            <td>
                <b>
                    add @rolandtyler as maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This is a proposal to add Roland Tyler (@rolandtyler) as a maintainer.

### Disclosure

Roland is part of Consensys Protocol doc team.

### Process

Change will be accepted if the following rules are followed:

- [x] 5 significant changes have been authored by the proposed maintainer and accepted.
  Here is [the list of changes Roland recently made](https://github.com/hyperledger/besu-docs/pulls?q=is%3Apr+is%3Amerged+author%3Arolandtyler).
- [x] The proposed maintainer has the sponsorship of at least one other maintainer.
    - [x] This sponsoring maintainer will create a PR modifying the list of maintainers. **-> that's me**
    - [x] The proposed maintainer accepts the nomination and expresses a willingness to be a long-term (more than 6 months) committer.
    - [x] This would be a comment in the above PR. **@rolandtyler can you comment on this PR to accept please?**
- [x] This PR will be communicated in all appropriate communication channels.
      It should be mentioned in any maintainer/community call.
      It should also be posted to the appropriate mailing list or chat channels if they exist.
      **See Hyperledger [RocketChat](https://chat.hyperledger.org/channel/besu-contributors) and [mailing list](https://lists.hyperledger.org/g/besu)**
- [x] Approval by at least 3 current maintainers within two weeks **(until 2021, September 17)** of the proposal,
- [ ] or an absolute majority of current maintainers.
    - These votes will be recorded as review approval, comments or 👍 in the PR modifying the list of maintainers.
- [ ] No veto by another maintainer within two weeks of proposal are recorded **(until 2021, September 17)**.
    - All vetoes must be accompanied by a public explanation as a comment in the PR for adding this maintainer
    - The explanation of the veto must be reasonable.
    - A veto can be retracted, in that case the approval/veto timeframe is reset.
    - It is bad form to veto, retract, and veto again.
- The proposed maintainer becomes a maintainer
    - Either two weeks have passed since the third approval **(on 2021, September 17)**,
    - Or an absolute majority of maintainers approve.
    - In either case, no maintainer presents a veto.

## Maintainers able to vote on this

All users in https://github.com/orgs/hyperledger/teams/besu-docs-maintainers/members and https://github.com/orgs/hyperledger/teams/besu-maintainers/members

Total is 28 unique users => absolute majority is 15 users.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 17:26:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/784" class=".btn">#784</a>
            </td>
            <td>
                <b>
                    Permissioning contracts v2.0.1 migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

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

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

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
        Created At 2021-09-02 23:11:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/783" class=".btn">#783</a>
            </td>
            <td>
                <b>
                    update genesis file content
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

Update genesis file content for clarity and consistency with GoQuorum docs (see https://github.com/ConsenSys/doc.goquorum/pull/128).

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #745 

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
        Created At 2021-09-02 22:54:58 +0000 UTC
    </div>
</div>

