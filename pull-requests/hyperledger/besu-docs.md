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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    Add docs for new BesuService plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * note links to hyperledger wiki are temporary and should be removed once javadoc publishing is automated

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 12:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    Add note to eth_syncing to clarify behaviour
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">external</span>
            </td>
            <td>
                ## Pull request checklist

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

Clarifying be haviour of `eth_syncing`.

Based on https://chat.hyperledger.org/channel/besu?msg=upgTmbuQNczHr8RBK

## Issue fixed

N/A

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
        Created At 2021-10-11 02:31:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    Document using DNS for permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Describe the change

Document using DNS for node permissioning, and restructure node and account allowlist content to make it easier to follow.

## Issue fixed

Fixes #819 

## Documentation preview

- https://hyperledger-besu--821.org.readthedocs.build/en/821/Concepts/Node-Keys/#enode-url
- https://hyperledger-besu--821.org.readthedocs.build/en/821/Reference/API-Methods/#perm_addnodestoallowlist
- https://hyperledger-besu--821.org.readthedocs.build/en/821/HowTo/Limit-Access/Local-Permissioning/
- https://hyperledger-besu--821.org.readthedocs.build/en/821/HowTo/Limit-Access/Updating-Permission-Lists/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-09 06:17:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    doc autocomplete usage
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

Add info for using subcommand and option autocomplete.

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #817 

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

See https://hyperledger-besu--820.org.readthedocs.build/en/820/

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-09 02:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Remove an old tip and fix some typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removed an old tip and fixed a couple of typos
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
        Created At 2021-10-06 22:33:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    [MINOR] fixed typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Mesage -> Message
I checked besu code and it has the correct spelling

  public int getDuplicateMessageLimit() {
    return JsonUtil.getInt(bftConfigRoot, "duplicatemessagelimit", DEFAULT_DUPLICATE_MESSAGE_LIMIT);
  }

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
        Created At 2021-10-05 04:50:52 +0000 UTC
    </div>
</div>

